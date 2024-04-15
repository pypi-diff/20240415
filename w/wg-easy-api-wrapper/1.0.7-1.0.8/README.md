# Comparing `tmp/wg-easy-api-wrapper-1.0.7.tar.gz` & `tmp/wg_easy_api_wrapper-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg-easy-api-wrapper-1.0.7.tar", last modified: Tue Jan  2 18:29:31 2024, max compression
+gzip compressed data, was "wg_easy_api_wrapper-1.0.8.tar", last modified: Mon Apr 15 06:32:42 2024, max compression
```

## Comparing `wg-easy-api-wrapper-1.0.7.tar` & `wg_easy_api_wrapper-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:29:31.837822 wg-easy-api-wrapper-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-02 18:29:31.837822 wg-easy-api-wrapper-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-02 18:29:31.837822 wg-easy-api-wrapper-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:29:31.833822 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-01-02 18:29:26.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:29:31.837822 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-02 18:29:31.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-02 18:29:31.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 18:29:31.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-02 18:29:31.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-02 18:29:31.000000 wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:42.838543 wg_easy_api_wrapper-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-15 06:32:42.838543 wg_easy_api_wrapper-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-15 06:32:42.838543 wg_easy_api_wrapper-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:42.838543 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-15 06:32:32.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:42.838543 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-15 06:32:42.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 06:32:42.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:32:42.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 06:32:42.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 06:32:42.000000 wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/top_level.txt
```

### Comparing `wg-easy-api-wrapper-1.0.7/LICENSE` & `wg_easy_api_wrapper-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wg-easy-api-wrapper-1.0.7/PKG-INFO` & `wg_easy_api_wrapper-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wg-easy-api-wrapper
-Version: 1.0.7
+Version: 1.0.8
 Summary: Wrapper for wg-easy API
 Home-page: https://github.com/Shandeika/wg-easy-api-wrapper
 Author: MrShandy
 Author-email: mrshandy@shandy-dev.ru
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.0
+Requires-Dist: aiohttp~=3.9.0
 
 # wg-easy-api-wrapper
 Python module for convenient interaction with the application API [wg-easy](https://github.com/wg-easy/wg-easy)
 
 You can see all the methods in the documentation on GitHub
 
 ## Usage
```

### Comparing `wg-easy-api-wrapper-1.0.7/README.md` & `wg_easy_api_wrapper-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wg-easy-api-wrapper-1.0.7/setup.cfg` & `wg_easy_api_wrapper-1.0.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wg-easy-api-wrapper
-version = 1.0.7
+version = 1.0.8
 author = MrShandy
 author_email = mrshandy@shandy-dev.ru
 description = Wrapper for wg-easy API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Shandeika/wg-easy-api-wrapper
 license = GPL-3.0
@@ -14,13 +14,13 @@
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 install_requires = 
-	aiohttp==3.9.0
+	aiohttp~=3.9.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/client.py` & `wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper/server.py` & `wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import aiohttp
 
 from .client import Client
 from .errors import AlreadyLoggedInError
 
 
 class Server:
-    def __init__(self, host: str, port: int, password: str, session: aiohttp.ClientSession = None):
-        self.host = host
-        self.port = port
+    def __init__(self, url: str, password: str, session: aiohttp.ClientSession = None):
+        self.url = url
         self._password = password
         self._session = aiohttp.ClientSession() if session is None else session
 
-    async def is_logged_in(self):
+    async def is_logged_in(self) -> bool:
         session = await self.get_session()
         json_response = await session.json()
         return json_response["authenticated"]
 
     def url_builder(self, path: str) -> str:
-        return f"http://{self.host}:{self.port}{path}"
+        return f"{self.url}{path}"
 
     async def __aenter__(self):
         await self.login()
         return self
 
     async def __aexit__(self, exc_type, exc, exc_tb):
         if await self.is_logged_in():
```

### Comparing `wg-easy-api-wrapper-1.0.7/wg_easy_api_wrapper.egg-info/PKG-INFO` & `wg_easy_api_wrapper-1.0.8/wg_easy_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wg-easy-api-wrapper
-Version: 1.0.7
+Version: 1.0.8
 Summary: Wrapper for wg-easy API
 Home-page: https://github.com/Shandeika/wg-easy-api-wrapper
 Author: MrShandy
 Author-email: mrshandy@shandy-dev.ru
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.0
+Requires-Dist: aiohttp~=3.9.0
 
 # wg-easy-api-wrapper
 Python module for convenient interaction with the application API [wg-easy](https://github.com/wg-easy/wg-easy)
 
 You can see all the methods in the documentation on GitHub
 
 ## Usage
```

