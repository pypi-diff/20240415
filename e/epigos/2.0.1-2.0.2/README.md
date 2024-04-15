# Comparing `tmp/epigos-2.0.1.tar.gz` & `tmp/epigos-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epigos-2.0.1.tar", max compression
+gzip compressed data, was "epigos-2.0.2.tar", max compression
```

## Comparing `epigos-2.0.1.tar` & `epigos-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2024-03-28 23:59:34.378088 epigos-2.0.1/LICENSE
--rw-r--r--   0        0        0     3301 2024-03-28 23:59:34.378088 epigos-2.0.1/README.md
--rw-r--r--   0        0        0      192 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/__init__.py
--rw-r--r--   0        0        0      115 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/__version__.py
--rw-r--r--   0        0        0     5339 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/client.py
--rw-r--r--   0        0        0      198 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/__init__.py
--rw-r--r--   0        0        0     1039 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/base.py
--rw-r--r--   0        0        0     1055 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/classification.py
--rw-r--r--   0        0        0     1538 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/object_detection.py
--rw-r--r--   0        0        0     7649 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/project.py
--rw-r--r--   0        0        0     9253 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/core/uploader.py
--rw-r--r--   0        0        0        0 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/data_classes/__init__.py
--rw-r--r--   0        0        0     2077 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/data_classes/prediction.py
--rw-r--r--   0        0        0      203 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/data_classes/project.py
--rw-r--r--   0        0        0     1843 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/typings.py
--rw-r--r--   0        0        0      814 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/utils/__init__.py
--rw-r--r--   0        0        0     8364 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/utils/dataset.py
--rw-r--r--   0        0        0     1660 2024-03-28 23:59:34.378088 epigos-2.0.1/epigos/utils/image.py
--rw-r--r--   0        0        0     1941 2024-03-28 23:59:34.382088 epigos-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 epigos-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-15 13:11:57.375805 epigos-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3301 2024-04-15 13:11:57.375805 epigos-2.0.2/README.md
+-rw-r--r--   0        0        0      192 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/__version__.py
+-rw-r--r--   0        0        0     5339 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/client.py
+-rw-r--r--   0        0        0      198 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/__init__.py
+-rw-r--r--   0        0        0     1039 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/base.py
+-rw-r--r--   0        0        0     1055 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/classification.py
+-rw-r--r--   0        0        0     1538 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/object_detection.py
+-rw-r--r--   0        0        0     7649 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/project.py
+-rw-r--r--   0        0        0     9253 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/core/uploader.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/data_classes/__init__.py
+-rw-r--r--   0        0        0     2077 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/data_classes/prediction.py
+-rw-r--r--   0        0        0      203 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/data_classes/project.py
+-rw-r--r--   0        0        0     1843 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/typings.py
+-rw-r--r--   0        0        0      814 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/utils/__init__.py
+-rw-r--r--   0        0        0     8334 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/utils/dataset.py
+-rw-r--r--   0        0        0     1660 2024-04-15 13:11:57.375805 epigos-2.0.2/epigos/utils/image.py
+-rw-r--r--   0        0        0     1941 2024-04-15 13:11:57.375805 epigos-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 epigos-2.0.2/PKG-INFO
```

### Comparing `epigos-2.0.1/LICENSE` & `epigos-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/README.md` & `epigos-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/client.py` & `epigos-2.0.2/epigos/client.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/core/base.py` & `epigos-2.0.2/epigos/core/base.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/core/classification.py` & `epigos-2.0.2/epigos/core/classification.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/core/object_detection.py` & `epigos-2.0.2/epigos/core/object_detection.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/core/project.py` & `epigos-2.0.2/epigos/core/project.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/core/uploader.py` & `epigos-2.0.2/epigos/core/uploader.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/data_classes/prediction.py` & `epigos-2.0.2/epigos/data_classes/prediction.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/typings.py` & `epigos-2.0.2/epigos/typings.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/utils/__init__.py` & `epigos-2.0.2/epigos/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/epigos/utils/dataset.py` & `epigos-2.0.2/epigos/utils/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import yaml
 from pybboxes import BoundingBox
 
 from epigos.utils import logger
 
-FILE_EXTENSIONS = (".jpg", ".jpeg", ".png")
+IMAGE_FILE_EXTENSIONS = (".jpg", ".jpeg", ".png")
 
 
 def _extract_bbox_from_element(
     bb: ET.Element,
 ) -> typing.Optional[typing.Tuple[int, ...]]:
     attrs = ["xmin", "ymin", "xmax", "ymax"]
 
@@ -207,15 +207,15 @@
     dictionary of image paths and the class name.
     :param data_dir:
     :return:
     """
     imgs_paths = (
         p.resolve()
         for p in data_dir.glob("**/*")
-        if p.suffix.lower() in FILE_EXTENSIONS
+        if p.suffix.lower() in IMAGE_FILE_EXTENSIONS
     )
     return {p: p.parent.name for p in imgs_paths}
 
 
 def read_yolo_directory(
     data_dir: Path, config_file: str, annotations_dir: str = "labels"
 ) -> typing.Tuple[typing.Dict[Path, Path], typing.Dict[int, str]]:
@@ -235,20 +235,18 @@
         labels_map = dict(enumerate(yolo_names))
     elif isinstance(yolo_names, dict):
         labels_map = yolo_names
 
     imgs_paths = (
         p.resolve()
         for p in data_dir.glob("**/*")
-        if p.suffix.lower() in FILE_EXTENSIONS
+        if p.suffix.lower() in IMAGE_FILE_EXTENSIONS
     )
     paths = {
-        p: (
-            data_dir / p.parent.parent.name / annotations_dir / f"{p.stem}.txt"
-        ).resolve()
+        p: (p.parent.parent.absolute() / annotations_dir / f"{p.stem}.txt").resolve()
         for p in imgs_paths
     }
     return paths, labels_map
 
 
 def read_pascal_voc_directory(
     data_dir: Path, annotations_dir: str = "Annotations"
@@ -260,15 +258,13 @@
     :param data_dir:
     :param annotations_dir:
     :return:
     """
     imgs_paths = (
         p.resolve()
         for p in data_dir.glob("**/*")
-        if p.suffix.lower() in FILE_EXTENSIONS
+        if p.suffix.lower() in IMAGE_FILE_EXTENSIONS
     )
     return {
-        p: (
-            data_dir / p.parent.parent.name / annotations_dir / f"{p.stem}.xml"
-        ).resolve()
+        p: (p.parent.parent.absolute() / annotations_dir / f"{p.stem}.xml").resolve()
         for p in imgs_paths
     }
```

### Comparing `epigos-2.0.1/epigos/utils/image.py` & `epigos-2.0.2/epigos/utils/image.py`

 * *Files identical despite different names*

### Comparing `epigos-2.0.1/pyproject.toml` & `epigos-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epigos"
-version = "2.0.1"
+version = "2.0.2"
 description = "Epigos AI Python SDK"
 authors = ["Philip Adzanoukpe <philip@epigos.ai>"]
 license = "MIT"
 readme = "README.md"
 keywords = []
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", ]
 homepage = "https://github.com/Epigos-AI/epigos-python"
```

### Comparing `epigos-2.0.1/PKG-INFO` & `epigos-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epigos
-Version: 2.0.1
+Version: 2.0.2
 Summary: Epigos AI Python SDK
 Home-page: https://github.com/Epigos-AI/epigos-python
 License: MIT
 Author: Philip Adzanoukpe
 Author-email: philip@epigos.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

