# Comparing `tmp/tabled-0.1.8.tar.gz` & `tmp/tabled-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabled-0.1.8.tar", last modified: Fri Feb  9 14:12:14 2024, max compression
+gzip compressed data, was "tabled-0.1.9.tar", last modified: Mon Feb 12 16:41:39 2024, max compression
```

## Comparing `tabled-0.1.8.tar` & `tabled-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:12:14.188103 tabled-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-09 14:11:38.000000 tabled-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-09 14:12:14.188103 tabled-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-09 14:11:38.000000 tabled-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-09 14:12:14.188103 tabled-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-09 14:11:38.000000 tabled-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:12:14.188103 tabled-0.1.8/tabled/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-02-09 14:12:11.000000 tabled-0.1.8/tabled/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:12:14.188103 tabled-0.1.8/tabled/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/tests/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/tests/join_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-02-09 14:11:38.000000 tabled-0.1.8/tabled/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:12:14.188103 tabled-0.1.8/tabled.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-09 14:12:14.000000 tabled-0.1.8/tabled.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:41:39.414151 tabled-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-12 16:41:10.000000 tabled-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-12 16:41:39.414151 tabled-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-12 16:41:10.000000 tabled-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-12 16:41:39.414151 tabled-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-12 16:41:10.000000 tabled-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:41:39.410151 tabled-0.1.9/tabled/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:41:39.414151 tabled-0.1.9/tabled/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/tests/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/tests/join_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-02-12 16:41:10.000000 tabled-0.1.9/tabled/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:41:39.414151 tabled-0.1.9/tabled.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-12 16:41:39.000000 tabled-0.1.9/tabled.egg-info/top_level.txt
```

### Comparing `tabled-0.1.8/LICENSE` & `tabled-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/setup.cfg` & `tabled-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tabled
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/i2mint/tabled
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = Thor Whalen
 description = A (key-value) data-object-layer to get (pandas) tables from a variety of sources with ease
```

### Comparing `tabled-0.1.8/tabled/base.py` & `tabled-0.1.9/tabled/base.py`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/tabled/html.py` & `tabled-0.1.9/tabled/html.py`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/tabled/multi.py` & `tabled-0.1.9/tabled/multi.py`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/tabled/tests/data.py` & `tabled-0.1.9/tabled/tests/data.py`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/tabled/tests/join_tables.py` & `tabled-0.1.9/tabled/tests/join_tables.py`

 * *Files identical despite different names*

### Comparing `tabled-0.1.8/tabled/util.py` & `tabled-0.1.9/tabled/util.py`

 * *Files identical despite different names*

