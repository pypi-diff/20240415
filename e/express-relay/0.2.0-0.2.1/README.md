# Comparing `tmp/express_relay-0.2.0.tar.gz` & `tmp/express_relay-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express_relay-0.2.0.tar", max compression
+gzip compressed data, was "express_relay-0.2.1.tar", max compression
```

## Comparing `express_relay-0.2.0.tar` & `express_relay-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      949 2024-03-15 19:40:32.475793 express_relay-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-15 20:11:28.659300 express_relay-0.2.0/express_relay/__init__.py
--rw-r--r--   0        0        0    16068 2024-03-15 20:11:28.659938 express_relay-0.2.0/express_relay/client.py
--rw-r--r--   0        0        0     5003 2024-03-15 20:11:28.660344 express_relay-0.2.0/express_relay/searcher/examples/simple_searcher.py
--rw-r--r--   0        0        0     8809 2024-03-15 20:11:28.660570 express_relay-0.2.0/express_relay/types.py
--rw-r--r--   0        0        0      612 2024-03-15 20:11:28.661293 express_relay-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      949 2024-03-15 19:40:32.475793 express_relay-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-15 20:11:28.659300 express_relay-0.2.1/express_relay/__init__.py
+-rw-r--r--   0        0        0    16242 2024-04-11 20:24:03.675164 express_relay-0.2.1/express_relay/client.py
+-rw-r--r--   0        0        0     5160 2024-04-11 20:24:03.675474 express_relay-0.2.1/express_relay/searcher/examples/simple_searcher.py
+-rw-r--r--   0        0        0     9248 2024-04-11 20:24:03.675769 express_relay-0.2.1/express_relay/types.py
+-rw-r--r--   0        0        0      612 2024-04-11 20:24:03.678556 express_relay-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.2.1/PKG-INFO
```

### Comparing `express_relay-0.2.0/README.md` & `express_relay-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `express_relay-0.2.0/express_relay/client.py` & `express_relay-0.2.1/express_relay/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,18 +318,22 @@
                         )
                         if opportunity:
                             asyncio.create_task(opportunity_callback(opportunity))
 
                 elif msg_json.get("type") == "bid_status_update":
                     if bid_status_callback is not None:
                         id = msg_json["status"]["id"]
-                        bid_status = msg_json["status"]["bid_status"]["status"]
+                        bid_status = msg_json["status"]["bid_status"]["type"]
                         result = msg_json["status"]["bid_status"].get("result")
+                        index = msg_json["status"]["bid_status"].get("index")
                         bid_status_update = BidStatusUpdate(
-                            id=id, bid_status=BidStatus(bid_status), result=result
+                            id=id,
+                            bid_status=BidStatus(bid_status),
+                            result=result,
+                            index=index,
                         )
                         asyncio.create_task(bid_status_callback(bid_status_update))
 
             elif msg_json.get("id"):
                 future = self.ws_msg_futures.pop(msg_json["id"])
                 future.set_result(msg_json)
```

### Comparing `express_relay-0.2.0/express_relay/searcher/examples/simple_searcher.py` & `express_relay-0.2.1/express_relay/searcher/examples/simple_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,21 @@
             bid_status_update: An object representing an update to the status of a bid.
         """
         id = bid_status_update.id
         bid_status = bid_status_update.bid_status
         result = bid_status_update.result
 
         if bid_status == BidStatus("submitted"):
-            logger.info(f"Bid {id} has been submitted in hash {result}")
+            logger.info(
+                f"Bid {id} has been submitted in transaction {result} at index {bid_status_update.index} of the multicall"
+            )
         elif bid_status == BidStatus("lost"):
-            logger.info(f"Bid {id} was unsuccessful")
+            logger.info(
+                f"Bid {id} was unsuccessful, not included in transaction {result}"
+            )
         elif bid_status == BidStatus("pending"):
             logger.info(f"Bid {id} is pending")
         else:
             logger.error(f"Unrecognized status {bid_status} for bid {id}")
 
 
 async def main():
```

### Comparing `express_relay-0.2.0/express_relay/types.py` & `express_relay-0.2.1/express_relay/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,27 +108,37 @@
 
 
 class BidStatusUpdate(BaseModel):
     """
     Attributes:
         id: The ID of the bid.
         bid_status: The status enum, either SUBMITTED, LOST, or PENDING.
-        result: The result of the bid: a transaction hash if the status is SUBMITTED, else None.
+        result: The result of the bid: a transaction hash if the status is SUBMITTED or LOST, else None.
+        index: The index of the bid in the submitted transaction; None if the status is not SUBMITTED.
     """
 
     id: UUIDString
     bid_status: BidStatus
     result: Bytes32 | None = Field(default=None)
+    index: int | None = Field(default=None)
 
     @model_validator(mode="after")
     def check_result(self):
-        if self.bid_status == BidStatus("submitted"):
+        if self.bid_status == BidStatus("pending"):
+            assert self.result is None, "result must be None"
+        else:
             assert self.result is not None, "result must be a valid 32-byte hash"
+        return self
+
+    @model_validator(mode="after")
+    def check_index(self):
+        if self.bid_status == BidStatus("submitted"):
+            assert self.index is not None, "index must be a valid integer"
         else:
-            assert self.result is None, "result must be None"
+            assert self.index is None, "index must be None"
         return self
 
 
 class OpportunityBid(BaseModel):
     """
     Attributes:
         opportunity_id: The ID of the opportunity.
```

### Comparing `express_relay-0.2.0/pyproject.toml` & `express_relay-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "express-relay"
-version = "0.2.0"
+version = "0.2.1"
 description = "Utilities for searchers and protocols to interact with the Express Relay protocol."
 authors = ["dourolabs"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `express_relay-0.2.0/PKG-INFO` & `express_relay-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-relay
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for searchers and protocols to interact with the Express Relay protocol.
 License: Proprietary
 Author: dourolabs
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

