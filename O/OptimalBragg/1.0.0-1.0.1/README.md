# Comparing `tmp/optimalbragg-1.0.0.tar.gz` & `tmp/optimalbragg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimalbragg-1.0.0.tar", last modified: Sun Apr 14 19:13:56 2024, max compression
+gzip compressed data, was "optimalbragg-1.0.1.tar", last modified: Sun Apr 14 19:36:09 2024, max compression
```

## Comparing `optimalbragg-1.0.0.tar` & `optimalbragg-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:13:56.286462 optimalbragg-1.0.0/
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     1541 2024-04-14 04:08:14.000000 optimalbragg-1.0.0/LICENSE
-drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:13:56.283129 optimalbragg-1.0.0/OptimalBragg/
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     5652 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/__init__.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     2354 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/analysis.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     6453 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/costs.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     9131 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/layers.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     8276 2024-04-14 18:59:40.000000 optimalbragg-1.0.0/OptimalBragg/materials.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    35483 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/noise.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    12432 2024-04-14 04:08:59.000000 optimalbragg-1.0.0/OptimalBragg/optimizer.py
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    10406 2024-04-14 18:51:50.000000 optimalbragg-1.0.0/OptimalBragg/plot.py
-drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:13:56.286462 optimalbragg-1.0.0/OptimalBragg.egg-info/
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     4531 2024-04-14 19:13:56.000000 optimalbragg-1.0.0/OptimalBragg.egg-info/PKG-INFO
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)      395 2024-04-14 19:13:56.000000 optimalbragg-1.0.0/OptimalBragg.egg-info/SOURCES.txt
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)        1 2024-04-14 19:13:56.000000 optimalbragg-1.0.0/OptimalBragg.egg-info/dependency_links.txt
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       58 2024-04-14 19:13:56.000000 optimalbragg-1.0.0/OptimalBragg.egg-info/requires.txt
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       13 2024-04-14 19:13:56.000000 optimalbragg-1.0.0/OptimalBragg.egg-info/top_level.txt
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     4531 2024-04-14 19:13:56.286462 optimalbragg-1.0.0/PKG-INFO
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     3850 2024-04-14 18:54:04.000000 optimalbragg-1.0.0/README.md
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       38 2024-04-14 19:13:56.286462 optimalbragg-1.0.0/setup.cfg
--rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)      901 2024-04-14 04:13:39.000000 optimalbragg-1.0.0/setup.py
+drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:36:09.082314 optimalbragg-1.0.1/
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     1541 2024-04-14 04:08:14.000000 optimalbragg-1.0.1/LICENSE
+drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:36:09.082314 optimalbragg-1.0.1/OptimalBragg/
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     5652 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/__init__.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     2354 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/analysis.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     6453 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/costs.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     9131 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/layers.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     8276 2024-04-14 18:59:40.000000 optimalbragg-1.0.1/OptimalBragg/materials.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    35483 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/noise.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    12432 2024-04-14 04:08:59.000000 optimalbragg-1.0.1/OptimalBragg/optimizer.py
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)    10406 2024-04-14 18:51:50.000000 optimalbragg-1.0.1/OptimalBragg/plot.py
+drwxr-xr-x   0 pacosalces  (1000) pacosalces  (1000)        0 2024-04-14 19:36:09.082314 optimalbragg-1.0.1/OptimalBragg.egg-info/
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     4547 2024-04-14 19:36:09.000000 optimalbragg-1.0.1/OptimalBragg.egg-info/PKG-INFO
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)      395 2024-04-14 19:36:09.000000 optimalbragg-1.0.1/OptimalBragg.egg-info/SOURCES.txt
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)        1 2024-04-14 19:36:09.000000 optimalbragg-1.0.1/OptimalBragg.egg-info/dependency_links.txt
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       58 2024-04-14 19:36:09.000000 optimalbragg-1.0.1/OptimalBragg.egg-info/requires.txt
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       13 2024-04-14 19:36:09.000000 optimalbragg-1.0.1/OptimalBragg.egg-info/top_level.txt
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     4547 2024-04-14 19:36:09.082314 optimalbragg-1.0.1/PKG-INFO
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)     3850 2024-04-14 18:54:04.000000 optimalbragg-1.0.1/README.md
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)       38 2024-04-14 19:36:09.082314 optimalbragg-1.0.1/setup.cfg
+-rw-r--r--   0 pacosalces  (1000) pacosalces  (1000)      917 2024-04-14 19:36:04.000000 optimalbragg-1.0.1/setup.py
```

### Comparing `optimalbragg-1.0.0/LICENSE` & `optimalbragg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/__init__.py` & `optimalbragg-1.0.1/OptimalBragg/__init__.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/analysis.py` & `optimalbragg-1.0.1/OptimalBragg/analysis.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/costs.py` & `optimalbragg-1.0.1/OptimalBragg/costs.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/layers.py` & `optimalbragg-1.0.1/OptimalBragg/layers.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/materials.py` & `optimalbragg-1.0.1/OptimalBragg/materials.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/noise.py` & `optimalbragg-1.0.1/OptimalBragg/noise.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/optimizer.py` & `optimalbragg-1.0.1/OptimalBragg/optimizer.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg/plot.py` & `optimalbragg-1.0.1/OptimalBragg/plot.py`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/OptimalBragg.egg-info/PKG-INFO` & `optimalbragg-1.0.1/OptimalBragg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: OptimalBragg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for the design and optimization of dielectric coatings
 Home-page: https://github.com/CaltechExperimentalGravity/OptimalBragg/
-Author: pacosalces
+Author: CaltechExperimentalGravity
 Author-email: pacosalces@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
```

### Comparing `optimalbragg-1.0.0/PKG-INFO` & `optimalbragg-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: OptimalBragg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for the design and optimization of dielectric coatings
 Home-page: https://github.com/CaltechExperimentalGravity/OptimalBragg/
-Author: pacosalces
+Author: CaltechExperimentalGravity
 Author-email: pacosalces@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
```

### Comparing `optimalbragg-1.0.0/README.md` & `optimalbragg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `optimalbragg-1.0.0/setup.py` & `optimalbragg-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OptimalBragg",
-    version="1.0.0",
-    author="pacosalces",
+    version="1.0.1",
+    author="CaltechExperimentalGravity",
     author_email="pacosalces@gmail.com",
     description="Package for the design and optimization of dielectric coatings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CaltechExperimentalGravity/OptimalBragg/",
     license="LICENSE",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "numpy",
         "scipy",
         "matplotlib",
         "h5py",
```

