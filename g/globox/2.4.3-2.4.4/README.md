# Comparing `tmp/globox-2.4.3.tar.gz` & `tmp/globox-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globox-2.4.3.tar", max compression
+gzip compressed data, was "globox-2.4.4.tar", max compression
```

## Comparing `globox-2.4.3.tar` & `globox-2.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1048 2024-03-04 21:50:31.850988 globox-2.4.3/LICENCE
--rw-r--r--   0        0        0     9077 2024-03-04 21:50:31.850988 globox-2.4.3/README.md
--rw-r--r--   0        0        0     1093 2024-03-04 21:50:31.850988 globox-2.4.3/pyproject.toml
--rw-r--r--   0        0        0      273 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/__init__.py
--rw-r--r--   0        0        0       30 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/__main__.py
--rw-r--r--   0        0        0    20558 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/annotation.py
--rw-r--r--   0        0        0    35859 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/annotationset.py
--rw-r--r--   0        0        0     1015 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/atomic.py
--rw-r--r--   0        0        0    20952 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/boundingbox.py
--rw-r--r--   0        0        0    14350 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/cli.py
--rw-r--r--   0        0        0      492 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/errors.py
--rw-r--r--   0        0        0    23249 2024-03-04 21:50:31.850988 globox-2.4.3/src/globox/evaluation.py
--rw-r--r--   0        0        0      719 2024-03-04 21:50:31.854988 globox-2.4.3/src/globox/file_utils.py
--rw-r--r--   0        0        0     6844 2024-03-04 21:50:31.854988 globox-2.4.3/src/globox/image_utils.py
--rw-r--r--   0        0        0      844 2024-03-04 21:50:31.854988 globox-2.4.3/src/globox/thread_utils.py
--rw-r--r--   0        0        0      746 2024-03-04 21:50:31.854988 globox-2.4.3/src/globox/utils.py
--rw-r--r--   0        0        0    10130 1970-01-01 00:00:00.000000 globox-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-04-15 21:21:16.341961 globox-2.4.4/LICENCE
+-rw-r--r--   0        0        0     9077 2024-04-15 21:21:16.341961 globox-2.4.4/README.md
+-rw-r--r--   0        0        0     1093 2024-04-15 21:21:16.341961 globox-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0      273 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/__main__.py
+-rw-r--r--   0        0        0    20558 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/annotation.py
+-rw-r--r--   0        0        0    35859 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/annotationset.py
+-rw-r--r--   0        0        0     1015 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/atomic.py
+-rw-r--r--   0        0        0    20952 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/boundingbox.py
+-rw-r--r--   0        0        0    14355 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/cli.py
+-rw-r--r--   0        0        0      492 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/errors.py
+-rw-r--r--   0        0        0    23249 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/evaluation.py
+-rw-r--r--   0        0        0      719 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/file_utils.py
+-rw-r--r--   0        0        0     6844 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/image_utils.py
+-rw-r--r--   0        0        0      844 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/thread_utils.py
+-rw-r--r--   0        0        0      746 2024-04-15 21:21:16.341961 globox-2.4.4/src/globox/utils.py
+-rw-r--r--   0        0        0    10130 1970-01-01 00:00:00.000000 globox-2.4.4/PKG-INFO
```

### Comparing `globox-2.4.3/LICENCE` & `globox-2.4.4/LICENCE`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/README.md` & `globox-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/pyproject.toml` & `globox-2.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "globox"
-version = "2.4.3"
+version = "2.4.4"
 authors = ["Louis Lac <lac.louis5@gmail.com>"]
 license = "MIT"
 packages = [{include = "globox", from = "src"}]
 readme = "README.md"
 description = "Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC."
 homepage = "https://github.com/laclouis5/globox"
 repository = "https://github.com/laclouis5/globox"
```

### Comparing `globox-2.4.3/src/globox/annotation.py` & `globox-2.4.4/src/globox/annotation.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/annotationset.py` & `globox-2.4.4/src/globox/annotationset.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/atomic.py` & `globox-2.4.4/src/globox/atomic.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/boundingbox.py` & `globox-2.4.4/src/globox/boundingbox.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/cli.py` & `globox-2.4.4/src/globox/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             )
         elif format_in == "yolov7":
             annotations = AnnotationSet.from_yolo_v7(
                 input, image_folder=image_dir, image_extension=img_ext, verbose=verbose
             )
         elif format_in == "txt":
             format = BoxFormat.from_string(args.bb_fmt_in)
-            relative: bool = args.norm_in == "rel"
+            relative: bool = args.norm_in_dets == "rel"
             extension: str = args.ext_in
             sep: str = args.sep_in
 
             annotations = AnnotationSet.from_txt(
                 input,
                 image_folder=image_dir,
                 box_format=format,
```

### Comparing `globox-2.4.3/src/globox/evaluation.py` & `globox-2.4.4/src/globox/evaluation.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/file_utils.py` & `globox-2.4.4/src/globox/file_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/image_utils.py` & `globox-2.4.4/src/globox/image_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/thread_utils.py` & `globox-2.4.4/src/globox/thread_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/src/globox/utils.py` & `globox-2.4.4/src/globox/utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.4.3/PKG-INFO` & `globox-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.4.3
+Version: 2.4.4
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
 Author: Louis Lac
 Author-email: lac.louis5@gmail.com
 Requires-Python: >=3.9,<3.13
```

