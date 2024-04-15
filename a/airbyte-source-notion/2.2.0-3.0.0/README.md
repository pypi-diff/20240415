# Comparing `tmp/airbyte_source_notion-2.2.0.tar.gz` & `tmp/airbyte_source_notion-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_notion-2.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_notion-3.0.0.tar", max compression
```

## Comparing `airbyte_source_notion-2.2.0.tar` & `airbyte_source_notion-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     4501 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/README.md
--rw-r--r--   0        0        0      782 2024-04-10 12:34:33.618347 airbyte_source_notion-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      124 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/__init__.py
--rw-r--r--   0        0        0      230 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/run.py
--rw-r--r--   0        0        0     6701 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/blocks.json
--rw-r--r--   0        0        0     1957 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/comments.json
--rw-r--r--   0        0        0    15580 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/databases.json
--rw-r--r--   0        0        0    10213 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/pages.json
--rw-r--r--   0        0        0      168 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/child.json
--rw-r--r--   0        0        0      280 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/date.json
--rw-r--r--   0        0        0      232 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/emoji.json
--rw-r--r--   0        0        0      764 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/file.json
--rw-r--r--   0        0        0      299 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/heading.json
--rw-r--r--   0        0        0      123 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/icon.json
--rw-r--r--   0        0        0      444 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/options.json
--rw-r--r--   0        0        0      416 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/parent.json
--rw-r--r--   0        0        0     1936 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/rich_text.json
--rw-r--r--   0        0        0      313 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/text_element.json
--rw-r--r--   0        0        0     1401 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/title.json
--rw-r--r--   0        0        0     1726 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/shared/user.json
--rw-r--r--   0        0        0       82 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/schemas/users.json
--rw-r--r--   0        0        0     4550 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/source.py
--rw-r--r--   0        0        0     4671 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/spec.json
--rw-r--r--   0        0        0    17739 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/streams.py
--rw-r--r--   0        0        0     1538 2024-04-10 12:21:37.000000 airbyte_source_notion-2.2.0/source_notion/utils.py
--rw-r--r--   0        0        0     5237 1970-01-01 00:00:00.000000 airbyte_source_notion-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4501 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/README.md
+-rw-r--r--   0        0        0      761 2024-04-15 16:05:56.790950 airbyte_source_notion-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/components.py
+-rw-r--r--   0        0        0    14612 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/run.py
+-rw-r--r--   0        0        0     6701 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/blocks.json
+-rw-r--r--   0        0        0     1957 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/comments.json
+-rw-r--r--   0        0        0    15580 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/databases.json
+-rw-r--r--   0        0        0    10213 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/pages.json
+-rw-r--r--   0        0        0      168 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/child.json
+-rw-r--r--   0        0        0      280 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/date.json
+-rw-r--r--   0        0        0      232 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/emoji.json
+-rw-r--r--   0        0        0      764 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/file.json
+-rw-r--r--   0        0        0      299 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/heading.json
+-rw-r--r--   0        0        0      123 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/icon.json
+-rw-r--r--   0        0        0      444 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/options.json
+-rw-r--r--   0        0        0      416 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/parent.json
+-rw-r--r--   0        0        0     1936 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/rich_text.json
+-rw-r--r--   0        0        0      313 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/text_element.json
+-rw-r--r--   0        0        0     1401 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/title.json
+-rw-r--r--   0        0        0     1726 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/shared/user.json
+-rw-r--r--   0        0        0       82 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/schemas/users.json
+-rw-r--r--   0        0        0     1941 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/source.py
+-rw-r--r--   0        0        0     4638 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/spec.json
+-rw-r--r--   0        0        0    13631 2024-04-15 07:19:58.000000 airbyte_source_notion-3.0.0/source_notion/streams.py
+-rw-r--r--   0        0        0     5203 1970-01-01 00:00:00.000000 airbyte_source_notion-3.0.0/PKG-INFO
```

### Comparing `airbyte_source_notion-2.2.0/README.md` & `airbyte_source_notion-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/pyproject.toml` & `airbyte_source_notion-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.2.0"
+version = "3.0.0"
 name = "airbyte-source-notion"
 description = "Source implementation for Notion."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -19,15 +19,14 @@
 packages = [
     { include = "source_notion" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 airbyte-cdk = "^0"
-pendulum = "==2.1.2"
 
 [tool.poetry.scripts]
 source-notion = "source_notion.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/blocks.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/blocks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/comments.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/databases.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/databases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/pages.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/shared/file.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/shared/file.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/shared/rich_text.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/shared/rich_text.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/shared/title.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/shared/title.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/schemas/shared/user.json` & `airbyte_source_notion-3.0.0/source_notion/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-2.2.0/source_notion/spec.json` & `airbyte_source_notion-3.0.0/source_notion/spec.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'connectionSpecification'": "{delete: ['required']}"}*

```diff
@@ -124,15 +124,12 @@
                 "format": "date-time",
                 "pattern": "^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}.[0-9]{3}Z$",
                 "pattern_descriptor": "YYYY-MM-DDTHH:MM:SS.000Z",
                 "title": "Start Date",
                 "type": "string"
             }
         },
-        "required": [
-            "credentials"
-        ],
         "title": "Notion Source Spec",
         "type": "object"
     },
     "documentationUrl": "https://docs.airbyte.com/integrations/sources/notion"
 }
```

### Comparing `airbyte_source_notion-2.2.0/source_notion/streams.py` & `airbyte_source_notion-3.0.0/source_notion/streams.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from airbyte_cdk.sources import Source
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
 from airbyte_cdk.sources.streams.http.availability_strategy import HttpAvailabilityStrategy
 from airbyte_cdk.sources.streams.http.exceptions import UserDefinedBackoffException
 from requests import HTTPError
 
-from .utils import transform_properties
-
 # maximum block hierarchy recursive request depth
 MAX_BLOCK_DEPTH = 30
 
 
 class NotionAvailabilityStrategy(HttpAvailabilityStrategy):
     """
     Inherit from HttpAvailabilityStrategy with slight modification to 403 error message.
@@ -217,15 +215,15 @@
         records = super().parse_response(response, stream_state=stream_state, **kwargs)
         for record in records:
             record_lmd = record.get(self.cursor_field, "")
             state_lmd = stream_state.get(self.cursor_field, "")
             if isinstance(state_lmd, StateValueWrapper):
                 state_lmd = state_lmd.value
             if (not stream_state or record_lmd >= state_lmd) and record_lmd >= self.start_date:
-                yield from transform_properties(record)
+                yield record
 
     def get_updated_state(
         self,
         current_stream_state: MutableMapping[str, Any],
         latest_record: Mapping[str, Any],
     ) -> Mapping[str, Any]:
         state_value = (current_stream_state or {}).get(self.cursor_field, "")
@@ -234,56 +232,14 @@
 
         record_time = latest_record.get(self.cursor_field, self.start_date)
         state_value.max_cursor_time = max(state_value.max_cursor_time, record_time)
 
         return {self.cursor_field: state_value}
 
 
-class Users(NotionStream):
-    """
-    Docs: https://developers.notion.com/reference/get-users
-    """
-
-    def path(self, **kwargs) -> str:
-        return "users"
-
-    def request_params(self, next_page_token: Mapping[str, Any] = None, **kwargs) -> MutableMapping[str, Any]:
-        params = {"page_size": self.page_size}
-        if next_page_token:
-            params["start_cursor"] = next_page_token["next_cursor"]
-        return params
-
-    def transform(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
-        owner = record.get("bot", {}).get("owner")
-        if owner:
-            owner_type = owner.get("type")
-            owner_info = owner.get(owner_type)
-            if owner_type and owner_info:
-                record["bot"]["owner"]["info"] = owner_info
-                del record["bot"]["owner"][owner_type]
-        return record
-
-    def parse_response(self, response: requests.Response, **kwargs) -> Iterable[Mapping]:
-        # sometimes notion api returns response without results object
-        data = response.json().get("results", [])
-        for record in data:
-            yield self.transform(record)
-
-
-class Databases(IncrementalNotionStream):
-    """
-    Docs: https://developers.notion.com/reference/post-search
-    """
-
-    state_checkpoint_interval = 100
-
-    def __init__(self, **kwargs):
-        super().__init__(obj_type="database", **kwargs)
-
-
 class Pages(IncrementalNotionStream):
     """
     Docs: https://developers.notion.com/reference/post-search
     """
 
     state_checkpoint_interval = 100
 
@@ -386,68 +342,7 @@
                 self.logger.error(
                     f"Stream {self.name}: `ai_block` type is not supported, skipping. See https://developers.notion.com/reference/block for available block type."
                 )
                 return False
             else:
                 return super().should_retry(response)
         return super().should_retry(response)
-
-
-class Comments(HttpSubStream, IncrementalNotionStream):
-    """
-    Comments Object Docs: https://developers.notion.com/reference/comment-object
-    Comments Endpoint Docs: https://developers.notion.com/reference/retrieve-a-comment
-    """
-
-    http_method = "GET"
-    # We can use the "last edited time" of the parent Page as the cursor field,
-    # since we cannot guarantee the order of comments between pages.
-    cursor_field = "page_last_edited_time"
-
-    def path(self, **kwargs) -> str:
-        return "comments"
-
-    def request_params(
-        self, next_page_token: Mapping[str, Any] = None, stream_slice: Mapping[str, Any] = None, **kwargs
-    ) -> MutableMapping[str, Any]:
-        block_id = stream_slice.get("block_id")
-        params = {"block_id": block_id, "page_size": self.page_size}
-
-        if next_page_token:
-            params["start_cursor"] = next_page_token["next_cursor"]
-
-        return params
-
-    def parse_response(
-        self, response: requests.Response, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, **kwargs
-    ) -> Iterable[Mapping]:
-
-        # Get the parent's "last edited time" to compare against state
-        page_last_edited_time = stream_slice.get("page_last_edited_time", "")
-        records = response.json().get("results", [])
-
-        for record in records:
-            record["page_last_edited_time"] = page_last_edited_time
-            state_last_edited_time = stream_state.get(self.cursor_field, "")
-
-            if isinstance(state_last_edited_time, StateValueWrapper):
-                state_last_edited_time = state_last_edited_time.value
-
-            if not stream_state or page_last_edited_time >= state_last_edited_time:
-                yield from transform_properties(record)
-
-    def read_records(self, **kwargs) -> Iterable[Mapping[str, Any]]:
-
-        yield from IncrementalNotionStream.read_records(self, **kwargs)
-
-    def stream_slices(
-        self, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, **kwargs
-    ) -> Iterable[Optional[Mapping[str, Any]]]:
-
-        # Gather parent stream records in full
-        parent_records = self.parent.read_records(sync_mode=SyncMode.full_refresh, cursor_field=self.parent.cursor_field)
-
-        # The parent stream is the Pages stream, but we have to pass its id to the request_params as "block_id"
-        # because pages are also blocks in the Notion API.
-        # We also grab the last_edited_time from the parent record to use as the cursor field.
-        for record in parent_records:
-            yield {"block_id": record["id"], "page_last_edited_time": record["last_edited_time"]}
```

### Comparing `airbyte_source_notion-2.2.0/PKG-INFO` & `airbyte_source_notion-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-notion
-Version: 2.2.0
+Version: 3.0.0
 Summary: Source implementation for Notion.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: airbyte-cdk (>=0,<1)
-Requires-Dist: pendulum (==2.1.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/notion
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Notion source connector
```

