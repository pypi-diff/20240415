# Comparing `tmp/resolutecns-0.0.6.tar.gz` & `tmp/resolutecns-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.6.tar", last modified: Mon Apr 15 17:28:43 2024, max compression
+gzip compressed data, was "resolutecns-0.0.7.tar", last modified: Mon Apr 15 17:36:31 2024, max compression
```

## Comparing `resolutecns-0.0.6.tar` & `resolutecns-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.959048 resolutecns-0.0.6/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:28:43.953059 resolutecns-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.923047 resolutecns-0.0.6/ResoluteCNS/
--rw-rw-rw-   0        0        0     3341 2024-04-15 17:28:10.000000 resolutecns-0.0.6/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.6/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:28:43.947319 resolutecns-0.0.6/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:28:43.000000 resolutecns-0.0.6/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:28:43.959048 resolutecns-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1052 2024-04-15 17:28:29.000000 resolutecns-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.909770 resolutecns-0.0.7/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:36:31.899770 resolutecns-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.845871 resolutecns-0.0.7/ResoluteCNS/
+-rw-rw-rw-   0        0        0     3405 2024-04-15 17:35:35.000000 resolutecns-0.0.7/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.7/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.891773 resolutecns-0.0.7/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:36:31.910780 resolutecns-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-04-15 17:36:18.000000 resolutecns-0.0.7/setup.py
```

### Comparing `resolutecns-0.0.6/PKG-INFO` & `resolutecns-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.6
+Version: 0.0.7
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.6/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.0.7/ResoluteCNS/ResoluteCNS.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 
 username = 'jdingman@resolutecommercial.com'
 password = 'ResComm!1'
 
 
 class CNS:
 
-    def __init__(self, opts):
+    def __init__(self):
         self._logged_in = False
         self._username = username
         self._password = password
-        self._opts = opts
+        self._opts = FirefoxOptions()
         self._ublock_path = os.path.join(os.path.dirname(__file__), 'uBlock0.xpi')
         
 
     def login(self):
         self._driver = webdriver.Firefox(options=self._opts)
         self._driver.install_addon(self._ublock_path, temporary=True)
         self._baseurl = "https://cnsplus.courthousenews.com/"
+        self._driver.get(self._baseurl)
         print('Logging in')
         username_field = self._driver.find_element(By.ID, 'UserName')
         username_field.send_keys(username)
         time.sleep(2)
         password_field = self._driver.find_element(By.ID, 'Password')
         password_field.send_keys(password)
         time.sleep(2)
@@ -41,28 +42,29 @@
         #time.sleep(10)
         self._logged_in = True
         print('Logged in')
 
     def get_bankruptcies(self, courts, from_date, to_date):
         if not self._logged_in:
             self.login()
-            
+
         #URL of the website     
         url = self._baseurl + "SearchBeta/Bankruptcy"
         self._driver.get(url)
-        self.setup_filters(courts, from_date, to_date)
+        self.setup_date_filters(from_date, to_date)
+        self.setup_court_filters(courts)
         self.click_search()
         return self.download_excel()
-        
-    def setup_filters(self, in_courts, from_date, to_date):
-
+    
+    def setup_date_filters(self, from_date, to_date):
         from_date_field = self._driver.find_element(By.CLASS_NAME, 'datepicker')
         from_date_field.send_keys(from_date)
+        
+    def setup_court_filters(self, in_courts):
 
-        #driver.find_elements(By.NAME, 'BankoCourts')
         courts = self._driver.find_elements(By.XPATH, "//input[@name='BankoCourts']/following-sibling::label")
 
         for court in courts:
             if self.validate_court(in_courts, court):
                 court_check = self._driver.find_element(By.ID, court.get_attribute('for'))
                 court_check.click()
```

### Comparing `resolutecns-0.0.6/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.0.7/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.6
+Version: 0.0.7
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.6/setup.py` & `resolutecns-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

