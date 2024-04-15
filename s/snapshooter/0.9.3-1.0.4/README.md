# Comparing `tmp/snapshooter-0.9.3.tar.gz` & `tmp/snapshooter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-0.9.3.tar", last modified: Mon Apr 15 21:28:59 2024, max compression
+gzip compressed data, was "snapshooter-1.0.4.tar", last modified: Mon Apr 15 21:32:43 2024, max compression
```

## Comparing `snapshooter-0.9.3.tar` & `snapshooter-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:28:44.000000 snapshooter-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:28:59.866552 snapshooter-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 21:28:44.000000 snapshooter-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:28:59.866552 snapshooter-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 21:28:44.000000 snapshooter-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 21:28:52.000000 snapshooter-0.9.3/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34032 2024-04-15 21:28:44.000000 snapshooter-0.9.3/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:28:59.000000 snapshooter-0.9.3/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:59.866552 snapshooter-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:28:44.000000 snapshooter-0.9.3/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:32:26.000000 snapshooter-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:32:43.290494 snapshooter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 21:32:26.000000 snapshooter-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:32:43.290494 snapshooter-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 21:32:26.000000 snapshooter-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 21:32:35.000000 snapshooter-1.0.4/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34032 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/snapshooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-0.9.3/LICENSE` & `snapshooter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/PKG-INFO` & `snapshooter-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.9.3
+Version: 1.0.4
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-0.9.3/README.md` & `snapshooter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/setup.py` & `snapshooter-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/snapshooter/cli.py` & `snapshooter-1.0.4/snapshooter/cli.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/snapshooter/fsspec_utils.py` & `snapshooter-1.0.4/snapshooter/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/snapshooter/jsonl_utils.py` & `snapshooter-1.0.4/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/snapshooter/snapshooter.py` & `snapshooter-1.0.4/snapshooter/snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/snapshooter.egg-info/PKG-INFO` & `snapshooter-1.0.4/snapshooter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.9.3
+Version: 1.0.4
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-0.9.3/tests/test_fsspec_snapshooter.py` & `snapshooter-1.0.4/tests/test_fsspec_snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.9.3/tests/test_fsspec_utils.py` & `snapshooter-1.0.4/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

