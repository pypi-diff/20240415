# Comparing `tmp/pymysqls-0.3.tar.gz` & `tmp/pymysqls-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysqls-0.3.tar", last modified: Fri Apr 12 17:35:00 2024, max compression
+gzip compressed data, was "pymysqls-0.4.tar", last modified: Mon Apr 15 14:42:54 2024, max compression
```

## Comparing `pymysqls-0.3.tar` & `pymysqls-0.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:35:00.311905 pymysqls-0.3/
--rw-rw-rw-   0        0        0       53 2024-04-12 17:35:00.310539 pymysqls-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 17:35:00.303989 pymysqls-0.3/pymysqls/
--rw-rw-rw-   0        0        0      388 2024-03-22 09:00:24.000000 pymysqls-0.3/pymysqls/ImportType.py
--rw-rw-rw-   0        0        0     2689 2024-03-22 09:48:40.000000 pymysqls-0.3/pymysqls/MainWindow.py
--rw-rw-rw-   0        0        0     1635 2024-03-22 09:00:24.000000 pymysqls-0.3/pymysqls/PieChartWindow.py
--rw-rw-rw-   0        0        0        0 2024-04-12 17:34:54.000000 pymysqls-0.3/pymysqls/__init__.py
--rw-rw-rw-   0        0        0      813 2024-02-20 21:06:39.000000 pymysqls-0.3/pymysqls/db.py
--rw-rw-rw-   0        0        0      949 2024-03-22 10:08:42.000000 pymysqls-0.3/pymysqls/db2.py
--rw-rw-rw-   0        0        0     4334 2024-03-22 09:45:06.000000 pymysqls-0.3/pymysqls/import_fles.py
--rw-rw-rw-   0        0        0      244 2024-04-12 17:26:40.000000 pymysqls-0.3/pymysqls/main.py
--rw-rw-rw-   0        0        0     1844 2024-04-12 17:26:34.000000 pymysqls-0.3/pymysqls/main2.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:35:00.308526 pymysqls-0.3/pymysqls.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-12 17:35:00.000000 pymysqls-0.3/pymysqls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-12 17:35:00.000000 pymysqls-0.3/pymysqls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:35:00.000000 pymysqls-0.3/pymysqls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 17:35:00.000000 pymysqls-0.3/pymysqls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 17:35:00.000000 pymysqls-0.3/pymysqls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 17:35:00.311905 pymysqls-0.3/setup.cfg
--rw-rw-rw-   0        0        0      215 2024-04-12 17:33:39.000000 pymysqls-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.550709 pymysqls-0.4/
+-rw-rw-rw-   0        0        0       53 2024-04-15 14:42:54.548593 pymysqls-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.535412 pymysqls-0.4/pymysqls/
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.542024 pymysqls-0.4/pymysqls/DB/
+-rw-rw-rw-   0        0        0      755 2024-04-15 14:28:01.000000 pymysqls-0.4/pymysqls/DB/DB.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:27:43.000000 pymysqls-0.4/pymysqls/DB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.545600 pymysqls-0.4/pymysqls/OTHER/
+-rw-rw-rw-   0        0        0     8287 2024-04-15 14:26:43.000000 pymysqls-0.4/pymysqls/OTHER/MAIN.iu.py
+-rw-rw-rw-   0        0        0     2143 2024-04-15 10:24:40.000000 pymysqls-0.4/pymysqls/OTHER/TESTW.iu.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:37:45.000000 pymysqls-0.4/pymysqls/OTHER/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.548593 pymysqls-0.4/pymysqls/TESTS/
+-rw-rw-rw-   0        0        0     2869 2024-04-15 14:38:41.000000 pymysqls-0.4/pymysqls/TESTS/MAIN.py
+-rw-rw-rw-   0        0        0      788 2024-04-15 14:39:04.000000 pymysqls-0.4/pymysqls/TESTS/TESTW.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:34:46.000000 pymysqls-0.4/pymysqls/TESTS/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:07:07.000000 pymysqls-0.4/pymysqls/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.539979 pymysqls-0.4/pymysqls.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:42:54.550709 pymysqls-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-04-15 14:31:17.000000 pymysqls-0.4/setup.py
```

### Comparing `pymysqls-0.3/pymysqls/db.py` & `pymysqls-0.4/pymysqls/DB/DB.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-import mysql.connector
-
-host = '46.188.59.18'
-user = 'service_yvu'
-password = 'd1Ha6rmu5Q/eDOwZ'
-database = 'service_yvu'
+import pymysql
 
 
 class DB:
     def __init__(self):
-        self.con = self.connect_to_mysql()
+        self.cursor = None
+        self.connection = None
+        self.connect()
+
+    def connect(self):
+        self.connection = pymysql.connect(host="127.0.0.1", user="root", passwd="root", db="main", charset="utf8")
+        self.cursor = self.connection.cursor()
+
+    def get(self, name, table):
+        self.cursor.execute(f"SELECT * FROM `{table}` WHERE `name` = '{name}';")
+        return self.cursor.fetchone()
+
+    def insert(self, table, into, values):
+        self.cursor.execute(f"INSERT INTO `{table}`({','.join(into)}) VALUES ({','.join(values)})")
+        self.connection.commit()
 
     def __del__(self):
-        if self.con is not None:
-            print("Отключение от БД...")
-            self.con.close()
-
-    def connect_to_mysql(self):
-        try:
-            connection = mysql.connector.connect(
-                host=host,
-                user=user,
-                password=password,
-                database=database
-            )
-            print("Подключение к БД...")
-            return connection
-        except Exception as e:
-            print("Ошибка при подключении.", e)
-            return None
+        self.cursor.close()
+        self.connection.close()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

