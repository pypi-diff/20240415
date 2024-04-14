# Comparing `tmp/inkscape_layer_utils-0.2.3.tar.gz` & `tmp/inkscape_layer_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_layer_utils-0.2.3.tar", last modified: Sun Mar 31 23:23:18 2024, max compression
+gzip compressed data, was "inkscape_layer_utils-0.3.0.tar", last modified: Sun Apr 14 22:30:21 2024, max compression
```

## Comparing `inkscape_layer_utils-0.2.3.tar` & `inkscape_layer_utils-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/inkscape_layer_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/inkscape_layer_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-31 23:23:18.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 23:23:18.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:23:18.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 23:23:18.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-31 23:23:18.000000 inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:23:18.517721 inkscape_layer_utils-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/tests/image_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/tests/test_image_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/tests/test_image_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-03-31 23:23:14.000000 inkscape_layer_utils-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20568 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/image_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/test_image_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/test_image_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/versioneer.py
```

### Comparing `inkscape_layer_utils-0.2.3/LICENSE` & `inkscape_layer_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/PKG-INFO` & `inkscape_layer_utils-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_layer_utils
-Version: 0.2.3
+Version: 0.3.0
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
```

### Comparing `inkscape_layer_utils-0.2.3/README.rst` & `inkscape_layer_utils-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/inkscape_layer_utils/__init__.py` & `inkscape_layer_utils-0.3.0/inkscape_layer_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/inkscape_layer_utils/image.py` & `inkscape_layer_utils-0.3.0/inkscape_layer_utils/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# Copyright (C) 2023 twyleg
+# Copyright (C) 2024 twyleg
 import copy
 import os
 import xml.etree.ElementTree as ET
-from os import PathLike
 from collections import OrderedDict
 from pathlib import Path
 from typing import List, Optional, Dict
 from xml.etree.ElementTree import Element, ElementTree
 
 
 class LayerUnknownError(Exception):
@@ -412,21 +411,21 @@
     ----------
     element_tree: ElementTree
         ElementTree that represents the image.
 
     """
 
     @classmethod
-    def load_from_file(cls, file_path: PathLike) -> "Image":
+    def load_from_file(cls, file_path: Path) -> "Image":
         """
         Load a SVG image from file.
 
         Parameters
         ----------
-        file_path: PathLike
+        file_path: Path
             Path of file to load.
 
         Returns
         -------
         Image
             Loaded image.
 
@@ -526,22 +525,22 @@
         dict[str, Image]
             Dictionary with layers byt their path.
 
         """
         layer_path_list = self.get_all_layer_paths()
         return dict((layer_path, self.extract_layer(layer_path)) for layer_path in layer_path_list)
 
-    def extract_all_layers_to_file(self, output_dir: PathLike, base_name: str) -> Dict[str, Path]:
+    def extract_all_layers_to_file(self, output_dir: Path, base_name: str) -> Dict[str, Path]:
         """
         Extract all layers to file by providing an output directory and a base name for
         the extracted layers output file names.
 
         Parameters
         ----------
-        output_dir: PathLike
+        output_dir: Path
             Output directory to write files to.
         base_name: str
             Base name of the files that will be saved.
         Returns
         -------
         dict[str, Path]
             Dictionary with file paths by layer paths.
@@ -553,18 +552,54 @@
                 output_file_path = Path(output_dir) / f"{base_name}.svg"
             else:
                 output_file_path = Path(output_dir) / f'{base_name}{layer_path.replace("/", "_")}.svg'
             extracted_image.save(output_file_path)
             extracted_layer_file_paths_by_layer_path[layer_path] = output_file_path
         return extracted_layer_file_paths_by_layer_path
 
-    def save(self, path: PathLike) -> None:
+    def extract_all_layers_to_file_lazy(
+        self, output_dir: Path, base_name: str, input_file_path: Path
+    ) -> Dict[str, Path]:
+        """
+        Extract all layers to file by providing an output directory and a base name for
+        the extracted layers output file names.
+        Only write output to file when either the output file is not yet existing or the input files modification
+        timestamp is more recent than the output file timestamp (comparable with GNU makes timestamp check).
+
+        Parameters
+        ----------
+        output_dir: Path
+            Output directory to write files to.
+        base_name: str
+            Base name of the files that will be saved.
+        input_file_path: Path
+            The input file path to determine the change timestamp.
+        Returns
+        -------
+        dict[str, Path]
+            Dictionary with file paths by layer paths.
+        """
+        extracted_layer_file_paths_by_layer_path: Dict[str, Path] = {}
+        extracted_images = self.extract_all_layers()
+        for layer_path, extracted_image in extracted_images.items():
+            if layer_path == "/":
+                output_file_path = Path(output_dir) / f"{base_name}.svg"
+            else:
+                output_file_path = Path(output_dir) / f'{base_name}{layer_path.replace("/", "_")}.svg'
+            if output_file_path.exists() is False or os.path.getmtime(input_file_path) > os.path.getmtime(
+                output_file_path
+            ):
+                extracted_image.save(output_file_path)
+            extracted_layer_file_paths_by_layer_path[layer_path] = output_file_path
+        return extracted_layer_file_paths_by_layer_path
+
+    def save(self, path: Path) -> None:
         """
         Save image to file.
 
         Parameters
         ----------
-        path: PathLike
+        path: Path
             File location to write image to.
         """
-        os.makedirs(Path(path).parent, exist_ok=True)
+        path.parent.mkdir(exist_ok=True)
         self.element_tree.write(path)
```

### Comparing `inkscape_layer_utils-0.2.3/inkscape_layer_utils/main.py` & `inkscape_layer_utils-0.3.0/inkscape_layer_utils/main.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/PKG-INFO` & `inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_layer_utils
-Version: 0.2.3
+Version: 0.3.0
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
```

### Comparing `inkscape_layer_utils-0.2.3/inkscape_layer_utils.egg-info/SOURCES.txt` & `inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/setup.py` & `inkscape_layer_utils-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/tests/image_test_case.py` & `inkscape_layer_utils-0.3.0/tests/image_test_case.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2024 twyleg
+import os
 import unittest
 import tempfile
 import xml.etree.ElementTree as ET
 
 from pathlib import Path
 from inkscape_layer_utils.image import Image, LayerUnknownError
 
@@ -37,13 +38,16 @@
     def assert_images_from_file_equal(self, expected_image_filepath: Path, actual_image_filepath: Path):
         expected_element_tree = ET.parse(expected_image_filepath)
         actual_element_tree = ET.parse(actual_image_filepath)
         expected_root_node = expected_element_tree.getroot()
         actual_root_node = actual_element_tree.getroot()
         self.assert_image_element_trees_equal(expected_root_node, actual_root_node)
 
+    def assert_mtime_newer(self, newer_file_path: Path, older_file_path: Path):
+        self.assertGreater(os.path.getmtime(newer_file_path), os.path.getmtime(older_file_path))
+
     def save_image_to_tmp_directory(self, image: Image) -> None:
         image.save(self.output_dir_path / f"{self.shortDescription()}.svg")
 
     def setUp(self) -> None:
         self.output_dir_path = self.prepare_output_directory()
         self.test_image = self.prepare_test_image()
```

### Comparing `inkscape_layer_utils-0.2.3/tests/test_image_1.py` & `inkscape_layer_utils-0.3.0/tests/test_image_1.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.2.3/versioneer.py` & `inkscape_layer_utils-0.3.0/versioneer.py`

 * *Files identical despite different names*

