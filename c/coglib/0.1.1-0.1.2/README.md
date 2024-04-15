# Comparing `tmp/coglib-0.1.1.tar.gz` & `tmp/coglib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coglib-0.1.1.tar", last modified: Mon Apr 15 04:13:13 2024, max compression
+gzip compressed data, was "coglib-0.1.2.tar", last modified: Mon Apr 15 07:35:02 2024, max compression
```

## Comparing `coglib-0.1.1.tar` & `coglib-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.905079 coglib-0.1.1/
--rw-rw-rw-   0        0        0      548 2024-04-15 04:13:13.902082 coglib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.878068 coglib-0.1.1/coglib/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.1/coglib/__init__.py
--rw-rw-rw-   0        0        0     2819 2024-04-15 04:05:37.000000 coglib-0.1.1/coglib/coglib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.899071 coglib-0.1.1/coglib.egg-info/
--rw-rw-rw-   0        0        0      548 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 04:13:13.905079 coglib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-15 04:10:22.000000 coglib-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.575369 coglib-0.1.2/
+-rw-rw-rw-   0        0        0      548 2024-04-15 07:35:02.572369 coglib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.551364 coglib-0.1.2/coglib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.2/coglib/__init__.py
+-rw-rw-rw-   0        0        0     5517 2024-04-15 07:31:55.000000 coglib-0.1.2/coglib/coglib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.570370 coglib-0.1.2/coglib.egg-info/
+-rw-rw-rw-   0        0        0      548 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:35:02.575369 coglib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-04-15 07:34:55.000000 coglib-0.1.2/setup.py
```

### Comparing `coglib-0.1.1/PKG-INFO` & `coglib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.1/coglib.egg-info/PKG-INFO` & `coglib-0.1.2/coglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.1/setup.py` & `coglib-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='coglib',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```
