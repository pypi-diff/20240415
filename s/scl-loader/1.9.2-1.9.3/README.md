# Comparing `tmp/scl_loader-1.9.2.tar.gz` & `tmp/scl_loader-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scl_loader-1.9.2.tar", last modified: Thu Nov 18 15:15:03 2021, max compression
+gzip compressed data, was "scl_loader-1.9.3.tar", last modified: Thu Nov 18 15:33:37 2021, max compression
```

## Comparing `scl_loader-1.9.2.tar` & `scl_loader-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.961846 scl_loader-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11558 2021-11-18 15:14:48.000000 scl_loader-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-11-18 15:14:48.000000 scl_loader-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-11-18 15:15:03.961846 scl_loader-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-11-18 15:14:48.000000 scl_loader-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-18 15:14:48.000000 scl_loader-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 15:15:03.961846 scl_loader-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2021-11-18 15:14:48.000000 scl_loader-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.957846 scl_loader-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.957846 scl_loader-1.9.2/src/scl_loader/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.957846 scl_loader-1.9.2/src/scl_loader/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.961846 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7511 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_BaseSimpleTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_BaseTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    14565 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Communication.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     8030 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_DataTypeTemplates.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    24967 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Enums.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    40806 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_IED.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    28617 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Substation.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    41251 2021-11-18 15:14:48.000000 scl_loader-1.9.2/src/scl_loader/scl_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:15:03.961846 scl_loader-1.9.2/src/scl_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-18 15:15:03.000000 scl_loader-1.9.2/src/scl_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.156849 scl_loader-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    11558 2021-11-18 15:33:25.000000 scl_loader-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-11-18 15:33:25.000000 scl_loader-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2021-11-18 15:33:37.156849 scl_loader-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2021-11-18 15:33:25.000000 scl_loader-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-18 15:33:25.000000 scl_loader-1.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 15:33:37.156849 scl_loader-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2021-11-18 15:33:25.000000 scl_loader-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.140849 scl_loader-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.144849 scl_loader-1.9.3/src/scl_loader/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.140849 scl_loader-1.9.3/src/scl_loader/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.156849 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     7511 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_BaseSimpleTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_BaseTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    14565 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Communication.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     8030 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_DataTypeTemplates.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    24967 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Enums.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    40806 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_IED.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    28617 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Substation.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    41251 2021-11-18 15:33:25.000000 scl_loader-1.9.3/src/scl_loader/scl_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:33:37.148849 scl_loader-1.9.3/src/scl_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2021-11-18 15:33:36.000000 scl_loader-1.9.3/src/scl_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-11-18 15:33:37.000000 scl_loader-1.9.3/src/scl_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 15:33:36.000000 scl_loader-1.9.3/src/scl_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-18 15:33:36.000000 scl_loader-1.9.3/src/scl_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-11-18 15:33:36.000000 scl_loader-1.9.3/src/scl_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-18 15:33:36.000000 scl_loader-1.9.3/src/scl_loader.egg-info/top_level.txt
```

### Comparing `scl_loader-1.9.2/LICENSE` & `scl_loader-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/PKG-INFO` & `scl_loader-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scl_loader
-Version: 1.9.2
+Version: 1.9.3
 Summary: Outil de manipulation de SCD
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lint and Test Python 🐍 ](https://github.com/rte-france/SCL_Loader/workflows/Lint%20and%20Test%20Python%20%F0%9F%90%8D%20distribution%20%F0%9F%93%A6/badge.svg)
 # RTE - scl_loader
 
 ## Installation
```

### Comparing `scl_loader-1.9.2/setup.py` & `scl_loader-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
     REQUIREMENTS = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 setup(
     name='scl_loader',  # Required
-    version='1.9.2',  # Required
+    version='1.9.3',  # Required
     description='Outil de manipulation de SCD',  # Required
     long_description=LONG_DESCRIPTION,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     package_dir={'': 'src'},  # Optional
     packages=["scl_loader"],  # Required
-    python_requires='>=3.8, <4',
+    python_requires='>=3.6, <4',
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
     ],
 
     # If there are data files included in your packages that need to be
```

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_BaseSimpleTypes.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_BaseSimpleTypes.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_BaseTypes.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_BaseTypes.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Communication.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Communication.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_DataTypeTemplates.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_DataTypeTemplates.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Enums.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Enums.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_IED.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_IED.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/resources/SCL_Schema/SCL_Substation.xsd` & `scl_loader-1.9.3/src/scl_loader/resources/SCL_Schema/SCL_Substation.xsd`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader/scl_loader.py` & `scl_loader-1.9.3/src/scl_loader/scl_loader.py`

 * *Files identical despite different names*

### Comparing `scl_loader-1.9.2/src/scl_loader.egg-info/PKG-INFO` & `scl_loader-1.9.3/src/scl_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scl-loader
-Version: 1.9.2
+Version: 1.9.3
 Summary: Outil de manipulation de SCD
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lint and Test Python 🐍 ](https://github.com/rte-france/SCL_Loader/workflows/Lint%20and%20Test%20Python%20%F0%9F%90%8D%20distribution%20%F0%9F%93%A6/badge.svg)
 # RTE - scl_loader
 
 ## Installation
```

### Comparing `scl_loader-1.9.2/src/scl_loader.egg-info/SOURCES.txt` & `scl_loader-1.9.3/src/scl_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

