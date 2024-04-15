# Comparing `tmp/npsam-1.4.9.2.tar.gz` & `tmp/npsam-1.4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npsam-1.4.9.2.tar", last modified: Mon Apr 15 07:45:54 2024, max compression
+gzip compressed data, was "npsam-1.4.9.3.tar", last modified: Mon Apr 15 07:49:42 2024, max compression
```

## Comparing `npsam-1.4.9.2.tar` & `npsam-1.4.9.3.tar`

### file list

```diff
@@ -1,31 +1,43 @@
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.946721 npsam-1.4.9.2/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.9.2/LICENSE.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:45:54.946443 npsam-1.4.9.2/PKG-INFO
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.9.2/README.md
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.940235 npsam-1.4.9.2/npsam/
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.946078 npsam-1.4.9.2/npsam/npsam.egg-info/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:45:54.000000 npsam-1.4.9.2/npsam/npsam.egg-info/PKG-INFO
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      844 2024-04-15 07:45:54.000000 npsam-1.4.9.2/npsam/npsam.egg-info/SOURCES.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-15 07:45:54.000000 npsam-1.4.9.2/npsam/npsam.egg-info/dependency_links.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-15 07:45:54.000000 npsam-1.4.9.2/npsam/npsam.egg-info/requires.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)       31 2024-04-15 07:45:54.000000 npsam-1.4.9.2/npsam/npsam.egg-info/top_level.txt
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.942519 npsam-1.4.9.2/npsam/segment_anything/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/build_sam.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.944786 npsam-1.4.9.2/npsam/segment_anything/modeling/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/common.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/sam.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/predictor.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:45:54.945806 npsam-1.4.9.2/npsam/segment_anything/utils/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/utils/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/utils/amg.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/utils/onnx.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.9.2/npsam/segment_anything/utils/transforms.py
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1126 2024-04-15 07:45:42.000000 npsam-1.4.9.2/pyproject.toml
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-15 07:45:54.946784 npsam-1.4.9.2/setup.cfg
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.218246 npsam-1.4.9.3/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.9.3/LICENSE.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:49:42.217955 npsam-1.4.9.3/PKG-INFO
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.9.3/README.md
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.209325 npsam-1.4.9.3/npsam/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.4.9.3/npsam/__init__.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.212802 npsam-1.4.9.3/npsam/button_images/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11501 2024-04-14 18:07:35.000000 npsam-1.4.9.3/npsam/button_images/Save_close.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11524 2024-04-14 18:04:36.000000 npsam-1.4.9.3/npsam/button_images/Save_close_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8142 2024-04-14 18:04:53.000000 npsam-1.4.9.3/npsam/button_images/arrow.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8037 2024-04-14 18:05:30.000000 npsam-1.4.9.3/npsam/button_images/arrow_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15018 2024-04-14 18:06:27.000000 npsam-1.4.9.3/npsam/button_images/plus_all.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15098 2024-04-14 18:06:46.000000 npsam-1.4.9.3/npsam/button_images/plus_all_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11171 2024-04-14 18:07:02.000000 npsam-1.4.9.3/npsam/button_images/plus_one.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11326 2024-04-14 18:07:18.000000 npsam-1.4.9.3/npsam/button_images/plus_one_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    62035 2024-04-14 19:08:51.000000 npsam-1.4.9.3/npsam/npsam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.213931 npsam-1.4.9.3/npsam/segment_anything/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/build_sam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.216208 npsam-1.4.9.3/npsam/segment_anything/modeling/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/common.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/predictor.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.217244 npsam-1.4.9.3/npsam/segment_anything/utils/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/amg.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/transforms.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.4.9.3/npsam/utils.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.217493 npsam-1.4.9.3/npsam.egg-info/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/PKG-INFO
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1144 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/SOURCES.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/dependency_links.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/requires.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/top_level.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1075 2024-04-15 07:49:20.000000 npsam-1.4.9.3/pyproject.toml
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-15 07:49:42.218317 npsam-1.4.9.3/setup.cfg
```

### Comparing `npsam-1.4.9.2/LICENSE.txt` & `npsam-1.4.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/PKG-INFO` & `npsam-1.4.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.9.2
+Version: 1.4.9.3
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.9.2/README.md` & `npsam-1.4.9.3/README.md`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/npsam.egg-info/PKG-INFO` & `npsam-1.4.9.3/npsam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.9.2
+Version: 1.4.9.3
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.9.2/npsam/segment_anything/automatic_mask_generator.py` & `npsam-1.4.9.3/npsam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/build_sam.py` & `npsam-1.4.9.3/npsam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/common.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/image_encoder.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/mask_decoder.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/prompt_encoder.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/sam.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/modeling/transformer.py` & `npsam-1.4.9.3/npsam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/predictor.py` & `npsam-1.4.9.3/npsam/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/utils/amg.py` & `npsam-1.4.9.3/npsam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/utils/onnx.py` & `npsam-1.4.9.3/npsam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/npsam/segment_anything/utils/transforms.py` & `npsam-1.4.9.3/npsam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.2/pyproject.toml` & `npsam-1.4.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages.find]
-where = ["npsam"]
-
 [tool.setuptools.package-data]
 "npsam.button_images" = ["*.png"]
 
 [project]
 name = "npsam"
-version = "1.4.9.2"
+version = "1.4.9.3"
 dependencies = [
     "numba==0.58.1",
     "opencv-python==4.9.0.80",
     "pandas==2.1.4",
     "matplotlib==3.8.2",
     "scikit-image==0.22.0",
     "ipympl==0.9.3",
```

