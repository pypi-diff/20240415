# Comparing `tmp/onebusaway-1.0.0.tar.gz` & `tmp/onebusaway-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onebusaway-1.0.0.tar", last modified: Fri Mar 22 02:09:19 2024, max compression
+gzip compressed data, was "onebusaway-1.0.1.tar", last modified: Sun Apr 14 22:59:47 2024, max compression
```

## Comparing `onebusaway-1.0.0.tar` & `onebusaway-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-03-22 02:09:19.767607 onebusaway-1.0.0/
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9796 2024-03-22 02:09:19.767374 onebusaway-1.0.0/PKG-INFO
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9363 2024-03-22 00:57:03.000000 onebusaway-1.0.0/README.md
-drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-03-22 02:09:19.767142 onebusaway-1.0.0/onebusaway.egg-info/
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9796 2024-03-22 02:09:19.000000 onebusaway-1.0.0/onebusaway.egg-info/PKG-INFO
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)      196 2024-03-22 02:09:19.000000 onebusaway-1.0.0/onebusaway.egg-info/SOURCES.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)        1 2024-03-22 02:09:19.000000 onebusaway-1.0.0/onebusaway.egg-info/dependency_links.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)       11 2024-03-22 02:09:19.000000 onebusaway-1.0.0/onebusaway.egg-info/top_level.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)       38 2024-03-22 02:09:19.767649 onebusaway-1.0.0/setup.cfg
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)      582 2024-03-22 02:09:16.000000 onebusaway-1.0.0/setup.py
-drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-03-22 02:09:19.766937 onebusaway-1.0.0/tests/
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)    10228 2024-03-22 01:58:15.000000 onebusaway-1.0.0/tests/test_client.py
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)    13122 2024-03-22 02:08:04.000000 onebusaway-1.0.0/tests/test_models.py
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-14 22:59:47.645151 onebusaway-1.0.1/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9796 2024-04-14 22:59:47.644922 onebusaway-1.0.1/PKG-INFO
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9363 2024-03-22 00:57:03.000000 onebusaway-1.0.1/README.md
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-14 22:59:47.643596 onebusaway-1.0.1/onebusaway/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2202 2024-03-22 01:14:56.000000 onebusaway-1.0.1/onebusaway/__init__.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    16068 2024-04-02 15:27:12.000000 onebusaway-1.0.1/onebusaway/client.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    10682 2024-03-19 05:36:43.000000 onebusaway-1.0.1/onebusaway/client_json.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     1500 2024-03-22 00:30:24.000000 onebusaway-1.0.1/onebusaway/exceptions.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    18536 2024-04-02 15:31:29.000000 onebusaway-1.0.1/onebusaway/models.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    16334 2024-03-18 03:13:36.000000 onebusaway-1.0.1/onebusaway/modelsMTA.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     3372 2024-03-22 00:36:56.000000 onebusaway-1.0.1/onebusaway/utils.py
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-14 22:59:47.644660 onebusaway-1.0.1/onebusaway.egg-info/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     9796 2024-04-14 22:59:47.000000 onebusaway-1.0.1/onebusaway.egg-info/PKG-INFO
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)      356 2024-04-14 22:59:47.000000 onebusaway-1.0.1/onebusaway.egg-info/SOURCES.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)        1 2024-04-14 22:59:47.000000 onebusaway-1.0.1/onebusaway.egg-info/dependency_links.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)       11 2024-04-14 22:59:47.000000 onebusaway-1.0.1/onebusaway.egg-info/top_level.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)       38 2024-04-14 22:59:47.645205 onebusaway-1.0.1/setup.cfg
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)      580 2024-04-14 22:59:44.000000 onebusaway-1.0.1/setup.py
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-14 22:59:47.644484 onebusaway-1.0.1/tests/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    10228 2024-03-22 01:58:15.000000 onebusaway-1.0.1/tests/test_client.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)    13122 2024-03-22 02:08:04.000000 onebusaway-1.0.1/tests/test_models.py
```

### Comparing `onebusaway-1.0.0/PKG-INFO` & `onebusaway-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onebusaway
-Version: 1.0.0
+Version: 1.0.1
 Summary: The OneBusAway Python Client is a Python library for interacting with the OneBusAway API. It provides a simple and convenient way to access real-time transit data, schedules, and other information from various transit agencies.
 Home-page: https://github.com/CheeksTheGeek/onebusaway-python
 Author: Chaitanya Sharma
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneBusAway Python Client
```

### Comparing `onebusaway-1.0.0/README.md` & `onebusaway-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `onebusaway-1.0.0/onebusaway.egg-info/PKG-INFO` & `onebusaway-1.0.1/onebusaway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onebusaway
-Version: 1.0.0
+Version: 1.0.1
 Summary: The OneBusAway Python Client is a Python library for interacting with the OneBusAway API. It provides a simple and convenient way to access real-time transit data, schedules, and other information from various transit agencies.
 Home-page: https://github.com/CheeksTheGeek/onebusaway-python
 Author: Chaitanya Sharma
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneBusAway Python Client
```

### Comparing `onebusaway-1.0.0/setup.py` & `onebusaway-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 from setuptools import setup
 
 setup(
     name="onebusaway",
-    version="1.0.0",
+    version="1.0.1",
     description="The OneBusAway Python Client is a Python library for interacting with the OneBusAway API. It provides a simple and convenient way to access real-time transit data, schedules, and other information from various transit agencies.",
     author="Chaitanya Sharma",
     url="https://github.com/CheeksTheGeek/onebusaway-python",
     license="MIT",
-    py_modules=["onebusaway"],
+    packages=["onebusaway"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `onebusaway-1.0.0/tests/test_client.py` & `onebusaway-1.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `onebusaway-1.0.0/tests/test_models.py` & `onebusaway-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

