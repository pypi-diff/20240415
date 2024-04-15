# Comparing `tmp/whaox-wconfig-1.0.1.tar.gz` & `tmp/whaox-wconfig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wconfig-1.0.1.tar", last modified: Mon Apr 15 12:23:28 2024, max compression
+gzip compressed data, was "whaox-wconfig-1.0.2.tar", last modified: Mon Apr 15 12:47:55 2024, max compression
```

## Comparing `whaox-wconfig-1.0.1.tar` & `whaox-wconfig-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.336054 whaox-wconfig-1.0.1/
--rw-rw-rw-   0        0        0     1083 2024-04-15 10:34:39.000000 whaox-wconfig-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-04-15 12:23:28.335051 whaox-wconfig-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2024-04-15 12:23:10.000000 whaox-wconfig-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 12:23:28.336054 whaox-wconfig-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-15 12:23:25.000000 whaox-wconfig-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.314061 whaox-wconfig-1.0.1/wconfig/
--rw-rw-rw-   0        0        0       27 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.1/wconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.317051 whaox-wconfig-1.0.1/wconfig/features/
--rw-rw-rw-   0        0        0      946 2024-04-15 11:14:31.000000 whaox-wconfig-1.0.1/wconfig/features/Config.py
--rw-rw-rw-   0        0        0      636 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.1/wconfig/features/VAR.py
--rw-rw-rw-   0        0        0       52 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.1/wconfig/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.318055 whaox-wconfig-1.0.1/wconfig/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wconfig-1.0.1/wconfig/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 10:44:07.000000 whaox-wconfig-1.0.1/wconfig/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.322059 whaox-wconfig-1.0.1/wconfig/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/__init__.py
--rw-rw-rw-   0        0        0      319 2024-04-15 11:00:43.000000 whaox-wconfig-1.0.1/wconfig/utils/get_path.py
--rw-rw-rw-   0        0        0       56 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/is_dataclass.py
--rw-rw-rw-   0        0        0      494 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.1/wconfig/utils/lead.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.334057 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.774460 whaox-wconfig-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2024-04-15 10:34:39.000000 whaox-wconfig-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2101 2024-04-15 12:47:55.773220 whaox-wconfig-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2024-04-15 12:23:10.000000 whaox-wconfig-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:47:55.774460 whaox-wconfig-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      815 2024-04-15 12:47:52.000000 whaox-wconfig-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.743843 whaox-wconfig-1.0.2/wconfig/
+-rw-rw-rw-   0        0        0       27 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.2/wconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.746101 whaox-wconfig-1.0.2/wconfig/features/
+-rw-rw-rw-   0        0        0      946 2024-04-15 11:14:31.000000 whaox-wconfig-1.0.2/wconfig/features/Config.py
+-rw-rw-rw-   0        0        0      636 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.2/wconfig/features/VAR.py
+-rw-rw-rw-   0        0        0       52 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.2/wconfig/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.748110 whaox-wconfig-1.0.2/wconfig/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wconfig-1.0.2/wconfig/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 10:44:07.000000 whaox-wconfig-1.0.2/wconfig/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.751849 whaox-wconfig-1.0.2/wconfig/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.2/wconfig/utils/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-04-15 11:00:43.000000 whaox-wconfig-1.0.2/wconfig/utils/get_path.py
+-rw-rw-rw-   0        0        0       56 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.2/wconfig/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.2/wconfig/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0      494 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.2/wconfig/utils/lead.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:47:55.772710 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/
+-rw-rw-rw-   0        0        0     2101 2024-04-15 12:47:55.000000 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2024-04-15 12:47:55.000000 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:47:55.000000 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 12:47:55.000000 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 12:47:55.000000 whaox-wconfig-1.0.2/whaox_wconfig.egg-info/top_level.txt
```

### Comparing `whaox-wconfig-1.0.1/LICENSE` & `whaox-wconfig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.1/PKG-INFO` & `whaox-wconfig-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: whaox-wconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to simplify working with the environment
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,env,environment,config
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
 
 # WConfig: Library to simplify working with the environment
 
 [![PyPI version](https://badge.fury.io/py/whaox-wconfig.svg)](https://badge.fury.io/py/whaox-wconfig)
 
 ## Libraries used
  * [dotenv](https://github.com/theskumar/python-dotenv)
```

### Comparing `whaox-wconfig-1.0.1/README.md` & `whaox-wconfig-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.1/setup.py` & `whaox-wconfig-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.1'
+version = '1.0.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wconfig',
     version=version,
@@ -26,11 +26,11 @@
     long_description_content_type='text/markdown',
 
     url='https://github.com/topanim/WApi',
 
     license='MIT LICENSE, see LICENSE file',
 
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['python-dotenv'],
 
     keywords=['python', 'env', 'environment', 'config']
 )
```

### Comparing `whaox-wconfig-1.0.1/wconfig/features/Config.py` & `whaox-wconfig-1.0.2/wconfig/features/Config.py`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.1/wconfig/features/VAR.py` & `whaox-wconfig-1.0.2/wconfig/features/VAR.py`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.1/whaox_wconfig.egg-info/PKG-INFO` & `whaox-wconfig-1.0.2/whaox_wconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: whaox-wconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to simplify working with the environment
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,env,environment,config
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
 
 # WConfig: Library to simplify working with the environment
 
 [![PyPI version](https://badge.fury.io/py/whaox-wconfig.svg)](https://badge.fury.io/py/whaox-wconfig)
 
 ## Libraries used
  * [dotenv](https://github.com/theskumar/python-dotenv)
```

