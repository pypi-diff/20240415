# Comparing `tmp/yplib-5.6.1.tar.gz` & `tmp/yplib-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-5.6.1.tar", last modified: Mon Apr 15 04:15:08 2024, max compression
+gzip compressed data, was "dist\yplib-5.6.2.tar", last modified: Mon Apr 15 06:53:06 2024, max compression
```

## Comparing `yplib-5.6.1.tar` & `yplib-5.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.699082 yplib-5.6.1/
--rw-rw-rw-   0        0        0      400 2024-04-15 04:15:08.699082 yplib-5.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 04:15:08.700086 yplib-5.6.1/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-15 04:14:06.000000 yplib-5.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.694119 yplib-5.6.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.1/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0    10190 2024-04-12 03:50:53.000000 yplib-5.6.1/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.1/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.1/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.698097 yplib-5.6.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 06:53:06.900908 yplib-5.6.2/
+-rw-rw-rw-   0        0        0      400 2024-04-15 06:53:06.900908 yplib-5.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:53:06.900908 yplib-5.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-15 06:52:52.000000 yplib-5.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:53:06.890045 yplib-5.6.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.2/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    10673 2024-04-15 06:52:21.000000 yplib-5.6.2/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.2/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:53:06.900908 yplib-5.6.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-15 06:53:05.000000 yplib-5.6.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-15 06:53:06.000000 yplib-5.6.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:53:05.000000 yplib-5.6.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 06:53:05.000000 yplib-5.6.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.1/setup.py` & `yplib-5.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.1",
+    version="5.6.2",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.1/yplib/__init__.py` & `yplib-5.6.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/chart.py` & `yplib-5.6.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/chart_html.py` & `yplib-5.6.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/db.py` & `yplib-5.6.2/yplib/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
 
 
 # 有关数据库操作的类
-def get_connect(database='MoneyKing', user='moneyking_uer', password='3^qp3Xqt4bG7', charset='utf8mb4', port=3306, host='192.168.40.230'):
+def get_connect(database=None, user=None, password=None, charset='utf8mb4', port=3306, host=None):
     return pymysql.connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
+def get_connect_from_config(db_config='stock_db', database=None, user=None, password=None, charset=None, port=None, host=None):
+    config_db = get_config_data(db_config)
+    database = database if database is not None else config_db['database']
+    user = user if user is not None else config_db['user']
+    host = host if host is not None else config_db['host']
+    password = password if password is not None else config_db['password']
+    port = port if port is not None else config_db['port'] if 'port' in config_db else 3306
+    charset = charset if charset is not None else config_db['charset'] if 'charset' in config_db else 'utf8mb4'
+    return get_connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
+
+
 # 执行 sql 语句, 并且提交, 默认值提交的了
-def exec_sql(sql='', db_conn=None, db_config='stock_db', commit=True, is_log=False):
-    if db_conn is None:
-        config_db = get_config_data(db_config)
-        db_conn = get_connect(database=config_db['database'], user=config_db['user'], password=config_db['password'], port=config_db['port'], host=config_db['host'])
-    if db_conn is None or sql is None or sql == '':
+def exec_sql(sql='', db_conn=None, db_config='stock_db', commit=True, is_log=False, database=None):
+    db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
+    if sql is None or sql == '':
         if is_log:
             to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     if isinstance(sql, list) or isinstance(sql, set):
         for s in sql:
             if is_log:
@@ -28,24 +37,22 @@
             to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
 
 # 执行 sql 语句, 不提交
-def exec_sql_un_commit(sql='', db_conn=None):
-    exec_sql(sql=sql, db_conn=db_conn, commit=False)
+def exec_sql_un_commit(sql='', db_conn=None, database=None):
+    exec_sql(sql=sql, db_conn=db_conn, commit=False, database=database)
 
 
 # 执行 sql 获得 数据
-def get_data_from_sql(sql='', db_conn=None, db_config='stock_db', is_log=False):
-    if db_conn is None:
-        config_db = get_config_data(db_config)
-        db_conn = get_connect(database=config_db['database'], user=config_db['user'], password=config_db['password'], port=config_db['port'], host=config_db['host'])
-    if db_conn is None or sql is None or sql == '':
+def get_data_from_sql(sql='', db_conn=None, db_config='stock_db', is_log=False, database=None):
+    db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
+    if sql is None or sql == '':
         if is_log:
             to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     if is_log:
         to_log_file(sql)
     db_cursor.execute(str(sql))
```

### Comparing `yplib-5.6.1/yplib/file.py` & `yplib-5.6.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/http_util.py` & `yplib-5.6.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/index.py` & `yplib-5.6.2/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/mail.py` & `yplib-5.6.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/mail_html.py` & `yplib-5.6.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.1/yplib/markdown.py` & `yplib-5.6.2/yplib/markdown.py`

 * *Files identical despite different names*

