# Comparing `tmp/dqc_toolkit-0.1.0b2.tar.gz` & `tmp/dqc_toolkit-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc_toolkit-0.1.0b2.tar", last modified: Mon Apr 15 11:57:39 2024, max compression
+gzip compressed data, was "dqc_toolkit-0.1.0b4.tar", last modified: Mon Apr 15 15:04:31 2024, max compression
```

## Comparing `dqc_toolkit-0.1.0b2.tar` & `dqc_toolkit-0.1.0b4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.131095 dqc_toolkit-0.1.0b2/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b2/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 11:57:39.130379 dqc_toolkit-0.1.0b2/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b2/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.110712 dqc_toolkit-0.1.0b2/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc_toolkit-0.1.0b2/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)    14405 2024-04-15 11:55:41.000000 dqc_toolkit-0.1.0b2/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.119762 dqc_toolkit-0.1.0b2/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      329 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7539 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_curation.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_dataprocessing.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4680 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_sanitychecks.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/logging.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.127744 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      431 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/top_level.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1659 2024-04-15 11:56:48.000000 dqc_toolkit-0.1.0b2/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-15 11:57:39.131298 dqc_toolkit-0.1.0b2/setup.cfg
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.126546 dqc_toolkit-0.1.0b2/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc_toolkit-0.1.0b2/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6078 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 15:04:31.100431 dqc_toolkit-0.1.0b4/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b4/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 15:04:31.099345 dqc_toolkit-0.1.0b4/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b4/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 15:04:31.073135 dqc_toolkit-0.1.0b4/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc_toolkit-0.1.0b4/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    14405 2024-04-15 11:55:41.000000 dqc_toolkit-0.1.0b4/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 15:04:31.085862 dqc_toolkit-0.1.0b4/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      329 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7539 2024-04-15 14:53:36.000000 dqc_toolkit-0.1.0b4/dqc/utils/_curation.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4680 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/dqc/utils/_sanitychecks.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/dqc/utils/logging.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 15:04:31.096856 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 15:04:31.000000 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      431 2024-04-15 15:04:31.000000 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-15 15:04:31.000000 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-15 15:04:31.000000 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-15 15:04:31.000000 dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1659 2024-04-15 15:04:07.000000 dqc_toolkit-0.1.0b4/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-15 15:04:31.100602 dqc_toolkit-0.1.0b4/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 15:04:31.095880 dqc_toolkit-0.1.0b4/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc_toolkit-0.1.0b4/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b4/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6078 2024-04-15 14:53:36.000000 dqc_toolkit-0.1.0b4/tests/test_crossval.py
```

### Comparing `dqc_toolkit-0.1.0b2/LICENSE` & `dqc_toolkit-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/PKG-INFO` & `dqc_toolkit-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b2
+Version: 0.1.0b4
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dqc_toolkit-0.1.0b2/dqc/base.py` & `dqc_toolkit-0.1.0b4/dqc/base.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc/crossval.py` & `dqc_toolkit-0.1.0b4/dqc/crossval.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc/utils/_curation.py` & `dqc_toolkit-0.1.0b4/dqc/utils/_curation.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc/utils/_dataprocessing.py` & `dqc_toolkit-0.1.0b4/dqc/utils/_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc/utils/_sanitychecks.py` & `dqc_toolkit-0.1.0b4/dqc/utils/_sanitychecks.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc/utils/logging.py` & `dqc_toolkit-0.1.0b4/dqc/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/PKG-INFO` & `dqc_toolkit-0.1.0b4/dqc_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b2
+Version: 0.1.0b4
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dqc_toolkit-0.1.0b2/pyproject.toml` & `dqc_toolkit-0.1.0b4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dqc-toolkit"
-version = "0.1.0-beta2"
+version = "0.1.0-beta4"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `dqc_toolkit-0.1.0b2/tests/test_crossval.py` & `dqc_toolkit-0.1.0b4/tests/test_crossval.py`

 * *Files identical despite different names*

