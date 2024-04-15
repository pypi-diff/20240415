# Comparing `tmp/resolutecns-0.0.7.tar.gz` & `tmp/resolutecns-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.7.tar", last modified: Mon Apr 15 17:36:31 2024, max compression
+gzip compressed data, was "resolutecns-0.0.8.tar", last modified: Mon Apr 15 17:47:32 2024, max compression
```

## Comparing `resolutecns-0.0.7.tar` & `resolutecns-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.909770 resolutecns-0.0.7/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:36:31.899770 resolutecns-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.845871 resolutecns-0.0.7/ResoluteCNS/
--rw-rw-rw-   0        0        0     3405 2024-04-15 17:35:35.000000 resolutecns-0.0.7/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.7/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:36:31.891773 resolutecns-0.0.7/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:36:31.000000 resolutecns-0.0.7/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 17:36:31.910780 resolutecns-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1052 2024-04-15 17:36:18.000000 resolutecns-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.516186 resolutecns-0.0.8/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:47:32.510184 resolutecns-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.484184 resolutecns-0.0.8/ResoluteCNS/
+-rw-rw-rw-   0        0        0     3422 2024-04-15 17:46:05.000000 resolutecns-0.0.8/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.8/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:47:32.507187 resolutecns-0.0.8/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:47:32.000000 resolutecns-0.0.8/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:47:32.516186 resolutecns-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-04-15 17:47:27.000000 resolutecns-0.0.8/setup.py
```

### Comparing `resolutecns-0.0.7/PKG-INFO` & `resolutecns-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.7
+Version: 0.0.8
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.7/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.0.8/ResoluteCNS/ResoluteCNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         password_field = self._driver.find_element(By.ID, 'Password')
         password_field.send_keys(password)
         time.sleep(2)
         login_button = self._driver.find_element(By.CLASS_NAME, 'submitbutton')
         login_button.click()
         #time.sleep(10)
         self._logged_in = True
+        return self._logged_in
         print('Logged in')
 
     def get_bankruptcies(self, courts, from_date, to_date):
         if not self._logged_in:
             self.login()
 
         #URL of the website     
@@ -60,27 +61,19 @@
         from_date_field.send_keys(from_date)
         
     def setup_court_filters(self, in_courts):
 
         courts = self._driver.find_elements(By.XPATH, "//input[@name='BankoCourts']/following-sibling::label")
 
         for court in courts:
-            if self.validate_court(in_courts, court):
+            if validate_court(in_courts, court):
                 court_check = self._driver.find_element(By.ID, court.get_attribute('for'))
                 court_check.click()
 
 
-    def validate_court(in_courts, court_to_check):
-        result = False
-        for c in in_courts:
-            if c == court_to_check.text:
-                result = True
-        return result
-
-
     def click_search(self):
         self._driver.find_element(By.ID, 'button_submitbanko').click()
 
     def download_excel(self):
         self._driver.set_page_load_timeout(10)
         try:
             self._driver.get('https://cnsplus.courthousenews.com/SearchBeta/GetBankoExcel')
@@ -98,7 +91,13 @@
     if platform.system() == "Darwin" or "Linux":
         return download_path + "/" + filename
     else:
         return download_path + "\\" + filename
 
 
 
+def validate_court(in_courts, court_to_check):
+        result = False
+        for c in in_courts:
+            if c == court_to_check.text:
+                result = True
+        return result
```

### Comparing `resolutecns-0.0.7/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.0.8/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.7
+Version: 0.0.8
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.7/setup.py` & `resolutecns-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

