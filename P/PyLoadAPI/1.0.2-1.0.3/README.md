# Comparing `tmp/PyLoadAPI-1.0.2.tar.gz` & `tmp/pyloadapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLoadAPI-1.0.2.tar", last modified: Wed Apr 10 03:37:04 2024, max compression
+gzip compressed data, was "pyloadapi-1.0.3.tar", last modified: Mon Apr 15 06:55:13 2024, max compression
```

## Comparing `PyLoadAPI-1.0.2.tar` & `pyloadapi-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:37:04.972833 PyLoadAPI-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 03:37:04.972833 PyLoadAPI-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 03:37:04.972833 PyLoadAPI-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:37:04.968833 PyLoadAPI-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:37:04.968833 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 03:37:04.000000 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 03:37:04.000000 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:37:04.000000 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 03:37:04.000000 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 03:37:04.000000 PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:37:04.968833 PyLoadAPI-1.0.2/src/pyloadapi/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/src/pyloadapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/src/pyloadapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/src/pyloadapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 03:37:00.000000 PyLoadAPI-1.0.2/src/pyloadapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.328340 pyloadapi-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/src/pyloadapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/types.py
```

### Comparing `PyLoadAPI-1.0.2/LICENSE` & `pyloadapi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLoadAPI-1.0.2/PKG-INFO` & `pyloadapi-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLoadAPI
-Version: 1.0.2
+Version: 1.0.3
 Summary: "Simple wrapper for pyLoad's API."
 Home-page: https://github.com/tr4nt0r/PyLoadAPI
 Author: Manfred Dennerlein Rodelo
 Author-email: manfred@dennerlein.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,23 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp~=3.9
 
 # PyLoadAPI
 Simple wrapper for pyLoad's API.
 
-# 1.0.2
+# 1.0.3
+
+* Change logging to debug
 
-### Bugfixes
+# 1.0.2
 
 * username and password changed to mandatory arguments
 * Make dataclasses subscriptable
 
 # 1.0.1
 
-### Bugfixes
-
 * Fix login and get_status not raising InvalidAuth when unauthorized
 
 # 1.0.0
 
 * Initial commit
```

### Comparing `PyLoadAPI-1.0.2/pyproject.toml` & `pyloadapi-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyLoadAPI-1.0.2/setup.cfg` & `pyloadapi-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyLoadAPI
-version = 1.0.2
+version = 1.0.3
 author = Manfred Dennerlein Rodelo
 author_email = manfred@dennerlein.name
 description = "Simple wrapper for pyLoad's API."
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/tr4nt0r/PyLoadAPI
```

### Comparing `PyLoadAPI-1.0.2/src/PyLoadAPI.egg-info/PKG-INFO` & `pyloadapi-1.0.3/src/PyLoadAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLoadAPI
-Version: 1.0.2
+Version: 1.0.3
 Summary: "Simple wrapper for pyLoad's API."
 Home-page: https://github.com/tr4nt0r/PyLoadAPI
 Author: Manfred Dennerlein Rodelo
 Author-email: manfred@dennerlein.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,23 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp~=3.9
 
 # PyLoadAPI
 Simple wrapper for pyLoad's API.
 
-# 1.0.2
+# 1.0.3
+
+* Change logging to debug
 
-### Bugfixes
+# 1.0.2
 
 * username and password changed to mandatory arguments
 * Make dataclasses subscriptable
 
 # 1.0.1
 
-### Bugfixes
-
 * Fix login and get_status not raising InvalidAuth when unauthorized
 
 # 1.0.0
 
 * Initial commit
```

### Comparing `PyLoadAPI-1.0.2/src/pyloadapi/api.py` & `pyloadapi-1.0.3/src/pyloadapi/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,81 +32,76 @@
     async def login(self) -> LoginResponse:
         """Login to pyLoad API."""
 
         user_data = {"username": self.username, "password": self.password}
         url = f"{self.api_url}api/login"
         try:
             async with self._session.post(url, data=user_data) as r:
-                _LOGGER.debug(
-                    "Response from %s [%s]: %s", url, r.status, (await r.text())
-                )
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+
                 r.raise_for_status()
                 try:
                     data = await r.json()
                     if not data:
                         raise InvalidAuth
                     return LoginResponse.from_dict(data)
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot parse login response:\n %s",
                         traceback.format_exc(),
                     )
                     raise ParserError(
                         "Login failed during parsing of request response."
                     ) from e
         except (TimeoutError, aiohttp.ClientError) as e:
-            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot login:\n %s", traceback.format_exc())
             raise CannotConnect from e
 
     async def get_status(self) -> StatusServerResponse:
         """Get general status information of pyLoad."""
         url = f"{self.api_url}api/statusServer"
         try:
             async with self._session.get(url) as r:
-                _LOGGER.debug(
-                    "Response from %s [%s]: %s", url, r.status, (await r.text())
-                )
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     raise InvalidAuth
                 r.raise_for_status()
                 try:
                     data = await r.json()
                     return StatusServerResponse.from_dict(data)
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot parse status response:\n %s",
                         traceback.format_exc(),
                     )
                     raise ParserError(
                         "Get status failed during parsing of request response."
                     ) from e
 
         except (TimeoutError, aiohttp.ClientError) as e:
-            _LOGGER.error("Exception: Cannot get status:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot get status:\n %s", traceback.format_exc())
             raise CannotConnect("Get status failed due to request exception") from e
 
     async def version(self) -> str:
         """Get version of pyLoad."""
         url = f"{self.api_url}api/getServerVersion"
         try:
             async with self._session.get(url) as r:
-                _LOGGER.debug(
-                    "Response from %s [%s]: %s", url, r.status, (await r.text())
-                )
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     raise InvalidAuth
                 r.raise_for_status()
                 try:
                     data = await r.json()
                     return str(data)
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot parse status response:\n %s",
                         traceback.format_exc(),
                     )
                     raise ParserError(
                         "Get version failed during parsing of request response."
                     ) from e
         except (TimeoutError, aiohttp.ClientError) as e:
-            _LOGGER.error("Exception: Cannot get version:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot get version:\n %s", traceback.format_exc())
             raise CannotConnect("Get version failed due to request exception") from e
```

### Comparing `PyLoadAPI-1.0.2/src/pyloadapi/types.py` & `pyloadapi-1.0.3/src/pyloadapi/types.py`

 * *Files identical despite different names*

