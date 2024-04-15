# Comparing `tmp/eptools-8.8.1.tar.gz` & `tmp/eptools-8.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpd10gaxt0\eptools-8.8.1.tar", last modified: Thu Nov 23 10:51:38 2023, max compression
+gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpikib8_on\eptools-8.8.2.tar", last modified: Mon Apr 15 08:53:56 2024, max compression
```

## Comparing `eptools-8.8.1.tar` & `eptools-8.8.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools/
--rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.8.1/eptools/configuration.py
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools/db_connector/
--rw-rw-rw-   0        0        0     2131 2023-10-02 12:05:22.000000 eptools-8.8.1/eptools/db_connector/connection_factory.py
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools/db_connector/connectors/
--rw-rw-rw-   0        0        0      851 2023-10-02 12:47:48.000000 eptools-8.8.1/eptools/db_connector/connectors/mysql_connector.py
--rw-rw-rw-   0        0        0      436 2023-10-02 12:37:45.000000 eptools-8.8.1/eptools/db_connector/connectors/sql_server_connector.py
--rw-rw-rw-   0        0        0       97 2023-09-20 13:42:04.000000 eptools-8.8.1/eptools/db_connector/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools/db_connector/credentials/
--rw-rw-rw-   0        0        0     1954 2023-10-02 12:37:30.000000 eptools-8.8.1/eptools/db_connector/credentials/config_provider.py
--rw-rw-rw-   0        0        0      164 2023-10-02 12:46:10.000000 eptools-8.8.1/eptools/db_connector/credentials/credential_provider.py
--rw-rw-rw-   0        0        0     2304 2023-10-02 12:36:25.000000 eptools-8.8.1/eptools/db_connector/credentials/env_provider.py
--rw-rw-rw-   0        0        0      162 2023-10-02 12:45:08.000000 eptools-8.8.1/eptools/db_connector/credentials/__init__.py
--rw-rw-rw-   0        0        0     3744 2023-10-02 12:50:44.000000 eptools-8.8.1/eptools/db_connector/database_manager.py
--rw-rw-rw-   0        0        0       96 2023-09-20 14:53:49.000000 eptools-8.8.1/eptools/db_connector/__init__.py
--rw-rw-rw-   0        0        0     6382 2023-09-21 14:32:53.000000 eptools-8.8.1/eptools/InvoiceDate.py
--rw-rw-rw-   0        0        0    10240 2023-10-06 09:56:41.000000 eptools-8.8.1/eptools/logger.py
--rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.8.1/eptools/mail_factory.py
--rw-rw-rw-   0        0        0    19536 2023-08-18 13:09:40.000000 eptools-8.8.1/eptools/SalesForceApiIntegration.py
--rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.8.1/eptools/sf_factory.py
--rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.8.1/eptools/slacker.py
--rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.8.1/eptools/slack_factory.py
--rw-rw-rw-   0        0        0    13207 2023-10-06 10:01:07.000000 eptools-8.8.1/eptools/SQLFactory.py
--rw-rw-rw-   0        0        0    31142 2023-11-23 10:48:08.000000 eptools-8.8.1/eptools/WindowsServiceBase.py
--rw-rw-rw-   0        0        0        0 2023-09-20 14:53:33.000000 eptools-8.8.1/eptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      929 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      939 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-11-23 10:51:38.000000 eptools-8.8.1/eptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.8.1/LICENSE
--rw-rw-rw-   0        0        0      929 2023-11-23 10:51:38.000000 eptools-8.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.8.1/pyproject.toml
--rw-rw-rw-   0        0        0      485 2023-05-16 11:41:56.000000 eptools-8.8.1/README.md
--rw-rw-rw-   0        0        0      571 2023-11-23 10:51:38.000000 eptools-8.8.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/eptools/
+-rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.8.2/eptools/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/eptools/db_connector/
+-rw-rw-rw-   0        0        0     2131 2023-10-02 12:05:22.000000 eptools-8.8.2/eptools/db_connector/connection_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/eptools/db_connector/connectors/
+-rw-rw-rw-   0        0        0      851 2023-10-02 12:47:48.000000 eptools-8.8.2/eptools/db_connector/connectors/mysql_connector.py
+-rw-rw-rw-   0        0        0      436 2023-10-02 12:37:45.000000 eptools-8.8.2/eptools/db_connector/connectors/sql_server_connector.py
+-rw-rw-rw-   0        0        0       97 2023-09-20 13:42:04.000000 eptools-8.8.2/eptools/db_connector/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/eptools/db_connector/credentials/
+-rw-rw-rw-   0        0        0     1954 2023-10-02 12:37:30.000000 eptools-8.8.2/eptools/db_connector/credentials/config_provider.py
+-rw-rw-rw-   0        0        0      164 2023-10-02 12:46:10.000000 eptools-8.8.2/eptools/db_connector/credentials/credential_provider.py
+-rw-rw-rw-   0        0        0     2304 2023-10-02 12:36:25.000000 eptools-8.8.2/eptools/db_connector/credentials/env_provider.py
+-rw-rw-rw-   0        0        0      162 2024-01-04 07:58:53.000000 eptools-8.8.2/eptools/db_connector/credentials/__init__.py
+-rw-rw-rw-   0        0        0     3744 2023-10-02 12:50:44.000000 eptools-8.8.2/eptools/db_connector/database_manager.py
+-rw-rw-rw-   0        0        0       96 2023-09-20 14:53:49.000000 eptools-8.8.2/eptools/db_connector/__init__.py
+-rw-rw-rw-   0        0        0     6778 2024-04-15 08:51:38.000000 eptools-8.8.2/eptools/InvoiceDate.py
+-rw-rw-rw-   0        0        0    10240 2023-10-06 09:56:41.000000 eptools-8.8.2/eptools/logger.py
+-rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.8.2/eptools/mail_factory.py
+-rw-rw-rw-   0        0        0    19536 2023-08-18 13:09:40.000000 eptools-8.8.2/eptools/SalesForceApiIntegration.py
+-rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.8.2/eptools/sf_factory.py
+-rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.8.2/eptools/slacker.py
+-rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.8.2/eptools/slack_factory.py
+-rw-rw-rw-   0        0        0    13207 2023-10-06 10:01:07.000000 eptools-8.8.2/eptools/SQLFactory.py
+-rw-rw-rw-   0        0        0    31142 2023-11-23 10:48:08.000000 eptools-8.8.2/eptools/WindowsServiceBase.py
+-rw-rw-rw-   0        0        0        0 2023-09-20 14:53:33.000000 eptools-8.8.2/eptools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:56.000000 eptools-8.8.2/eptools.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:53:55.000000 eptools-8.8.2/eptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      929 2024-04-15 08:53:55.000000 eptools-8.8.2/eptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2024-04-15 08:53:55.000000 eptools-8.8.2/eptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      939 2024-04-15 08:53:55.000000 eptools-8.8.2/eptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 08:53:55.000000 eptools-8.8.2/eptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.8.2/LICENSE
+-rw-rw-rw-   0        0        0      929 2024-04-15 08:53:56.000000 eptools-8.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0      485 2023-05-16 11:41:56.000000 eptools-8.8.2/README.md
+-rw-rw-rw-   0        0        0      600 2024-04-15 08:53:56.000000 eptools-8.8.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.8.2/setup.py
```

### Comparing `eptools-8.8.1/eptools/configuration.py` & `eptools-8.8.2/eptools/configuration.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/db_connector/connection_factory.py` & `eptools-8.8.2/eptools/db_connector/connection_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/db_connector/connectors/mysql_connector.py` & `eptools-8.8.2/eptools/db_connector/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/db_connector/credentials/config_provider.py` & `eptools-8.8.2/eptools/db_connector/credentials/config_provider.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/db_connector/credentials/env_provider.py` & `eptools-8.8.2/eptools/db_connector/credentials/env_provider.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/db_connector/database_manager.py` & `eptools-8.8.2/eptools/db_connector/database_manager.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/InvoiceDate.py` & `eptools-8.8.2/eptools/InvoiceDate.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         return conn
     except Exception as ex:
         print("No Connection: " + str(ex))
         if retry < 3:
             return get_conn(retry=retry+1)
         return False
 
-
 def generate_dates(inputdate = None, customer_id =None, retry: int = 0,defaults=None,holidays_country='BE', logger = None):
     """
     Returns start and end of facturation date as datetimes or False, False if failed
 
     params:
     ----
     inputdate: 
@@ -132,16 +131,18 @@
         except Exception as ex:
             customer_id = 0
     sameday = (customer_id in defaults["samedaycustomers"])
 
     try:
         if holidays_country == "FR":
             holidays_list = holidays.France(years= inputdate.year)
+            holidays_list += holidays.France(years= inputdate.year + 1)
         else:
             holidays_list = holidays.Belgium(years= inputdate.year)
+            holidays_list += holidays.Belgium(years= inputdate.year + 1)
         cutoff = datetime.strptime('00:00:00.000','%H:%M:%S.%f')
         if not sameday:
             cutoff = defaults["cutoff"]
         
         fact_date = datetime.combine(inputdate.date(), cutoff.time())
         # 1 time calculate time before or after cutoff (after do nothing, before substract one)
         if inputdate.time() < cutoff.time():
@@ -160,13 +161,20 @@
     except Exception as ex:
             print(ex)
             if retry < 3:
                 return generate_dates(inputdate=inputdate,retry=retry+1, defaults=defaults)
             return False, False, defaults
 
 if __name__ == "__main__":
-    # input_date = datetime(2023, 5, 17, hour=17)
     input_date = datetime.now()
     dates = generate_dates(inputdate=input_date, customer_id=7255)
     print(f"Invoice date start and end for date '{input_date}'")
     print("-> Start invoice datetime:", dates[0])
-    print("-> End invoice datetime:", dates[1])
+    print("-> End invoice datetime:", dates[1])
+    
+    
+    input_date = datetime(2113, 12, 29, hour=17)
+    dates = generate_dates(inputdate=input_date, customer_id=7255)
+    print(f"Invoice date start and end for date '{input_date}'")
+    print("-> Start invoice datetime:", dates[0])
+    print("-> End invoice datetime:", dates[1])
+
```

### Comparing `eptools-8.8.1/eptools/logger.py` & `eptools-8.8.2/eptools/logger.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/mail_factory.py` & `eptools-8.8.2/eptools/mail_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/SalesForceApiIntegration.py` & `eptools-8.8.2/eptools/SalesForceApiIntegration.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/sf_factory.py` & `eptools-8.8.2/eptools/sf_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/slacker.py` & `eptools-8.8.2/eptools/slacker.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/slack_factory.py` & `eptools-8.8.2/eptools/slack_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/SQLFactory.py` & `eptools-8.8.2/eptools/SQLFactory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools/WindowsServiceBase.py` & `eptools-8.8.2/eptools/WindowsServiceBase.py`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/eptools.egg-info/PKG-INFO` & `eptools-8.8.2/eptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.8.1
+Version: 8.8.2
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.8.1/eptools.egg-info/SOURCES.txt` & `eptools-8.8.2/eptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/LICENSE` & `eptools-8.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eptools-8.8.1/PKG-INFO` & `eptools-8.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.8.1
+Version: 8.8.2
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.8.1/setup.cfg` & `eptools-8.8.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7074 6f6f 6c73 0d0a 7665 7273   = eptools..vers
-00000020: 696f 6e20 3d20 382e 382e 310d 0a61 7574  ion = 8.8.1..aut
+00000020: 696f 6e20 3d20 382e 382e 320d 0a61 7574  ion = 8.8.2..aut
 00000030: 686f 7220 3d20 4172 6e6f 2044 6520 4465  hor = Arno De De
 00000040: 636b 6572 0d0a 6175 7468 6f72 5f65 6d61  cker..author_ema
 00000050: 696c 203d 2061 726e 6f2e 6465 6465 636b  il = arno.dedeck
 00000060: 6572 4065 6173 7970 6f73 742e 6575 0d0a  er@easypost.eu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4561  description = Ea
 00000080: 7379 506f 7374 2054 6f6f 6c73 0d0a 6c6f  syPost Tools..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
@@ -26,11 +26,13 @@
 00000190: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
 000001a0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
 000001b0: 0d0a 0973 6c61 636b 2d73 646b 0d0a 0970  ...slack-sdk...p
 000001c0: 796f 6462 630d 0a09 686f 6c69 6461 7973  yodbc...holidays
 000001d0: 0d0a 094f 3336 350d 0a09 7369 6d70 6c65  ...O365...simple
 000001e0: 2d73 616c 6573 666f 7263 650d 0a09 7371  -salesforce...sq
 000001f0: 6c61 6c63 6865 6d79 0d0a 0972 6571 7565  lalchemy...reque
-00000200: 7374 730d 0a09 7079 6d79 7371 6c0d 0a0d  sts...pymysql...
-00000210: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000220: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000230: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000200: 7374 730d 0a09 7079 6d79 7371 6c0d 0a09  sts...pymysql...
+00000210: 7079 7069 7769 6e33 320d 0a09 7365 7276  pypiwin32...serv
+00000220: 6963 656d 616e 6167 6572 0d0a 0d0a 5b65  icemanager....[e
+00000230: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000240: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000250: 203d 2030 0d0a 0d0a                       = 0....
```

