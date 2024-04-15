# Comparing `tmp/whaox-wapi-1.0.26.tar.gz` & `tmp/whaox-wapi-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.26.tar", last modified: Mon Apr 15 09:11:40 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.27.tar", last modified: Mon Apr 15 09:32:16 2024, max compression
```

## Comparing `whaox-wapi-1.0.26.tar` & `whaox-wapi-1.0.27.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.26/LICENSE
--rw-rw-rw-   0        0        0     2834 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.26/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-15 09:11:34.000000 whaox-wapi-1.0.26/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.842166 whaox-wapi-1.0.26/wapi/
--rw-rw-rw-   0        0        0       26 2024-04-12 10:19:11.000000 whaox-wapi-1.0.26/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.888988 whaox-wapi-1.0.26/wapi/features/
--rw-rw-rw-   0        0        0      989 2024-04-11 20:01:35.000000 whaox-wapi-1.0.26/wapi/features/GET.py
--rw-rw-rw-   0        0        0      835 2024-04-11 20:01:35.000000 whaox-wapi-1.0.26/wapi/features/POST.py
--rw-rw-rw-   0        0        0      939 2024-04-11 20:45:55.000000 whaox-wapi-1.0.26/wapi/features/Route.py
--rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.26/wapi/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2834 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.054835 whaox-wapi-1.0.27/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.27/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-04-15 09:32:16.054835 whaox-wapi-1.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2024-04-15 09:18:10.000000 whaox-wapi-1.0.27/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:32:16.056515 whaox-wapi-1.0.27/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-15 09:32:13.000000 whaox-wapi-1.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.010673 whaox-wapi-1.0.27/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.27/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.025157 whaox-wapi-1.0.27/wapi/features/
+-rw-rw-rw-   0        0        0      989 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      835 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      939 2024-04-11 20:45:55.000000 whaox-wapi-1.0.27/wapi/features/Route.py
+-rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.27/wapi/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.025157 whaox-wapi-1.0.27/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.27/wapi/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.032425 whaox-wapi-1.0.27/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.27/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      307 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0       56 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.27/wapi/utils/is_dataclass.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:32:16.054835 whaox-wapi-1.0.27/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-04-15 09:32:15.000000 whaox-wapi-1.0.27/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-04-15 09:32:15.000000 whaox-wapi-1.0.27/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:32:15.000000 whaox-wapi-1.0.27/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 09:32:15.000000 whaox-wapi-1.0.27/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 09:32:15.000000 whaox-wapi-1.0.27/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.26/LICENSE` & `whaox-wapi-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.26/PKG-INFO` & `whaox-wapi-1.0.27/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.26
+Version: 1.0.27
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
+[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
```

### Comparing `whaox-wapi-1.0.26/README.md` & `whaox-wapi-1.0.27/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # WApi: Web-Library for Python
 
+[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
```

### Comparing `whaox-wapi-1.0.26/setup.py` & `whaox-wapi-1.0.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.26'
+version = '1.0.27'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.26/wapi/features/GET.py` & `whaox-wapi-1.0.27/wapi/features/GET.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.26/wapi/features/POST.py` & `whaox-wapi-1.0.27/wapi/features/POST.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.26/wapi/features/Route.py` & `whaox-wapi-1.0.27/wapi/features/Route.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.26/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.27/whaox_wapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.26
+Version: 1.0.27
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
+[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
```

