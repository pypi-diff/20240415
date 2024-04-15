# Comparing `tmp/wikipedia_zh-0.0.4.tar.gz` & `tmp/wikipedia_zh-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipedia_zh-0.0.4.tar", last modified: Mon Apr 15 14:56:51 2024, max compression
+gzip compressed data, was "wikipedia_zh-0.0.5.tar", last modified: Mon Apr 15 15:09:45 2024, max compression
```

## Comparing `wikipedia_zh-0.0.4.tar` & `wikipedia_zh-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.652214 wikipedia_zh-0.0.4/
--rw-rw-rw-   0        0        0      403 2024-04-15 14:56:51.651214 wikipedia_zh-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 14:56:51.652214 wikipedia_zh-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      665 2024-04-15 14:56:27.000000 wikipedia_zh-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.647215 wikipedia_zh-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1711 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/geosearch_test.py
--rw-rw-rw-   0        0        0      344 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/lang_test.py
--rw-rw-rw-   0        0        0     7156 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/page_test.py
--rw-rw-rw-   0        0        0    69689 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/request_mock_data.py
--rw-rw-rw-   0        0        0     1399 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/tests/search_test.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.649214 wikipedia_zh-0.0.4/wikipedia_zh/
--rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia_zh-0.0.4/wikipedia_zh/__init__.py
--rw-rw-rw-   0        0        0     2363 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/wikipedia_zh/exceptions.py
--rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.4/wikipedia_zh/util.py
--rw-rw-rw-   0        0        0    23565 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.4/wikipedia_zh/wikipedia.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:56:51.651214 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/
--rw-rw-rw-   0        0        0      403 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 14:56:51.000000 wikipedia_zh-0.0.4/wikipedia_zh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:09:45.796235 wikipedia_zh-0.0.5/
+-rw-rw-rw-   0        0        0      403 2024-04-15 15:09:45.795235 wikipedia_zh-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 15:09:45.796235 wikipedia_zh-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      621 2024-04-15 15:09:44.000000 wikipedia_zh-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:09:45.790331 wikipedia_zh-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/tests/geosearch_test.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/tests/lang_test.py
+-rw-rw-rw-   0        0        0     7156 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/tests/page_test.py
+-rw-rw-rw-   0        0        0    69689 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/tests/request_mock_data.py
+-rw-rw-rw-   0        0        0     1399 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/tests/search_test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:09:45.792615 wikipedia_zh-0.0.5/wikipedia_zh/
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:08:11.000000 wikipedia_zh-0.0.5/wikipedia_zh/__init__.py
+-rw-rw-rw-   0        0        0     2363 2024-04-15 14:53:52.000000 wikipedia_zh-0.0.5/wikipedia_zh/exceptions.py
+-rw-rw-rw-   0        0        0     1026 2024-04-15 13:49:15.000000 wikipedia_zh-0.0.5/wikipedia_zh/util.py
+-rw-rw-rw-   0        0        0    23580 2024-04-15 15:09:38.000000 wikipedia_zh-0.0.5/wikipedia_zh/wikipedia.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:09:45.795235 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/
+-rw-rw-rw-   0        0        0      403 2024-04-15 15:09:45.000000 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-04-15 15:09:45.000000 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:09:45.000000 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-15 15:09:45.000000 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 15:09:45.000000 wikipedia_zh-0.0.5/wikipedia_zh.egg-info/top_level.txt
```

### Comparing `wikipedia_zh-0.0.4/setup.py` & `wikipedia_zh-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import find_packages
 
 setuptools.setup(
     name="wikipedia_zh",
-    version='0.0.4',
+    version='0.0.5',
     author="Heng Zhang",
     author_email="1093869292@qq.com",
     description="Wikipedia Zh API for Python",
     url="https://gitee.com/zh19990906/wikipedia_zh",
     install_requires=[
         'beautifulsoup4',
         'requests>=2.0.0,<3.0.0'
@@ -17,11 +17,8 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
 
-import wikipedia_zh
-
-wikipedia_zh.search
```

### Comparing `wikipedia_zh-0.0.4/tests/geosearch_test.py` & `wikipedia_zh-0.0.5/tests/geosearch_test.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/tests/page_test.py` & `wikipedia_zh-0.0.5/tests/page_test.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/tests/request_mock_data.py` & `wikipedia_zh-0.0.5/tests/request_mock_data.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/tests/search_test.py` & `wikipedia_zh-0.0.5/tests/search_test.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/wikipedia_zh/exceptions.py` & `wikipedia_zh-0.0.5/wikipedia_zh/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/wikipedia_zh/util.py` & `wikipedia_zh-0.0.5/wikipedia_zh/util.py`

 * *Files identical despite different names*

### Comparing `wikipedia_zh-0.0.4/wikipedia_zh/wikipedia.py` & `wikipedia_zh-0.0.5/wikipedia_zh/wikipedia.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .util import cache, stdout_encode, debug
 import re
 
 API_URL = 'http://en.wikipedia.org/w/api.php'
 RATE_LIMIT = False
 RATE_LIMIT_MIN_WAIT = None
 RATE_LIMIT_LAST_CALL = None
-USER_AGENT = 'wikipedia_zh (https://github.com/goldsmith/Wikipedia/)'
+USER_AGENT = 'wikipedia (https://github.com/goldsmith/Wikipedia/)'
 PROXIES = None
 
 
 def set_lang(prefix):
     """
   Change the language of the API being requested.
   Set `prefix` to one of the two letter prefixes found on the `list of all Wikipedias <http://meta.wikimedia.org/wiki/List_of_Wikipedias>`_.
@@ -729,14 +729,14 @@
     if RATE_LIMIT and RATE_LIMIT_LAST_CALL and \
             RATE_LIMIT_LAST_CALL + RATE_LIMIT_MIN_WAIT > datetime.now():
         # it hasn't been long enough since the last API call
         # so wait until we're in the clear to make the request
 
         wait_time = (RATE_LIMIT_LAST_CALL + RATE_LIMIT_MIN_WAIT) - datetime.now()
         time.sleep(int(wait_time.total_seconds()))
-
+    global PROXIES
     r = requests.get(API_URL, params=params, headers=headers, proxies=PROXIES)
 
     if RATE_LIMIT:
         RATE_LIMIT_LAST_CALL = datetime.now()
 
     return r.json()
```

