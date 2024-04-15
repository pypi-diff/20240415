# Comparing `tmp/sangreal-wind-0.0.8.tar.gz` & `tmp/sangreal-wind-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sangreal-wind-0.0.8.tar", last modified: Fri Nov 30 04:03:50 2018, max compression
+gzip compressed data, was "dist/sangreal-wind-0.0.9.tar", last modified: Tue Dec 11 02:24:02 2018, max compression
```

## Comparing `sangreal-wind-0.0.8.tar` & `sangreal-wind-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      538 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2018-11-08 08:17:44.000000 sangreal-wind-0.0.8/README.md
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       43 2018-11-08 09:33:51.000000 sangreal-wind-0.0.8/sangreal_wind/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind/api/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       86 2018-11-26 01:48:05.000000 sangreal-wind-0.0.8/sangreal_wind/api/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3112 2018-11-30 04:03:07.000000 sangreal-wind-0.0.8/sangreal_wind/api/get_industry.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     1735 2018-11-26 02:19:19.000000 sangreal-wind-0.0.8/sangreal_wind/api/get_ret.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind/utils/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       76 2018-11-26 01:26:35.000000 sangreal-wind-0.0.8/sangreal_wind/utils/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2018-11-26 01:26:15.000000 sangreal-wind-0.0.8/sangreal_wind/utils/datetime_handle.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     1098 2018-11-08 08:36:12.000000 sangreal-wind-0.0.8/sangreal_wind/utils/engines.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      538 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)      423 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/SOURCES.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/dependency_links.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       23 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/requires.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       14 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/sangreal_wind.egg-info/top_level.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2018-11-30 04:03:50.000000 sangreal-wind-0.0.8/setup.cfg
--rwxr-xr-x   0 liubola   (1000) liubola   (1000)      873 2018-11-30 04:03:49.000000 sangreal-wind-0.0.8/setup.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      538 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2018-11-08 08:17:44.000000 sangreal-wind-0.0.9/README.md
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/sangreal_wind/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       43 2018-11-08 09:33:51.000000 sangreal-wind-0.0.9/sangreal_wind/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/sangreal_wind/api/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      149 2018-12-11 02:18:30.000000 sangreal-wind-0.0.9/sangreal_wind/api/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     1456 2018-12-11 02:23:26.000000 sangreal-wind-0.0.9/sangreal_wind/api/get_index_weight.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3112 2018-11-30 04:03:07.000000 sangreal-wind-0.0.9/sangreal_wind/api/get_industry.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     1735 2018-11-26 02:19:19.000000 sangreal-wind-0.0.9/sangreal_wind/api/get_ret.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/sangreal_wind/utils/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       76 2018-11-26 01:26:35.000000 sangreal-wind-0.0.9/sangreal_wind/utils/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2018-11-26 01:26:15.000000 sangreal-wind-0.0.9/sangreal_wind/utils/datetime_handle.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     1098 2018-11-08 08:36:12.000000 sangreal-wind-0.0.9/sangreal_wind/utils/engines.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      538 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      461 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/SOURCES.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/dependency_links.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       23 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/requires.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       14 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/sangreal_wind.egg-info/top_level.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2018-12-11 02:24:02.000000 sangreal-wind-0.0.9/setup.cfg
+-rwxr-xr-x   0 liubola   (1000) liubola   (1000)      873 2018-12-11 02:24:01.000000 sangreal-wind-0.0.9/setup.py
```

### Comparing `sangreal-wind-0.0.8/PKG-INFO` & `sangreal-wind-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sangreal-wind
-Version: 0.0.8
+Version: 0.0.9
 Summary: short cut api for wind
 Home-page: https://github.com/liubola/sangreal-wind
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `sangreal-wind-0.0.8/sangreal_wind/api/get_industry.py` & `sangreal-wind-0.0.9/sangreal_wind/api/get_industry.py`

 * *Files identical despite different names*

### Comparing `sangreal-wind-0.0.8/sangreal_wind/api/get_ret.py` & `sangreal-wind-0.0.9/sangreal_wind/api/get_ret.py`

 * *Files identical despite different names*

### Comparing `sangreal-wind-0.0.8/sangreal_wind/utils/engines.py` & `sangreal-wind-0.0.9/sangreal_wind/utils/engines.py`

 * *Files identical despite different names*

### Comparing `sangreal-wind-0.0.8/sangreal_wind.egg-info/PKG-INFO` & `sangreal-wind-0.0.9/sangreal_wind.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sangreal-wind
-Version: 0.0.8
+Version: 0.0.9
 Summary: short cut api for wind
 Home-page: https://github.com/liubola/sangreal-wind
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `sangreal-wind-0.0.8/setup.py` & `sangreal-wind-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sangreal-wind',
-    version='0.0.8',
+    version='0.0.9',
     description=('short cut api for wind'),
     install_requires=[
         'sangreal-db',
         'sqlalchemy',
     ],
     # long_description=open('README.rst').read(),
     author='liubola',
```

