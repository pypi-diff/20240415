# Comparing `tmp/pymysqls-0.4.tar.gz` & `tmp/pymysqls-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysqls-0.4.tar", last modified: Mon Apr 15 14:42:54 2024, max compression
+gzip compressed data, was "pymysqls-0.5.tar", last modified: Mon Apr 15 14:45:35 2024, max compression
```

## Comparing `pymysqls-0.4.tar` & `pymysqls-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.550709 pymysqls-0.4/
--rw-rw-rw-   0        0        0       53 2024-04-15 14:42:54.548593 pymysqls-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.535412 pymysqls-0.4/pymysqls/
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.542024 pymysqls-0.4/pymysqls/DB/
--rw-rw-rw-   0        0        0      755 2024-04-15 14:28:01.000000 pymysqls-0.4/pymysqls/DB/DB.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:27:43.000000 pymysqls-0.4/pymysqls/DB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.545600 pymysqls-0.4/pymysqls/OTHER/
--rw-rw-rw-   0        0        0     8287 2024-04-15 14:26:43.000000 pymysqls-0.4/pymysqls/OTHER/MAIN.iu.py
--rw-rw-rw-   0        0        0     2143 2024-04-15 10:24:40.000000 pymysqls-0.4/pymysqls/OTHER/TESTW.iu.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:37:45.000000 pymysqls-0.4/pymysqls/OTHER/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.548593 pymysqls-0.4/pymysqls/TESTS/
--rw-rw-rw-   0        0        0     2869 2024-04-15 14:38:41.000000 pymysqls-0.4/pymysqls/TESTS/MAIN.py
--rw-rw-rw-   0        0        0      788 2024-04-15 14:39:04.000000 pymysqls-0.4/pymysqls/TESTS/TESTW.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:34:46.000000 pymysqls-0.4/pymysqls/TESTS/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:07:07.000000 pymysqls-0.4/pymysqls/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:42:54.539979 pymysqls-0.4/pymysqls.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 14:42:54.000000 pymysqls-0.4/pymysqls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 14:42:54.550709 pymysqls-0.4/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-04-15 14:31:17.000000 pymysqls-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.833153 pymysqls-0.5/
+-rw-rw-rw-   0        0        0       53 2024-04-15 14:45:35.832034 pymysqls-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.817043 pymysqls-0.5/pymysqls/
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.824670 pymysqls-0.5/pymysqls/DB/
+-rw-rw-rw-   0        0        0      755 2024-04-15 14:28:01.000000 pymysqls-0.5/pymysqls/DB/DB.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:27:43.000000 pymysqls-0.5/pymysqls/DB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.827289 pymysqls-0.5/pymysqls/OTHER/
+-rw-rw-rw-   0        0        0     8287 2024-04-15 14:26:43.000000 pymysqls-0.5/pymysqls/OTHER/MAIN.iu.py
+-rw-rw-rw-   0        0        0     2143 2024-04-15 10:24:40.000000 pymysqls-0.5/pymysqls/OTHER/TESTW.iu.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:37:45.000000 pymysqls-0.5/pymysqls/OTHER/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.830927 pymysqls-0.5/pymysqls/TESTS/
+-rw-rw-rw-   0        0        0     2869 2024-04-15 14:38:41.000000 pymysqls-0.5/pymysqls/TESTS/MAIN.py
+-rw-rw-rw-   0        0        0      788 2024-04-15 14:39:04.000000 pymysqls-0.5/pymysqls/TESTS/TESTW.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:34:46.000000 pymysqls-0.5/pymysqls/TESTS/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:07:07.000000 pymysqls-0.5/pymysqls/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:45:35.822646 pymysqls-0.5/pymysqls.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-04-15 14:45:35.000000 pymysqls-0.5/pymysqls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-04-15 14:45:35.000000 pymysqls-0.5/pymysqls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:45:35.000000 pymysqls-0.5/pymysqls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-15 14:45:35.000000 pymysqls-0.5/pymysqls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 14:45:35.000000 pymysqls-0.5/pymysqls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:45:35.833153 pymysqls-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      255 2024-04-15 14:45:32.000000 pymysqls-0.5/setup.py
```

### Comparing `pymysqls-0.4/pymysqls/DB/DB.py` & `pymysqls-0.5/pymysqls/DB/DB.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.4/pymysqls/OTHER/MAIN.iu.py` & `pymysqls-0.5/pymysqls/OTHER/MAIN.iu.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.4/pymysqls/OTHER/TESTW.iu.py` & `pymysqls-0.5/pymysqls/OTHER/TESTW.iu.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.4/pymysqls/TESTS/MAIN.py` & `pymysqls-0.5/pymysqls/TESTS/MAIN.py`

 * *Files identical despite different names*

### Comparing `pymysqls-0.4/pymysqls/TESTS/TESTW.py` & `pymysqls-0.5/pymysqls/TESTS/TESTW.py`

 * *Files identical despite different names*

