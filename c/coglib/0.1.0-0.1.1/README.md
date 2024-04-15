# Comparing `tmp/coglib-0.1.0.tar.gz` & `tmp/coglib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coglib-0.1.0.tar", last modified: Mon Apr 15 03:30:10 2024, max compression
+gzip compressed data, was "coglib-0.1.1.tar", last modified: Mon Apr 15 04:13:13 2024, max compression
```

## Comparing `coglib-0.1.0.tar` & `coglib-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:30:10.528836 coglib-0.1.0/
--rw-rw-rw-   0        0        0      548 2024-04-15 03:30:10.525831 coglib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:30:10.500306 coglib-0.1.0/coglib/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.0/coglib/__init__.py
--rw-rw-rw-   0        0        0     2656 2024-04-15 03:29:59.000000 coglib-0.1.0/coglib/coglib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:30:10.523833 coglib-0.1.0/coglib.egg-info/
--rw-rw-rw-   0        0        0      548 2024-04-15 03:30:10.000000 coglib-0.1.0/coglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-15 03:30:10.000000 coglib-0.1.0/coglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:30:10.000000 coglib-0.1.0/coglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 03:30:10.000000 coglib-0.1.0/coglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 03:30:10.000000 coglib-0.1.0/coglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 03:30:10.529837 coglib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      621 2024-04-15 03:28:43.000000 coglib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.905079 coglib-0.1.1/
+-rw-rw-rw-   0        0        0      548 2024-04-15 04:13:13.902082 coglib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.878068 coglib-0.1.1/coglib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.1/coglib/__init__.py
+-rw-rw-rw-   0        0        0     2819 2024-04-15 04:05:37.000000 coglib-0.1.1/coglib/coglib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:13:13.899071 coglib-0.1.1/coglib.egg-info/
+-rw-rw-rw-   0        0        0      548 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 04:13:13.000000 coglib-0.1.1/coglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 04:13:13.905079 coglib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-04-15 04:10:22.000000 coglib-0.1.1/setup.py
```

### Comparing `coglib-0.1.0/PKG-INFO` & `coglib-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.0/coglib/coglib.py` & `coglib-0.1.1/coglib/coglib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 from datetime import datetime
 import json
 from xmlrpc.client import boolean
 import requests
 import pandas as pd
-
+from typing import NewType
+EconDataList = NewType('EconDataList', list['EconData'])
+LoginResponse = NewType('LoginResponse','LoginResponse')
 class DataFeedAdaptor:   
     base_url='https://marketwatch.cogencis.com/v2/staging/analyticsapi/api/v2/'
     isConnected:boolean=False;
     token=None
     expiry=None
     headers={
             'Content-Type': 'application/json; charset=utf-8',
@@ -16,15 +18,15 @@
             'Accept-Language' : 'en-US,en;q=0.9,hi;q=0.8',
             'Accept-Encoding': 'gzip,deflate,br',
             'Referer': 'https://marketwatch.cogencis.com',
             }  
     def __init__(self):
         self
         
-    def login(self,username,password) -> None:
+    def login(self,username,password) -> LoginResponse:
         self.username=username
         self.password=password
         
         url = f"{self.base_url}login"        
         payload={'username':self.username, 'password':self.password}
       
         response = requests.post(url, data=json.dumps(payload),headers=self.headers)
@@ -39,29 +41,28 @@
                 
             return LoginResponse(resp)
       
         else:
             return response            
 
         
-    def get_econ_history(self,codes,as_dataframe=False):
+    def get_econ_history(self,codes,as_dataframe=False)->EconDataList:
         url = f"{self.base_url}econ/eventhistory?events={codes}&ccy=USD"        
         response = requests.get(url,headers=self.headers)
         output=[]
         if response.status_code == 200:
             json_data = response.json()['response']
             
             for obj in json_data:
                 output.append(EconData(obj,as_dataframe))
                
             return output                
         else:
             return response;
 
-
 class EconData:
     def __init__(self, data,as_dataframe=False):        
         self.baseunit=data['baseunit'];
         self.country=data['country'];
         self.countryCode=data['countryCode'];
         self.frequency=data['frequency'];
         self.name=data['name'];
```

### Comparing `coglib-0.1.0/coglib.egg-info/PKG-INFO` & `coglib-0.1.1/coglib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.0/setup.py` & `coglib-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='coglib',
-    version='0.1.0',
-    packages=find_packages(),
+    version='0.1.1',
+    packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://cogencis.com',
```

