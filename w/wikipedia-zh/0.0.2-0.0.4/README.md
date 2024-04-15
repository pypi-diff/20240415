# Comparing `tmp/wikipedia_zh-0.0.2.tar.gz` & `tmp/wikipedia_zh-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipedia_zh-0.0.2.tar", last modified: Mon Apr 15 14:45:43 2024, max compression
+gzip compressed data, was "wikipedia_zh-0.0.4.tar", last modified: Mon Apr 15 14:56:51 2024, max compression
```

## Comparing `wikipedia_zh-0.0.2.tar` & `wikipedia_zh-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/
--rw-rw-rw-   0        0        0      251 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.342907 wikipedia_zh-0.0.2/code/
--rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia_zh-0.0.2/code/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-04-15 14:45:10.000000 wikipedia_zh-0.0.2/code/exceptions.py
--rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.2/code/util.py
--rw-rw-rw-   0        0        0    23501 2024-04-15 14:45:10.000000 wikipedia_zh-0.0.2/code/wikipedia.py
--rw-rw-rw-   0        0        0       42 2024-04-15 14:45:43.346908 wikipedia_zh-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-15 14:45:39.000000 wikipedia_zh-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.652214 wikipedia_zh-0.0.4/
+-rw-rw-rw-   0        0        0      403 2024-04-15 14:56:51.651214 wikipedia_zh-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:56:51.652214 wikipedia_zh-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      665 2024-04-15 14:56:27.000000 wikipedia_zh-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.647215 wikipedia_zh-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/geosearch_test.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/lang_test.py
+-rw-rw-rw-   0        0        0     7156 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/page_test.py
+-rw-rw-rw-   0        0        0    69689 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/request_mock_data.py
+-rw-rw-rw-   0        0        0     1399 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/search_test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.649214 wikipedia_zh-0.0.4/wikipedia_zh/
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia_zh-0.0.4/wikipedia_zh/__init__.py
+-rw-rw-rw-   0        0        0     2363 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/wikipedia_zh/exceptions.py
+-rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.4/wikipedia_zh/util.py
+-rw-rw-rw-   0        0        0    23565 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/wikipedia_zh/wikipedia.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.651214 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/
+-rw-rw-rw-   0        0        0      403 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/top_level.txt
```

### Comparing `wikipedia_zh-0.0.2/code/exceptions.py` & `wikipedia_zh-0.0.4/wikipedia_zh/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Global code exception and warning classes.
+Global wikipedia_zh exception and warning classes.
 """
 
 import sys
 
 
 ODD_ERROR_MESSAGE = "This shouldn't happen. Please report on GitHub: github.com/goldsmith/Wikipedia"
```

### Comparing `wikipedia_zh-0.0.2/code/util.py` & `wikipedia_zh-0.0.4/wikipedia_zh/util.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.2/code/wikipedia.py` & `wikipedia_zh-0.0.4/wikipedia_zh/wikipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 from .util import cache, stdout_encode, debug
 import re
 
 API_URL = 'http://en.wikipedia.org/w/api.php'
 RATE_LIMIT = False
 RATE_LIMIT_MIN_WAIT = None
 RATE_LIMIT_LAST_CALL = None
-USER_AGENT = 'code (https://github.com/goldsmith/Wikipedia/)'
+USER_AGENT = 'wikipedia_zh (https://github.com/goldsmith/Wikipedia/)'
 PROXIES = None
 
 
 def set_lang(prefix):
     """
   Change the language of the API being requested.
   Set `prefix` to one of the two letter prefixes found on the `list of all Wikipedias <http://meta.wikimedia.org/wiki/List_of_Wikipedias>`_.
 
   After setting the language, the cache for ``search``, ``suggest``, and ``summary`` will be cleared.
 
   .. note:: Make sure you search for page titles in the language that you have set.
   """
     global API_URL
-    API_URL = 'http://' + prefix.lower() + '.code.org/w/api.php'
+    API_URL = 'http://' + prefix.lower() + '.wikipedia_zh.org/w/api.php'
 
     for cached_func in (search, suggest, summary):
         cached_func.clear_cache()
 
 
 def set_user_agent(user_agent_string):
     """
@@ -48,15 +48,15 @@
     USER_AGENT = user_agent_string
 
 
 def set_rate_limiting(rate_limit, min_wait=timedelta(milliseconds=50)):
     """
   Enable or disable rate limiting on requests to the Mediawiki servers.
   If rate limiting is not enabled, under some circumstances (depending on
-  load on Wikipedia, the number of requests you and other `code` users
+  load on Wikipedia, the number of requests you and other `wikipedia_zh` users
   are making, and other factors), Wikipedia may return an HTTP timeout error.
 
   Enabling rate limiting generally prevents that issue, but please note that
   HTTPTimeoutError still might be raised.
 
   Arguments:
 
@@ -119,15 +119,15 @@
 
     return list(search_results)
 
 
 @cache
 def geosearch(latitude, longitude, title=None, results=10, radius=1000):
     """
-  Do a code geo search for `latitude` and `longitude`
+  Do a wikipedia_zh geo search for `latitude` and `longitude`
   using HTTP API described in http://www.mediawiki.org/wiki/Extension:GeoData
 
   Arguments:
 
   * latitude (float or decimal.Decimal)
   * longitude (float or decimal.Decimal)
 
@@ -676,31 +676,31 @@
 
         return self.content[index:next_index].lstrip("=").strip()
 
 
 @cache
 def languages():
     """
-  List all the currently supported language prefixes (usually ISO language code).
+  List all the currently supported language prefixes (usually ISO language wikipedia_zh).
 
-  Can be inputted to `set_lang` to change the Mediawiki that `code` requests
+  Can be inputted to `set_lang` to change the Mediawiki that `wikipedia_zh` requests
   results from.
 
   Returns: dict of <prefix>: <local_lang_name> pairs. To get just a list of prefixes,
-  use `code.languages().keys()`.
+  use `wikipedia_zh.languages().keys()`.
   """
     response = _wiki_request({
         'meta': 'siteinfo',
         'siprop': 'languages'
     })
 
     languages = response['query']['languages']
 
     return {
-        lang['code']: lang['*']
+        lang['wikipedia_zh']: lang['*']
         for lang in languages
     }
 
 
 def donate():
     """
   Open up the Wikimedia donate page in your favorite browser.
```

