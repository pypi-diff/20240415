# Comparing `tmp/coglib-0.1.3.tar.gz` & `tmp/coglib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coglib-0.1.3.tar", last modified: Mon Apr 15 08:25:17 2024, max compression
+gzip compressed data, was "coglib-0.1.4.tar", last modified: Mon Apr 15 08:38:45 2024, max compression
```

## Comparing `coglib-0.1.3.tar` & `coglib-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.732686 coglib-0.1.3/
--rw-rw-rw-   0        0        0      548 2024-04-15 08:25:17.729687 coglib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.707651 coglib-0.1.3/coglib/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.3/coglib/__init__.py
--rw-rw-rw-   0        0        0     5574 2024-04-15 08:24:57.000000 coglib-0.1.3/coglib/coglib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:25:17.726686 coglib-0.1.3/coglib.egg-info/
--rw-rw-rw-   0        0        0      548 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 08:25:17.000000 coglib-0.1.3/coglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 08:25:17.732686 coglib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-15 08:25:11.000000 coglib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:38:45.210343 coglib-0.1.4/
+-rw-rw-rw-   0        0        0      548 2024-04-15 08:38:45.207322 coglib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:38:45.187320 coglib-0.1.4/coglib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.4/coglib/__init__.py
+-rw-rw-rw-   0        0        0     5444 2024-04-15 08:38:22.000000 coglib-0.1.4/coglib/coglib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:38:45.204318 coglib-0.1.4/coglib.egg-info/
+-rw-rw-rw-   0        0        0      548 2024-04-15 08:38:45.000000 coglib-0.1.4/coglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-15 08:38:45.000000 coglib-0.1.4/coglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:38:45.000000 coglib-0.1.4/coglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 08:38:45.000000 coglib-0.1.4/coglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 08:38:45.000000 coglib-0.1.4/coglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:38:45.211322 coglib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-04-15 08:38:38.000000 coglib-0.1.4/setup.py
```

### Comparing `coglib-0.1.3/PKG-INFO` & `coglib-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.3/coglib/coglib.py` & `coglib-0.1.4/coglib/coglib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
 from datetime import datetime
 import json
 from xmlrpc.client import boolean
 import requests
 import pandas as pd
 from typing import List, NewType
-EconDataList = NewType('EconDataList', List['EconData'])
-LoginResponse = NewType('LoginResponse','LoginResponse')
-cog_response=NewType("CogResponse",'CogResponse')
 class DataFeedAdaptor:   
     base_url='https://marketwatch.cogencis.com/v2/staging/analyticsapi/api/v2/'
     local_base_url='http://localhost:5051/api/v2/'
     isConnected:boolean=False;
     token=None
     expiry=None
     headers={
@@ -20,15 +17,15 @@
             'Accept-Language' : 'en-US,en;q=0.9,hi;q=0.8',
             'Accept-Encoding': 'gzip,deflate,br',
             'Referer': 'https://marketwatch.cogencis.com',
             }  
     def __init__(self):
         self
         
-    def login(self,username,password) -> LoginResponse:
+    def login(self,username,password):
         self.username=username
         self.password=password
         
         url = f"{self.base_url}login"        
         payload={'username':self.username, 'password':self.password}
       
         response = requests.post(url, data=json.dumps(payload),headers=self.headers)
@@ -42,15 +39,15 @@
                 self.headers['Authorization']=f"Bearer {self.token}"  
                 
             return LoginResponse(resp)
       
         else:
             return response            
         
-    def get_econ_timeseries(self,indicators:str,as_dataframe:boolean=True)->EconDataList:
+    def get_econ_timeseries(self,indicators:str,as_dataframe:boolean=True):
         url = f"{self.base_url}econ/eventhistory?events={indicators}&ccy=USD"        
         response = requests.get(url,headers=self.headers)
         output=[]
         if response.status_code == 200:
             json_data = response.json()['response']
             
             for obj in json_data:
@@ -64,15 +61,17 @@
             #return response;
 
     def get_financials(self,isin):
         qs=f"isin={isin}"
         response =self.get_command("equity/financials",qs)        
         if response.status_code==200:
             json_data=response.json()['response'];
-            return CogResponse(True,"Sucess",json_data)        
+            return CogResponse(True,"Sucess",json_data)
+        else:
+            return CogResponse(False,"Failed",response)    
 
     def get_timeseries(self,symbol:str,fields:str='open,high,low,close,volume,date,time',
     timescale:int=1440,pageSize:int=250,direction:str='backward',start:str=None,end:str=None,as_dataframe:boolean=True):        
         qs=f"symbol={symbol}&fields={fields}&timescale={timescale}&pageSize={pageSize}&direction={direction}"
         if start!=None:
             qs = f"{qs}&&from={start}"
```

### Comparing `coglib-0.1.3/coglib.egg-info/PKG-INFO` & `coglib-0.1.4/coglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.3/setup.py` & `coglib-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='coglib',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

