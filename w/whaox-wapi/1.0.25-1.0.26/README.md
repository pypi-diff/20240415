# Comparing `tmp/whaox-wapi-1.0.25.tar.gz` & `tmp/whaox-wapi-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.25.tar", last modified: Fri Apr 12 10:13:15 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.26.tar", last modified: Mon Apr 15 09:11:40 2024, max compression
```

## Comparing `whaox-wapi-1.0.25.tar` & `whaox-wapi-1.0.26.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 10:13:15.030358 whaox-wapi-1.0.25/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.25/LICENSE
--rw-rw-rw-   0        0        0     2790 2024-04-12 10:13:15.028274 whaox-wapi-1.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.25/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 10:13:15.030358 whaox-wapi-1.0.25/setup.cfg
--rw-rw-rw-   0        0        0      726 2024-04-12 10:13:11.000000 whaox-wapi-1.0.25/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:13:14.972458 whaox-wapi-1.0.25/wapi/
--rw-rw-rw-   0        0        0       98 2024-04-12 10:13:11.000000 whaox-wapi-1.0.25/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:13:15.026286 whaox-wapi-1.0.25/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2790 2024-04-12 10:13:14.000000 whaox-wapi-1.0.25/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-12 10:13:14.000000 whaox-wapi-1.0.25/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 10:13:14.000000 whaox-wapi-1.0.25/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 10:13:14.000000 whaox-wapi-1.0.25/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-12 10:13:14.000000 whaox-wapi-1.0.25/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.26/LICENSE
+-rw-rw-rw-   0        0        0     2834 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.26/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-15 09:11:34.000000 whaox-wapi-1.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.842166 whaox-wapi-1.0.26/wapi/
+-rw-rw-rw-   0        0        0       26 2024-04-12 10:19:11.000000 whaox-wapi-1.0.26/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.888988 whaox-wapi-1.0.26/wapi/features/
+-rw-rw-rw-   0        0        0      989 2024-04-11 20:01:35.000000 whaox-wapi-1.0.26/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      835 2024-04-11 20:01:35.000000 whaox-wapi-1.0.26/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      939 2024-04-11 20:45:55.000000 whaox-wapi-1.0.26/wapi/features/Route.py
+-rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.26/wapi/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:11:40.951454 whaox-wapi-1.0.26/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     2834 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 09:11:40.000000 whaox-wapi-1.0.26/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.25/LICENSE` & `whaox-wapi-1.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.25/PKG-INFO` & `whaox-wapi-1.0.26/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.25
+Version: 1.0.26
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
+Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
```

### Comparing `whaox-wapi-1.0.25/README.md` & `whaox-wapi-1.0.26/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.25/setup.py` & `whaox-wapi-1.0.26/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 
 from io import open
-from setuptools import setup
+from setuptools import setup, find_packages
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.25'
+version = '1.0.26'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
 
     author='WHAOX',
     author_email='gorogannisan641@gmail.com',
 
-    description=(
-        "Web-Library for Python"
-    ),
+    description="Web-Library for Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/topanim/WApi',
 
     license='MIT LICENSE, see LICENSE file',
 
-    packages=['wapi'],
+    packages=find_packages(),
     install_requires=['jsons', 'requests'],
-)
+
+    keywords=['python', 'web', 'api', 'requests', 'post', 'get']
+)
```

### Comparing `whaox-wapi-1.0.25/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.26/whaox_wapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.25
+Version: 1.0.26
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
+Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
```

