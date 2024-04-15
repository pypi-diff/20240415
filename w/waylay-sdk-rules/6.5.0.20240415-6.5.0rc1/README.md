# Comparing `tmp/waylay_sdk_rules-6.5.0.20240415.tar.gz` & `tmp/waylay-sdk-rules-6.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_rules-6.5.0.20240415.tar", last modified: Mon Apr 15 08:15:05 2024, max compression
+gzip compressed data, was "waylay-sdk-rules-6.5.0rc1.tar", last modified: Wed Mar 27 15:35:55 2024, max compression
```

## Comparing `waylay_sdk_rules-6.5.0.20240415.tar` & `waylay-sdk-rules-6.5.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.519546 waylay_sdk_rules-6.5.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 08:15:05.519546 waylay_sdk_rules-6.5.0.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:15:05.519546 waylay_sdk_rules-6.5.0.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.511546 waylay_sdk_rules-6.5.0.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.511546 waylay_sdk_rules-6.5.0.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.511546 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.511546 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.515546 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36569 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/plugs_execution_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/push_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/task_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/tasks_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/template_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45622 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/templates_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.515546 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/service/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-15 08:14:58.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:05.515546 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:15:05.000000 waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.220704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36569 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/plugs_execution_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/push_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/task_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/template_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45622 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.220704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/top_level.txt
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/LICENSE.txt` & `waylay-sdk-rules-6.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/PKG-INFO` & `waylay-sdk-rules-6.5.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules
-Version: 6.5.0.20240415
+Version: 6.5.0rc1
 Summary: Waylay rules engine
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-rules==6.5.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,53 @@
 Requires-Dist: waylay-sdk-rules-types; extra == "types"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/README.md` & `waylay-sdk-rules-6.5.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/pyproject.toml` & `waylay-sdk-rules-6.5.0rc1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-rules"
-version = "6.5.0.20240415"
+version = "6.5.0rc1"
 description = "Waylay rules engine"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay rules engine"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-rules == 6.5.0rc1",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-rules-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/rules.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/__init__.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Waylay rules engine: apis."""
 
 # import apis into api package
-from .about_api import AboutApi
 from .plugs_execution_api import PlugsExecutionApi
 from .push_data_api import PushDataApi
 from .task_nodes_api import TaskNodesApi
 from .tasks_api import TasksApi
 from .tasks_batch_operations_api import TasksBatchOperationsApi
 from .template_runs_api import TemplateRunsApi
 from .templates_api import TemplatesApi
+from .version_api import VersionApi
 
 __all__ = [
-    "AboutApi",
     "PlugsExecutionApi",
     "PushDataApi",
     "TaskNodesApi",
     "TasksApi",
     "TasksBatchOperationsApi",
     "TemplateRunsApi",
     "TemplatesApi",
+    "VersionApi",
 ]
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/about_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/version_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import VersionResponse
-    from waylay.services.rules.queries.about_api import GetQuery
+    from waylay.services.rules.queries.version_api import GetQuery
 
 
 try:
     from waylay.services.rules.models import VersionResponse
-    from waylay.services.rules.queries.about_api import GetQuery
+    from waylay.services.rules.queries.version_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         VersionResponse = Model
 
 
 T = TypeVar("T")
 
 
-class AboutApi(WithApiClient):
-    """AboutApi service methods.
+class VersionApi(WithApiClient):
+    """VersionApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -127,17 +127,17 @@
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse | T | Response | Model:
-        """Get Service Information.
+        """Get Version.
 
-        Get the name and version of the service.
+        Get the status and version of the service.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/plugs_execution_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/plugs_execution_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/push_data_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/push_data_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/task_nodes_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/task_nodes_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/tasks_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/tasks_batch_operations_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_batch_operations_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/template_runs_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/template_runs_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
-    AsyncIterator,
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
@@ -31,15 +30,14 @@
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
-from waylay.sdk.api.constants import STREAM_TIMEOUTS
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import (
         ErrorResponse,
         ErrorWithDetailsResponse,
         TemplateRunInvocation,
@@ -98,92 +96,75 @@
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[TemplateRunInvocation]: ...
+    ) -> TemplateRunInvocation: ...
 
     @overload
     async def run_graph(
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def run_graph(
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def run_graph(
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def run_graph(
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def run_graph(
         self,
         *,
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[TemplateRunInvocation]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> TemplateRunInvocation | T | Response | Model:
         """Run Graph Or Bayesian Network.
 
         Run a graph or Bayesian Network. If `data` is specified, template will be run as reactive template. If `data` is not specified, template will be run as a one-time template (1 tick)
         :param query: URL Query parameters.
         :type query: RunGraphQuery | QueryParamTypes, optional
         :param query['logLevel'] (dict) <br> query.log_level (Query) : sets the log level for filtering out logs to requested log level or higher from the template run output. Value `NONE` will disable all logs. If not specified all logs will be returned.
         :type query['logLevel']: RunTemplateLogLevelParameter
@@ -241,16 +222,14 @@
         return await self.api_client.request(
             method="POST",
             resource_path="/rules/v1/templates/run",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
-            stream=stream,
-            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
@@ -259,97 +238,80 @@
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[TemplateRunInvocation]: ...
+    ) -> TemplateRunInvocation: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[TemplateRunInvocation]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> TemplateRunInvocation | T | Response | Model:
         """Run Template.
 
         Run a template. If `data` is specified, template will be run as reactive template. If `data` is not specified, template will be run as a one-time template (1 tick)
         :param name: Unique Template identifier (required)
         :type name: str
         :param query: URL Query parameters.
         :type query: RunQuery | QueryParamTypes, optional
@@ -412,14 +374,12 @@
         return await self.api_client.request(
             method="POST",
             resource_path="/rules/v1/templates/{name}/run",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
-            stream=stream,
-            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/api/templates_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay/services/rules/service/service.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Rules Service."""
 
 from waylay.sdk import ApiClient, WaylayService
 
-from ..api.about_api import AboutApi
 from ..api.plugs_execution_api import PlugsExecutionApi
 from ..api.push_data_api import PushDataApi
 from ..api.task_nodes_api import TaskNodesApi
 from ..api.tasks_api import TasksApi
 from ..api.tasks_batch_operations_api import TasksBatchOperationsApi
 from ..api.template_runs_api import TemplateRunsApi
 from ..api.templates_api import TemplatesApi
+from ..api.version_api import VersionApi
 
 
 class RulesService(WaylayService):
     """Rules Service Class."""
 
     name = "rules"
     title = "Rules Service"
 
-    about: AboutApi
     plugs_execution: PlugsExecutionApi
     push_data: PushDataApi
     task_nodes: TaskNodesApi
     tasks: TasksApi
     tasks_batch_operations: TasksBatchOperationsApi
     template_runs: TemplateRunsApi
     templates: TemplatesApi
+    version: VersionApi
 
     def __init__(self, api_client: ApiClient):
         """Create the rules service."""
 
         super().__init__(api_client)
-        self.about = AboutApi(api_client)
         self.plugs_execution = PlugsExecutionApi(api_client)
         self.push_data = PushDataApi(api_client)
         self.task_nodes = TaskNodesApi(api_client)
         self.tasks = TasksApi(api_client)
         self.tasks_batch_operations = TasksBatchOperationsApi(api_client)
         self.template_runs = TemplateRunsApi(api_client)
         self.templates = TemplatesApi(api_client)
+        self.version = VersionApi(api_client)
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/PKG-INFO` & `waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules
-Version: 6.5.0.20240415
+Version: 6.5.0rc1
 Summary: Waylay rules engine
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-rules==6.5.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,53 @@
 Requires-Dist: waylay-sdk-rules-types; extra == "types"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240415/src/waylay_sdk_rules.egg-info/SOURCES.txt` & `waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/rules/api/__init__.py
-src/waylay/services/rules/api/about_api.py
 src/waylay/services/rules/api/plugs_execution_api.py
 src/waylay/services/rules/api/push_data_api.py
 src/waylay/services/rules/api/py.typed
 src/waylay/services/rules/api/task_nodes_api.py
 src/waylay/services/rules/api/tasks_api.py
 src/waylay/services/rules/api/tasks_batch_operations_api.py
 src/waylay/services/rules/api/template_runs_api.py
 src/waylay/services/rules/api/templates_api.py
+src/waylay/services/rules/api/version_api.py
 src/waylay/services/rules/service/__init__.py
 src/waylay/services/rules/service/py.typed
 src/waylay/services/rules/service/service.py
 src/waylay_sdk_rules.egg-info/PKG-INFO
 src/waylay_sdk_rules.egg-info/SOURCES.txt
 src/waylay_sdk_rules.egg-info/dependency_links.txt
 src/waylay_sdk_rules.egg-info/entry_points.txt
```

