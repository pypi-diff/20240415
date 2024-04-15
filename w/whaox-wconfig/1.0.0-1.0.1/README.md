# Comparing `tmp/whaox-wconfig-1.0.0.tar.gz` & `tmp/whaox-wconfig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wconfig-1.0.0.tar", last modified: Mon Apr 15 12:21:56 2024, max compression
+gzip compressed data, was "whaox-wconfig-1.0.1.tar", last modified: Mon Apr 15 12:23:28 2024, max compression
```

## Comparing `whaox-wconfig-1.0.0.tar` & `whaox-wconfig-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.678623 whaox-wconfig-1.0.0/
--rw-rw-rw-   0        0        0     1083 2024-04-15 10:34:39.000000 whaox-wconfig-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2068 2024-04-15 12:21:56.677637 whaox-wconfig-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1700 2024-04-15 12:20:37.000000 whaox-wconfig-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 12:21:56.678623 whaox-wconfig-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-15 11:23:44.000000 whaox-wconfig-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.615505 whaox-wconfig-1.0.0/wconfig/
--rw-rw-rw-   0        0        0       27 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.0/wconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.623734 whaox-wconfig-1.0.0/wconfig/features/
--rw-rw-rw-   0        0        0      946 2024-04-15 11:14:31.000000 whaox-wconfig-1.0.0/wconfig/features/Config.py
--rw-rw-rw-   0        0        0      636 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.0/wconfig/features/VAR.py
--rw-rw-rw-   0        0        0       52 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.0/wconfig/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.626743 whaox-wconfig-1.0.0/wconfig/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wconfig-1.0.0/wconfig/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 10:44:07.000000 whaox-wconfig-1.0.0/wconfig/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.635549 whaox-wconfig-1.0.0/wconfig/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.0/wconfig/utils/__init__.py
--rw-rw-rw-   0        0        0      319 2024-04-15 11:00:43.000000 whaox-wconfig-1.0.0/wconfig/utils/get_path.py
--rw-rw-rw-   0        0        0       56 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.0/wconfig/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.0/wconfig/utils/is_dataclass.py
--rw-rw-rw-   0        0        0      494 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.0/wconfig/utils/lead.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:21:56.676621 whaox-wconfig-1.0.0/whaox_wconfig.egg-info/
--rw-rw-rw-   0        0        0     2068 2024-04-15 12:21:56.000000 whaox-wconfig-1.0.0/whaox_wconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-04-15 12:21:56.000000 whaox-wconfig-1.0.0/whaox_wconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 12:21:56.000000 whaox-wconfig-1.0.0/whaox_wconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 12:21:56.000000 whaox-wconfig-1.0.0/whaox_wconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.336054 whaox-wconfig-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2024-04-15 10:34:39.000000 whaox-wconfig-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-04-15 12:23:28.335051 whaox-wconfig-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2024-04-15 12:23:10.000000 whaox-wconfig-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:23:28.336054 whaox-wconfig-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-15 12:23:25.000000 whaox-wconfig-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.314061 whaox-wconfig-1.0.1/wconfig/
+-rw-rw-rw-   0        0        0       27 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.1/wconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.317051 whaox-wconfig-1.0.1/wconfig/features/
+-rw-rw-rw-   0        0        0      946 2024-04-15 11:14:31.000000 whaox-wconfig-1.0.1/wconfig/features/Config.py
+-rw-rw-rw-   0        0        0      636 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.1/wconfig/features/VAR.py
+-rw-rw-rw-   0        0        0       52 2024-04-15 11:11:43.000000 whaox-wconfig-1.0.1/wconfig/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.318055 whaox-wconfig-1.0.1/wconfig/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wconfig-1.0.1/wconfig/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 10:44:07.000000 whaox-wconfig-1.0.1/wconfig/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.322059 whaox-wconfig-1.0.1/wconfig/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-04-15 11:00:43.000000 whaox-wconfig-1.0.1/wconfig/utils/get_path.py
+-rw-rw-rw-   0        0        0       56 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-15 10:37:59.000000 whaox-wconfig-1.0.1/wconfig/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0      494 2024-04-15 12:04:34.000000 whaox-wconfig-1.0.1/wconfig/utils/lead.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:23:28.334057 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 12:23:28.000000 whaox-wconfig-1.0.1/whaox_wconfig.egg-info/top_level.txt
```

### Comparing `whaox-wconfig-1.0.0/LICENSE` & `whaox-wconfig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.0/PKG-INFO` & `whaox-wconfig-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: whaox-wconfig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to simplify working with the environment
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,env,environment,config
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WConfig: Library to simplify working with the environment
 
-[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wconfig)
+[![PyPI version](https://badge.fury.io/py/whaox-wconfig.svg)](https://badge.fury.io/py/whaox-wconfig)
 
 ## Libraries used
  * [dotenv](https://github.com/theskumar/python-dotenv)
 
 ## Installation
 
 ```commandline
```

### Comparing `whaox-wconfig-1.0.0/README.md` & `whaox-wconfig-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WConfig: Library to simplify working with the environment
 
-[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wconfig)
+[![PyPI version](https://badge.fury.io/py/whaox-wconfig.svg)](https://badge.fury.io/py/whaox-wconfig)
 
 ## Libraries used
  * [dotenv](https://github.com/theskumar/python-dotenv)
 
 ## Installation
 
 ```commandline
```

### Comparing `whaox-wconfig-1.0.0/setup.py` & `whaox-wconfig-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.0'
+version = '1.0.1'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wconfig',
     version=version,
```

### Comparing `whaox-wconfig-1.0.0/wconfig/features/Config.py` & `whaox-wconfig-1.0.1/wconfig/features/Config.py`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.0/wconfig/features/VAR.py` & `whaox-wconfig-1.0.1/wconfig/features/VAR.py`

 * *Files identical despite different names*

### Comparing `whaox-wconfig-1.0.0/whaox_wconfig.egg-info/PKG-INFO` & `whaox-wconfig-1.0.1/whaox_wconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: whaox-wconfig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to simplify working with the environment
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,env,environment,config
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WConfig: Library to simplify working with the environment
 
-[![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wconfig)
+[![PyPI version](https://badge.fury.io/py/whaox-wconfig.svg)](https://badge.fury.io/py/whaox-wconfig)
 
 ## Libraries used
  * [dotenv](https://github.com/theskumar/python-dotenv)
 
 ## Installation
 
 ```commandline
```

