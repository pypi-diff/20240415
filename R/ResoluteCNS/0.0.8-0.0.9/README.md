# Comparing `tmp/resolutecns-0.0.8.tar.gz` & `tmp/resolutecns-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.8.tar", last modified: Mon Apr 15 17:47:32 2024, max compression
+gzip compressed data, was "resolutecns-0.0.9.tar", last modified: Mon Apr 15 18:05:14 2024, max compression
```

## Comparing `resolutecns-0.0.8.tar` & `resolutecns-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.516186 resolutecns-0.0.8/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:47:32.510184 resolutecns-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.484184 resolutecns-0.0.8/ResoluteCNS/
--rw-rw-rw-   0        0        0     3422 2024-04-15 17:46:05.000000 resolutecns-0.0.8/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.8/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.507187 resolutecns-0.0.8/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:47:32.516186 resolutecns-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1052 2024-04-15 17:47:27.000000 resolutecns-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.997681 resolutecns-0.0.9/
+-rw-rw-rw-   0        0        0      553 2024-04-15 18:05:13.991682 resolutecns-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.957683 resolutecns-0.0.9/ResoluteCNS/
+-rw-rw-rw-   0        0        0     3460 2024-04-15 18:04:44.000000 resolutecns-0.0.9/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.9/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.985680 resolutecns-0.0.9/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 18:05:13.998679 resolutecns-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-04-15 18:04:50.000000 resolutecns-0.0.9/setup.py
```

### Comparing `resolutecns-0.0.8/PKG-INFO` & `resolutecns-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.8
+Version: 0.0.9
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.8/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.0.9/ResoluteCNS/ResoluteCNS.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 import time
 import pandas as pd
 import platform
 from os.path import expanduser
 import os
 import urllib
 from datetime import datetime
+from pkg_resources import resource_filename
 
 username = 'jdingman@resolutecommercial.com'
 password = 'ResComm!1'
 
 
 class CNS:
 
     def __init__(self):
         self._logged_in = False
         self._username = username
         self._password = password
         self._opts = FirefoxOptions()
-        self._ublock_path = os.path.join(os.path.dirname(__file__), 'uBlock0.xpi')
+        self._ublock_path = resource_filename('ResoluteCNS', 'uBlock0.xpi')
         
 
     def login(self):
         self._driver = webdriver.Firefox(options=self._opts)
         self._driver.install_addon(self._ublock_path, temporary=True)
         self._baseurl = "https://cnsplus.courthousenews.com/"
         self._driver.get(self._baseurl)
@@ -37,16 +38,16 @@
         password_field = self._driver.find_element(By.ID, 'Password')
         password_field.send_keys(password)
         time.sleep(2)
         login_button = self._driver.find_element(By.CLASS_NAME, 'submitbutton')
         login_button.click()
         #time.sleep(10)
         self._logged_in = True
-        return self._logged_in
         print('Logged in')
+        return self._logged_in
 
     def get_bankruptcies(self, courts, from_date, to_date):
         if not self._logged_in:
             self.login()
 
         #URL of the website     
         url = self._baseurl + "SearchBeta/Bankruptcy"
```

### Comparing `resolutecns-0.0.8/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.0.9/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.8
+Version: 0.0.9
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.8/setup.py` & `resolutecns-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

