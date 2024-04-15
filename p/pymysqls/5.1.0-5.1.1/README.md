# Comparing `tmp/pymysqls-5.1.0.tar.gz` & `tmp/pymysqls-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymysqls-5.1.0.tar", last modified: Mon Apr 15 14:47:46 2024, max compression
+gzip compressed data, was "pymysqls-5.1.1.tar", last modified: Mon Apr 15 14:52:11 2024, max compression
```

## Comparing `pymysqls-5.1.0.tar` & `pymysqls-5.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.064962 pymysqls-5.1.0/
--rw-rw-rw-   0        0        0       55 2024-04-15 14:47:46.062968 pymysqls-5.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.048598 pymysqls-5.1.0/pymysqls/
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.056543 pymysqls-5.1.0/pymysqls/DB/
--rw-rw-rw-   0        0        0      755 2024-04-15 14:28:01.000000 pymysqls-5.1.0/pymysqls/DB/DB.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:27:43.000000 pymysqls-5.1.0/pymysqls/DB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.059046 pymysqls-5.1.0/pymysqls/OTHER/
--rw-rw-rw-   0        0        0     8287 2024-04-15 14:26:43.000000 pymysqls-5.1.0/pymysqls/OTHER/MAIN.iu.py
--rw-rw-rw-   0        0        0     2143 2024-04-15 10:24:40.000000 pymysqls-5.1.0/pymysqls/OTHER/TESTW.iu.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:37:45.000000 pymysqls-5.1.0/pymysqls/OTHER/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.061962 pymysqls-5.1.0/pymysqls/TESTS/
--rw-rw-rw-   0        0        0     2869 2024-04-15 14:38:41.000000 pymysqls-5.1.0/pymysqls/TESTS/MAIN.py
--rw-rw-rw-   0        0        0      788 2024-04-15 14:39:04.000000 pymysqls-5.1.0/pymysqls/TESTS/TESTW.py
--rw-rw-rw-   0        0        0        0 2024-04-15 14:34:46.000000 pymysqls-5.1.0/pymysqls/TESTS/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:07:07.000000 pymysqls-5.1.0/pymysqls/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:47:46.054543 pymysqls-5.1.0/pymysqls.egg-info/
--rw-rw-rw-   0        0        0       55 2024-04-15 14:47:45.000000 pymysqls-5.1.0/pymysqls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2024-04-15 14:47:46.000000 pymysqls-5.1.0/pymysqls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:47:45.000000 pymysqls-5.1.0/pymysqls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-15 14:47:45.000000 pymysqls-5.1.0/pymysqls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 14:47:45.000000 pymysqls-5.1.0/pymysqls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 14:47:46.064962 pymysqls-5.1.0/setup.cfg
--rw-rw-rw-   0        0        0      257 2024-04-15 14:47:36.000000 pymysqls-5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.847972 pymysqls-5.1.1/
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:52:11.846976 pymysqls-5.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.830816 pymysqls-5.1.1/pymysqls/
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.840407 pymysqls-5.1.1/pymysqls/DB/
+-rw-rw-rw-   0        0        0      755 2024-04-15 14:28:01.000000 pymysqls-5.1.1/pymysqls/DB/DB.py
+-rw-rw-rw-   0        0        0      908 2024-04-15 14:51:51.000000 pymysqls-5.1.1/pymysqls/DB/ST.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:27:43.000000 pymysqls-5.1.1/pymysqls/DB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.842956 pymysqls-5.1.1/pymysqls/OTHER/
+-rw-rw-rw-   0        0        0     8287 2024-04-15 14:26:43.000000 pymysqls-5.1.1/pymysqls/OTHER/MAIN.iu.py
+-rw-rw-rw-   0        0        0     2143 2024-04-15 10:24:40.000000 pymysqls-5.1.1/pymysqls/OTHER/TESTW.iu.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:37:45.000000 pymysqls-5.1.1/pymysqls/OTHER/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.845947 pymysqls-5.1.1/pymysqls/TESTS/
+-rw-rw-rw-   0        0        0     2869 2024-04-15 14:38:41.000000 pymysqls-5.1.1/pymysqls/TESTS/MAIN.py
+-rw-rw-rw-   0        0        0      788 2024-04-15 14:39:04.000000 pymysqls-5.1.1/pymysqls/TESTS/TESTW.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 14:34:46.000000 pymysqls-5.1.1/pymysqls/TESTS/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:07:07.000000 pymysqls-5.1.1/pymysqls/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:11.837391 pymysqls-5.1.1/pymysqls.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:52:11.000000 pymysqls-5.1.1/pymysqls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-15 14:52:11.000000 pymysqls-5.1.1/pymysqls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:52:11.000000 pymysqls-5.1.1/pymysqls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-15 14:52:11.000000 pymysqls-5.1.1/pymysqls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 14:52:11.000000 pymysqls-5.1.1/pymysqls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:52:11.847972 pymysqls-5.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      257 2024-04-15 14:52:06.000000 pymysqls-5.1.1/setup.py
```

### Comparing `pymysqls-5.1.0/pymysqls/DB/DB.py` & `pymysqls-5.1.1/pymysqls/DB/DB.py`

 * *Files identical despite different names*

### Comparing `pymysqls-5.1.0/pymysqls/OTHER/MAIN.iu.py` & `pymysqls-5.1.1/pymysqls/OTHER/MAIN.iu.py`

 * *Files identical despite different names*

### Comparing `pymysqls-5.1.0/pymysqls/OTHER/TESTW.iu.py` & `pymysqls-5.1.1/pymysqls/OTHER/TESTW.iu.py`

 * *Files identical despite different names*

### Comparing `pymysqls-5.1.0/pymysqls/TESTS/MAIN.py` & `pymysqls-5.1.1/pymysqls/TESTS/MAIN.py`

 * *Files identical despite different names*

### Comparing `pymysqls-5.1.0/pymysqls/TESTS/TESTW.py` & `pymysqls-5.1.1/pymysqls/TESTS/TESTW.py`

 * *Files identical despite different names*

