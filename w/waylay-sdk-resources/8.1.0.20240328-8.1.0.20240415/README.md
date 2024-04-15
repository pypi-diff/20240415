# Comparing `tmp/waylay-sdk-resources-8.1.0.20240328.tar.gz` & `tmp/waylay_sdk_resources-8.1.0.20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-resources-8.1.0.20240328.tar", last modified: Thu Mar 28 09:44:06 2024, max compression
+gzip compressed data, was "waylay_sdk_resources-8.1.0.20240415.tar", last modified: Mon Apr 15 09:59:09 2024, max compression
```

## Comparing `waylay-sdk-resources-8.1.0.20240328.tar` & `waylay_sdk_resources-8.1.0.20240415.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.611441 waylay-sdk-resources-8.1.0.20240328/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      745 2024-03-28 09:35:37.000000 waylay-sdk-resources-8.1.0.20240328/LICENSE.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4978 2024-03-28 09:44:06.610518 waylay-sdk-resources-8.1.0.20240328/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2819 2024-03-28 09:35:36.000000 waylay-sdk-resources-8.1.0.20240328/README.md
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1768 2024-03-28 09:35:36.000000 waylay-sdk-resources-8.1.0.20240328/pyproject.toml
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-03-28 09:44:06.611556 waylay-sdk-resources-8.1.0.20240328/setup.cfg
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.578718 waylay-sdk-resources-8.1.0.20240328/src/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.578026 waylay-sdk-resources-8.1.0.20240328/src/waylay/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.578173 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.578518 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.599283 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      501 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    13271 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/batch_operations_api.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     6300 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/metadata_events_api.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:35:36.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/py.typed
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    56362 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_api.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    30375 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_constraint_api.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    55935 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_type_api.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     5823 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/version_api.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.600489 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      795 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:35:36.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/py.typed
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1208 2024-03-28 09:36:18.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/service.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 09:44:06.608682 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4978 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      891 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/SOURCES.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/dependency_links.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       73 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/entry_points.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      323 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/requires.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-03-28 09:44:06.000000 waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13271 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/metadata_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56362 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30375 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_constraint_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55935 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_type_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/top_level.txt
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/LICENSE.txt` & `waylay_sdk_resources-8.1.0.20240415/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-resources-8.1.0.20240328/PKG-INFO` & `waylay_sdk_resources-8.1.0.20240415/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources
-Version: 8.1.0.20240328
+Version: 8.1.0.20240415
 Summary: Waylay Resources
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,21 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
+Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-core~=0.2.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -53,53 +54,51 @@
 and provides a context when processing data in the Rule Engine.
 
 You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model, 
 a process that's also called _resource provisioning_.
 
 This Python package is automatically generated based on the 
 Waylay Resources OpenAPI specification (API version: 8.1.0)
+For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/resources.html).
 
-It consists of a plugin for the waylay-sdk package, and contains the Resources api methods.
+It consists of a plugin for the waylay-sdk-core package, and contains the Resources api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-resources-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-resources is included in:
-- ```pip install waylay-sdk[resources]``` to install `waylay-sdk` along with only this service, or
-- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
+- ```pip install waylay-sdk-core[resources]``` to install `waylay-sdk-core` along with only this service, or
+- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
 When the typed models are required, both waylay-sdk-resources and waylay-sdk-resources-types are included in:
-- ```pip install waylay-sdk[resources,resources-types]``` to install `waylay-sdk` along with only this service including the typed models, or
-- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
+- ```pip install waylay-sdk-core[resources,resources-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
+- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
 
 ## Usage
 
-
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk package
+# Import the waylay-client from the waylay-sdk-core package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-resources-types` is installed
-from resources.models.batch_operation_enqueued import BatchOperationEnqueued
-from resources.models.batch_resource_operation import BatchResourceOperation
+from waylay.services.resources.models.version_response import VersionResponse
 try:
-    # Bulk Delete
-    # calls `POST /resources/v1/batch`
-    api_response = await waylay_client.resources.batch_operations.start(
-        # json data: use a generated model or a json-serializable python data structure (dict, list)
-        json = resources.BatchResourceOperation() # BatchResourceOperation | Resource Batch Operation
+    # Get Service Information
+    # calls `GET /resources/v1/`
+    api_response = await waylay_client.resources.about.get(
     )
-    print("The response of resources.batch_operations.start:\n")
+    print("The response of resources.about.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling resources.batch_operations.start: %s\n" % e)
+    print("Exception when calling resources.about.get: %s\n" % e)
 ```
 
 
+For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/README.md` & `waylay_sdk_resources-8.1.0.20240415/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,53 +6,51 @@
 and provides a context when processing data in the Rule Engine.
 
 You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model, 
 a process that's also called _resource provisioning_.
 
 This Python package is automatically generated based on the 
 Waylay Resources OpenAPI specification (API version: 8.1.0)
+For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/resources.html).
 
-It consists of a plugin for the waylay-sdk package, and contains the Resources api methods.
+It consists of a plugin for the waylay-sdk-core package, and contains the Resources api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-resources-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-resources is included in:
-- ```pip install waylay-sdk[resources]``` to install `waylay-sdk` along with only this service, or
-- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
+- ```pip install waylay-sdk-core[resources]``` to install `waylay-sdk-core` along with only this service, or
+- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
 When the typed models are required, both waylay-sdk-resources and waylay-sdk-resources-types are included in:
-- ```pip install waylay-sdk[resources,resources-types]``` to install `waylay-sdk` along with only this service including the typed models, or
-- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
+- ```pip install waylay-sdk-core[resources,resources-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
+- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
 
 ## Usage
 
-
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk package
+# Import the waylay-client from the waylay-sdk-core package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-resources-types` is installed
-from resources.models.batch_operation_enqueued import BatchOperationEnqueued
-from resources.models.batch_resource_operation import BatchResourceOperation
+from waylay.services.resources.models.version_response import VersionResponse
 try:
-    # Bulk Delete
-    # calls `POST /resources/v1/batch`
-    api_response = await waylay_client.resources.batch_operations.start(
-        # json data: use a generated model or a json-serializable python data structure (dict, list)
-        json = resources.BatchResourceOperation() # BatchResourceOperation | Resource Batch Operation
+    # Get Service Information
+    # calls `GET /resources/v1/`
+    api_response = await waylay_client.resources.about.get(
     )
-    print("The response of resources.batch_operations.start:\n")
+    print("The response of resources.about.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling resources.batch_operations.start: %s\n" % e)
+    print("Exception when calling resources.about.get: %s\n" % e)
 ```
 
 
+For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/pyproject.toml` & `waylay_sdk_resources-8.1.0.20240415/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-resources"
-version = "8.1.0.20240328"
+version = "8.1.0.20240415"
 description = "Waylay Resources"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Resources"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-core ~= 0.2.0",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/"
+Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
 Repository = "https://github.com/waylayio/waylay-sdk-resources-py.git"
+"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/resources.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/batch_operations_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/batch_operations_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/metadata_events_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/metadata_events_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
+    AsyncIterator,
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
@@ -25,14 +26,15 @@
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
+from waylay.sdk.api.constants import STREAM_TIMEOUTS
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.resources.models import NdJsonResponseStream
     from waylay.services.resources.queries.metadata_events_api import GetStreamQuery
 
 
@@ -66,75 +68,92 @@
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> NdJsonResponseStream: ...
+    ) -> AsyncIterator[NdJsonResponseStream]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> T: ...
+    ) -> AsyncIterator[T]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> Model: ...
+    ) -> AsyncIterator[Model]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> T: ...
+    ) -> AsyncIterator[T]: ...
 
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
+        stream: bool = True,
+        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> NdJsonResponseStream | T | Response | Model:
+    ) -> (
+        AsyncIterator[NdJsonResponseStream]
+        | AsyncIterator[T]
+        | Response
+        | AsyncIterator[Model]
+    ):
         """Events.
 
         Opens a data stream for all Metadata events for this tenant.
         :param query: URL Query parameters.
         :type query: GetStreamQuery | QueryParamTypes, optional
         :param query['eventFormat'] (dict) <br> query.event_format (Query) : The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)
         :type query['eventFormat']: GetStreamEventFormatParameter
@@ -188,12 +207,14 @@
         return await self.api_client.request(
             method="GET",
             resource_path="/resources/v1/events",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
+            stream=stream,
+            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_constraint_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_constraint_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/resource_type_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_type_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/api/version_api.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/about_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.resources.models import VersionResponse
-    from waylay.services.resources.queries.version_api import GetQuery
+    from waylay.services.resources.queries.about_api import GetQuery
 
 
 try:
     from waylay.services.resources.models import VersionResponse
-    from waylay.services.resources.queries.version_api import GetQuery
+    from waylay.services.resources.queries.about_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         VersionResponse = Model
 
 
 T = TypeVar("T")
 
 
-class VersionApi(WithApiClient):
-    """VersionApi service methods.
+class AboutApi(WithApiClient):
+    """AboutApi service methods.
 
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
-        """Get Version.
+        """Get Service Information.
 
-        Gets the status and version of the service.
+        Get the name and version of the service.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/__init__.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This service manages  [Waylay Resources](/#/features/resources/?id=resource) and related entities.  A _Waylay Resource_ models a real-world device or abstract entity of your IoT solution, and provides a context when processing data in the Rule Engine.  You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model,  a process that's also called _resource provisioning_.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "8.1.0.20240328"
+__version__ = "8.1.0.20240415"
 
 from .service import ResourcesService
 
 PLUGINS = [ResourcesService]
 
 __all__ = [
     "__version__",
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay/services/resources/service/service.py` & `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Resources Service."""
 
 from waylay.sdk import ApiClient, WaylayService
 
+from ..api.about_api import AboutApi
 from ..api.batch_operations_api import BatchOperationsApi
 from ..api.metadata_events_api import MetadataEventsApi
 from ..api.resource_api import ResourceApi
 from ..api.resource_constraint_api import ResourceConstraintApi
 from ..api.resource_type_api import ResourceTypeApi
-from ..api.version_api import VersionApi
 
 
 class ResourcesService(WaylayService):
     """Resources Service Class."""
 
     name = "resources"
     title = "Resources Service"
 
+    about: AboutApi
     batch_operations: BatchOperationsApi
     metadata_events: MetadataEventsApi
     resource: ResourceApi
     resource_constraint: ResourceConstraintApi
     resource_type: ResourceTypeApi
-    version: VersionApi
 
     def __init__(self, api_client: ApiClient):
         """Create the resources service."""
 
         super().__init__(api_client)
+        self.about = AboutApi(api_client)
         self.batch_operations = BatchOperationsApi(api_client)
         self.metadata_events = MetadataEventsApi(api_client)
         self.resource = ResourceApi(api_client)
         self.resource_constraint = ResourceConstraintApi(api_client)
         self.resource_type = ResourceTypeApi(api_client)
-        self.version = VersionApi(api_client)
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/PKG-INFO` & `waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources
-Version: 8.1.0.20240328
+Version: 8.1.0.20240415
 Summary: Waylay Resources
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,21 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
+Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-core~=0.2.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -53,53 +54,51 @@
 and provides a context when processing data in the Rule Engine.
 
 You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model, 
 a process that's also called _resource provisioning_.
 
 This Python package is automatically generated based on the 
 Waylay Resources OpenAPI specification (API version: 8.1.0)
+For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/resources.html).
 
-It consists of a plugin for the waylay-sdk package, and contains the Resources api methods.
+It consists of a plugin for the waylay-sdk-core package, and contains the Resources api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-resources-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-resources is included in:
-- ```pip install waylay-sdk[resources]``` to install `waylay-sdk` along with only this service, or
-- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
+- ```pip install waylay-sdk-core[resources]``` to install `waylay-sdk-core` along with only this service, or
+- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
 When the typed models are required, both waylay-sdk-resources and waylay-sdk-resources-types are included in:
-- ```pip install waylay-sdk[resources,resources-types]``` to install `waylay-sdk` along with only this service including the typed models, or
-- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
+- ```pip install waylay-sdk-core[resources,resources-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
+- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
 
 ## Usage
 
-
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk package
+# Import the waylay-client from the waylay-sdk-core package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-resources-types` is installed
-from resources.models.batch_operation_enqueued import BatchOperationEnqueued
-from resources.models.batch_resource_operation import BatchResourceOperation
+from waylay.services.resources.models.version_response import VersionResponse
 try:
-    # Bulk Delete
-    # calls `POST /resources/v1/batch`
-    api_response = await waylay_client.resources.batch_operations.start(
-        # json data: use a generated model or a json-serializable python data structure (dict, list)
-        json = resources.BatchResourceOperation() # BatchResourceOperation | Resource Batch Operation
+    # Get Service Information
+    # calls `GET /resources/v1/`
+    api_response = await waylay_client.resources.about.get(
     )
-    print("The response of resources.batch_operations.start:\n")
+    print("The response of resources.about.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling resources.batch_operations.start: %s\n" % e)
+    print("Exception when calling resources.about.get: %s\n" % e)
 ```
 
 
+For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay-sdk-resources-8.1.0.20240328/src/waylay_sdk_resources.egg-info/SOURCES.txt` & `waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/resources/api/__init__.py
+src/waylay/services/resources/api/about_api.py
 src/waylay/services/resources/api/batch_operations_api.py
 src/waylay/services/resources/api/metadata_events_api.py
 src/waylay/services/resources/api/py.typed
 src/waylay/services/resources/api/resource_api.py
 src/waylay/services/resources/api/resource_constraint_api.py
 src/waylay/services/resources/api/resource_type_api.py
-src/waylay/services/resources/api/version_api.py
 src/waylay/services/resources/service/__init__.py
 src/waylay/services/resources/service/py.typed
 src/waylay/services/resources/service/service.py
 src/waylay_sdk_resources.egg-info/PKG-INFO
 src/waylay_sdk_resources.egg-info/SOURCES.txt
 src/waylay_sdk_resources.egg-info/dependency_links.txt
 src/waylay_sdk_resources.egg-info/entry_points.txt
```

