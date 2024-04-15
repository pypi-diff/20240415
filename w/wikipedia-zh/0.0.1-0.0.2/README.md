# Comparing `tmp/wikipedia-zh-0.0.1.tar.gz` & `tmp/wikipedia_zh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipedia-zh-0.0.1.tar", last modified: Mon Apr 15 14:24:08 2024, max compression
+gzip compressed data, was "wikipedia_zh-0.0.2.tar", last modified: Mon Apr 15 14:45:43 2024, max compression
```

## Comparing `wikipedia-zh-0.0.1.tar` & `wikipedia_zh-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:24:08.664345 wikipedia-zh-0.0.1/
--rw-rw-rw-   0        0        0      282 2024-04-15 14:24:08.663345 wikipedia-zh-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 14:24:08.664345 wikipedia-zh-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      502 2024-04-15 14:22:46.000000 wikipedia-zh-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:24:08.658345 wikipedia-zh-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 13:49:15.000000 wikipedia-zh-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1711 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/tests/geosearch_test.py
--rw-rw-rw-   0        0        0      344 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/tests/lang_test.py
--rw-rw-rw-   0        0        0     7156 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/tests/page_test.py
--rw-rw-rw-   0        0        0    69689 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/tests/request_mock_data.py
--rw-rw-rw-   0        0        0     1399 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/tests/search_test.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:24:08.660345 wikipedia-zh-0.0.1/wikipedia-zh/
--rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia-zh-0.0.1/wikipedia-zh/__init__.py
--rw-rw-rw-   0        0        0     2363 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/wikipedia-zh/exceptions.py
--rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia-zh-0.0.1/wikipedia-zh/util.py
--rw-rw-rw-   0        0        0    23549 2024-04-15 14:17:56.000000 wikipedia-zh-0.0.1/wikipedia-zh/wikipedia.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:24:08.663345 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/
--rw-rw-rw-   0        0        0      282 2024-04-15 14:24:08.000000 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2024-04-15 14:24:08.000000 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:24:08.000000 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-15 14:24:08.000000 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 14:24:08.000000 wikipedia-zh-0.0.1/wikipedia_zh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/
+-rw-rw-rw-   0        0        0      251 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.342907 wikipedia_zh-0.0.2/code/
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia_zh-0.0.2/code/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-04-15 14:45:10.000000 wikipedia_zh-0.0.2/code/exceptions.py
+-rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.2/code/util.py
+-rw-rw-rw-   0        0        0    23501 2024-04-15 14:45:10.000000 wikipedia_zh-0.0.2/code/wikipedia.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:45:43.346908 wikipedia_zh-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-04-15 14:45:39.000000 wikipedia_zh-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:43.345908 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/
+-rw-rw-rw-   0        0        0      251 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 14:45:43.000000 wikipedia_zh-0.0.2/wikipedia_zh.egg-info/top_level.txt
```

### Comparing `wikipedia-zh-0.0.1/wikipedia-zh/exceptions.py` & `wikipedia_zh-0.0.2/code/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Global wikipedia-zh exception and warning classes.
+Global code exception and warning classes.
 """
 
 import sys
 
 
 ODD_ERROR_MESSAGE = "This shouldn't happen. Please report on GitHub: github.com/goldsmith/Wikipedia"
```

### Comparing `wikipedia-zh-0.0.1/wikipedia-zh/util.py` & `wikipedia_zh-0.0.2/code/util.py`

 * *Files identical despite different names*

### Comparing `wikipedia-zh-0.0.1/wikipedia-zh/wikipedia.py` & `wikipedia_zh-0.0.2/code/wikipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 from .util import cache, stdout_encode, debug
 import re
 
 API_URL = 'http://en.wikipedia.org/w/api.php'
 RATE_LIMIT = False
 RATE_LIMIT_MIN_WAIT = None
 RATE_LIMIT_LAST_CALL = None
-USER_AGENT = 'wikipedia-zh (https://github.com/goldsmith/Wikipedia/)'
+USER_AGENT = 'code (https://github.com/goldsmith/Wikipedia/)'
 PROXIES = None
 
 
 def set_lang(prefix):
     """
   Change the language of the API being requested.
   Set `prefix` to one of the two letter prefixes found on the `list of all Wikipedias <http://meta.wikimedia.org/wiki/List_of_Wikipedias>`_.
 
   After setting the language, the cache for ``search``, ``suggest``, and ``summary`` will be cleared.
 
   .. note:: Make sure you search for page titles in the language that you have set.
   """
     global API_URL
-    API_URL = 'http://' + prefix.lower() + '.wikipedia-zh.org/w/api.php'
+    API_URL = 'http://' + prefix.lower() + '.code.org/w/api.php'
 
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
-  load on Wikipedia, the number of requests you and other `wikipedia-zh` users
+  load on Wikipedia, the number of requests you and other `code` users
   are making, and other factors), Wikipedia may return an HTTP timeout error.
 
   Enabling rate limiting generally prevents that issue, but please note that
   HTTPTimeoutError still might be raised.
 
   Arguments:
 
@@ -119,15 +119,15 @@
 
     return list(search_results)
 
 
 @cache
 def geosearch(latitude, longitude, title=None, results=10, radius=1000):
     """
-  Do a wikipedia-zh geo search for `latitude` and `longitude`
+  Do a code geo search for `latitude` and `longitude`
   using HTTP API described in http://www.mediawiki.org/wiki/Extension:GeoData
 
   Arguments:
 
   * latitude (float or decimal.Decimal)
   * longitude (float or decimal.Decimal)
 
@@ -678,19 +678,19 @@
 
 
 @cache
 def languages():
     """
   List all the currently supported language prefixes (usually ISO language code).
 
-  Can be inputted to `set_lang` to change the Mediawiki that `wikipedia-zh` requests
+  Can be inputted to `set_lang` to change the Mediawiki that `code` requests
   results from.
 
   Returns: dict of <prefix>: <local_lang_name> pairs. To get just a list of prefixes,
-  use `wikipedia-zh.languages().keys()`.
+  use `code.languages().keys()`.
   """
     response = _wiki_request({
         'meta': 'siteinfo',
         'siprop': 'languages'
     })
 
     languages = response['query']['languages']
```

