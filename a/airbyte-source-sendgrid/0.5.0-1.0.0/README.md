# Comparing `tmp/airbyte_source_sendgrid-0.5.0.tar.gz` & `tmp/airbyte_source_sendgrid-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_sendgrid-0.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_sendgrid-1.0.0.tar", max compression
```

## Comparing `airbyte_source_sendgrid-0.5.0.tar` & `airbyte_source_sendgrid-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,10 @@
--rw-r--r--   0        0        0     4532 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/README.md
--rw-r--r--   0        0        0      770 2024-03-26 21:02:51.281133 airbyte_source_sendgrid-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       65 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/__init__.py
--rw-r--r--   0        0        0     7542 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/manifest.yaml
--rw-r--r--   0        0        0      236 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/run.py
--rw-r--r--   0        0        0      286 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/blocks.json
--rw-r--r--   0        0        0      286 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/bounces.json
--rw-r--r--   0        0        0      461 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/campaigns.json
--rw-r--r--   0        0        0     1362 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/contacts.json
--rw-r--r--   0        0        0      194 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/global_suppressions.json
--rw-r--r--   0        0        0      240 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/invalid_emails.json
--rw-r--r--   0        0        0      376 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/lists.json
--rw-r--r--   0        0        0      676 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/segments.json
--rw-r--r--   0        0        0     1156 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/single_sends.json
--rw-r--r--   0        0        0      236 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/spam_reports.json
--rw-r--r--   0        0        0     1079 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/stats_automations.json
--rw-r--r--   0        0        0      296 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/suppression_group_members.json
--rw-r--r--   0        0        0      343 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/suppression_groups.json
--rw-r--r--   0        0        0      397 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/templates.json
--rw-r--r--   0        0        0      494 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/unsubscribe_groups.json
--rw-r--r--   0        0        0     2572 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/source.py
--rw-r--r--   0        0        0      986 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/spec.json
--rw-r--r--   0        0        0    16396 2024-03-26 14:44:10.000000 airbyte_source_sendgrid-0.5.0/source_sendgrid/streams.py
--rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 airbyte_source_sendgrid-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4537 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/README.md
+-rw-r--r--   0        0        0      770 2024-04-15 16:09:45.408602 airbyte_source_sendgrid-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/__init__.py
+-rw-r--r--   0        0        0     3498 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/config_migrations.py
+-rw-r--r--   0        0        0    25729 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/manifest.yaml
+-rw-r--r--   0        0        0      362 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/run.py
+-rw-r--r--   0        0        0     1362 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/schemas/contacts.json
+-rw-r--r--   0        0        0      998 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/source.py
+-rw-r--r--   0        0        0     8694 2024-04-15 06:49:50.000000 airbyte_source_sendgrid-1.0.0/source_sendgrid/streams.py
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 airbyte_source_sendgrid-1.0.0/PKG-INFO
```

### Comparing `airbyte_source_sendgrid-0.5.0/README.md` & `airbyte_source_sendgrid-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-sendgrid spec
 poetry run source-sendgrid check --config secrets/config.json
 poetry run source-sendgrid discover --config secrets/config.json
-poetry run source-sendgrid read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-sendgrid read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_sendgrid-0.5.0/pyproject.toml` & `airbyte_source_sendgrid-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.0"
+version = "1.0.0"
 name = "airbyte-source-sendgrid"
 description = "Source implementation for Sendgrid."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_sendgrid-0.5.0/source_sendgrid/schemas/contacts.json` & `airbyte_source_sendgrid-1.0.0/source_sendgrid/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_sendgrid-0.5.0/PKG-INFO` & `airbyte_source_sendgrid-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-sendgrid
-Version: 0.5.0
+Version: 1.0.0
 Summary: Source implementation for Sendgrid.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-sendgrid spec
 poetry run source-sendgrid check --config secrets/config.json
 poetry run source-sendgrid discover --config secrets/config.json
-poetry run source-sendgrid read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-sendgrid read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

