# Comparing `tmp/amino.fix.fix-1.0.7b4.tar.gz` & `tmp/amino_fix_fix-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.7b4.tar", last modified: Sun Apr  7 22:31:27 2024, max compression
+gzip compressed data, was "amino_fix_fix-1.0.8.tar", last modified: Sun Apr 14 22:59:31 2024, max compression
```

## Comparing `amino.fix.fix-1.0.7b4.tar` & `amino_fix_fix-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.186361 amino.fix.fix-1.0.7b4/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b4/LICENSE
--rw-rw-rw-   0        0        0     4047 2024-04-07 22:31:27.186361 amino.fix.fix-1.0.7b4/PKG-INFO
--rw-rw-rw-   0        0        0     3564 2024-04-07 22:25:41.000000 amino.fix.fix-1.0.7b4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.160331 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     4047 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 22:31:27.000000 amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.167839 amino.fix.fix-1.0.7b4/aminofixfix/
--rw-rw-rw-   0        0        0     1269 2024-04-04 01:14:49.000000 amino.fix.fix-1.0.7b4/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b4/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.173845 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1270 2024-04-04 01:15:01.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   109087 2024-04-07 22:24:44.000000 amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0   102159 2024-04-07 22:30:09.000000 amino.fix.fix-1.0.7b4/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.179353 amino.fix.fix-1.0.7b4/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:31:27.185361 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     5113 2024-04-07 22:31:01.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b4/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b4/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   145289 2024-04-07 22:29:41.000000 amino.fix.fix-1.0.7b4/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-04-07 22:31:27.187360 amino.fix.fix-1.0.7b4/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-04-07 22:30:52.000000 amino.fix.fix-1.0.7b4/setup.py
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.525980 amino_fix_fix-1.0.8/
+-rw-r--r--   0 josephattano   (501) staff       (20)     1075 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/LICENSE
+-rw-r--r--   0 josephattano   (501) staff       (20)     4548 2024-04-14 22:59:31.525911 amino_fix_fix-1.0.8/PKG-INFO
+-rw-r--r--   0 josephattano   (501) staff       (20)     3474 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/README.md
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.525225 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/
+-rw-r--r--   0 josephattano   (501) staff       (20)     4548 2024-04-14 22:59:31.000000 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/PKG-INFO
+-rw-r--r--   0 josephattano   (501) staff       (20)      799 2024-04-14 22:59:31.000000 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/SOURCES.txt
+-rw-r--r--   0 josephattano   (501) staff       (20)        1 2024-04-14 22:59:31.000000 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/dependency_links.txt
+-rw-r--r--   0 josephattano   (501) staff       (20)      227 2024-04-14 22:59:31.000000 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/requires.txt
+-rw-r--r--   0 josephattano   (501) staff       (20)       12 2024-04-14 22:59:31.000000 amino_fix_fix-1.0.8/amino.fix.fix.egg-info/top_level.txt
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.514962 amino_fix_fix-1.0.8/aminofixfix/
+-rw-r--r--   0 josephattano   (501) staff       (20)     1284 2024-04-14 22:54:03.000000 amino_fix_fix-1.0.8/aminofixfix/__init__.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    24271 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/acm.py
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.518752 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/
+-rw-r--r--   0 josephattano   (501) staff       (20)     1270 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/__init__.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    16275 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/acm.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    95303 2024-04-14 22:47:44.000000 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/client.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    14887 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/socket.py
+-rw-r--r--   0 josephattano   (501) staff       (20)   109097 2024-04-14 22:47:47.000000 amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/sub_client.py
+-rw-r--r--   0 josephattano   (501) staff       (20)   103030 2024-04-14 22:52:03.000000 amino_fix_fix-1.0.8/aminofixfix/client.py
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.522646 amino_fix_fix-1.0.8/aminofixfix/lib/
+-rw-r--r--   0 josephattano   (501) staff       (20)       95 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/__init__.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    33502 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/exceptions.py
+drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-14 22:59:31.524989 amino_fix_fix-1.0.8/aminofixfix/lib/facades/
+-rw-r--r--   0 josephattano   (501) staff       (20)      243 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/facades/__init__.py
+-rw-r--r--   0 josephattano   (501) staff       (20)     3388 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/facades/aiohttp.py
+-rw-r--r--   0 josephattano   (501) staff       (20)     2610 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/facades/requests.py
+-rw-r--r--   0 josephattano   (501) staff       (20)      657 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-r--r--   0 josephattano   (501) staff       (20)     5911 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/lib/headers.py
+-rw-r--r--   0 josephattano   (501) staff       (20)     5121 2024-04-14 22:48:00.000000 amino_fix_fix-1.0.8/aminofixfix/lib/helpers.py
+-rw-r--r--   0 josephattano   (501) staff       (20)   200156 2024-04-14 22:46:06.000000 amino_fix_fix-1.0.8/aminofixfix/lib/objects.py
+-rw-r--r--   0 josephattano   (501) staff       (20)    14885 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8/aminofixfix/socket.py
+-rw-r--r--   0 josephattano   (501) staff       (20)   146160 2024-04-14 22:51:45.000000 amino_fix_fix-1.0.8/aminofixfix/sub_client.py
+-rw-r--r--   0 josephattano   (501) staff       (20)       38 2024-04-14 22:59:31.526186 amino_fix_fix-1.0.8/setup.cfg
+-rw-r--r--   0 josephattano   (501) staff       (20)     1361 2024-04-14 22:58:57.000000 amino_fix_fix-1.0.8/setup.py
```

### Comparing `amino.fix.fix-1.0.7b4/LICENSE` & `amino_fix_fix-1.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 - 2024 imperialwool
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 - 2024 imperialwool
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `amino.fix.fix-1.0.7b4/PKG-INFO` & `amino_fix_fix-1.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,66 @@
-Metadata-Version: 2.1
-Name: amino.fix.fix
-Version: 1.0.7b4
-Summary: Library for Aminoapps
-Home-page: https://github.com/imperialwool/Amino.fix.fix
-Author: imperialwool
-Author-email: hi@iwool.dev
-License: MIT
-Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: requests
-Provides-Extra: aiohttp
-License-File: LICENSE
-
-# Amino.fix.fix
-
-[![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
-![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
-[![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
-
-Fork of Amino.fix to improve this library.
-
-## Important notices
-
-- in subclient you should pass `client`, **not** `profile`
-- if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
-- `lib/util` -> `lib/`
-- supporting python3.8+, lower will be never supported
-- if you have issues in pydroid, reinstall/update it
-
-## How to install?
-
-`pip install amino.fix.fix`
-
-## How to use it?
-
-If you want to use sync version of library, you should `import aminofixfix`.
-
-If you want to use Async version of library, you should `import aminofixfix.asyncfixfix`.
-
-Also instead HTTPX you can use aiohttp, Requests or Urllib3. Just install additional dependencies, if you wanna use them:
-
-- `pip install amino.fix.fix[requests]` # only sync
-- `pip install amino.fix.fix[aiohttp]` # only async
-
-Please report any issues and bugs that Request and aiohttp are causing when you use them instead of HTTPX! This feature in beta and not tested well.
-
-Example:
-
-```python
-import aminofixfix
-
-client = aminofixfix.Client()
-client.login("she.a@lil.freak", "sheforthestreets")
-
-@client.event("on_text_message")
-def on_text_message(data):
-    if data.message.content == "Six digits on the check, took it to the bank":
-        client.send_message(data.message.chatId, "Commas after commas, make ya boy— (Freak out)")
-
-```
-
-## API Reference
-
-[Read the Docs Link](https://aminopy.readthedocs.io/en/latest/)
-
-## Licenses
-
-- [HTTPX](https://github.com/encode/httpx) is [BSD licensed](https://github.com/encode/httpx/blob/master/LICENSE.md) code. Used as main library to build and send API async and sync requests.
-- [Requests](https://github.com/psf/requests) is [Apache 2.0 licensed](https://github.com/psf/requests/blob/main/LICENSE) code. Used as alternative library to build and send API requests.
-- [aiohttp](https://github.com/aio-libs/aiohttp) is [Apache 2.0 licensed](https://github.com/aio-libs/aiohttp/blob/master/LICENSE.txt) code. Used as alternative async library to build and send API requests.
-- [websocket-client](https://github.com/websocket-client/websocket-client) is [Apache 2.0 licensed](https://github.com/websocket-client/websocket-client/blob/master/LICENSE) code. Used for sockets.
-- [python-socks](https://github.com/romis2012/python-socks) is [Apache 2.0 licensed](https://github.com/romis2012/python-socks/blob/master/LICENSE.txt) code. Used for SOCKS proxies in API requests and (in future) sockets.
-- [amino.fix](https://github.com/Minori101/Amino.fix) is [MIT licensed](https://github.com/Minori101/Amino.fix/blob/main/LICENSE). Forked to do this library.
-- [setuptools](https://github.com/pypa/setuptools) is [MIT licensed](https://github.com/pypa/setuptools/blob/main/LICENSE). Used to build PyPI releases.
-
-This library is [MIT licensed](https://github.com/imperialwool/Amino.fix.fix/blob/main/LICENSE) code.
+# Amino.fix.fix
+
+[![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b4-blue)](https://pypi.org/project/amino.fix.fix/#history)
+![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
+[![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
+
+Fork of Amino.fix to improve this library.
+
+## Important notices
+
+- in subclient you should pass `client`, **not** `profile`
+- if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
+- `lib/util` -> `lib/`
+- if you have issues in pydroid, reinstall/update it
+
+## How to install?
+
+`pip install amino.fix.fix`
+
+## How to use it?
+
+If you want to use sync version of library, you should `import aminofixfix`.
+
+If you want to use Async version of library, you should `import aminofixfix.asyncfixfix`.
+
+Also instead HTTPX you can use aiohttp, Requests or Urllib3. Just install additional dependencies, if you wanna use them:
+
+- `pip install amino.fix.fix[requests]` # only sync
+- `pip install amino.fix.fix[aiohttp]` # only async
+
+Please report any issues and bugs that Request and aiohttp are causing when you use them instead of HTTPX! This feature in beta and not tested well.
+
+Example:
+
+```python
+import aminofixfix
+
+client = aminofixfix.Client()
+client.login("she.a@lil.freak", "sheforthestreets")
+
+@client.event("on_text_message")
+def on_text_message(data):
+    if data.message.content == "Six digits on the check, took it to the bank":
+        client.send_message(data.message.chatId, "Commas after commas, make ya boy— (Freak out)")
+
+```
+
+## API Reference
+
+[old documentation](https://aminopy.readthedocs.io/en/latest/)
+
+new documentation in progress
+
+## Licenses
+
+- [HTTPX](https://github.com/encode/httpx) is [BSD licensed](https://github.com/encode/httpx/blob/master/LICENSE.md) code. Used as main library to build and send API async and sync requests.
+- [Requests](https://github.com/psf/requests) is [Apache 2.0 licensed](https://github.com/psf/requests/blob/main/LICENSE) code. Used as alternative library to build and send API requests.
+- [aiohttp](https://github.com/aio-libs/aiohttp) is [Apache 2.0 licensed](https://github.com/aio-libs/aiohttp/blob/master/LICENSE.txt) code. Used as alternative async library to build and send API requests.
+- [websocket-client](https://github.com/websocket-client/websocket-client) is [Apache 2.0 licensed](https://github.com/websocket-client/websocket-client/blob/master/LICENSE) code. Used for sockets.
+- [python-socks](https://github.com/romis2012/python-socks) is [Apache 2.0 licensed](https://github.com/romis2012/python-socks/blob/master/LICENSE.txt) code. Used for SOCKS proxies in API requests and (in future) sockets.
+- [amino.fix](https://github.com/Minori101/Amino.fix) is [MIT licensed](https://github.com/Minori101/Amino.fix/blob/main/LICENSE). Forked to do this library.
+- [setuptools](https://github.com/pypa/setuptools) is [MIT licensed](https://github.com/pypa/setuptools/blob/main/LICENSE). Used to build PyPI releases.
+
+This library is [MIT licensed](https://github.com/imperialwool/Amino.fix.fix/blob/main/LICENSE) code.
```

### Comparing `amino.fix.fix-1.0.7b4/amino.fix.fix.egg-info/SOURCES.txt` & `amino_fix_fix-1.0.8/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/__init__.py` & `amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .socket import Callbacks, SocketHandler
-from .lib import exceptions, helpers, objects, headers
+from ..lib import exceptions, helpers, objects, headers
 
 from json import loads
 from threading import Thread
 from urllib.request import urlopen
 from pkg_resources import parse_version as version
 
 def work():
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/acm.py` & `amino_fix_fix-1.0.8/aminofixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/__init__.py` & `amino_fix_fix-1.0.8/aminofixfix/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .socket import Callbacks, SocketHandler
-from ..lib import exceptions, helpers, objects, headers
+from .lib import exceptions, helpers, objects, headers
 
 from json import loads
 from threading import Thread
 from urllib.request import urlopen
 from pkg_resources import parse_version as version
 
 def work():
@@ -26,11 +26,11 @@
         elif version(__newest__) < version(helpers.LIBRARY_VERSION):
             print(
                 "\n! Using preview version {} of amino.fix.fix !".format(helpers.LIBRARY_VERSION),
                 "| Latest stable available: {} |\n".format(__newest__),
                 
                 sep="\n"
             )
-    except:
+    except Exception as e:
         print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
 
 Thread(target=work).start()
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/acm.py` & `amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/client.py` & `amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -740,15 +740,15 @@
         List of Communities the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if not self.authenticated: raise exceptions.NotLoggedIn()
         response = await self.session.get(f"/g/s/community/joined?v=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -767,15 +767,15 @@
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <aminofixfix.lib.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -792,15 +792,15 @@
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -810,15 +810,15 @@
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <aminofixfix.lib.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -955,15 +955,15 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <aminofixfix.lib.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if pageToken is not None: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = await self.session.get(url, headers=self.additional_headers())
@@ -977,15 +977,15 @@
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **messageId** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <aminofixfix.lib.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -995,15 +995,15 @@
         """
         Information of an Community.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
+            - **Success** : :meth:`Community Object <aminofixfix.lib.objects.Community>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1013,15 +1013,15 @@
         """
         Search a Community byt its Amino ID.
 
         **Parameters**
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/search/amino-id-and-link?q={aminoId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1036,15 +1036,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1056,15 +1056,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1076,15 +1076,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
+            - **Success** : :meth:`Visitors List <aminofixfix.lib.objects.VisitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1095,15 +1095,15 @@
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1179,15 +1179,15 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <aminofixfix.lib.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
@@ -1879,15 +1879,15 @@
         """
         Get a List of Linked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1897,15 +1897,15 @@
         """
         Get a List of Unlinked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2184,15 +2184,15 @@
         """
         Get Information about your Amino+ Membership.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
+            - **Success** : :meth:`Membership Object <aminofixfix.lib.objects.Membership>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/membership?force=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2205,15 +2205,15 @@
         **Parameters**
             - **language** : Language of the Blogs.
                 - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
+            - **Success** : :meth:`Blogs List <aminofixfix.lib.objects.BlogList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if language not in await self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
         response = await self.session.get(f"/g/s/announcement?language={language}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -2224,15 +2224,15 @@
         """
         Get Information about the account's Wallet.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <aminofixfix.lib.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/wallet", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2243,15 +2243,15 @@
         Get the Wallet's History Information.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <aminofixfix.lib.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/wallet/coin/history?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2261,15 +2261,15 @@
         """
         Get the User ID from an Device ID.
 
         **Parameters**
             - **deviceID** : ID of the Device.
 
         **Returns**
-            - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
+            - **Success** : :meth:`User ID <aminofixfix.lib.objects.UserProfile.userId>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/auid?deviceId={deviceId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2280,15 +2280,15 @@
         Get the Object Information from the Amino URL Code.
 
         **Parameters**
             - **code** : Code from the Amino URL.
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <aminofixfix.lib.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/link-resolution?q={code}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2300,15 +2300,15 @@
 
         **Parameters**
             - **objectID** : ID of the Object. User ID, Blog ID, etc.
             - **objectType** : Type of the Object.
             - *comId* : ID of the Community. Use if the Object is in a Community.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <aminofixfix.lib.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
@@ -2382,15 +2382,15 @@
         Get list of users of Amino.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
+            - **Success** : :meth:`User Profile Count List Object <aminofixfix.lib.objects.UserProfileCountList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2482,15 +2482,15 @@
         """
         Get public communites
 
         **Parameters**
             - **language** - Set up language
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = await self.session.get(f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/socket.py` & `amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/asyncfixfix/sub_client.py` & `amino_fix_fix-1.0.8/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
         self, mainClient: Client,
         comId: str = None, aminoId: str = None,
-         
+        
         get_community: bool = False,
         get_profile: bool = False,
         **kwargs
     ):
         """
         Init subclient.
 
@@ -1310,15 +1310,15 @@
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <aminofixfix.lib.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfile(response.json()["userProfile"]).UserProfile
@@ -1329,15 +1329,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -1348,15 +1348,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -1367,15 +1367,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
+            - **Success** : :meth:`Visitors List <aminofixfix.lib.objects.visitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VisitorsList(response.json()).VisitorsList
@@ -1415,15 +1415,15 @@
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -1511,15 +1511,15 @@
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
@@ -1529,15 +1529,15 @@
         List of Public Chats of the Community.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
@@ -1546,15 +1546,15 @@
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <aminofixfix.lib.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
@@ -1565,15 +1565,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <aminofixfix.lib.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if pageToken is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
@@ -1587,15 +1587,15 @@
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **message** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <aminofixfix.lib.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Message(response.json()["message"]).Message
@@ -1664,15 +1664,15 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <aminofixfix.lib.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/client.py` & `amino_fix_fix-1.0.8/aminofixfix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -860,15 +860,15 @@
         List of Communities the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if not self.authenticated: raise exceptions.NotLoggedIn()
         response = self.session.get(f"/g/s/community/joined?v=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -900,15 +900,15 @@
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <aminofixfix.lib.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -929,15 +929,15 @@
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -947,15 +947,15 @@
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <aminofixfix.lib.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1119,15 +1119,15 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <aminofixfix.lib.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if pageToken is not None: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = self.session.get(url, headers=self.additional_headers())
@@ -1141,15 +1141,15 @@
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **messageId** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <aminofixfix.lib.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1159,15 +1159,15 @@
         """
         Information of an Community.
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
+            - **Success** : :meth:`Community Object <aminofixfix.lib.objects.Community>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1177,15 +1177,15 @@
         """
         Search a Community byt its Amino ID.
 
         **Parameters**
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/search/amino-id-and-link?q={aminoId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1200,15 +1200,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1220,15 +1220,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1240,15 +1240,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
+            - **Success** : :meth:`Visitors List <aminofixfix.lib.objects.VisitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1259,15 +1259,15 @@
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1375,15 +1375,15 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <aminofixfix.lib.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
@@ -2097,15 +2097,15 @@
         """
         Get a List of Linked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2115,15 +2115,15 @@
         """
         Get a List of Unlinked Communities of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2402,15 +2402,15 @@
         """
         Get Information about your Amino+ Membership.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
+            - **Success** : :meth:`Membership Object <aminofixfix.lib.objects.Membership>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/membership?force=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2423,15 +2423,15 @@
         **Parameters**
             - **language** : Language of the Blogs.
                 - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
+            - **Success** : :meth:`Blogs List <aminofixfix.lib.objects.BlogList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
         response = self.session.get(f"/g/s/announcement?language={language}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -2442,15 +2442,15 @@
         """
         Get Information about the account's Wallet.
 
         **Parameters**
             - No parameters required.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <aminofixfix.lib.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/wallet", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2461,15 +2461,15 @@
         Get the Wallet's History Information.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+            - **Success** : :meth:`Wallet Object <aminofixfix.lib.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/wallet/coin/history?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2479,15 +2479,15 @@
         """
         Get the User ID from an Device ID.
 
         **Parameters**
             - **deviceID** : ID of the Device.
 
         **Returns**
-            - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
+            - **Success** : :meth:`User ID <aminofixfix.lib.objects.UserProfile.userId>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/auid?deviceId={deviceId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2498,15 +2498,15 @@
         Get the Object Information from the Amino URL Code.
 
         **Parameters**
             - **code** : Code from the Amino URL.
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <aminofixfix.lib.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/link-resolution?q={code}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2518,15 +2518,15 @@
 
         **Parameters**
             - **objectID** : ID of the Object. User ID, Blog ID, etc.
             - **objectType** : Type of the Object.
             - *comId* : ID of the Community. Use if the Object is in a Community.
 
         **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+            - **Success** : :meth:`From Code Object <aminofixfix.lib.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
@@ -2600,15 +2600,15 @@
         Get list of users of Amino.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
+            - **Success** : :meth:`User Profile Count List Object <aminofixfix.lib.objects.UserProfileCountList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2751,17 +2751,41 @@
         """
         Get public communites
 
         **Parameters**
             - **language** - Set up language
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = self.session.get(f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["communityList"]).CommunityList
+
+    def get_link_from_id(self, objectId: str, objectType: int = 0):
+        """
+        Get link from id
+
+        **Parameters**
+            - **objectId** - id of object
+            - **objectType** - type of object
+
+        **Returns**
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
+        data = dumps({
+            "objectId": objectId,
+            "objectType": objectType,
+            "timestamp": inttime()
+        })
+        response = self.session.post(f"/g/s/link-translation", data=data, headers=self.additional_headers(data=data))
+        if response.status_code != 200: 
+            return exceptions.CheckException(response)
+        else:
+            return objects.LinkInfo(response.json()).LinkInfo
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/exceptions.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/aiohttp.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/facades/aiohttp.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from __future__ import annotations
-# ^ this thing should fix problem for python3.9 and lower(?)
-
-from json import loads
-from aiohttp import ClientSession, ClientResponse
-
-class AiohttpClient:
-    '''
-        Facade for aiohttp library to be compactable with HTTPX client style.
-
-        [TODO]: timeouts
-    '''
-    def __init__(self, headers: dict, base_url: str, proxies: dict | str | None = {}, **kwargs):
-        '''
-            Init of aiohttp Client.
-
-            If you pass dict as proxies, first proxy in dict will be chosen.
-        '''
-        self.__proxies = list(proxies.values())[0] if isinstance(proxies, dict) else proxies
-        self.__base_url = base_url
-        self.__main_headers = headers
-
-        self.__client: ClientSession = ClientSession(
-            base_url=self.__base_url,
-            headers=self.__main_headers,
-            proxies=self.__proxies
-        )
-    
-    async def get(self, url: str, headers: dict = {}, **kwargs) -> AiohttpResponse:
-        '''
-            Get request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `AiohttpResponse`
-        '''
-        async with await self.__client.get(
-            url=url,
-            headers=headers,
-            ssl=False
-        ) as resp:
-            return AiohttpResponse(resp)    
-    
-    async def post(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> AiohttpResponse:
-        '''
-            Post request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `AiohttpResponse`
-        '''
-        async with await self.__client.post(
-            url=url,
-            data=data if not isinstance(data, dict) else None,
-            json=data if isinstance(data, dict) else None,
-            headers=headers,
-            ssl=False
-        ) as resp:
-            return AiohttpResponse(resp) 
-    
-    async def delete(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> AiohttpResponse:
-        '''
-            Delete request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `AiohttpResponse`
-        '''
-        async with await self.__client.delete(
-            url=url,
-            data=data if not isinstance(data, dict) else None,
-            json=data if isinstance(data, dict) else None,
-            headers=headers,
-            ssl=False
-        ) as resp:
-            return AiohttpResponse(resp) 
-    
-class AiohttpResponse:
-    '''
-        Facade-response for aiohttp to be compactable with code on HTTPX.
-    '''
-
-    def __init__(self, response: ClientResponse):
-        self.__response: ClientResponse = response
-
-        self.status_code: int = self.__response.status
-
-    async def _init(self):
-        self.content = await self.__response.text()
-
-    def json(self):
-        return loads(self.content)
+from __future__ import annotations
+# ^ this thing should fix problem for python3.9 and lower(?)
+
+from json import loads
+from aiohttp import ClientSession, ClientResponse
+
+class AiohttpClient:
+    '''
+        Facade for aiohttp library to be compactable with HTTPX client style.
+
+        [TODO]: timeouts
+    '''
+    def __init__(self, headers: dict, base_url: str, proxies: dict | str | None = {}, **kwargs):
+        '''
+            Init of aiohttp Client.
+
+            If you pass dict as proxies, first proxy in dict will be chosen.
+        '''
+        self.__proxies = list(proxies.values())[0] if isinstance(proxies, dict) else proxies
+        self.__base_url = base_url
+        self.__main_headers = headers
+
+        self.__client: ClientSession = ClientSession(
+            base_url=self.__base_url,
+            headers=self.__main_headers,
+            proxies=self.__proxies
+        )
+    
+    async def get(self, url: str, headers: dict = {}, **kwargs) -> AiohttpResponse:
+        '''
+            Get request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `AiohttpResponse`
+        '''
+        async with await self.__client.get(
+            url=url,
+            headers=headers,
+            ssl=False
+        ) as resp:
+            return AiohttpResponse(resp)    
+    
+    async def post(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> AiohttpResponse:
+        '''
+            Post request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `AiohttpResponse`
+        '''
+        async with await self.__client.post(
+            url=url,
+            data=data if not isinstance(data, dict) else None,
+            json=data if isinstance(data, dict) else None,
+            headers=headers,
+            ssl=False
+        ) as resp:
+            return AiohttpResponse(resp) 
+    
+    async def delete(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> AiohttpResponse:
+        '''
+            Delete request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `AiohttpResponse`
+        '''
+        async with await self.__client.delete(
+            url=url,
+            data=data if not isinstance(data, dict) else None,
+            json=data if isinstance(data, dict) else None,
+            headers=headers,
+            ssl=False
+        ) as resp:
+            return AiohttpResponse(resp) 
+    
+class AiohttpResponse:
+    '''
+        Facade-response for aiohttp to be compactable with code on HTTPX.
+    '''
+
+    def __init__(self, response: ClientResponse):
+        self.__response: ClientResponse = response
+
+        self.status_code: int = self.__response.status
+
+    async def _init(self):
+        self.content = await self.__response.text()
+
+    def json(self):
+        return loads(self.content)
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/requests.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/facades/requests.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from __future__ import annotations
-# ^ this thing should fix problem for python3.9 and lower(?)
-
-from requests import Session, Response
-
-class RequestsClient:
-    '''
-        Facade for Requests library to be compactable with HTTPX client style.
-
-        [TODO]: timeouts
-    '''
-    def __init__(self, headers: dict, base_url: str, proxies: dict = {}, **kwargs):
-        '''
-            Init of Requests Client.
-        '''
-        self.__client: Session = Session()
-        self.__base_url = base_url
-        self.__proxies = proxies
-        self.__main_headers = headers
-    
-    def get(self, url: str, headers: dict = {}, **kwargs) -> Response:
-        '''
-            Get request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `requests.Response`
-        '''
-        return self.__client.get(
-            url = self.__base_url + url,
-            headers=self.__main_headers | headers,
-            proxies=self.__proxies
-        )    
-    
-    def post(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> Response:
-        '''
-            Post request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `requests.Response`
-        '''
-        return self.__client.post(
-            url = self.__base_url + url,
-            data=data if not isinstance(data, dict) else None,
-            json=data if isinstance(data, dict) else None,
-            headers=self.__main_headers | headers,
-            proxies=self.__proxies
-        )   
-    
-    def delete(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> Response:
-        '''
-            Delete request.
-
-            Args: 
-            - url: str
-            - headers: dict = {}
-            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
-            - etc. just for not breaking stuff
-
-            Returns:
-            - object `requests.Response`
-        '''
-        return self.__client.delete(
-            url = self.__base_url + url,
-            data=data if not isinstance(data, dict) else None,
-            json=data if isinstance(data, dict) else None,
-            headers=self.__main_headers | headers,
-            proxies=self.__proxies
+from __future__ import annotations
+# ^ this thing should fix problem for python3.9 and lower(?)
+
+from requests import Session, Response
+
+class RequestsClient:
+    '''
+        Facade for Requests library to be compactable with HTTPX client style.
+
+        [TODO]: timeouts
+    '''
+    def __init__(self, headers: dict, base_url: str, proxies: dict = {}, **kwargs):
+        '''
+            Init of Requests Client.
+        '''
+        self.__client: Session = Session()
+        self.__base_url = base_url
+        self.__proxies = proxies
+        self.__main_headers = headers
+    
+    def get(self, url: str, headers: dict = {}, **kwargs) -> Response:
+        '''
+            Get request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `requests.Response`
+        '''
+        return self.__client.get(
+            url = self.__base_url + url,
+            headers=self.__main_headers | headers,
+            proxies=self.__proxies
+        )    
+    
+    def post(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> Response:
+        '''
+            Post request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `requests.Response`
+        '''
+        return self.__client.post(
+            url = self.__base_url + url,
+            data=data if not isinstance(data, dict) else None,
+            json=data if isinstance(data, dict) else None,
+            headers=self.__main_headers | headers,
+            proxies=self.__proxies
+        )   
+    
+    def delete(self, url: str, headers: dict = {}, data: str | dict | bytes | None = None, **kwargs) -> Response:
+        '''
+            Delete request.
+
+            Args: 
+            - url: str
+            - headers: dict = {}
+            - data: str | dict | bytes | None = None (it will autodetect if its dict and send it as json but not just data)
+            - etc. just for not breaking stuff
+
+            Returns:
+            - object `requests.Response`
+        '''
+        return self.__client.delete(
+            url = self.__base_url + url,
+            data=data if not isinstance(data, dict) else None,
+            json=data if isinstance(data, dict) else None,
+            headers=self.__main_headers | headers,
+            proxies=self.__proxies
         )
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/facades/unsuccessful_import.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-class AiohttpClient:
-    def __init__(self, **kwargs):
-        raise Exception("You need to install aiohttp.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[aiohttp]")
-    
-class AiohttpResponse:
-    def __init__(self, **kwargs):
-        raise Exception("You need to install aiohttp.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[aiohttp]")
-
-class RequestsClient:
-    def __init__(self, **kwargs):
-        raise Exception("You need to install requests.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[requests]")
+class AiohttpClient:
+    def __init__(self, **kwargs):
+        raise Exception("You need to install aiohttp.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[aiohttp]")
+    
+class AiohttpResponse:
+    def __init__(self, **kwargs):
+        raise Exception("You need to install aiohttp.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[aiohttp]")
+
+class RequestsClient:
+    def __init__(self, **kwargs):
+        raise Exception("You need to install requests.\nBest way to do this without breaking anything, type this command:\npip install amino.fix.fix[requests]")
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/headers.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/helpers.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from hashlib import sha1
 from os import urandom
 from json import loads
 from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.7b4"
+LIBRARY_VERSION = "1.0.8"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
@@ -30,15 +30,15 @@
 IOS_VERSIONS = [
     "14.2", "14.3", "14.4", "14.4.1", "14.4.2", "14.5", "14.5.1", "14.6", "14.7", "14.7.1", "14.8", "14.8.1",
     "15.0", "15.0.1", "15.0.2", "15.1", "15.1.1", "15.2", "15.2.1", "15.3", "15.3.1", "15.4", "15.4.1", "15.5", "15.6", "15.6.1", "15.7", "15.7.1",
     "16.0", "16.0.2", "16.0.3", "16.1", "16.1.1", "16.1.2", "16.2", "16.3", "16.3.1", "16.4", "16.4.1", "16.5", "16.5.1", "16.6", "16.6.1", "16.7", "16.7.1", "16.7.2",
     "17.0", "17.0.1", "17.0.2", "17.0.3", "17.1", "17.1.1", "17.1.2", "17.2", "17.2.1", "17.3", "17.3.1", "17.4"
 ]
 APP_VERSIONS = [
-    "3.23.0", "3.22.0", "3.21.0", "3.20.0"
+    "3.24.0", "3.23.0", "3.22.0", "3.21.0", "3.20.0"
 ]
 
 LOCAL_TIMEZONE = -tz_raw // 1000
 
 def str_uuid4() -> str: return str(uuid4())
 
 def inttime() -> int: return int(timestamp() * 1000)
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/lib/objects.py` & `amino_fix_fix-1.0.8/aminofixfix/lib/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1827,14 +1827,48 @@
         try: self.renewedTime = self.json["membership"]["renewedTime"]
         except (KeyError, TypeError): pass
         try: self.expiredTime = self.json["membership"]["expiredTime"]
         except (KeyError, TypeError): pass
 
         return self
 
+class LinkInfo:
+    def __init__(self, data):
+        self.json = data
+
+        self.objectId = None
+        self.shareURLShortCode = None
+        self.targetCode = None
+        self.ndcId = None
+        self.fullPath = None
+        self.shortCode = None
+        self.shareURLFullPath = None
+        self.objectType = None
+
+    @property
+    def LinkInfo(self):
+        try: self.objectId = self.json["linkInfo"]["objectId"]
+        except (KeyError, TypeError): pass
+        try: self.shareURLShortCode = self.json["linkInfo"]["shareURLShortCode"]
+        except (KeyError, TypeError): pass
+        try: self.targetCode = self.json["linkInfo"]["targetCode"]
+        except (KeyError, TypeError): pass
+        try: self.ndcId = self.json["linkInfo"]["ndcId"]
+        except (KeyError, TypeError): pass
+        try: self.fullPath = self.json["linkInfo"]["fullPath"]
+        except (KeyError, TypeError): pass
+        try: self.shortCode = self.json["linkInfo"]["shortCode"]
+        except (KeyError, TypeError): pass
+        try: self.shareURLFullPath = self.json["linkInfo"]["shareURLFullPath"]
+        except (KeyError, TypeError): pass
+        try: self.objectType = self.json["linkInfo"]["objectType"]
+        except (KeyError, TypeError): pass
+        
+        return self
+
 class FromCode:
     def __init__(self, data):
         self.json = data
 
         try: self.community: Community = Community(data["extensions"]["community"]).Community
         except (KeyError, TypeError): self.community: Community = Community({})
```

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/socket.py` & `amino_fix_fix-1.0.8/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b4/aminofixfix/sub_client.py` & `amino_fix_fix-1.0.8/aminofixfix/sub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
         self, mainClient: Client,
         comId: str = None, aminoId: str = None,
-         
+        
         get_community: bool = False,
         get_profile: bool = False,
         **kwargs
     ):
         """
         Init subclient.
 
@@ -1926,15 +1926,15 @@
         """
         Information of an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : :meth:`User Object <aminofixfix.lib.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfile(response.json()["userProfile"]).UserProfile
@@ -1945,15 +1945,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -1964,15 +1964,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`User List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -1983,15 +1983,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
+            - **Success** : :meth:`Visitors List <aminofixfix.lib.objects.visitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VisitorsList(response.json()).VisitorsList
@@ -2085,15 +2085,15 @@
         List of Users that the User Blocked.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : :meth:`Users List <aminofixfix.lib.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
@@ -2293,15 +2293,15 @@
         List of Chats the account is in.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
@@ -2311,15 +2311,15 @@
         List of Public Chats of the Community.
 
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Chat List <aminofixfix.lib.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
@@ -2328,15 +2328,15 @@
         """
         Get the Chat Object from an Chat ID.
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : :meth:`Chat Object <aminofixfix.lib.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
@@ -2347,15 +2347,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : :meth:`Message List <aminofixfix.lib.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if pageToken is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
@@ -2369,15 +2369,15 @@
         Information of an Message from an Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
             - **message** : ID of the Message.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : :meth:`Message Object <aminofixfix.lib.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Message(response.json()["message"]).Message
@@ -2521,15 +2521,15 @@
             - **userId** : ID of the User.
             - **sorting** : Order of the Comments.
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : :meth:`Comments List <aminofixfix.lib.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
@@ -3763,8 +3763,32 @@
         response = self.session.post(
             f"/x{self.comId}/s/chat/thread/{chatId}/message",
             headers=self.additional_headers(data=data, content_type="default"),
             files=files
         )
         
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return response.status_code
+        else: return response.status_code
+
+    def get_link_from_id(self, objectId: str, objectType: int = 0):
+        """
+        Get link from id
+
+        **Parameters**
+            - **objectId** - id of object
+            - **objectType** - type of object
+
+        **Returns**
+            - **Success** : :meth:`Community List <aminofixfix.lib.objects.CommunityList>`
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
+        data = dumps({
+            "objectId": objectId,
+            "objectType": objectType,
+            "timestamp": inttime()
+        })
+        response = self.session.post(f"/g/s-x{self.comId}/link-translation", data=data, headers=self.additional_headers(data=data))
+        if response.status_code != 200: 
+            return exceptions.CheckException(response)
+        else:
+            return objects.LinkInfo(response.json()).LinkInfo
```

### Comparing `amino.fix.fix-1.0.7b4/setup.py` & `amino_fix_fix-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.7b4"
+LIBRARY_VERSION = "1.0.8"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
@@ -18,14 +18,21 @@
 ]
 aiohttp_requirements = [
     "aiohttp>=3.9.0",
     "aiohttp[speedups]",
     "aiohttp_socks"
 ]
 
+dev_requirements = [
+    "setuptools",
+    "wheel",
+    "build",
+    "twine"
+]
+
 # keywords
 
 keywords = [
     'aminoapps',
     'amino.fix',
     'amino.fix.fix',
     'amino',
@@ -61,9 +68,10 @@
     packages=find_packages(),
 
     keywords=keywords,
     install_requires=requirements,
     extras_require={
         "requests": requests_requirements,
         "aiohttp": aiohttp_requirements,
+        "dev": dev_requirements
     },
 )
```

