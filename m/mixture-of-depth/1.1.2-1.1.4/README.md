# Comparing `tmp/mixture-of-depth-1.1.2.tar.gz` & `tmp/mixture-of-depth-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-depth-1.1.2.tar", last modified: Sat Apr 13 16:27:30 2024, max compression
+gzip compressed data, was "mixture-of-depth-1.1.4.tar", last modified: Mon Apr 15 20:05:08 2024, max compression
```

## Comparing `mixture-of-depth-1.1.2.tar` & `mixture-of-depth-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 16:27:30.124301 mixture-of-depth-1.1.2/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 16:27:30.120301 mixture-of-depth-1.1.2/MoD/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4517 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.2/MoD/MoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.2/MoD/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 16:27:30.120301 mixture-of-depth-1.1.2/MoD/modeling/
--rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.2/MoD/modeling/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.2/MoD/modeling/automodeling.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 16:27:30.120301 mixture-of-depth-1.1.2/MoD/modeling/models/
--rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.2/MoD/modeling/models/BloomMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    75771 2024-04-13 11:04:53.000000 mixture-of-depth-1.1.2/MoD/modeling/models/FalconMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.2/MoD/modeling/models/GemmaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.2/MoD/modeling/models/LlamaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.2/MoD/modeling/models/MistralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.2/MoD/modeling/models/MixtralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    68490 2024-04-13 11:05:11.000000 mixture-of-depth-1.1.2/MoD/modeling/models/PhiMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.2/MoD/modeling/models/QwenMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73663 2024-04-13 11:06:21.000000 mixture-of-depth-1.1.2/MoD/modeling/models/QwenMoEMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.2/MoD/modeling/models/StarCoderMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.2/MoD/modeling/models/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-13 16:27:30.124301 mixture-of-depth-1.1.2/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2415 2024-04-13 10:55:20.000000 mixture-of-depth-1.1.2/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 16:27:30.120301 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-13 16:27:30.000000 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-13 16:27:30.000000 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-13 16:27:30.000000 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-13 16:27:30.000000 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-13 16:27:30.000000 mixture-of-depth-1.1.2/mixture_of_depth.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-13 16:27:30.124301 mixture-of-depth-1.1.2/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-13 16:27:13.000000 mixture-of-depth-1.1.2/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.174667 mixture-of-depth-1.1.4/MoD/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5265 2024-04-15 20:03:15.000000 mixture-of-depth-1.1.4/MoD/MoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.4/MoD/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.174667 mixture-of-depth-1.1.4/MoD/modeling/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.4/MoD/modeling/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.4/MoD/modeling/automodeling.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/MoD/modeling/models/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/BloomMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    75771 2024-04-13 11:04:53.000000 mixture-of-depth-1.1.4/MoD/modeling/models/FalconMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/GemmaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/LlamaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/MistralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/MixtralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    68490 2024-04-13 11:05:11.000000 mixture-of-depth-1.1.4/MoD/modeling/models/PhiMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73663 2024-04-13 11:06:21.000000 mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoEMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.4/MoD/modeling/models/StarCoderMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.4/MoD/modeling/models/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2415 2024-04-13 10:55:20.000000 mixture-of-depth-1.1.4/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-15 20:04:53.000000 mixture-of-depth-1.1.4/setup.py
```

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/automodeling.py` & `mixture-of-depth-1.1.4/MoD/modeling/automodeling.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/BloomMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/BloomMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/FalconMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/FalconMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/GemmaMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/GemmaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/LlamaMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/LlamaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/MistralMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/MistralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/MixtralMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/MixtralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/PhiMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/PhiMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/QwenMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/QwenMoEMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoEMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/MoD/modeling/models/StarCoderMoD.py` & `mixture-of-depth-1.1.4/MoD/modeling/models/StarCoderMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/PKG-INFO` & `mixture-of-depth-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.2
+Version: 1.1.4
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-1.1.2/README.md` & `mixture-of-depth-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/mixture_of_depth.egg-info/PKG-INFO` & `mixture-of-depth-1.1.4/mixture_of_depth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.2
+Version: 1.1.4
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-1.1.2/mixture_of_depth.egg-info/SOURCES.txt` & `mixture-of-depth-1.1.4/mixture_of_depth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.2/setup.py` & `mixture-of-depth-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mixture-of-depth',
-    version='1.1.2',
+    version='1.1.4',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/Mixture-of-depths',
     packages=find_packages(),
```

