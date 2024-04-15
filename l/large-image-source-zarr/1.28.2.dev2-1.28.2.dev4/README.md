# Comparing `tmp/large-image-source-zarr-1.28.2.dev2.tar.gz` & `tmp/large-image-source-zarr-1.28.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.28.2.dev2.tar", last modified: Fri Apr 12 15:26:30 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.28.2.dev4.tar", last modified: Mon Apr 15 12:58:23 2024, max compression
```

## Comparing `large-image-source-zarr-1.28.2.dev2.tar` & `large-image-source-zarr-1.28.2.dev4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34406 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2705 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:58:23.819412 large-image-source-zarr-1.28.2.dev4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-15 12:58:23.819412 large-image-source-zarr-1.28.2.dev4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:58:23.815412 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34406 2024-04-15 12:52:04.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-15 12:52:04.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:58:23.819412 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-15 12:58:23.000000 large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-15 12:52:04.000000 large-image-source-zarr-1.28.2.dev4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-15 12:58:23.819412 large-image-source-zarr-1.28.2.dev4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2705 2024-04-15 12:52:04.000000 large-image-source-zarr-1.28.2.dev4/setup.py
```

### Comparing `large-image-source-zarr-1.28.2.dev2/LICENSE` & `large-image-source-zarr-1.28.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.2.dev2/PKG-INFO` & `large-image-source-zarr-1.28.2.dev4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.2.dev2
+Version: 1.28.2.dev4
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev2
+Requires-Dist: large-image>=1.28.2.dev4
 Requires-Dist: zarr
 Requires-Dist: imagecodecs-numcodecs
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev2; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
 Provides-Extra: all
 Requires-Dist: large-image-converter; extra == "all"
 
 A OME Zarr tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-zarr-1.28.2.dev2/README.rst` & `large-image-source-zarr-1.28.2.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.28.2.dev4/large_image_source_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/PKG-INFO` & `large-image-source-zarr-1.28.2.dev4/large_image_source_zarr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.2.dev2
+Version: 1.28.2.dev4
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev2
+Requires-Dist: large-image>=1.28.2.dev4
 Requires-Dist: zarr
 Requires-Dist: imagecodecs-numcodecs
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev2; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
 Provides-Extra: all
 Requires-Dist: large-image-converter; extra == "all"
 
 A OME Zarr tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-zarr-1.28.2.dev2/setup.py` & `large-image-source-zarr-1.28.2.dev4/setup.py`

 * *Files identical despite different names*

