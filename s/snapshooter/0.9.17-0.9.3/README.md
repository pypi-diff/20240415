# Comparing `tmp/snapshooter-0.9.17.tar.gz` & `tmp/snapshooter-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-0.9.17.tar", last modified: Mon Apr 15 20:46:39 2024, max compression
+gzip compressed data, was "snapshooter-0.9.3.tar", last modified: Mon Apr 15 21:28:59 2024, max compression
```

## Comparing `snapshooter-0.9.17.tar` & `snapshooter-0.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:46:39.368027 snapshooter-0.9.17/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 20:46:23.000000 snapshooter-0.9.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-15 20:46:39.364027 snapshooter-0.9.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-15 20:46:23.000000 snapshooter-0.9.17/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:46:39.368027 snapshooter-0.9.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 20:46:23.000000 snapshooter-0.9.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:46:39.364027 snapshooter-0.9.17/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 20:46:31.000000 snapshooter-0.9.17/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 20:46:23.000000 snapshooter-0.9.17/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 20:46:23.000000 snapshooter-0.9.17/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 20:46:23.000000 snapshooter-0.9.17/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:46:23.000000 snapshooter-0.9.17/snapshooter/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34032 2024-04-15 20:46:23.000000 snapshooter-0.9.17/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:46:39.364027 snapshooter-0.9.17/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 20:46:39.000000 snapshooter-0.9.17/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:46:39.364027 snapshooter-0.9.17/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:46:23.000000 snapshooter-0.9.17/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 20:46:23.000000 snapshooter-0.9.17/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 20:46:23.000000 snapshooter-0.9.17/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 20:46:23.000000 snapshooter-0.9.17/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:28:44.000000 snapshooter-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:28:59.866552 snapshooter-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 21:28:44.000000 snapshooter-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:28:59.866552 snapshooter-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 21:28:44.000000 snapshooter-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 21:28:52.000000 snapshooter-0.9.3/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34032 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/snapshooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-0.9.17/LICENSE` & `snapshooter-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/PKG-INFO` & `snapshooter-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.9.17
+Version: 0.9.3
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Tests](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml)
-[![Publish](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml)
-
+[![CI/CD Pipeline](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml)
+[![Coverage](https://codecov.io/gh/jeromerg/snapshooter/graph/badge.svg?token=KC6KDDOBUF)](https://codecov.io/gh/jeromerg/snapshooter)
 
 # Snapshooter (fsspec folder backup and restore tooling)
 
 Snapshooter is a tool to back up and restore a folder in a fsspec file system. It is designed to be used with the 
 fsspec file system library, which provides a unified interface to various file systems (e.g. local, azure, s3, ...).
 
 Key features:
```

### Comparing `snapshooter-0.9.17/README.md` & `snapshooter-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-[![Tests](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml)
-[![Publish](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml)
-
+[![CI/CD Pipeline](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml)
+[![Coverage](https://codecov.io/gh/jeromerg/snapshooter/graph/badge.svg?token=KC6KDDOBUF)](https://codecov.io/gh/jeromerg/snapshooter)
 
 # Snapshooter (fsspec folder backup and restore tooling)
 
 Snapshooter is a tool to back up and restore a folder in a fsspec file system. It is designed to be used with the 
 fsspec file system library, which provides a unified interface to various file systems (e.g. local, azure, s3, ...).
 
 Key features:
```

### Comparing `snapshooter-0.9.17/setup.py` & `snapshooter-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/snapshooter/cli.py` & `snapshooter-0.9.3/snapshooter/cli.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/snapshooter/fsspec_utils.py` & `snapshooter-0.9.3/snapshooter/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/snapshooter/jsonl_utils.py` & `snapshooter-0.9.3/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/snapshooter/snapshooter.py` & `snapshooter-0.9.3/snapshooter/snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/snapshooter.egg-info/PKG-INFO` & `snapshooter-0.9.3/snapshooter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.9.17
+Version: 0.9.3
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Tests](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-app.yml)
-[![Publish](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/python-publish.yml)
-
+[![CI/CD Pipeline](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml/badge.svg)](https://github.com/jeromerg/snapshooter/actions/workflows/cicd.yml)
+[![Coverage](https://codecov.io/gh/jeromerg/snapshooter/graph/badge.svg?token=KC6KDDOBUF)](https://codecov.io/gh/jeromerg/snapshooter)
 
 # Snapshooter (fsspec folder backup and restore tooling)
 
 Snapshooter is a tool to back up and restore a folder in a fsspec file system. It is designed to be used with the 
 fsspec file system library, which provides a unified interface to various file systems (e.g. local, azure, s3, ...).
 
 Key features:
```

### Comparing `snapshooter-0.9.17/tests/test_fsspec_snapshooter.py` & `snapshooter-0.9.3/tests/test_fsspec_snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.17/tests/test_fsspec_utils.py` & `snapshooter-0.9.3/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

