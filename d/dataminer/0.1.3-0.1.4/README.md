# Comparing `tmp/dataminer-0.1.3.tar.gz` & `tmp/dataminer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataminer-0.1.3.tar", last modified: Fri Apr 12 03:34:49 2024, max compression
+gzip compressed data, was "dataminer-0.1.4.tar", last modified: Mon Apr 15 09:34:58 2024, max compression
```

## Comparing `dataminer-0.1.3.tar` & `dataminer-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.246152 dataminer-0.1.3/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-12 03:34:23.000000 dataminer-0.1.3/LICENSE
--rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-12 03:34:49.246152 dataminer-0.1.3/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/README.md
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/__init__.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer/datax/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/job_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/runner.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.246152 dataminer-0.1.3/dataminer/sqla/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1618 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/engine_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/query_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1443 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/table_helpers.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer.egg-info/
--rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      421 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/SOURCES.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/dependency_links.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       20 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/requires.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/top_level.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-12 03:34:49.246152 dataminer-0.1.3/setup.cfg
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      725 2024-04-12 03:34:23.000000 dataminer-0.1.3/setup.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-15 09:34:42.000000 dataminer-0.1.4/LICENSE
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-15 09:34:58.124333 dataminer-0.1.4/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/README.md
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.120333 dataminer-0.1.4/dataminer/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/__init__.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/dataminer/datax/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/job_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/runner.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/dataminer/sqla/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1618 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/engine_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1627 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/inspect_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/query_helpers.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.120333 dataminer-0.1.4/dataminer.egg-info/
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      423 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/SOURCES.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/dependency_links.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       20 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/requires.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/top_level.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-15 09:34:58.124333 dataminer-0.1.4/setup.cfg
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      725 2024-04-15 09:34:42.000000 dataminer-0.1.4/setup.py
```

### Comparing `dataminer-0.1.3/LICENSE` & `dataminer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.3/PKG-INFO` & `dataminer-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `dataminer-0.1.3/dataminer/datax/job_helpers.py` & `dataminer-0.1.4/dataminer/datax/job_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.3/dataminer/datax/runner.py` & `dataminer-0.1.4/dataminer/datax/runner.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.3/dataminer/sqla/engine_helpers.py` & `dataminer-0.1.4/dataminer/sqla/engine_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.3/dataminer.egg-info/PKG-INFO` & `dataminer-0.1.4/dataminer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `dataminer-0.1.3/setup.py` & `dataminer-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataminer',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'sqlalchemy',
         'oracledb',
     ],
     author='javaite',
     author_email='javaite@126.com',
```

