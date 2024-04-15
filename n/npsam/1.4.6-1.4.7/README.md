# Comparing `tmp/npsam-1.4.6.tar.gz` & `tmp/npsam-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npsam-1.4.6.tar", last modified: Sun Apr 14 19:37:08 2024, max compression
+gzip compressed data, was "npsam-1.4.7.tar", last modified: Sun Apr 14 19:59:01 2024, max compression
```

## Comparing `npsam-1.4.6.tar` & `npsam-1.4.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.016373 npsam-1.4.6/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.6/LICENSE.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:37:08.016115 npsam-1.4.6/PKG-INFO
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.6/README.md
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.008980 npsam-1.4.6/npsam/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.4.6/npsam/__init__.py
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    62035 2024-04-14 19:08:51.000000 npsam-1.4.6/npsam/npsam.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.012029 npsam-1.4.6/npsam/segment_anything/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    63209 2024-01-02 10:53:37.000000 npsam-1.4.6/npsam/segment_anything/NPSAM.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/build_sam.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.014522 npsam-1.4.6/npsam/segment_anything/modeling/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/common.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/sam.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/predictor.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.015585 npsam-1.4.6/npsam/segment_anything/utils/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/amg.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/onnx.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/transforms.py
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.4.6/npsam/utils.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.015797 npsam-1.4.6/npsam.egg-info/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/PKG-INFO
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      894 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/SOURCES.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/dependency_links.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/requires.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/top_level.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1005 2024-04-14 19:11:59.000000 npsam-1.4.6/pyproject.toml
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-14 19:37:08.016430 npsam-1.4.6/setup.cfg
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.586423 npsam-1.4.7/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.7/LICENSE.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:59:01.586164 npsam-1.4.7/PKG-INFO
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.7/README.md
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.579058 npsam-1.4.7/npsam/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.4.7/npsam/__init__.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    62035 2024-04-14 19:08:51.000000 npsam-1.4.7/npsam/npsam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.581973 npsam-1.4.7/npsam/segment_anything/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    63209 2024-01-02 10:53:37.000000 npsam-1.4.7/npsam/segment_anything/NPSAM.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/build_sam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.584577 npsam-1.4.7/npsam/segment_anything/modeling/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/common.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/predictor.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.585646 npsam-1.4.7/npsam/segment_anything/utils/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/utils/amg.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.7/npsam/segment_anything/utils/transforms.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.4.7/npsam/utils.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:59:01.585850 npsam-1.4.7/npsam.egg-info/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:59:01.000000 npsam-1.4.7/npsam.egg-info/PKG-INFO
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      894 2024-04-14 19:59:01.000000 npsam-1.4.7/npsam.egg-info/SOURCES.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-14 19:59:01.000000 npsam-1.4.7/npsam.egg-info/dependency_links.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-14 19:59:01.000000 npsam-1.4.7/npsam.egg-info/requires.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-14 19:59:01.000000 npsam-1.4.7/npsam.egg-info/top_level.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1005 2024-04-14 19:45:25.000000 npsam-1.4.7/pyproject.toml
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-14 19:59:01.586473 npsam-1.4.7/setup.cfg
```

### Comparing `npsam-1.4.6/LICENSE.txt` & `npsam-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/PKG-INFO` & `npsam-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.6
+Version: 1.4.7
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.6/README.md` & `npsam-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/npsam.py` & `npsam-1.4.7/npsam/npsam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/NPSAM.py` & `npsam-1.4.7/npsam/segment_anything/NPSAM.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/automatic_mask_generator.py` & `npsam-1.4.7/npsam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/build_sam.py` & `npsam-1.4.7/npsam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/common.py` & `npsam-1.4.7/npsam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/image_encoder.py` & `npsam-1.4.7/npsam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/mask_decoder.py` & `npsam-1.4.7/npsam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/prompt_encoder.py` & `npsam-1.4.7/npsam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/sam.py` & `npsam-1.4.7/npsam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/modeling/transformer.py` & `npsam-1.4.7/npsam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/predictor.py` & `npsam-1.4.7/npsam/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/utils/amg.py` & `npsam-1.4.7/npsam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/utils/onnx.py` & `npsam-1.4.7/npsam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/segment_anything/utils/transforms.py` & `npsam-1.4.7/npsam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam/utils.py` & `npsam-1.4.7/npsam/utils.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/npsam.egg-info/PKG-INFO` & `npsam-1.4.7/npsam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.6
+Version: 1.4.7
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.6/npsam.egg-info/SOURCES.txt` & `npsam-1.4.7/npsam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npsam-1.4.6/pyproject.toml` & `npsam-1.4.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "npsam"
-version = "1.4.6"
+version = "1.4.7"
 dependencies = [
     "numba==0.58.1",
     "opencv-python==4.9.0.80",
     "pandas==2.1.4",
     "matplotlib==3.8.2",
     "scikit-image==0.22.0",
     "ipympl==0.9.3",
```

