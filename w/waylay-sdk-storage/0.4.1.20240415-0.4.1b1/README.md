# Comparing `tmp/waylay_sdk_storage-0.4.1.20240415.tar.gz` & `tmp/waylay-sdk-storage-0.4.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage-0.4.1.20240415.tar", last modified: Mon Apr 15 08:21:10 2024, max compression
+gzip compressed data, was "waylay-sdk-storage-0.4.1b1.tar", last modified: Thu Mar 28 13:38:29 2024, max compression
```

## Comparing `waylay_sdk_storage-0.4.1.20240415.tar` & `waylay-sdk-storage-0.4.1b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.028447 waylay_sdk_storage-0.4.1.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-15 08:21:10.028447 waylay_sdk_storage-0.4.1.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:21:10.028447 waylay_sdk_storage-0.4.1.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.020447 waylay_sdk_storage-0.4.1.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.020447 waylay_sdk_storage-0.4.1.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.020447 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.020447 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.024447 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26534 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.024447 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/service/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 08:21:00.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:10.024447 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:21:10.000000 waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26534 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage-0.4.1.20240415/LICENSE.txt` & `waylay-sdk-storage-0.4.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240415/PKG-INFO` & `waylay-sdk-storage-0.4.1b1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.1.20240415
+Version: 0.4.1b1
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -48,58 +47,50 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Storage api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Storage api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-storage-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
-from waylay.services.storage.models.tenant_status_report import TenantStatusReport
 try:
-    # Status
-    # calls `GET /storage/v1/status`
-    api_response = await waylay_client.storage.about.status(
-        # query parameters:
-        query = {
-            'include_buckets': True
-            'include_queues': True
-            'include_disk_usage': False
-        },
+    # Version
+    # calls `GET /storage/v1/`
+    api_response = await waylay_client.storage.about.version(
     )
-    print("The response of storage.about.status:\n")
+    print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling storage.about.status: %s\n" % e)
+    print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage-0.4.1.20240415/pyproject.toml` & `waylay-sdk-storage-0.4.1b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage"
-version = "0.4.1.20240415"
+version = "0.4.1b1"
 description = "Waylay Storage"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
+    "waylay-sdk ~= 0.0.4rc5",
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
 Repository = "https://github.com/waylayio/waylay-sdk-storage-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/storage.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/about_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/about_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,121 +29,129 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.storage.models import HTTPValidationError, TenantStatusReport
-    from waylay.services.storage.queries.about_api import GetQuery, StatusQuery
+    from waylay.services.storage.queries.about_api import StatusQuery, VersionQuery
 
 
 try:
     from waylay.services.storage.models import HTTPValidationError, TenantStatusReport
-    from waylay.services.storage.queries.about_api import GetQuery, StatusQuery
+    from waylay.services.storage.queries.about_api import StatusQuery, VersionQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
-        GetQuery = dict
-
         StatusQuery = dict
         TenantStatusReport = Model
 
         HTTPValidationError = Model
 
+        VersionQuery = dict
+
 
 T = TypeVar("T")
 
 
 class AboutApi(WithApiClient):
     """AboutApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     @overload
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> str: ...
+    ) -> TenantStatusReport: ...
 
     @overload
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def get(
+    async def status(
         self,
         *,
-        query: GetQuery | QueryParamTypes | None = None,
+        query: StatusQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> str | T | Response | Model:
-        """Version.
+    ) -> TenantStatusReport | T | Response | Model:
+        """Status.
 
-        Get the application version.
+        Validate consistency of buckets and notification queues for this tenant.
         :param query: URL Query parameters.
-        :type query: GetQuery | QueryParamTypes, optional
+        :type query: StatusQuery | QueryParamTypes, optional
+        :param query['store'] (dict) <br> query.store (Query) :
+        :type query['store']: str
+        :param query['include_buckets'] (dict) <br> query.include_buckets (Query) :
+        :type query['include_buckets']: bool
+        :param query['include_queues'] (dict) <br> query.include_queues (Query) :
+        :type query['include_queues']: bool
+        :param query['include_disk_usage'] (dict) <br> query.include_disk_usage (Query) :
+        :type query['include_disk_usage']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
@@ -170,123 +178,117 @@
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
         if query is not None and should_validate:
-            query = TypeAdapter(GetQuery).validate_python(query)
+            query = TypeAdapter(StatusQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": str if not select_path else Model,
+                "200": TenantStatusReport if not select_path else Model,
             }
         )
-        non_200_response_types_map: Dict[str, Any] = {}
+        non_200_response_types_map: Dict[str, Any] = {
+            "422": HTTPValidationError,
+        }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="GET",
-            resource_path="/storage/v1/",
+            resource_path="/storage/v1/status",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TenantStatusReport: ...
+    ) -> str: ...
 
     @overload
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def status(
+    async def version(
         self,
         *,
-        query: StatusQuery | QueryParamTypes | None = None,
+        query: VersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TenantStatusReport | T | Response | Model:
-        """Status.
+    ) -> str | T | Response | Model:
+        """Version.
 
-        Validate consistency of buckets and notification queues for this tenant.
+        Get the application version.
         :param query: URL Query parameters.
-        :type query: StatusQuery | QueryParamTypes, optional
-        :param query['store'] (dict) <br> query.store (Query) :
-        :type query['store']: str
-        :param query['include_buckets'] (dict) <br> query.include_buckets (Query) :
-        :type query['include_buckets']: bool
-        :param query['include_queues'] (dict) <br> query.include_queues (Query) :
-        :type query['include_queues']: bool
-        :param query['include_disk_usage'] (dict) <br> query.include_disk_usage (Query) :
-        :type query['include_disk_usage']: bool
+        :type query: VersionQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
@@ -313,32 +315,30 @@
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
         if query is not None and should_validate:
-            query = TypeAdapter(StatusQuery).validate_python(query)
+            query = TypeAdapter(VersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TenantStatusReport if not select_path else Model,
+                "200": str if not select_path else Model,
             }
         )
-        non_200_response_types_map: Dict[str, Any] = {
-            "422": HTTPValidationError,
-        }
+        non_200_response_types_map: Dict[str, Any] = {}
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="GET",
-            resource_path="/storage/v1/status",
+            resource_path="/storage/v1/",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
```

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/bucket_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/bucket_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/object_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/object_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/api/subscription_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/subscription_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay/services/storage/service/service.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/PKG-INFO` & `waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.1.20240415
+Version: 0.4.1b1
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -48,58 +47,50 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Storage api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Storage api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-storage-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
-from waylay.services.storage.models.tenant_status_report import TenantStatusReport
 try:
-    # Status
-    # calls `GET /storage/v1/status`
-    api_response = await waylay_client.storage.about.status(
-        # query parameters:
-        query = {
-            'include_buckets': True
-            'include_queues': True
-            'include_disk_usage': False
-        },
+    # Version
+    # calls `GET /storage/v1/`
+    api_response = await waylay_client.storage.about.version(
     )
-    print("The response of storage.about.status:\n")
+    print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling storage.about.status: %s\n" % e)
+    print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage-0.4.1.20240415/src/waylay_sdk_storage.egg-info/SOURCES.txt` & `waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

