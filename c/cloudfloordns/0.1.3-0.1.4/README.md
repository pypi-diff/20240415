# Comparing `tmp/cloudfloordns-0.1.3.tar.gz` & `tmp/cloudfloordns-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudfloordns-0.1.3.tar", max compression
+gzip compressed data, was "cloudfloordns-0.1.4.tar", max compression
```

## Comparing `cloudfloordns-0.1.3.tar` & `cloudfloordns-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,20 @@
--rw-r--r--   0        0        0     3000 2024-04-15 13:32:53.472219 cloudfloordns-0.1.3/README.md
--rw-r--r--   0        0        0       89 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/__init__.py
--rw-r--r--   0        0        0      470 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/__main__.py
--rw-r--r--   0        0        0       25 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/__init__.py
--rw-r--r--   0        0        0       27 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/__init__.py
--rw-r--r--   0        0        0     5506 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/client.py
--rw-r--r--   0        0        0     7406 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/domain.py
--rw-r--r--   0        0        0      141 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/domain_registration.py
--rw-r--r--   0        0        0     1475 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/groups.py
--rw-r--r--   0        0        0       50 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/client/sync/pool.py
--rw-r--r--   0        0        0     1547 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/client/sync/record.py
--rw-r--r--   0        0        0     3433 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client.py
--rw-r--r--   0        0        0     8725 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/domain.py
--rw-r--r--   0        0        0     3904 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/domain_registration.py
--rw-r--r--   0        0        0     2050 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/groups.py
--rw-r--r--   0        0        0       80 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/domain.py
--rw-r--r--   0        0        0     2611 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/domain_registration.py
--rw-r--r--   0        0        0      654 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/groups.py
--rw-r--r--   0        0        0     3439 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/record.py
--rw-r--r--   0        0        0     7196 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/record.py
--rw-r--r--   0        0        0     1882 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/utils/__init__.py
--rw-r--r--   0        0        0     2642 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/utils/make_async.py
--rw-r--r--   0        0        0      765 2024-04-15 13:32:53.484219 cloudfloordns-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 cloudfloordns-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3000 2024-04-15 13:32:53.472219 cloudfloordns-0.1.4/README.md
+-rw-r--r--   0        0        0       89 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/__main__.py
+-rw-r--r--   0        0        0       25 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/client/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/client/sync/__init__.py
+-rw-r--r--   0        0        0     5506 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/client/sync/client.py
+-rw-r--r--   0        0        0     7549 2024-04-15 13:48:18.277938 cloudfloordns-0.1.4/cloudfloordns/client/sync/domain.py
+-rw-r--r--   0        0        0      141 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/client/sync/domain_registration.py
+-rw-r--r--   0        0        0     1475 2024-04-15 13:32:53.476219 cloudfloordns-0.1.4/cloudfloordns/client/sync/groups.py
+-rw-r--r--   0        0        0       50 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/client/sync/pool.py
+-rw-r--r--   0        0        0     1547 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/client/sync/record.py
+-rw-r--r--   0        0        0       80 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/models/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/models/domain.py
+-rw-r--r--   0        0        0     2611 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/models/domain_registration.py
+-rw-r--r--   0        0        0      654 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/models/groups.py
+-rw-r--r--   0        0        0     3439 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/models/record.py
+-rw-r--r--   0        0        0     1882 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2024-04-15 13:32:53.480219 cloudfloordns-0.1.4/cloudfloordns/utils/make_async.py
+-rw-r--r--   0        0        0      765 2024-04-15 13:48:18.281938 cloudfloordns-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 cloudfloordns-0.1.4/PKG-INFO
```

### Comparing `cloudfloordns-0.1.3/README.md` & `cloudfloordns-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/client/sync/client.py` & `cloudfloordns-0.1.4/cloudfloordns/client/sync/client.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/client/sync/domain.py` & `cloudfloordns-0.1.4/cloudfloordns/client/sync/domain.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,20 +49,27 @@
         request_data = {**soa_data, **data}
         return self.client.patch(
             url,
             data=request_data,
             timeout=timeout,
         )
 
-    # def delete(self, domain: str, record_id: str, timeout=None):
-    #     url = f"/dns/zone/{domain}/record/{record_id}"
-    #     return self.client.delete(
-    #         url,
-    #         timeout=timeout,
-    #     )
+    def disable(self, domain: str, timeout=None):
+        url = f"/dns/zone/{domain}"
+        return self.client.delete(
+            url,
+            timeout=timeout,
+        )
+
+    def delete(self, domain: str, timeout=None):
+        url = f"/domain/{domain}/delete_domain"
+        return self.client.delete(
+            url,
+            timeout=timeout,
+        )
 
     def _list_all(self, timeout=None):
         url = "/dns"
         res = self.client.get(
             url,
             timeout=timeout,
         )
```

### Comparing `cloudfloordns-0.1.3/cloudfloordns/client/sync/groups.py` & `cloudfloordns-0.1.4/cloudfloordns/client/sync/groups.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/client/sync/record.py` & `cloudfloordns-0.1.4/cloudfloordns/client/sync/record.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/domain_registration.py` & `cloudfloordns-0.1.4/cloudfloordns/models/domain_registration.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,50 +82,7 @@
     def is_same(self, right: "Domain") -> bool:
         """
         This method check the identity (e.g. same id if defined, or same name/name+value)
         """
         if not isinstance(right, Domain):
             return NotImplemented
         return self.domainname == self.right
-
-
-class Domains:
-    def __init__(self, client) -> None:
-        self.client = client
-
-    # def create(self, domain: str, record: Record, timeout=None):
-    #     url = f"/dns/zone/{domain}/record"
-    #     return self.client.post(
-    #         url,
-    #         data=record.model_dump(),
-    #         timeout=timeout,
-    #     )
-
-    # def update(self, domain: str, record_id: str, record: Record, timeout=None):
-    #     url = f"/dns/zone/{domain}/record/{record_id}"
-    #     return self.client.patch(
-    #         url,
-    #         data=record.model_dump(exclude_unset=True),
-    #         timeout=timeout,
-    #     )
-
-    # def delete(self, domain: str, record_id: str, timeout=None):
-    #     url = f"/dns/zone/{domain}/record/{record_id}"
-    #     return self.client.delete(
-    #         url,
-    #         timeout=timeout,
-    #     )
-
-    def get(self, domain: str, timeout=None):
-        url = f"/domain/{domain}"
-        res = self.client.get(
-            url,
-            timeout=timeout,
-        )
-        return [Domain(**d) for d in res]
-
-    # def get(self, domain: str, record_id, timeout=None):
-    #     res = self.client.list(
-    #         domain,
-    #         timeout=timeout,
-    #     )
-    #     return next((r for r in res if r.id == record_id), None)
```

### Comparing `cloudfloordns-0.1.3/cloudfloordns/models/domain.py` & `cloudfloordns-0.1.4/cloudfloordns/models/domain.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/models/groups.py` & `cloudfloordns-0.1.4/cloudfloordns/models/groups.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/models/record.py` & `cloudfloordns-0.1.4/cloudfloordns/models/record.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/utils/__init__.py` & `cloudfloordns-0.1.4/cloudfloordns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/cloudfloordns/utils/make_async.py` & `cloudfloordns-0.1.4/cloudfloordns/utils/make_async.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.3/pyproject.toml` & `cloudfloordns-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloudfloordns"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "cloudfloordns", from="."}]
 
 # [tool.setuptools.dynamic]
 # version = {attr = "nagra_network_misc_utils.__version__"}
```

### Comparing `cloudfloordns-0.1.3/PKG-INFO` & `cloudfloordns-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudfloordns
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: David Gallay
 Author-email: david.gallay@nagra.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

