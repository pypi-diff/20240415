# Comparing `tmp/resolutecns-0.0.5.tar.gz` & `tmp/resolutecns-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.5.tar", last modified: Mon Apr 15 17:12:45 2024, max compression
+gzip compressed data, was "resolutecns-0.0.6.tar", last modified: Mon Apr 15 17:28:43 2024, max compression
```

## Comparing `resolutecns-0.0.5.tar` & `resolutecns-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.368214 resolutecns-0.0.5/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:12:45.363213 resolutecns-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.336211 resolutecns-0.0.5/ResoluteCNS/
--rw-rw-rw-   0        0        0     3164 2024-04-15 17:09:41.000000 resolutecns-0.0.5/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.5/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:12:45.358215 resolutecns-0.0.5/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:12:45.000000 resolutecns-0.0.5/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:12:45.368214 resolutecns-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1052 2024-04-15 17:12:17.000000 resolutecns-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.959048 resolutecns-0.0.6/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:28:43.953059 resolutecns-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.923047 resolutecns-0.0.6/ResoluteCNS/
+-rw-rw-rw-   0        0        0     3341 2024-04-15 17:28:10.000000 resolutecns-0.0.6/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.6/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.947319 resolutecns-0.0.6/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:28:43.959048 resolutecns-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-04-15 17:28:29.000000 resolutecns-0.0.6/setup.py
```

### Comparing `resolutecns-0.0.5/PKG-INFO` & `resolutecns-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.5
+Version: 0.0.6
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.5/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.0.6/ResoluteCNS/ResoluteCNS.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,38 @@
 class CNS:
 
     def __init__(self, opts):
         self._logged_in = False
         self._username = username
         self._password = password
         self._opts = opts
-        self._driver = webdriver.Firefox(options=opts)
-        self._driver.install_addon('uBlock0.xpi', temporary=True)
-        self._baseurl = "https://cnsplus.courthousenews.com/"
+        self._ublock_path = os.path.join(os.path.dirname(__file__), 'uBlock0.xpi')
+        
 
     def login(self):
+        self._driver = webdriver.Firefox(options=self._opts)
+        self._driver.install_addon(self._ublock_path, temporary=True)
+        self._baseurl = "https://cnsplus.courthousenews.com/"
         print('Logging in')
         username_field = self._driver.find_element(By.ID, 'UserName')
         username_field.send_keys(username)
         time.sleep(2)
         password_field = self._driver.find_element(By.ID, 'Password')
         password_field.send_keys(password)
         time.sleep(2)
         login_button = self._driver.find_element(By.CLASS_NAME, 'submitbutton')
         login_button.click()
         #time.sleep(10)
         self._logged_in = True
         print('Logged in')
 
     def get_bankruptcies(self, courts, from_date, to_date):
+        if not self._logged_in:
+            self.login()
+            
         #URL of the website     
         url = self._baseurl + "SearchBeta/Bankruptcy"
         self._driver.get(url)
         self.setup_filters(courts, from_date, to_date)
         self.click_search()
         return self.download_excel()
```

### Comparing `resolutecns-0.0.5/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.0.6/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.5
+Version: 0.0.6
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.5/setup.py` & `resolutecns-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

