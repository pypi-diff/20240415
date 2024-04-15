# Comparing `tmp/airbyte_source_linkedin_ads-0.8.0.tar.gz` & `tmp/airbyte_source_linkedin_ads-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_linkedin_ads-0.8.0.tar", max compression
+gzip compressed data, was "airbyte_source_linkedin_ads-1.0.0.tar", max compression
```

## Comparing `airbyte_source_linkedin_ads-0.8.0.tar` & `airbyte_source_linkedin_ads-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4604 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/README.md
--rw-r--r--   0        0        0      776 2024-03-21 02:08:00.044560 airbyte_source_linkedin_ads-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1179 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/__init__.py
--rw-r--r--   0        0        0    13824 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/analytics_streams.py
--rw-r--r--   0        0        0      246 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/run.py
--rw-r--r--   0        0        0      512 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/account_users.json
--rw-r--r--   0        0        0     1405 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/accounts.json
--rw-r--r--   0        0        0     7046 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/ad_analytics.json
--rw-r--r--   0        0        0     1399 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/campaign_groups.json
--rw-r--r--   0        0        0     4731 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/campaigns.json
--rw-r--r--   0        0        0     1511 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/conversions.json
--rw-r--r--   0        0        0     1404 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/creatives.json
--rw-r--r--   0        0        0     5505 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/source.py
--rw-r--r--   0        0        0     6880 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/spec.json
--rw-r--r--   0        0        0    16943 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/streams.py
--rw-r--r--   0        0        0    11445 2024-03-21 01:47:20.545994 airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/utils.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4604 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/README.md
+-rw-r--r--   0        0        0      776 2024-04-15 16:56:21.758140 airbyte_source_linkedin_ads-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1179 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/__init__.py
+-rw-r--r--   0        0        0    14052 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/analytics_streams.py
+-rw-r--r--   0        0        0      246 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/run.py
+-rw-r--r--   0        0        0      512 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/account_users.json
+-rw-r--r--   0        0        0     1405 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/accounts.json
+-rw-r--r--   0        0        0     7041 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/ad_analytics.json
+-rw-r--r--   0        0        0     1399 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/campaign_groups.json
+-rw-r--r--   0        0        0     4731 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/campaigns.json
+-rw-r--r--   0        0        0     1511 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/conversions.json
+-rw-r--r--   0        0        0     1404 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/creatives.json
+-rw-r--r--   0        0        0     5505 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/source.py
+-rw-r--r--   0        0        0     6880 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/spec.json
+-rw-r--r--   0        0        0    16943 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/streams.py
+-rw-r--r--   0        0        0    11445 2024-04-15 16:02:34.000000 airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/utils.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-1.0.0/PKG-INFO
```

### Comparing `airbyte_source_linkedin_ads-0.8.0/README.md` & `airbyte_source_linkedin_ads-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/pyproject.toml` & `airbyte_source_linkedin_ads-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.8.0"
+version = "1.0.0"
 name = "airbyte-source-linkedin-ads"
 description = "Source implementation for Linkedin Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/__init__.py` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/analytics_streams.py` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/analytics_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,23 @@
     """
     AdAnalytics Streams more info:
     https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/ads-reporting?tabs=curl&view=li-lms-2023-05#analytics-finder
     """
 
     endpoint = "adAnalytics"
     # For Analytics streams, the primary_key is the entity of the pivot [Campaign URN, Creative URN, etc.] + `end_date`
-    primary_key = ["pivotValue", "end_date"]
+    primary_key = ["pivotValues", "end_date"]
     cursor_field = "end_date"
     records_limit = 15000
-    FIELDS_CHUNK_SIZE = 19
+    FIELDS_CHUNK_SIZE = 18
 
     def get_json_schema(self) -> Mapping[str, Any]:
-        return ResourceSchemaLoader(package_name_from_class(self.__class__)).get_schema("ad_analytics")
+        schema = ResourceSchemaLoader(package_name_from_class(self.__class__)).get_schema("ad_analytics")
+        schema["properties"].update({self.search_param_value: {"type": ["null", "string"]}})
+        return schema
 
     def __init__(self, name: str = None, pivot_by: str = None, time_granularity: str = None, **kwargs):
         self.user_stream_name = name
         if pivot_by:
             self.pivot_by = pivot_by
         if time_granularity:
             self.time_granularity = time_granularity
@@ -282,31 +284,33 @@
         """
         # Make chunks
         chunks = list((fields[f : f + fields_chunk_size] for f in range(0, len(fields), fields_chunk_size)))
         # Make sure base_fields are within the chunks
         for chunk in chunks:
             if "dateRange" not in chunk:
                 chunk.append("dateRange")
+            if "pivotValues" not in chunk:
+                chunk.append("pivotValues")
         yield from chunks
 
     def read_records(
         self, stream_state: Mapping[str, Any] = None, stream_slice: Optional[Mapping[str, Any]] = None, **kwargs
     ) -> Iterable[Mapping[str, Any]]:
         merged_records = defaultdict(dict)
         for field_slice in stream_slice:
             for rec in super().read_records(stream_slice=field_slice, **kwargs):
-                merged_records[rec[self.cursor_field]].update(rec)
+                merged_records[f"{rec[self.cursor_field]}-{rec['pivotValues']}"].update(rec)
         yield from merged_records.values()
 
     def parse_response(self, response: requests.Response, **kwargs) -> Iterable[Mapping]:
         """
         We need to get out the nested complex data structures for further normalization, so the transform_data method is applied.
         """
         for rec in transform_data(response.json().get("elements")):
-            yield rec | {"pivotValue": f"urn:li:{self.search_param_value}:{self.get_primary_key_from_slice(kwargs.get('stream_slice'))}"}
+            yield rec | {self.search_param_value: self.get_primary_key_from_slice(kwargs.get("stream_slice")), "pivot": self.pivot_by}
 
 
 class AdCampaignAnalytics(LinkedInAdsAnalyticsStream):
     """
     Campaign Analytics stream.
     """
```

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/account_users.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/accounts.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/ad_analytics.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/ad_analytics.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979591836734694%*

 * *Differences: {"'properties'": "{'pivot': OrderedDict([('type', ['null', 'string'])]), delete: ['pivotValue']}"}*

```diff
@@ -203,15 +203,15 @@
         },
         "otherEngagements": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "pivotValue": {
+        "pivot": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "pivotValues": {
             "items": {
```

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/campaign_groups.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/campaigns.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/conversions.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/conversions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/schemas/creatives.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/source.py` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/spec.json` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/streams.py` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/source_linkedin_ads/utils.py` & `airbyte_source_linkedin_ads-1.0.0/source_linkedin_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-0.8.0/PKG-INFO` & `airbyte_source_linkedin_ads-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-linkedin-ads
-Version: 0.8.0
+Version: 1.0.0
 Summary: Source implementation for Linkedin Ads.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

