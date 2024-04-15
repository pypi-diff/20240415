# Comparing `tmp/h5io_browser-0.0.8.tar.gz` & `tmp/h5io_browser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5io_browser-0.0.8.tar", last modified: Mon Feb 12 08:44:19 2024, max compression
+gzip compressed data, was "h5io_browser-0.0.9.tar", last modified: Thu Feb 15 08:39:37 2024, max compression
```

## Comparing `h5io_browser-0.0.8.tar` & `h5io_browser-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 08:44:19.750072 h5io_browser-0.0.8/h5io_browser/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/h5io_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/h5io_browser/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/h5io_browser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/h5io_browser/pointer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/h5io_browser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-02-12 08:44:19.000000 h5io_browser-0.0.8/h5io_browser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-12 08:44:19.000000 h5io_browser-0.0.8/h5io_browser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 08:44:19.000000 h5io_browser-0.0.8/h5io_browser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-12 08:44:19.000000 h5io_browser-0.0.8/h5io_browser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 08:44:19.000000 h5io_browser-0.0.8/h5io_browser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-12 08:44:17.000000 h5io_browser-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 08:44:19.754072 h5io_browser-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-02-12 08:43:13.000000 h5io_browser-0.0.8/tests/test_pointer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/h5io_browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/h5io_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/h5io_browser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/h5io_browser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/h5io_browser/pointer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/h5io_browser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-02-15 08:39:37.000000 h5io_browser-0.0.9/h5io_browser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-15 08:39:37.000000 h5io_browser-0.0.9/h5io_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 08:39:37.000000 h5io_browser-0.0.9/h5io_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-15 08:39:37.000000 h5io_browser-0.0.9/h5io_browser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 08:39:37.000000 h5io_browser-0.0.9/h5io_browser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-15 08:39:36.000000 h5io_browser-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 08:39:37.985838 h5io_browser-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-02-15 08:38:38.000000 h5io_browser-0.0.9/tests/test_pointer.py
```

### Comparing `h5io_browser-0.0.8/LICENSE` & `h5io_browser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `h5io_browser-0.0.8/PKG-INFO` & `h5io_browser-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5io_browser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easy navigation and data storage for HDF5
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Jan Janssen
         All rights reserved.
         
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5io<=0.2.1,>=0.2.0
+Requires-Dist: h5io==0.2.2
 Requires-Dist: h5py<=3.10.0,>=3.6.0
 Requires-Dist: numpy<=1.26.4,>=1.23.5
 Requires-Dist: pandas<=2.2.0,>=1.5.3
 
 # Easy navigation and data storage for HDF5
 
 [![Python package](https://github.com/h5io/h5io_browser/actions/workflows/unittests.yml/badge.svg)](https://github.com/h5io/h5io_browser/actions)
```

### Comparing `h5io_browser-0.0.8/README.md` & `h5io_browser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `h5io_browser-0.0.8/h5io_browser/base.py` & `h5io_browser-0.0.9/h5io_browser/base.py`

 * *Files identical despite different names*

### Comparing `h5io_browser-0.0.8/h5io_browser/pointer.py` & `h5io_browser-0.0.9/h5io_browser/pointer.py`

 * *Files identical despite different names*

### Comparing `h5io_browser-0.0.8/h5io_browser.egg-info/PKG-INFO` & `h5io_browser-0.0.9/h5io_browser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5io_browser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easy navigation and data storage for HDF5
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Jan Janssen
         All rights reserved.
         
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5io<=0.2.1,>=0.2.0
+Requires-Dist: h5io==0.2.2
 Requires-Dist: h5py<=3.10.0,>=3.6.0
 Requires-Dist: numpy<=1.26.4,>=1.23.5
 Requires-Dist: pandas<=2.2.0,>=1.5.3
 
 # Easy navigation and data storage for HDF5
 
 [![Python package](https://github.com/h5io/h5io_browser/actions/workflows/unittests.yml/badge.svg)](https://github.com/h5io/h5io_browser/actions)
```

### Comparing `h5io_browser-0.0.8/pyproject.toml` & `h5io_browser-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "h5io>=0.2.0,<=0.2.1",
+    "h5io==0.2.2",
     "h5py>=3.6.0,<=3.10.0",
     "numpy>=1.23.5,<=1.26.4",
     "pandas>=1.5.3,<=2.2.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `h5io_browser-0.0.8/tests/test_base.py` & `h5io_browser-0.0.9/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,17 +246,23 @@
             ["/data_hierarchical/a", "/data_hierarchical/b", "/data_hierarchical/f"],
         )
         delete_item(file_name=self.file_name, h5_path="/data_hierarchical/i")
         delete_item(file_name=self.file_name, h5_path="/data_hierarchical/f")
         nodes, groups = list_hdf(file_name=self.file_name, h5_path="/data_hierarchical")
         self.assertEqual(groups, ["/data_hierarchical/c"])
         self.assertEqual(nodes, ["/data_hierarchical/a", "/data_hierarchical/b"])
-        with self.assertRaises(TypeError):
-            write_dict_to_hdf(
-                file_name=self.file_name, data_dict={"/data_hierarchical/j": ValueError}
+        write_dict_to_hdf(
+            file_name=self.file_name, data_dict={"/data_hierarchical/j": ValueError}
+        )
+        with h5py.File(self.file_name, "r") as hdf:
+            self.assertEqual(
+                ValueError,
+                _read_hdf(
+                    hdf_filehandle=hdf, h5_path="/data_hierarchical/j", slash="ignore"
+                ),
             )
 
 
 class TestBaseJSON(TestCase):
     def setUp(self):
         self.file_name = "test_json.h5"
         self.h5_path = "/data_json"
```

### Comparing `h5io_browser-0.0.8/tests/test_pointer.py` & `h5io_browser-0.0.9/tests/test_pointer.py`

 * *Files identical despite different names*

