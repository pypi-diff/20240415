# Comparing `tmp/xcloud_client-3.0.tar.gz` & `tmp/xcloud_client-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloud_client-3.0.tar", last modified: Mon Apr 15 03:03:16 2024, max compression
+gzip compressed data, was "xcloud_client-3.1.tar", last modified: Mon Apr 15 03:30:44 2024, max compression
```

## Comparing `xcloud_client-3.0.tar` & `xcloud_client-3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:16.382378 xcloud_client-3.0/
--rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      126 2024-04-15 03:03:16.381412 xcloud_client-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:16.354376 xcloud_client-3.0/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.0/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.0/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.0/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.0/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.0/resources/ojdbc14-10.2.0.4.0.jar
--rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.0/resources/slf4j-api-1.5.8.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.0/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.0/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.0/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0       42 2024-04-15 03:03:16.382378 xcloud_client-3.0/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-04-15 03:03:06.000000 xcloud_client-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:16.362378 xcloud_client-3.0/xcloud_client/
--rw-rw-rw-   0        0        0       23 2024-04-14 19:55:13.000000 xcloud_client-3.0/xcloud_client/__init__.py
--rw-rw-rw-   0        0        0     1730 2024-04-15 03:01:29.000000 xcloud_client-3.0/xcloud_client/xCloud_client.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:16.377376 xcloud_client-3.0/xcloud_client.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-15 03:03:15.000000 xcloud_client-3.0/xcloud_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-04-15 03:03:16.000000 xcloud_client-3.0/xcloud_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:03:15.000000 xcloud_client-3.0/xcloud_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 03:03:15.000000 xcloud_client-3.0/xcloud_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 03:03:15.000000 xcloud_client-3.0/xcloud_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 03:30:44.395371 xcloud_client-3.1/
+-rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      126 2024-04-15 03:30:44.394370 xcloud_client-3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 03:30:44.365177 xcloud_client-3.1/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.1/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.1/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.1/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.1/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.1/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.1/resources/ojdbc14-10.2.0.4.0.jar
+-rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.1/resources/slf4j-api-1.5.8.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.1/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.1/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.1/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:30:44.396372 xcloud_client-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-04-15 03:30:18.000000 xcloud_client-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:30:44.372762 xcloud_client-3.1/xcloud_client/
+-rw-rw-rw-   0        0        0       23 2024-04-15 03:30:26.000000 xcloud_client-3.1/xcloud_client/__init__.py
+-rw-rw-rw-   0        0        0     1774 2024-04-15 03:29:50.000000 xcloud_client-3.1/xcloud_client/xCloud_client.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:30:44.390370 xcloud_client-3.1/xcloud_client.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-15 03:30:43.000000 xcloud_client-3.1/xcloud_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-04-15 03:30:44.000000 xcloud_client-3.1/xcloud_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:30:43.000000 xcloud_client-3.1/xcloud_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 03:30:43.000000 xcloud_client-3.1/xcloud_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 03:30:43.000000 xcloud_client-3.1/xcloud_client.egg-info/top_level.txt
```

### Comparing `xcloud_client-3.0/resources/XCloudJDBC-2.10.6.7.jar` & `xcloud_client-3.1/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloud_client-3.1/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/libthrift-0.9.2.jar` & `xcloud_client-3.1/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/log4j-1.2.17.jar` & `xcloud_client-3.1/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/lz4-1.3.0.jar` & `xcloud_client-3.1/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/ojdbc14-10.2.0.4.0.jar` & `xcloud_client-3.1/resources/ojdbc14-10.2.0.4.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/slf4j-api-1.5.8.jar` & `xcloud_client-3.1/resources/slf4j-api-1.5.8.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/slf4j-api-1.7.5.jar` & `xcloud_client-3.1/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/slf4j-log4j12-1.7.5.jar` & `xcloud_client-3.1/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/resources/slf4j-simple-1.7.5.jar` & `xcloud_client-3.1/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.0/xcloud_client/xCloud_client.py` & `xcloud_client-3.1/xcloud_client/xCloud_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 current_path = Path.cwd()
 jar_files =[]
 for item in current_path.iterdir():
     if item.suffix =='.jar':
         jar_files.append(item.name)
-
+print(jar_files)
 class xCloud_client:
     def __init__(self, host, port, username, password):
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.conn = None
@@ -23,14 +23,15 @@
             """
             driver = 'com.bonc.xcloud.jdbc.XCloudDriver'
             #com\bonc\xcloud\jdbc
             url = 'jdbc:xcloud:@'+self.host+':'+self.port+'/SERVER_DATA?connectRetry=3&socketTimeOut=43200000&connectDirect=true&buffMemory=33554432'
             #user = config['acct_info']['user']  
             #password = config['acct_info']['password']
             jarFile = jar_files
+            print(jarFile)
             conn = jaydebeapi.connect(jclassname=driver, url=url, driver_args=[self.username, self.password], jars=jarFile)
             return conn
         except jaydebeapi.DatabaseError as e:
             print('the connection was not consistent ,because of {e}')
             raise
 
     def execute_query(self, query):
```

### Comparing `xcloud_client-3.0/xcloud_client.egg-info/SOURCES.txt` & `xcloud_client-3.1/xcloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

