# Comparing `tmp/xcloud_client-1.0.tar.gz` & `tmp/xcloud_client-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloud_client-1.0.tar", last modified: Sun Apr 14 06:54:15 2024, max compression
+gzip compressed data, was "xcloud_client-2.0.tar", last modified: Sun Apr 14 19:55:56 2024, max compression
```

## Comparing `xcloud_client-1.0.tar` & `xcloud_client-2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 06:54:15.085307 xcloud_client-1.0/
--rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      126 2024-04-14 06:54:15.083310 xcloud_client-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 06:54:15.048306 xcloud_client-1.0/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-1.0/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-1.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-1.0/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-1.0/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-1.0/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-1.0/resources/ojdbc14-10.2.0.4.0.jar
--rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-1.0/resources/slf4j-api-1.5.8.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-1.0/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-1.0/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-1.0/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0       42 2024-04-14 06:54:15.085307 xcloud_client-1.0/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-04-14 06:53:02.000000 xcloud_client-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:54:15.056308 xcloud_client-1.0/xcloud_client/
--rw-rw-rw-   0        0        0       23 2024-04-14 06:33:41.000000 xcloud_client-1.0/xcloud_client/__init__.py
--rw-rw-rw-   0        0        0     1717 2024-04-14 05:01:59.000000 xcloud_client-1.0/xcloud_client/xCloud_client.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:54:15.078308 xcloud_client-1.0/xcloud_client.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-14 06:54:13.000000 xcloud_client-1.0/xcloud_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-04-14 06:54:14.000000 xcloud_client-1.0/xcloud_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:54:14.000000 xcloud_client-1.0/xcloud_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 06:54:14.000000 xcloud_client-1.0/xcloud_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 06:54:14.000000 xcloud_client-1.0/xcloud_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 19:55:56.427209 xcloud_client-2.0/
+-rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      126 2024-04-14 19:55:56.426111 xcloud_client-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 19:55:56.397200 xcloud_client-2.0/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-2.0/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-2.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-2.0/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-2.0/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-2.0/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-2.0/resources/ojdbc14-10.2.0.4.0.jar
+-rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-2.0/resources/slf4j-api-1.5.8.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-2.0/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-2.0/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-2.0/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:55:56.427717 xcloud_client-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-04-14 19:55:26.000000 xcloud_client-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:55:56.403198 xcloud_client-2.0/xcloud_client/
+-rw-rw-rw-   0        0        0       23 2024-04-14 19:55:13.000000 xcloud_client-2.0/xcloud_client/__init__.py
+-rw-rw-rw-   0        0        0     1869 2024-04-14 19:53:30.000000 xcloud_client-2.0/xcloud_client/xCloud_client.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:55:56.422777 xcloud_client-2.0/xcloud_client.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-14 19:55:55.000000 xcloud_client-2.0/xcloud_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-04-14 19:55:56.000000 xcloud_client-2.0/xcloud_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 19:55:55.000000 xcloud_client-2.0/xcloud_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 19:55:55.000000 xcloud_client-2.0/xcloud_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 19:55:55.000000 xcloud_client-2.0/xcloud_client.egg-info/top_level.txt
```

### Comparing `xcloud_client-1.0/resources/XCloudJDBC-2.10.6.7.jar` & `xcloud_client-2.0/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloud_client-2.0/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/libthrift-0.9.2.jar` & `xcloud_client-2.0/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/log4j-1.2.17.jar` & `xcloud_client-2.0/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/lz4-1.3.0.jar` & `xcloud_client-2.0/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/ojdbc14-10.2.0.4.0.jar` & `xcloud_client-2.0/resources/ojdbc14-10.2.0.4.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/slf4j-api-1.5.8.jar` & `xcloud_client-2.0/resources/slf4j-api-1.5.8.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/slf4j-api-1.7.5.jar` & `xcloud_client-2.0/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/slf4j-log4j12-1.7.5.jar` & `xcloud_client-2.0/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/resources/slf4j-simple-1.7.5.jar` & `xcloud_client-2.0/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-1.0/xcloud_client/xCloud_client.py` & `xcloud_client-2.0/xcloud_client/xCloud_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,45 +2,49 @@
 
 class xCloud_client:
     def __init__(self, host, port, username, password):
         self.host = host
         self.port = port
         self.username = username
         self.password = password
+        self.conn = None
 
     def connect(self):
 
         try:
             """
             建立与数据库的连接
             """
             driver = 'com.bonc.xcloud.jdbc.XCloudDriver'
             #com\bonc\xcloud\jdbc
             url = 'jdbc:xcloud:@'+self.host+':'+self.port+'/SERVER_DATA?connectRetry=3&socketTimeOut=43200000&connectDirect=true&buffMemory=33554432'
             #user = config['acct_info']['user']  
             #password = config['acct_info']['password']
-            jarFile = ['XCloudJDBC-2.10.6.7.jar','slf4j-api-1.7.5.jar','slf4j-log4j12-1.7.5.jar','slf4j-simple-1.7.5.jar','log4j-1.2.17.jar','libthrift-0.9.2.jar',
-            'XCloudJDBC_SP_Procedure_Parser-0.1.3.jar'
-            ,'lz4-1.3.0.jar'
+            jarFile = ['resources/XCloudJDBC-2.10.6.7.jar','resources/slf4j-api-1.7.5.jar','resources/slf4j-log4j12-1.7.5.jar','resources/slf4j-simple-1.7.5.jar','resources/log4j-1.2.17.jar','resources/libthrift-0.9.2.jar',
+            'resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar'
+            ,'resources/lz4-1.3.0.jar'
             ]
             conn = jaydebeapi.connect(jclassname=driver, url=url, driver_args=[self.username, self.password], jars=jarFile)
             return conn
         except jaydebeapi.DatabaseError as e:
             print('the connection was not consistent ,because of {e}')
             raise
 
     def execute_query(self, query):
         """
         执行查询并返回结果
         """
-        conn = self.connect()
+        self.conn = self.connect()
         try:
-            with conn.cursor() as cursor:
+            with self.conn.cursor() as cursor:
                 cursor.execute(query)
                 result = cursor.fetchall()
         except jaydebeapi.Error as e:
             print(f"Error executing query: {e}")
             raise
         finally:
-            if conn:
-                conn.close()
+            if self.conn:
+                self.conn.close()
+            
         return result
+    
+
```

### Comparing `xcloud_client-1.0/xcloud_client.egg-info/SOURCES.txt` & `xcloud_client-2.0/xcloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

