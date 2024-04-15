# Comparing `tmp/dqc-toolkit-0.1.0b1.tar.gz` & `tmp/dqc_toolkit-0.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc-toolkit-0.1.0b1.tar", last modified: Sat Apr 13 04:47:16 2024, max compression
+gzip compressed data, was "dqc_toolkit-0.1.2b2.tar", last modified: Mon Apr 15 11:12:39 2024, max compression
```

## Comparing `dqc-toolkit-0.1.0b1.tar` & `dqc_toolkit-0.1.2b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.425813 dqc-toolkit-0.1.0b1/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc-toolkit-0.1.0b1/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-13 04:47:16.425176 dqc-toolkit-0.1.0b1/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc-toolkit-0.1.0b1/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.401839 dqc-toolkit-0.1.0b1/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1936 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)    11684 2024-04-12 11:34:46.000000 dqc-toolkit-0.1.0b1/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.411610 dqc-toolkit-0.1.0b1/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      277 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4893 2024-04-08 10:03:03.000000 dqc-toolkit-0.1.0b1/dqc/utils/_dataprocessing.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7543 2024-04-09 05:35:00.000000 dqc-toolkit-0.1.0b1/dqc/utils/_generic.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3258 2024-04-09 05:35:00.000000 dqc-toolkit-0.1.0b1/dqc/utils/_sklearn_artifacts.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.421625 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      414 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      306 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/top_level.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1624 2024-04-13 04:45:15.000000 dqc-toolkit-0.1.0b1/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-13 04:47:16.425985 dqc-toolkit-0.1.0b1/setup.cfg
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.419116 dqc-toolkit-0.1.0b1/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc-toolkit-0.1.0b1/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-08 17:00:40.000000 dqc-toolkit-0.1.0b1/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3084 2024-04-09 05:33:59.000000 dqc-toolkit-0.1.0b1/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:12:39.215680 dqc_toolkit-0.1.2b2/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.2b2/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-15 11:12:39.214887 dqc_toolkit-0.1.2b2/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.2b2/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:12:39.194905 dqc_toolkit-0.1.2b2/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc_toolkit-0.1.2b2/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1936 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    11684 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:12:39.202300 dqc_toolkit-0.1.2b2/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      277 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4893 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7543 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/utils/_generic.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3258 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/dqc/utils/_sklearn_artifacts.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:12:39.212191 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-15 11:12:39.000000 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      414 2024-04-15 11:12:39.000000 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-15 11:12:39.000000 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      306 2024-04-15 11:12:39.000000 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-15 11:12:39.000000 dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1624 2024-04-15 11:11:58.000000 dqc_toolkit-0.1.2b2/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-15 11:12:39.215967 dqc_toolkit-0.1.2b2/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:12:39.211037 dqc_toolkit-0.1.2b2/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc_toolkit-0.1.2b2/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3084 2024-04-14 20:06:23.000000 dqc_toolkit-0.1.2b2/tests/test_crossval.py
```

### Comparing `dqc-toolkit-0.1.0b1/LICENSE` & `dqc_toolkit-0.1.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/PKG-INFO` & `dqc_toolkit-0.1.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b1
+Version: 0.1.2b2
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dqc-toolkit-0.1.0b1/dqc/base.py` & `dqc_toolkit-0.1.2b2/dqc/base.py`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/dqc/crossval.py` & `dqc_toolkit-0.1.2b2/dqc/crossval.py`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/dqc/utils/_dataprocessing.py` & `dqc_toolkit-0.1.2b2/dqc/utils/_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/dqc/utils/_generic.py` & `dqc_toolkit-0.1.2b2/dqc/utils/_generic.py`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/dqc/utils/_sklearn_artifacts.py` & `dqc_toolkit-0.1.2b2/dqc/utils/_sklearn_artifacts.py`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/PKG-INFO` & `dqc_toolkit-0.1.2b2/dqc_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b1
+Version: 0.1.2b2
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dqc-toolkit-0.1.0b1/pyproject.toml` & `dqc_toolkit-0.1.2b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dqc-toolkit"
-version = "0.1.0-beta1"
+version = "0.1.2-beta2"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `dqc-toolkit-0.1.0b1/tests/test_crossval.py` & `dqc_toolkit-0.1.2b2/tests/test_crossval.py`

 * *Files identical despite different names*

