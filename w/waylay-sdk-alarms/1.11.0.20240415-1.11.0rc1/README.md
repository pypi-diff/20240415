# Comparing `tmp/waylay_sdk_alarms-1.11.0.20240415.tar.gz` & `tmp/waylay-sdk-alarms-1.11.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_alarms-1.11.0.20240415.tar", last modified: Mon Apr 15 08:23:24 2024, max compression
+gzip compressed data, was "waylay-sdk-alarms-1.11.0rc1.tar", last modified: Wed Mar 27 16:12:59 2024, max compression
```

## Comparing `waylay_sdk_alarms-1.11.0.20240415.tar` & `waylay-sdk-alarms-1.11.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.254460 waylay_sdk_alarms-1.11.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-15 08:23:24.254460 waylay_sdk_alarms-1.11.0.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:23:24.254460 waylay_sdk_alarms-1.11.0.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.246460 waylay_sdk_alarms-1.11.0.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.246460 waylay_sdk_alarms-1.11.0.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.246460 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.246460 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.250460 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarm_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32030 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarms_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.250460 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/service/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 08:23:08.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:24.250460 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:23:24.000000 waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.907630 waylay-sdk-alarms-1.11.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:12:59.907630 waylay-sdk-alarms-1.11.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarm_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32030 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/top_level.txt
```

### Comparing `waylay_sdk_alarms-1.11.0.20240415/LICENSE.txt` & `waylay-sdk-alarms-1.11.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms-1.11.0.20240415/PKG-INFO` & `waylay-sdk-alarms-1.11.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms
-Version: 1.11.0.20240415
+Version: 1.11.0rc1
 Summary: Waylay Alarms
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
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-alarms==1.11.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,55 @@
 Requires-Dist: waylay-sdk-alarms-types; extra == "types"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240415/README.md` & `waylay-sdk-alarms-1.11.0rc1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240415/pyproject.toml` & `waylay-sdk-alarms-1.11.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-alarms"
-version = "1.11.0.20240415"
+version = "1.11.0rc1"
 description = "Waylay Alarms"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Alarms"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-alarms == 1.11.0rc1",
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
 Repository = "https://github.com/waylayio/waylay-sdk-alarms-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/alarms.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/about_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/version_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.alarms.models import VersionResponse
-    from waylay.services.alarms.queries.about_api import GetQuery
+    from waylay.services.alarms.queries.version_api import GetQuery
 
 
 try:
     from waylay.services.alarms.models import VersionResponse
-    from waylay.services.alarms.queries.about_api import GetQuery
+    from waylay.services.alarms.queries.version_api import GetQuery
 
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
+        """Version.
 
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

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarm_events_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarm_events_api.py`

 * *Files 10% similar despite different names*

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
@@ -26,15 +25,14 @@
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
     from waylay.services.alarms.models import NdJsonResponseStream
     from waylay.services.alarms.queries.alarm_events_api import GetQuery
 
 
@@ -68,92 +66,75 @@
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[NdJsonResponseStream]: ...
+    ) -> NdJsonResponseStream: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
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
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
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
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[NdJsonResponseStream]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> NdJsonResponseStream | T | Response | Model:
         """Alarm Events.
 
         Opens a data stream for all Alarm Events for this tenant.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param query['eventFormat'] (dict) <br> query.event_format (Query) : The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)
         :type query['eventFormat']: GetEventstreamEventFormatParameter
@@ -207,14 +188,12 @@
         return await self.api_client.request(
             method="GET",
             resource_path="/alarms/v1/events",
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

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarms_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay/services/alarms/api/alarms_batch_operations_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_batch_operations_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/PKG-INFO` & `waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms
-Version: 1.11.0.20240415
+Version: 1.11.0rc1
 Summary: Waylay Alarms
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
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-alarms==1.11.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,55 @@
 Requires-Dist: waylay-sdk-alarms-types; extra == "types"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240415/src/waylay_sdk_alarms.egg-info/SOURCES.txt` & `waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/alarms/api/__init__.py
-src/waylay/services/alarms/api/about_api.py
 src/waylay/services/alarms/api/alarm_events_api.py
 src/waylay/services/alarms/api/alarms_api.py
 src/waylay/services/alarms/api/alarms_batch_operations_api.py
 src/waylay/services/alarms/api/py.typed
+src/waylay/services/alarms/api/version_api.py
 src/waylay/services/alarms/service/__init__.py
 src/waylay/services/alarms/service/py.typed
 src/waylay/services/alarms/service/service.py
 src/waylay_sdk_alarms.egg-info/PKG-INFO
 src/waylay_sdk_alarms.egg-info/SOURCES.txt
 src/waylay_sdk_alarms.egg-info/dependency_links.txt
 src/waylay_sdk_alarms.egg-info/entry_points.txt
```

