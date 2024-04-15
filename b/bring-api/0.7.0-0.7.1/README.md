# Comparing `tmp/bring-api-0.7.0.tar.gz` & `tmp/bring_api-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-api-0.7.0.tar", last modified: Wed Apr 10 11:38:34 2024, max compression
+gzip compressed data, was "bring_api-0.7.1.tar", last modified: Mon Apr 15 10:52:57 2024, max compression
```

## Comparing `bring-api-0.7.0.tar` & `bring_api-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-10 11:38:29.000000 bring-api-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-10 11:38:29.000000 bring-api-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-10 11:38:34.161381 bring-api-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-10 11:38:29.000000 bring-api-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.153381 bring-api-0.7.0/bring_api/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53071 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/bring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/bring_api/locales/
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-AT.json
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.de-DE.json
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-AU.json
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-CA.json
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-GB.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.es-ES.json
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.fr-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.fr-FR.json
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.hu-HU.json
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.it-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.it-IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.nb-NO.json
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.nl-NL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.pl-PL.json
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.ru-RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.sv-SE.json
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/locales/articles.tr-TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-10 11:38:29.000000 bring-api-0.7.0/bring_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/bring_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 11:38:34.000000 bring-api-0.7.0/bring_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-10 11:38:29.000000 bring-api-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 11:38:34.161381 bring-api-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:38:34.161381 bring-api-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    45727 2024-04-10 11:38:29.000000 bring-api-0.7.0/tests/test_bring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-15 10:52:52.000000 bring_api-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 10:52:52.000000 bring_api-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-15 10:52:57.540104 bring_api-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-15 10:52:52.000000 bring_api-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.536104 bring_api-0.7.1/bring_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54803 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/bring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/bring_api/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-AT.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-AU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-CA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.es-ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.fr-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.fr-FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.hu-HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.it-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.it-IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.nb-NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.nl-NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.pl-PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.ru-RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.sv-SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.tr-TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/bring_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-15 10:52:52.000000 bring_api-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-15 10:52:57.540104 bring_api-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    45864 2024-04-15 10:52:52.000000 bring_api-0.7.1/tests/test_bring.py
```

### Comparing `bring-api-0.7.0/CHANGELOG.md` & `bring_api-0.7.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG
 
+# 0.7.1
+
+* Fix get_list method not returning uuid and status from JSON response
+* Log to debug instead of error where exceptions are already raised.
+* Add raw server response to debug log messages.
+* Update docstrings
+
 # 0.7.0
 
 * **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
 * All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
 
 ## 0.6.0
```

### Comparing `bring-api-0.7.0/LICENSE` & `bring_api-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/PKG-INFO` & `bring_api-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.7.0
+Version: 0.7.1
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,21 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.1
+
+* Fix get_list method not returning uuid and status from JSON response
+* Log to debug instead of error where exceptions are already raised.
+* Add raw server response to debug log messages.
+* Update docstrings
+
 # 0.7.0
 
 * **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
 * All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
 
 ## 0.6.0
```

### Comparing `bring-api-0.7.0/README.md` & `bring_api-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/bring.py` & `bring_api-0.7.1/bring_api/bring.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from http import HTTPStatus
 import json
 from json import JSONDecodeError
 import logging
 import os
 import time
 import traceback
-from typing import Any, List, Optional, cast
+from typing import List, Optional, cast
 
 import aiohttp
 
 from .const import (
     API_BASE_URL,
     BRING_DEFAULT_LOCALE,
     BRING_SUPPORTED_LOCALES,
@@ -95,44 +95,44 @@
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
         BringAuthException
-            If the login fails due to missing data in the API response.
+            If the login fails due invalid credentials.
             You should check your email and password.
 
         """
         user_data = {"email": self.mail, "password": self.password}
 
         try:
             url = f"{self.url}v2/bringauth"
             async with self._session.post(url, data=user_data) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse login request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Login failed due to authorization failure "
                             "but error response could not be parsed."
                         ) from e
-                    _LOGGER.error("Exception: Cannot login: %s", errmsg["message"])
+                    _LOGGER.debug("Exception: Cannot login: %s", errmsg["message"])
                     raise BringAuthException(
                         "Login failed due to authorization failure, "
                         "please check your email and password."
                     )
                 if r.status == HTTPStatus.BAD_REQUEST:
-                    _LOGGER.error("Exception: Cannot login: %s", await r.text())
+                    _LOGGER.debug("Exception: Cannot login: %s", await r.text())
                     raise BringAuthException(
                         "Login failed due to bad request, please check your email."
                     )
                 r.raise_for_status()
 
                 try:
                     data = cast(
@@ -140,27 +140,27 @@
                         {
                             key: val
                             for key, val in (await r.json()).items()
                             if key in BringAuthResponse.__annotations__
                         },
                     )
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot login:\n %s", traceback.format_exc()
                     )
                     raise BringParseException(
                         "Cannot parse login request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot login:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Authentication failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot login:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Authentication failed due to request exception."
             ) from e
 
         self.uuid = data["uuid"]
         self.public_uuid = data.get("publicUuid", "")
         self.headers["X-BRING-USER-UUID"] = self.uuid
@@ -179,44 +179,45 @@
         return data
 
     async def load_lists(self) -> BringListResponse:
         """Load all shopping lists.
 
         Returns
         -------
-        dict
-
-        The JSON response as a dict.
+        BringListResponse
+            The JSON response.
 
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringusers/{self.uuid}/lists"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Loading lists failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get lists: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Loading lists failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
@@ -230,118 +231,118 @@
                             key: val
                             for key, val in (await r.json()).items()
                             if key in BringListResponse.__annotations__
                         },
                     )
                     return data
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get lists:\n %s", traceback.format_exc()
                     )
                     raise BringParseException(
                         "Loading lists failed during parsing of request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error("Exception: Cannot get lists:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot get lists:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Loading list failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error("Exception: Cannot get lists:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot get lists:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Loading lists failed due to request exception."
             ) from e
 
     async def get_list(self, list_uuid: str) -> BringItemsResponse:
         """Get all items from a shopping list.
 
         Parameters
         ----------
         list_uuid : str
-            A list uuid returned by loadLists()
+            A list uuid returned by load_lists()
 
         Returns
         -------
-        dict
-            The JSON response as a dict.
+        BringItemsResponse
+            The JSON response.
 
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Loading list items failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get list items: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Loading list items failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
 
                 r.raise_for_status()
 
                 try:
-                    data = cast(
-                        BringItemsResponse,
-                        {
-                            key: val
-                            for key, val in (await r.json())["items"].items()
-                            if key in BringItemsResponse.__annotations__
-                        },
-                    )
+                    data = await r.json()
 
-                    for lst in data.values():
-                        for item in cast(dict[Any, Any], lst):
+                    for lst in data["items"].values():
+                        for item in lst:
                             item["itemId"] = self.__translate(
                                 item["itemId"],
                                 to_locale=self.__locale(list_uuid),
                             )
 
-                    return data
-                except JSONDecodeError as e:
-                    _LOGGER.error(
+                    return BringItemsResponse(
+                        uuid=data["uuid"],
+                        status=data["status"],
+                        purchase=data["items"]["purchase"],
+                        recently=data["items"]["recently"],
+                    )
+                except (JSONDecodeError, KeyError) as e:
+                    _LOGGER.debug(
                         "Exception: Cannot get items for list %s:\n%s",
                         list_uuid,
                         traceback.format_exc(),
                     )
                     raise BringParseException(
                         "Loading list items failed during parsing of request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get items for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading list items failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get items for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading list items failed due to request exception."
             ) from e
@@ -354,47 +355,49 @@
         Parameters
         ----------
         list_uuid : str
             A list uuid returned by load_lists()
 
         Returns
         -------
-        list
-            The JSON response as a list. A list of item details.
+        BringListItemsDetailsResponse
+            The JSON response. A list of item details.
             Caution: This is NOT a list of the items currently marked as 'to buy'.
-            See getItems() for that.
+            See get_list() for that.
             This contains the items that where customized by changing
             their default icon, category or uploading an image.
 
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringlists/{list_uuid}/details"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Loading list details failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get list details: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Loading list details failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
@@ -411,33 +414,33 @@
                                 if key in BringListItemDetails.__annotations__
                             },
                         )
                         for item in await r.json()
                     ]
                     return cast(BringListItemsDetailsResponse, data)
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get item details for list %s:\n%s",
                         list_uuid,
                         traceback.format_exc(),
                     )
                     raise BringParseException(
                         "Loading list details failed during parsing of request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get item details for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading list details failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get item details for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading list details failed due to request exception."
             ) from e
@@ -456,15 +459,16 @@
         list_uuid : str
             A list uuid returned by load_lists()
         item_name : str
             The name of the item you want to save.
         specification : str, optional
             The details you want to add to the item.
         item_uuid : str, optional
-            The uuid for the item to add (usage of uuid4 recommended).
+            The uuid for the item to add. If a unique identifier is
+            required it is recommended to generate a random uuid4.
 
 
         Returns
         -------
         Response
             The server response object.
 
@@ -478,15 +482,15 @@
             itemId=item_name,
             spec=specification,
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(list_uuid, data, BringItemOperation.ADD)
         except BringRequestException as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot save item %s (%s) to list %s:\n%s",
                 item_name,
                 specification,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
@@ -534,15 +538,15 @@
             itemId=item_name,
             spec=specification,
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(list_uuid, data, BringItemOperation.ADD)
         except BringRequestException as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot update item %s (%s) to list %s:\n%s",
                 item_name,
                 specification,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
@@ -558,15 +562,16 @@
         Parameters
         ----------
         list_uuid : str
             A list uuid returned by load_lists()
         item_name : str
             The name of the item you want to remove.
         item_uuid : str, optional
-            The uuid of the item you want to remove.
+            The uuid of the item you want to remove. The item to remove can be remove by only
+            referencing its uuid and setting item_name to any nonempty string.
 
         Returns
         -------
         Response
             The server response object.
 
         Raises
@@ -581,15 +586,15 @@
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(
                 list_uuid, data, BringItemOperation.REMOVE
             )
         except BringRequestException as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot delete item %s from list %s:\n%s",
                 item_name,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Removing item {item_name} from list {list_uuid} "
@@ -635,15 +640,15 @@
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(
                 list_uuid, data, BringItemOperation.COMPLETE
             )
         except BringRequestException as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot complete item %s in list %s:\n%s",
                 item_name,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Completing item {item_name} from list {list_uuid} "
@@ -661,92 +666,103 @@
         Parameters
         ----------
         list_uuid : str
             A list uuid returned by loadLists()
         notification_type : BringNotificationType
             The type of notification to be sent
         item_name : str, optional
-            The text that **must** be included in the URGENT_MESSAGE BringNotificationType.
+            The item_name **must** be included when notication_type
+            is BringNotificationType.URGENT_MESSAGE
 
         Returns
         -------
         Response
             The server response object.
 
         Raises
         ------
         BringRequestException
             If the request fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
+        TypeError
+            if the notification_type parameter is invalid.
+        ValueError
+            If the value for item_name is invalid.
 
         """
         json_data = BringNotificationsConfigType(
             arguments=[],
             listNotificationType=notification_type.value,
             senderPublicUserUuid=self.public_uuid,
         )
 
         if not isinstance(notification_type, BringNotificationType):
-            _LOGGER.error(
-                "Exception: notificationType %s not supported.", notification_type
+            _LOGGER.debug(
+                "Exception: notificationType %s not supported. \n%s",
+                notification_type,
+                traceback.format_exc(),
             )
             raise TypeError(
                 f"notificationType {notification_type} not supported,"
                 "must be of type BringNotificationType."
             )
         if notification_type is BringNotificationType.URGENT_MESSAGE:
             if not item_name or len(item_name) == 0:
-                _LOGGER.error("Exception: Argument itemName missing.")
+                _LOGGER.debug(
+                    "Exception: Argument itemName missing:\n%s", traceback.format_exc()
+                )
                 raise ValueError(
                     "notificationType is URGENT_MESSAGE but argument itemName missing."
                 )
 
             json_data["arguments"] = [item_name]
         try:
             url = f"{self.url}v2/bringnotifications/lists/{list_uuid}"
             async with self._session.post(
                 url, headers=self.headers, json=json_data
             ) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Sending notification failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot send notification: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Sending notification failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
 
                 r.raise_for_status()
                 return r
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot send notification %s for list %s:\n%s",
                 notification_type,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Sending notification {notification_type} for list {list_uuid}"
                 "failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot send notification %s for list %s:\n%s",
                 notification_type,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Sending notification {notification_type} for list {list_uuid}"
@@ -782,41 +798,49 @@
             raise ValueError("Argument mail missing.")
 
         params = {"email": mail}
 
         try:
             url = f"{self.url}bringusers"
             async with self._session.get(url, headers=self.headers, params=params) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.NOT_FOUND:
-                    _LOGGER.error("Exception: User %s does not exist.", mail)
                     raise BringUserUnknownException(f"User {mail} does not exist.")
 
                 r.raise_for_status()
 
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get verification for %s:\n%s",
                 mail,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Verifying email failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
-                "Exception: E-mail %s is invalid.",
-                mail,
-            )
             raise BringEMailInvalidException(f"E-mail {mail} is invalid.") from e
 
         return True
 
     def __load_article_translations_from_file(self, locale: str) -> dict[str, str]:
+        """Read localization ressource files from disk.
+
+        Parameters
+        ----------
+        locale : str
+            A locale string
+
+        Returns
+        -------
+            dict[str, str]:
+                A translation table as a dict
+
+        """
         dictionary_from_file: dict[str, str]
 
         path = os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "locales",
             f"articles.{locale}.json",
         )
@@ -828,14 +852,16 @@
     async def __load_article_translations(self) -> dict[str, dict[str, str]]:
         """Load all required translation dictionaries into memory.
 
         Raises
         ------
         BringRequestException
             If the request fails.
+        BringParseException
+            If the parsing of the request response fails.
 
         Returns
         -------
         dict
             dict of downloaded dictionaries
 
         """
@@ -866,42 +892,42 @@
                     "Will continue trying to download locale.",
                     locale,
                 )
 
             try:
                 url = f"{LOCALES_BASE_URL}articles.{locale}.json"
                 async with self._session.get(url) as r:
-                    _LOGGER.debug("Response from %s: %s", url, r.status)
+                    _LOGGER.debug("Response from %s [%s]", url, r.status)
                     r.raise_for_status()
 
                     try:
                         dictionaries[locale] = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot load articles.%s.json:\n%s",
                             locale,
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             f"Loading article translations for locale {locale} "
                             "failed during parsing of request response."
                         ) from e
             except asyncio.TimeoutError as e:
-                _LOGGER.error(
+                _LOGGER.debug(
                     "Exception: Cannot load articles.%s.json::\n%s",
                     locale,
                     traceback.format_exc(),
                 )
                 raise BringRequestException(
                     f"Loading article translations for locale {locale} "
                     "failed due to connection timeout."
                 ) from e
 
             except aiohttp.ClientError as e:
-                _LOGGER.error(
+                _LOGGER.debug(
                     "Exception: Cannot load articles.%s.json:\n%s",
                     locale,
                     traceback.format_exc(),
                 )
                 raise BringRequestException(
                     f"Loading article translations for locale {locale} "
                     "failed due to request exception."
@@ -956,15 +982,15 @@
                 if to_locale
                 else (
                     {value: key for key, value in self.__translations[locale].items()}
                 ).get(item_id, item_id)
             )
 
         except Exception as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot load translation dictionary:\n%s",
                 traceback.format_exc(),
             )
             raise BringTranslationException(
                 "Translation failed due to error loading translation dictionary."
             ) from e
 
@@ -990,57 +1016,59 @@
                 }
                 for user_list_setting in (await self.get_all_user_settings())[
                     "userlistsettings"
                 ]
             }
 
         except Exception as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot load user list settings:\n%s",
                 traceback.format_exc(),
             )
             raise BringTranslationException(
                 "Translation failed due to error loading user list settings."
             ) from e
 
     async def get_all_user_settings(self) -> BringUserSettingsResponse:
         """Load all user settings and user list settings.
 
         Returns
         -------
-        dict
-            The JSON response as a dict.
+        BringUserSettingsResponse
+            The JSON response.
 
 
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringusersettings/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Loading user settings failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get user settings: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Loading user settings failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
@@ -1093,33 +1121,33 @@
                             "userlistsettings": userlistsettings,
                         },
                     )
 
                     return data
 
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get user settings for uuid %s:\n%s",
                         self.uuid,
                         traceback.format_exc(),
                     )
                     raise BringParseException(
                         "Loading user settings failed during parsing of request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get user settings for uuid %s:\n%s",
                 self.uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading user settings failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get user settings for uuid %s:\n%s",
                 self.uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading user settings failed due to request exception."
             ) from e
@@ -1176,44 +1204,46 @@
         return MAP_LANG_TO_LOCALE.get(user_locale["language"], BRING_DEFAULT_LOCALE)
 
     async def get_user_account(self) -> BringSyncCurrentUserResponse:
         """Get current user account.
 
         Returns
         -------
-        dict
-            The JSON response as a dict.
+        BringSyncCurrentUserResponse
+            The JSON response.
 
 
         Raises
         ------
         BringRequestException
             If the request fails.
         BringParseException
             If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}v2/bringusers/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Loading current user settings failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get current user settings: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Loading current user settings failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
@@ -1227,30 +1257,30 @@
                             key: val
                             for key, val in (await r.json()).items()
                             if key in BringSyncCurrentUserResponse.__annotations__
                         },
                     )
                     return data
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get lists:\n %s", traceback.format_exc()
                     )
                     raise BringParseException(
                         "Loading lists failed during parsing of request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot get current user settings:\n %s",
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 "Loading current user settings failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot  current user settings:\n %s", traceback.format_exc()
             )
             raise BringRequestException(
                 "Loading current user settings failed due to request exception."
             ) from e
 
     async def batch_update_list(
@@ -1278,14 +1308,18 @@
         Response
             The server response object.
 
         Raises
         ------
         BringRequestException
             If the request fails.
+        BringParseException
+            If the parsing of the request response fails.
+        BringAuthException
+            If the request fails due to invalid or expired authorization token.
 
         """
         if operation is None:
             operation = BringItemOperation.ADD
 
         _base_params = {
             "accuracy": "0.0",
@@ -1312,50 +1346,50 @@
         }
 
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}/items"
             async with self._session.put(
                 url, headers=self.headers, json=json_data
             ) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Batch operation failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot get execute batch operation: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Batch operation failed due to authorization failure, "
                         "the authorization token is invalid or expired."
                     )
 
                 r.raise_for_status()
                 return r
         except asyncio.TimeoutError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot execute batch operations for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Batch operation for list {list_uuid} failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error(
+            _LOGGER.debug(
                 "Exception: Cannot execute batch operations for %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
                 f"Batch operation for list {list_uuid} failed due to request exception."
             ) from e
@@ -1368,45 +1402,47 @@
         Parameters
         ----------
         refresh_token : str, optional
             The refresh token to use to retrieve a new access token
 
         Returns
         -------
-        dict
-            The JSON response as a dict.
+        BringAuthTokenRespone
+            The JSON response.
 
         Raises
         ------
         BringRequestException
             If the request fails.
+        BringAuthException
+            If the request fails due to invalid or expired refresh token.
 
         """
         refresh_token = refresh_token or self.refresh_token
 
         user_data = {"grant_type": "refresh_token", "refresh_token": refresh_token}
         try:
             url = f"{self.url}v2/bringauth/token"
             async with self._session.post(
                 url, headers=self.headers, data=user_data
             ) as r:
-                _LOGGER.debug("Response from %s: %s", url, r.status)
+                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
-                        _LOGGER.error(
+                        _LOGGER.debug(
                             "Exception: Cannot parse token request response:\n %s",
                             traceback.format_exc(),
                         )
                         raise BringParseException(
                             "Retrieve new access token failed due to authorization failure but "
                             "error response could not be parsed."
                         ) from e
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot retrieve new access token: %s",
                         errmsg["message"],
                     )
                     raise BringAuthException(
                         "Retrieve new access token failed due to authorization failure, "
                         "the refresh token is invalid or expired."
                     )
@@ -1419,28 +1455,28 @@
                         {
                             key: val
                             for key, val in (await r.json()).items()
                             if key in BringAuthTokenRespone.__annotations__
                         },
                     )
                 except JSONDecodeError as e:
-                    _LOGGER.error(
+                    _LOGGER.debug(
                         "Exception: Cannot retrieve new access token:\n %s",
                         traceback.format_exc(),
                     )
                     raise BringParseException(
                         "Cannot parse token request response."
                     ) from e
         except asyncio.TimeoutError as e:
-            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot login:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Retrieve new access token failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
-            _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
+            _LOGGER.debug("Exception: Cannot login:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Retrieve new access token failed due to request exception."
             ) from e
 
         self.headers["Authorization"] = f'{data["token_type"]} {data["access_token"]}'
         self.expires_in = data["expires_in"]
```

### Comparing `bring-api-0.7.0/bring_api/const.py` & `bring_api-0.7.1/bring_api/const.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/exceptions.py` & `bring_api-0.7.1/bring_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.de-AT.json` & `bring_api-0.7.1/bring_api/locales/articles.de-AT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.de-CH.json` & `bring_api-0.7.1/bring_api/locales/articles.de-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.de-DE.json` & `bring_api-0.7.1/bring_api/locales/articles.de-DE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.en-AU.json` & `bring_api-0.7.1/bring_api/locales/articles.en-AU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.en-CA.json` & `bring_api-0.7.1/bring_api/locales/articles.en-CA.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.en-GB.json` & `bring_api-0.7.1/bring_api/locales/articles.en-GB.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.en-US.json` & `bring_api-0.7.1/bring_api/locales/articles.en-US.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.es-ES.json` & `bring_api-0.7.1/bring_api/locales/articles.es-ES.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.fr-CH.json` & `bring_api-0.7.1/bring_api/locales/articles.fr-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.fr-FR.json` & `bring_api-0.7.1/bring_api/locales/articles.fr-FR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.hu-HU.json` & `bring_api-0.7.1/bring_api/locales/articles.hu-HU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.it-CH.json` & `bring_api-0.7.1/bring_api/locales/articles.it-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.it-IT.json` & `bring_api-0.7.1/bring_api/locales/articles.it-IT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.nb-NO.json` & `bring_api-0.7.1/bring_api/locales/articles.nb-NO.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.nl-NL.json` & `bring_api-0.7.1/bring_api/locales/articles.nl-NL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.pl-PL.json` & `bring_api-0.7.1/bring_api/locales/articles.pl-PL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.pt-BR.json` & `bring_api-0.7.1/bring_api/locales/articles.pt-BR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.ru-RU.json` & `bring_api-0.7.1/bring_api/locales/articles.ru-RU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.sv-SE.json` & `bring_api-0.7.1/bring_api/locales/articles.sv-SE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/locales/articles.tr-TR.json` & `bring_api-0.7.1/bring_api/locales/articles.tr-TR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api/types.py` & `bring_api-0.7.1/bring_api/types.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/bring_api.egg-info/PKG-INFO` & `bring_api-0.7.1/bring_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.7.0
+Version: 0.7.1
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,21 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.1
+
+* Fix get_list method not returning uuid and status from JSON response
+* Log to debug instead of error where exceptions are already raised.
+* Add raw server response to debug log messages.
+* Update docstrings
+
 # 0.7.0
 
 * **New API method:** `retrieve_new_access_token` retrieves a new access token and updates authorization headers. Time till expiration of the access token is stored in the property `expires_in` . ([tr4nt0r](https://github.com/tr4nt0r))
 * All API methods that require authentication now raise `BringAuthException` for 401 Unauthorized status ([tr4nt0r](https://github.com/tr4nt0r))
 
 ## 0.6.0
```

### Comparing `bring-api-0.7.0/bring_api.egg-info/SOURCES.txt` & `bring_api-0.7.1/bring_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/pyproject.toml` & `bring_api-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bring-api-0.7.0/setup.cfg` & `bring_api-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bring-api
-version = 0.7.0
+version = 0.7.1
 author = Cyrill Raccaud
 author_email = cyrill.raccaud+pypi@gmail.com
 description = Unofficial package to access Bring! shopping lists API.
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/miaucl/python-bring-api
```

### Comparing `bring-api-0.7.0/tests/test_bring.py` & `bring_api-0.7.1/tests/test_bring.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,19 @@
         )
 
         monkeypatch.setattr(Bring, "_Bring__locale", lambda _, x: "de-DE")
         monkeypatch.setattr(Bring, "_Bring__translate", mocked_translate)
         monkeypatch.setattr(bring, "uuid", UUID)
 
         data = await bring.get_list(UUID)
-        assert data == BRING_GET_LIST_RESPONSE["items"]
+        assert data == {
+            "uuid": BRING_GET_LIST_RESPONSE["uuid"],
+            "status": BRING_GET_LIST_RESPONSE["status"],
+            **BRING_GET_LIST_RESPONSE["items"],
+        }
 
 
 class TestGetAllItemDetails:
     """Test for get_all_item_details method."""
 
     async def test_get_all_item_details(self, mocked, bring):
         """Test get_all_item_details."""
```

