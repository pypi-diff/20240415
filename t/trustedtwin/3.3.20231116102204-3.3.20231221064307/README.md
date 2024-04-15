# Comparing `tmp/trustedtwin-3.3.20231116102204.tar.gz` & `tmp/trustedtwin-3.3.20231221064307.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustedtwin-3.3.20231116102204.tar", last modified: Thu Nov 16 10:22:22 2023, max compression
+gzip compressed data, was "trustedtwin-3.3.20231221064307.tar", last modified: Thu Dec 21 06:43:24 2023, max compression
```

## Comparing `trustedtwin-3.3.20231116102204.tar` & `trustedtwin-3.3.20231221064307.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 10:22:22.375742 trustedtwin-3.3.20231116102204/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2254 2023-11-16 10:22:22.375742 trustedtwin-3.3.20231116102204/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-11-16 10:22:22.375742 trustedtwin-3.3.20231116102204/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 10:22:22.373742 trustedtwin-3.3.20231116102204/trustedtwin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/trustedtwin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_api.py
--rw-r--r--   0 root         (0) root         (0)   111744 2023-11-16 10:22:21.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_api.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_api_async.py
--rw-r--r--   0 root         (0) root         (0)   134600 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_api_async.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-11-16 10:22:00.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_api_base.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-11-16 10:22:21.000000 trustedtwin-3.3.20231116102204/trustedtwin/tt_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 10:22:22.374742 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-11-16 10:22:22.000000 trustedtwin-3.3.20231116102204/trustedtwin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 06:43:24.610304 trustedtwin-3.3.20231221064307/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-12-21 06:43:24.610304 trustedtwin-3.3.20231221064307/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-12-21 06:43:24.611304 trustedtwin-3.3.20231221064307/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 06:43:24.608304 trustedtwin-3.3.20231221064307/trustedtwin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/trustedtwin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_api.py
+-rw-r--r--   0 root         (0) root         (0)   113686 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_api.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_api_async.py
+-rw-r--r--   0 root         (0) root         (0)   137134 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_api_async.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-12-21 06:43:04.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_api_base.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin/tt_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 06:43:24.609305 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-12-21 06:43:24.000000 trustedtwin-3.3.20231221064307/trustedtwin.egg-info/top_level.txt
```

### Comparing `trustedtwin-3.3.20231116102204/LICENSE` & `trustedtwin-3.3.20231221064307/LICENSE`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20231116102204/PKG-INFO` & `trustedtwin-3.3.20231221064307/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-Metadata-Version: 2.1
-Name: trustedtwin
-Version: 3.3.20231116102204
-Summary: Trusted Twin Python client
-Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
-Author: TrustedTwin
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: async
-License-File: LICENSE
-
-TrustedTwin Python Client
+TrustedTwin Python Client (external info)
 ===
 
 The Trusted Twin Python library makes it easy to use the Trusted Twin user infrastructure API in Python applications. 
 The library version is consistent with the Swagger version of the Trusted Twin API.
 
 Client offers synchronous and asynchronous versions which can be used for communication with TT API.
 
@@ -95,7 +83,19 @@
 }
 
 status, response = await TT_SERVICE.create_twin(body=_body)
 resp = json.loads(response)
 ```
 
 For more information please navigate to the official [documentation](https://trustedtwin.com/docs/libraries/library-python.html).
+
+TrustedTwin Python Client (internal info)
+===
+
+Updating the library
+---
+
+To update the Python library to the newest version:
+
+1. Upload a tt_api.yaml file corresponding with the respective API version.
+2. In the Gitlab interface in the left-hand side pane, select *Build* and go to the *Pipeline schedules* section.
+3. By the *Deploy to official pyPi repository* schedule, click on the *Run pipeline schedule* button.
```

### Comparing `trustedtwin-3.3.20231116102204/setup.py` & `trustedtwin-3.3.20231221064307/setup.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_api.py` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_api.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_api.pyi` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_api.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,73 @@
         tt_auth: str,
         tt_base: Optional[str] = None,
         tt_dict: Optional[Dict] = None,
         session: Optional[Any] = None,
         codes: Optional[Dict] = None,
     ) -> None:
         """Initialize object"""
+    def get_account(
+        self, dictionary: Optional[Dict] = None, **kwargs
+    ) -> Tuple[int, str]:
+        """Executes ``get_account`` API operation.
+
+        Calls: ``GET /account``
+
+        :param dictionary: Trusted Twin custom header dictionary.
+        :param kwargs: data, json, headers, cookies, files, auth, timeout, allow_redirects, proxies, verify, stream, cert
+
+        Example::
+
+            >>> from trustedtwin.tt_api import TTRESTService
+            >>> tt_client = TTRESTService(tt_auth="TT_SECRET")
+            >>> status, text = tt_client.get_account()
+            >>> status
+            200 (int)
+            >>> text
+            {
+                "resource_access_log": null,
+                "uuid": "dfe8e356-30a7-4b2c-bdfb-a7ae2c159f6d",
+                "created_ts": 1663753700.123,
+                "updated_ts": 1663753700.123
+            } (str)
+
+        """
+    def update_account(
+        self, body: Dict, dictionary: Optional[Dict] = None, **kwargs
+    ) -> Tuple[int, str]:
+        """Executes ``update_account`` API operation.
+
+        Calls: ``PATCH /account``
+
+        :param body: Request body in dict format.
+        :param dictionary: Trusted Twin custom header dictionary.
+        :param kwargs: data, json, headers, cookies, files, auth, timeout, allow_redirects, proxies, verify, stream, cert
+
+        Body::
+
+            {
+                "resource_access_log": null
+            }
+
+        Example::
+
+            >>> from trustedtwin.tt_api import TTRESTService
+            >>> tt_client = TTRESTService(tt_auth="TT_SECRET")
+            >>> status, text = tt_client.update_account()
+            >>> status
+            200 (int)
+            >>> text
+            {
+                "resource_access_log": null,
+                "uuid": "dfe8e356-30a7-4b2c-bdfb-a7ae2c159f6d",
+                "created_ts": 1663753700.123,
+                "updated_ts": 1663753700.123
+            } (str)
+
+        """
     def get_batches(
         self, dictionary: Optional[Dict] = None, **kwargs
     ) -> Tuple[int, str]:
         """Executes ``get_batches`` API operation.
 
         Calls: ``GET /batches``
```

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_api_async.py` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_api_async.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_api_async.pyi` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_api_async.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,79 @@
         tt_auth: str,
         tt_base: Optional[str] = None,
         tt_dict: Optional[Dict] = None,
         session: Optional[Any] = None,
         codes: Optional[Dict] = None,
     ) -> None:
         """Initialize object"""
+    async def get_account(
+        self, dictionary: Optional[Dict] = None, **kwargs
+    ) -> Coroutine[int, str]:
+        """Executes ``get_account`` API operation.
+
+        Calls: ``GET /account``
+
+        :param dictionary: Trusted Twin custom header dictionary.
+        :param kwargs: data, json, headers, skip_auto_headers, auth, allow_redirects, max_redirects, compress, chunked, expect100, raise_for_status, read_until_eof, proxy, proxy_auth, timeout, verify_ssl, fingerprint, ssl_context, ssl, proxy_headers, trace_request_ctx, read_bufsize
+
+        Example::
+
+            >>> import asyncio
+            >>> from trustedtwin.tt_api_async import TTAsyncRESTService
+            >>> tt_client = TTAsyncRESTService(tt_auth="TT_SECRET")
+            >>> async def loop():
+            >>>   status, text = await tt_client.get_account()
+            >>> asyncio.run(loop())
+            >>> status
+            200 (int)
+            >>> text
+            {
+                "resource_access_log": null,
+                "uuid": "dfe8e356-30a7-4b2c-bdfb-a7ae2c159f6d",
+                "created_ts": 1663753700.123,
+                "updated_ts": 1663753700.123
+            } (str)
+
+        """
+    async def update_account(
+        self, body: Dict, dictionary: Optional[Dict] = None, **kwargs
+    ) -> Coroutine[int, str]:
+        """Executes ``update_account`` API operation.
+
+        Calls: ``PATCH /account``
+
+        :param body: Request body in dict format.
+        :param dictionary: Trusted Twin custom header dictionary.
+        :param kwargs: data, json, headers, skip_auto_headers, auth, allow_redirects, max_redirects, compress, chunked, expect100, raise_for_status, read_until_eof, proxy, proxy_auth, timeout, verify_ssl, fingerprint, ssl_context, ssl, proxy_headers, trace_request_ctx, read_bufsize
+
+        Body::
+
+            {
+                "resource_access_log": null
+            }
+
+        Example::
+
+            >>> import asyncio
+            >>> from trustedtwin.tt_api_async import TTAsyncRESTService
+            >>> tt_client = TTAsyncRESTService(tt_auth="TT_SECRET")
+            >>> async def loop():
+            >>>   status, text = await tt_client.update_account()
+            >>> asyncio.run(loop())
+            >>> status
+            200 (int)
+            >>> text
+            {
+                "resource_access_log": null,
+                "uuid": "dfe8e356-30a7-4b2c-bdfb-a7ae2c159f6d",
+                "created_ts": 1663753700.123,
+                "updated_ts": 1663753700.123
+            } (str)
+
+        """
     async def get_batches(
         self, dictionary: Optional[Dict] = None, **kwargs
     ) -> Coroutine[int, str]:
         """Executes ``get_batches`` API operation.
 
         Calls: ``GET /batches``
```

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_api_base.py` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_api_base.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin/tt_endpoints.py` & `trustedtwin-3.3.20231221064307/trustedtwin/tt_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """This files contains definitions of TT API endpoints. This code is automatically generated."""
 
 ENDPOINTS = {
+    "get_account": ("GET", "/account"),
+    "update_account": ("PATCH", "/account"),
     "get_batches": ("GET", "/batches"),
     "create_batch": ("POST", "/batches"),
     "get_batch": ("GET", "/batches/{}"),
     "delete_batch": ("DELETE", "/batches/{}"),
     "update_batch": ("PATCH", "/batches/{}"),
     "trace": ("POST", "/trace"),
     "who_am_i": ("GET", "/whoami"),
```

### Comparing `trustedtwin-3.3.20231116102204/trustedtwin.egg-info/PKG-INFO` & `trustedtwin-3.3.20231221064307/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 3.3.20231116102204
+Version: 3.3.20231221064307
 Summary: Trusted Twin Python client
 Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
 Author: TrustedTwin
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: async
 License-File: LICENSE
+Requires-Dist: requests~=2.31.0
+Provides-Extra: async
+Requires-Dist: requests~=2.31.0; extra == "async"
+Requires-Dist: aiohttp~=3.8.6; extra == "async"
 
-TrustedTwin Python Client
+TrustedTwin Python Client (external info)
 ===
 
 The Trusted Twin Python library makes it easy to use the Trusted Twin user infrastructure API in Python applications. 
 The library version is consistent with the Swagger version of the Trusted Twin API.
 
 Client offers synchronous and asynchronous versions which can be used for communication with TT API.
 
@@ -95,7 +98,19 @@
 }
 
 status, response = await TT_SERVICE.create_twin(body=_body)
 resp = json.loads(response)
 ```
 
 For more information please navigate to the official [documentation](https://trustedtwin.com/docs/libraries/library-python.html).
+
+TrustedTwin Python Client (internal info)
+===
+
+Updating the library
+---
+
+To update the Python library to the newest version:
+
+1. Upload a tt_api.yaml file corresponding with the respective API version.
+2. In the Gitlab interface in the left-hand side pane, select *Build* and go to the *Pipeline schedules* section.
+3. By the *Deploy to official pyPi repository* schedule, click on the *Run pipeline schedule* button.
```

