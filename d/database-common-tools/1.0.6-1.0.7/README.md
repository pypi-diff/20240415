# Comparing `tmp/database-common-tools-1.0.6.tar.gz` & `tmp/database-common-tools-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.0.6.tar", last modified: Thu Mar 14 06:55:47 2024, max compression
+gzip compressed data, was "database-common-tools-1.0.7.tar", last modified: Mon Apr 15 02:57:38 2024, max compression
```

## Comparing `database-common-tools-1.0.6.tar` & `database-common-tools-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-03-14 06:55:47.097587 database-common-tools-1.0.6/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.6/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-03-14 06:55:47.097116 database-common-tools-1.0.6/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.6/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-03-14 06:55:47.089183 database-common-tools-1.0.6/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-03-14 06:55:47.000000 database-common-tools-1.0.6/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      547 2024-03-14 06:55:47.000000 database-common-tools-1.0.6/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-03-14 06:55:47.000000 database-common-tools-1.0.6/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       56 2024-03-14 06:55:47.000000 database-common-tools-1.0.6/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-03-14 06:55:47.000000 database-common-tools-1.0.6/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-03-14 06:55:47.095462 database-common-tools-1.0.6/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.6/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.6/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     1173 2024-01-24 09:06:09.000000 database-common-tools-1.0.6/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.6/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     2806 2024-01-26 08:20:48.000000 database-common-tools-1.0.6/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.6/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.6/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.6/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.6/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-03-14 06:55:47.097744 database-common-tools-1.0.6/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3889 2024-03-14 06:55:32.000000 database-common-tools-1.0.6/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-03-14 06:55:47.096568 database-common-tools-1.0.6/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.6/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.515877 database-common-tools-1.0.7/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.7/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-15 02:57:38.515358 database-common-tools-1.0.7/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.7/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.506814 database-common-tools-1.0.7/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      578 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       64 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.514295 database-common-tools-1.0.7/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.7/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1173 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2806 2024-01-26 08:20:48.000000 database-common-tools-1.0.7/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.7/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.7/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.7/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.7/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.7/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-15 02:57:38.516065 database-common-tools-1.0.7/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3904 2024-04-15 02:56:21.000000 database-common-tools-1.0.7/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.514838 database-common-tools-1.0.7/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.7/test/__init__.py
```

### Comparing `database-common-tools-1.0.6/LICENSE` & `database-common-tools-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/PKG-INFO` & `database-common-tools-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.6/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.0.7/database_common_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.6/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.0.7/database_common_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 databasetools/analysis_json.py
 databasetools/analysis_json_v2.py
 databasetools/data_analysis.py
 databasetools/data_analysis_v2.py
 databasetools/kafka_connect.py
 databasetools/mongo_connect.py
 databasetools/mt_wx_message.py
+databasetools/mysql_connect.py
 databasetools/redis_connect.py
 test/__init__.py
```

### Comparing `database-common-tools-1.0.6/databasetools/__init__.py` & `database-common-tools-1.0.7/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/analysis_json.py` & `database-common-tools-1.0.7/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/analysis_json_v2.py` & `database-common-tools-1.0.7/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/data_analysis.py` & `database-common-tools-1.0.7/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/data_analysis_v2.py` & `database-common-tools-1.0.7/databasetools/data_analysis_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/mongo_connect.py` & `database-common-tools-1.0.7/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/mt_wx_message.py` & `database-common-tools-1.0.7/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/databasetools/redis_connect.py` & `database-common-tools-1.0.7/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.6/setup.py` & `database-common-tools-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
     'setuptools',
-    'kafka-python'
+    'kafka-python',
+    'pymysql'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

