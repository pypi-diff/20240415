# Comparing `tmp/coglib-0.1.2.tar.gz` & `tmp/coglib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coglib-0.1.2.tar", last modified: Mon Apr 15 07:35:02 2024, max compression
+gzip compressed data, was "coglib-0.1.3.tar", last modified: Mon Apr 15 08:25:17 2024, max compression
```

## Comparing `coglib-0.1.2.tar` & `coglib-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.575369 coglib-0.1.2/
--rw-rw-rw-   0        0        0      548 2024-04-15 07:35:02.572369 coglib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.551364 coglib-0.1.2/coglib/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.2/coglib/__init__.py
--rw-rw-rw-   0        0        0     5517 2024-04-15 07:31:55.000000 coglib-0.1.2/coglib/coglib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:35:02.570370 coglib-0.1.2/coglib.egg-info/
--rw-rw-rw-   0        0        0      548 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 07:35:02.000000 coglib-0.1.2/coglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 07:35:02.575369 coglib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-15 07:34:55.000000 coglib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.732686 coglib-0.1.3/
+-rw-rw-rw-   0        0        0      548 2024-04-15 08:25:17.729687 coglib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.707651 coglib-0.1.3/coglib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.3/coglib/__init__.py
+-rw-rw-rw-   0        0        0     5574 2024-04-15 08:24:57.000000 coglib-0.1.3/coglib/coglib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.726686 coglib-0.1.3/coglib.egg-info/
+-rw-rw-rw-   0        0        0      548 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:25:17.732686 coglib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-04-15 08:25:11.000000 coglib-0.1.3/setup.py
```

### Comparing `coglib-0.1.2/PKG-INFO` & `coglib-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.2/coglib/coglib.py` & `coglib-0.1.3/coglib/coglib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 from datetime import datetime
 import json
 from xmlrpc.client import boolean
 import requests
 import pandas as pd
-from typing import NewType
-EconDataList = NewType('EconDataList', list['EconData'])
+from typing import List, NewType
+EconDataList = NewType('EconDataList', List['EconData'])
 LoginResponse = NewType('LoginResponse','LoginResponse')
+cog_response=NewType("CogResponse",'CogResponse')
 class DataFeedAdaptor:   
     base_url='https://marketwatch.cogencis.com/v2/staging/analyticsapi/api/v2/'
     local_base_url='http://localhost:5051/api/v2/'
     isConnected:boolean=False;
     token=None
     expiry=None
     headers={
```

### Comparing `coglib-0.1.2/coglib.egg-info/PKG-INFO` & `coglib-0.1.3/coglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.2/setup.py` & `coglib-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='coglib',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

