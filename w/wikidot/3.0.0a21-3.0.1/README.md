# Comparing `tmp/wikidot-3.0.0a21.tar.gz` & `tmp/wikidot-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidot-3.0.0a21.tar", last modified: Sat Apr 13 12:13:33 2024, max compression
+gzip compressed data, was "wikidot-3.0.1.tar", last modified: Mon Apr 15 08:08:01 2024, max compression
```

## Comparing `wikidot-3.0.0a21.tar` & `wikidot-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.514360 wikidot-3.0.0a21/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/LICENSE
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3124 2024-04-13 12:13:33.514170 wikidot-3.0.0a21/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2339 2024-04-13 12:13:01.000000 wikidot-3.0.0a21/README.md
--rw-r--r--   0 ukwhatn    (501) staff       (20)      735 2024-04-13 12:08:01.000000 wikidot-3.0.0a21/pyproject.toml
--rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-13 12:13:33.514401 wikidot-3.0.0a21/setup.cfg
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.509971 wikidot-3.0.0a21/wikidot/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.510988 wikidot-3.0.0a21/wikidot/common/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/common/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-13 11:47:29.000000 wikidot-3.0.0a21/wikidot/common/decorators.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/common/exceptions.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/common/logger.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.511365 wikidot-3.0.0a21/wikidot/connector/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/connector/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    13291 2024-04-13 11:01:08.000000 wikidot-3.0.0a21/wikidot/connector/ajax.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/connector/api.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.512614 wikidot-3.0.0a21/wikidot/module/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/module/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/module/auth.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-13 11:47:18.000000 wikidot-3.0.0a21/wikidot/module/client.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    10770 2024-04-13 11:51:58.000000 wikidot-3.0.0a21/wikidot/module/page.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     8521 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/module/private_message.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-13 11:36:34.000000 wikidot-3.0.0a21/wikidot/module/site.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/module/site_application.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7728 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/module/user.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.513136 wikidot-3.0.0a21/wikidot/util/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.513447 wikidot-3.0.0a21/wikidot/util/parser/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/parser/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/parser/odate.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/parser/user.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/quick_module.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/requestutil.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/stringutil.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.513640 wikidot-3.0.0a21/wikidot/util/table/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/table/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-13 10:37:49.000000 wikidot-3.0.0a21/wikidot/util/table/char_table.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:13:33.513847 wikidot-3.0.0a21/wikidot.egg-info/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3124 2024-04-13 12:13:33.000000 wikidot-3.0.0a21/wikidot.egg-info/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)      872 2024-04-13 12:13:33.000000 wikidot-3.0.0a21/wikidot.egg-info/SOURCES.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-13 12:13:33.000000 wikidot-3.0.0a21/wikidot.egg-info/dependency_links.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-13 12:13:33.000000 wikidot-3.0.0a21/wikidot.egg-info/requires.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-13 12:13:33.000000 wikidot-3.0.0a21/wikidot.egg-info/top_level.txt
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.400372 wikidot-3.0.1/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-11 05:41:21.000000 wikidot-3.0.1/LICENSE
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-15 08:08:01.400184 wikidot-3.0.1/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2339 2024-04-15 07:24:27.000000 wikidot-3.0.1/README.md
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      732 2024-04-15 08:07:05.000000 wikidot-3.0.1/pyproject.toml
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-15 08:08:01.400410 wikidot-3.0.1/setup.cfg
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.393803 wikidot-3.0.1/wikidot/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.395635 wikidot-3.0.1/wikidot/common/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/common/decorators.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/exceptions.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/logger.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.396209 wikidot-3.0.1/wikidot/connector/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/connector/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    10788 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/connector/ajax.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/connector/api.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.398148 wikidot-3.0.1/wikidot/module/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/auth.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/module/client.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    11798 2024-04-15 07:45:35.000000 wikidot-3.0.1/wikidot/module/page.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      194 2024-04-15 07:34:32.000000 wikidot-3.0.1/wikidot/module/page_source.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     8521 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/private_message.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/module/site.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/site_application.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7728 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/user.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.398804 wikidot-3.0.1/wikidot/util/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399245 wikidot-3.0.1/wikidot/util/parser/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/odate.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/user.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/quick_module.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/requestutil.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/stringutil.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399499 wikidot-3.0.1/wikidot/util/table/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/table/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/table/char_table.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399803 wikidot-3.0.1/wikidot.egg-info/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      902 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/SOURCES.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/dependency_links.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/requires.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/top_level.txt
```

### Comparing `wikidot-3.0.0a21/LICENSE` & `wikidot-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/PKG-INFO` & `wikidot-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.0a21
+Version: 3.0.1
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.0a21/README.md` & `wikidot-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/pyproject.toml` & `wikidot-3.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wikidot"
-version = "3.0.0a21"
+version = "3.0.1"
 authors = [{ name = "ukwhatn", email = "ukwhatn@gmail.com" }]
 description = "Wikidot Utility Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wikidot-3.0.0a21/wikidot/common/decorators.py` & `wikidot-3.0.1/wikidot/common/decorators.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/common/exceptions.py` & `wikidot-3.0.1/wikidot/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/connector/ajax.py` & `wikidot-3.0.1/wikidot/connector/ajax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import json.decoder
-from dataclasses import dataclass, field
-from typing import Any, Tuple
+from dataclasses import dataclass
+from typing import Any
 
 import httpx
 
 from ..common import wd_logger
 from ..common.exceptions import NotFoundException, AMCHttpStatusCodeException, ResponseDataException, \
     WikidotStatusCodeException
 
@@ -61,29 +61,14 @@
         ----------
         name: str
             Cookie名
         """
         del self.cookie[name]
         return
 
-    def is_cookie_set(self, name) -> bool:
-        """Cookieが設定されているかどうかを返す
-
-        Parameters
-        ----------
-        name: str
-            Cookie名
-
-        Returns
-        -------
-        bool
-            Cookieが設定されているかどうか
-        """
-        return name in self.cookie
-
     def get_header(self) -> dict:
         """ヘッダを構築して返す
 
         Returns
         -------
         dict
             ヘッダ
@@ -113,21 +98,14 @@
     """
     request_timeout: int = 20
     attempt_limit: int = 3
     retry_interval: int = 5
     semaphore_limit: int = 10
 
 
-@dataclass
-class HTTPRequestData:
-    url: str
-    headers: dict[str, any] = field(default_factory=dict)
-    data: dict[str, any] = field(default_factory=dict)
-
-
 class AjaxModuleConnectorClient:
     """ajax-module-connector.phpへのリクエストを行うクライアント"""
 
     def __init__(
             self,
             site_name: str | None = None,
             config: AjaxModuleConnectorConfig | None = None
@@ -291,50 +269,7 @@
                 return response
 
         async def _execute_requests():
             return await asyncio.gather(*[_request(body) for body in bodies], return_exceptions=return_exceptions)
 
         # 処理を実行
         return asyncio.run(_execute_requests())
-
-    def get(self, datas: list[HTTPRequestData | dict[str, Any]]) -> tuple[Any]:
-        semaphore_instance = asyncio.Semaphore(self.config.semaphore_limit)
-
-        # datasの中身をHTTPRequestDataに変換
-        datas = [data if isinstance(data, HTTPRequestData) else HTTPRequestData(**data) for data in datas]
-
-        async def _get(_data: HTTPRequestData) -> httpx.Response:
-            retry_count = 0
-
-            while True:
-                try:
-                    async with semaphore_instance:
-                        async with httpx.AsyncClient() as client:
-                            wd_logger.debug(f'GET Request: {_data.url} -> {_data.data}')
-                            response = await client.get(
-                                _data.url,
-                                headers=_data.headers,
-                                params=_data.data,
-                                timeout=self.config.request_timeout
-                            )
-                            response.raise_for_status()
-                except (httpx.HTTPStatusError, httpx.TimeoutException) as e:
-                    retry_count += 1
-
-                    if retry_count >= self.config.attempt_limit:
-                        wd_logger.error(f'HTTP GET is respond HTTP error code: {response.status_code} -> {_data.url}')
-                        raise AMCHttpStatusCodeException(
-                            f'HTTP GET is respond HTTP error code: {response.status_code}',
-                            response.status_code
-                        ) from e
-
-                    wd_logger.info(
-                        f'HTTP GET is respond status: {response.status_code} (retry: {retry_count}) -> {_data.url}')
-                    await asyncio.sleep(self.config.retry_interval)
-                    continue
-
-                return response
-
-        async def _execute_gets():
-            return await asyncio.gather(*[_get(data) for data in datas])
-
-        return asyncio.run(_execute_gets())
```

### Comparing `wikidot-3.0.0a21/wikidot/module/auth.py` & `wikidot-3.0.1/wikidot/module/auth.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/module/client.py` & `wikidot-3.0.1/wikidot/module/client.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/module/page.py` & `wikidot-3.0.1/wikidot/module/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from dataclasses import dataclass, asdict
 from datetime import datetime
 from typing import TYPE_CHECKING, Optional, Union, Any
 
 from bs4 import BeautifulSoup
 
 from wikidot.common import exceptions
+from wikidot.module.page_source import PageSource
 from wikidot.util.parser import user as user_parser, odate as odate_parser
+from wikidot.util.requestutil import RequestUtil
 
 if TYPE_CHECKING:
     from wikidot.module.site import Site
     from wikidot.module.user import User
 
 DEFAULT_MODULE_BODY = [
     "fullname",  # ページのフルネーム(str)
@@ -208,20 +210,19 @@
         target_pages = [page for page in pages if not page.is_id_acquired()]
 
         # なければ終了
         if len(target_pages) == 0:
             return pages
 
         # norender, noredirectでアクセス
-        request_datas = [
-            {
-                "url": f"{page.get_url()}/norender/true/noredirect/true"
-            } for page in target_pages
-        ]
-        responses = target_pages[0].site.client.amc_client.get(request_datas)
+        responses = RequestUtil.request(
+            target_pages[0].site.client,
+            "GET",
+            [f"{page.get_url()}/norender/true/noredirect/true" for page in target_pages]
+        )
 
         # "WIKIREQUEST.info.pageId = xxx;"の値をidに設定
         for index, response in enumerate(responses):
             source = response.text
 
             id_match = re.search(r'WIKIREQUEST\.info\.pageId = (\d+);', source)
             if id_match is None:
@@ -229,14 +230,34 @@
             target_pages[index].id = int(id_match.group(1))
 
         return pages
 
     def get_page_ids(self):
         return PageCollection._acquire_page_ids(self)
 
+    @staticmethod
+    def _acquire_page_sources(
+            pages: list['Page']
+    ):
+        if len(pages) == 0:
+            return []
+        response = pages[0].site.amc_request([{
+            "moduleName": "viewsource/ViewSourceModule",
+            "page_id": page.id
+        } for page in pages])
+
+        for page, response in zip(pages, response):
+            body = response.json()["body"]
+            source = BeautifulSoup(body, "lxml").select_one("div.page-source").text.strip().removeprefix("\t")
+            page.source = PageSource(page, source)
+        return pages
+
+    def get_page_sources(self):
+        return PageCollection._acquire_page_sources(self)
+
 
 @dataclass
 class Page:
     """ページオブジェクト
 
     Attributes
     ----------
@@ -300,38 +321,49 @@
     created_by: 'User'
     created_at: datetime
     updated_by: 'User'
     updated_at: datetime
     commented_by: Optional['User']
     commented_at: datetime
     _id: int = None
+    _source: Optional[PageSource] = None
 
     def get_url(self) -> str:
         return f"{self.site.get_url()}/{self.fullname}"
 
     @property
     def id(self) -> int:
         """ページID（必要であれば取得）
 
         Returns
         -------
         int
             ページID
         """
         if self._id is None:
-            PageCollection._acquire_page_ids([self])
+            PageCollection([self]).get_page_ids()
         return self._id
 
     @id.setter
     def id(self, value: int):
         self._id = value
 
     def is_id_acquired(self) -> bool:
         return self._id is not None
 
+    @property
+    def source(self) -> PageSource:
+        if self._source is None:
+            PageCollection([self]).get_page_sources()
+        return self._source
+
+    @source.setter
+    def source(self, value: PageSource):
+        self._source = value
+
     def destroy(self):
         self.site.client.login_check()
         self.site.amc_request([{
             "action": "WikiPageAction",
             "event": "deletePage",
             "page_id": self.id,
             "moduleName": "Empty"
```

### Comparing `wikidot-3.0.0a21/wikidot/module/private_message.py` & `wikidot-3.0.1/wikidot/module/private_message.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/module/site.py` & `wikidot-3.0.1/wikidot/module/site.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/module/site_application.py` & `wikidot-3.0.1/wikidot/module/site_application.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/module/user.py` & `wikidot-3.0.1/wikidot/module/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/parser/odate.py` & `wikidot-3.0.1/wikidot/util/parser/odate.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/parser/user.py` & `wikidot-3.0.1/wikidot/util/parser/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/quick_module.py` & `wikidot-3.0.1/wikidot/util/quick_module.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/requestutil.py` & `wikidot-3.0.1/wikidot/util/requestutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/stringutil.py` & `wikidot-3.0.1/wikidot/util/stringutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot/util/table/char_table.py` & `wikidot-3.0.1/wikidot/util/table/char_table.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a21/wikidot.egg-info/PKG-INFO` & `wikidot-3.0.1/wikidot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.0a21
+Version: 3.0.1
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.0a21/wikidot.egg-info/SOURCES.txt` & `wikidot-3.0.1/wikidot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 wikidot/connector/__init__.py
 wikidot/connector/ajax.py
 wikidot/connector/api.py
 wikidot/module/__init__.py
 wikidot/module/auth.py
 wikidot/module/client.py
 wikidot/module/page.py
+wikidot/module/page_source.py
 wikidot/module/private_message.py
 wikidot/module/site.py
 wikidot/module/site_application.py
 wikidot/module/user.py
 wikidot/util/__init__.py
 wikidot/util/quick_module.py
 wikidot/util/requestutil.py
```

