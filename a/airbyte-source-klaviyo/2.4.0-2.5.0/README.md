# Comparing `tmp/airbyte_source_klaviyo-2.4.0.tar.gz` & `tmp/airbyte_source_klaviyo-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_klaviyo-2.4.0.tar", max compression
+gzip compressed data, was "airbyte_source_klaviyo-2.5.0.tar", max compression
```

## Comparing `airbyte_source_klaviyo-2.4.0.tar` & `airbyte_source_klaviyo-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     4514 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/README.md
--rw-r--r--   0        0        0      746 2024-04-11 15:18:13.871414 airbyte_source_klaviyo-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/__init__.py
--rw-r--r--   0        0        0      975 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/availability_strategy.py
--rw-r--r--   0        0        0      196 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/exceptions.py
--rw-r--r--   0        0        0      233 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/run.py
--rw-r--r--   0        0        0     4491 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/campaigns.json
--rw-r--r--   0        0        0      935 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/email_templates.json
--rw-r--r--   0        0        0     2136 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/events.json
--rw-r--r--   0        0        0     2262 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/flows.json
--rw-r--r--   0        0        0     3931 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/global_exclusions.json
--rw-r--r--   0        0        0     1839 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/lists.json
--rw-r--r--   0        0        0      787 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/metrics.json
--rw-r--r--   0        0        0     3931 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/profiles.json
--rw-r--r--   0        0        0     2892 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/shared/subscriptions.json
--rw-r--r--   0        0        0     2851 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/source.py
--rw-r--r--   0        0        0     1114 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/spec.json
--rw-r--r--   0        0        0    14710 2024-04-11 12:05:25.000000 airbyte_source_klaviyo-2.4.0/source_klaviyo/streams.py
--rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/README.md
+-rw-r--r--   0        0        0      746 2024-04-15 16:12:34.687305 airbyte_source_klaviyo-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/availability_strategy.py
+-rw-r--r--   0        0        0      865 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/components/datetime_based_cursor.py
+-rw-r--r--   0        0        0      196 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/exceptions.py
+-rw-r--r--   0        0        0     5924 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/run.py
+-rw-r--r--   0        0        0     4491 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/campaigns.json
+-rw-r--r--   0        0        0      935 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/email_templates.json
+-rw-r--r--   0        0        0     2136 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/events.json
+-rw-r--r--   0        0        0     2262 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/flows.json
+-rw-r--r--   0        0        0     3931 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/global_exclusions.json
+-rw-r--r--   0        0        0     1839 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/lists.json
+-rw-r--r--   0        0        0      787 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/metrics.json
+-rw-r--r--   0        0        0     3931 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/profiles.json
+-rw-r--r--   0        0        0     2892 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/shared/subscriptions.json
+-rw-r--r--   0        0        0     1020 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/source.py
+-rw-r--r--   0        0        0     1114 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/spec.json
+-rw-r--r--   0        0        0    10876 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/streams.py
+-rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.5.0/PKG-INFO
```

### Comparing `airbyte_source_klaviyo-2.4.0/README.md` & `airbyte_source_klaviyo-2.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-klaviyo spec
 poetry run source-klaviyo check --config secrets/config.json
 poetry run source-klaviyo discover --config secrets/config.json
-poetry run source-klaviyo read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-klaviyo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_klaviyo-2.4.0/pyproject.toml` & `airbyte_source_klaviyo-2.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.4.0"
+version = "2.5.0"
 name = "airbyte-source-klaviyo"
 description = "Source implementation for Klaviyo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/availability_strategy.py` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/campaigns.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/email_templates.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/email_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/events.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/flows.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/flows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/global_exclusions.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/global_exclusions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/lists.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/metrics.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/profiles.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/profiles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/schemas/shared/subscriptions.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/shared/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/source_klaviyo/spec.json` & `airbyte_source_klaviyo-2.5.0/source_klaviyo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.4.0/PKG-INFO` & `airbyte_source_klaviyo-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-klaviyo
-Version: 2.4.0
+Version: 2.5.0
 Summary: Source implementation for Klaviyo.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +45,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-klaviyo spec
 poetry run source-klaviyo check --config secrets/config.json
 poetry run source-klaviyo discover --config secrets/config.json
-poetry run source-klaviyo read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-klaviyo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

