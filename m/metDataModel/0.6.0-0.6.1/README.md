# Comparing `tmp/metDataModel-0.6.0.tar.gz` & `tmp/metdatamodel-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metDataModel-0.6.0.tar", last modified: Wed Jan 17 17:13:31 2024, max compression
+gzip compressed data, was "metdatamodel-0.6.1.tar", last modified: Mon Apr 15 19:46:18 2024, max compression
```

## Comparing `metDataModel-0.6.0.tar` & `metdatamodel-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-01-17 17:13:31.981498 metDataModel-0.6.0/
--rwxr-xr-x   0 lish     (195676001) 1088672553     1508 2024-01-04 16:54:10.000000 metDataModel-0.6.0/LICENSE
--rw-r--r--   0 lish     (195676001) 1088672553     8911 2024-01-17 17:13:31.980831 metDataModel-0.6.0/PKG-INFO
--rwxr-xr-x   0 lish     (195676001) 1088672553     8147 2024-01-17 17:00:47.000000 metDataModel-0.6.0/README.md
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-01-17 17:13:31.969524 metDataModel-0.6.0/metDataModel/
--rwxr-xr-x   0 lish     (195676001) 1088672553       87 2024-01-16 22:28:17.000000 metDataModel-0.6.0/metDataModel/__init__.py
--rwxr-xr-x   0 lish     (195676001) 1088672553    27361 2024-01-17 17:08:29.000000 metDataModel-0.6.0/metDataModel/core.py
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-01-17 17:13:31.976411 metDataModel-0.6.0/metDataModel/data/
--rw-r--r--   0 lish     (195676001) 1088672553        0 2024-01-04 17:07:12.000000 metDataModel-0.6.0/metDataModel/data/__init__.py
--rwxr-xr-x   0 lish     (195676001) 1088672553     2965 2024-01-05 15:50:04.000000 metDataModel-0.6.0/metDataModel/derived.py
--rw-r--r--   0 lish     (195676001) 1088672553      785 2024-01-04 16:52:35.000000 metDataModel-0.6.0/metDataModel/simpleTuples.py
--rwxr-xr-x   0 lish     (195676001) 1088672553      838 2024-01-04 17:06:52.000000 metDataModel-0.6.0/metDataModel/util.py
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-01-17 17:13:31.980230 metDataModel-0.6.0/metDataModel.egg-info/
--rw-r--r--   0 lish     (195676001) 1088672553     8911 2024-01-17 17:13:31.000000 metDataModel-0.6.0/metDataModel.egg-info/PKG-INFO
--rw-r--r--   0 lish     (195676001) 1088672553      388 2024-01-17 17:13:31.000000 metDataModel-0.6.0/metDataModel.egg-info/SOURCES.txt
--rw-r--r--   0 lish     (195676001) 1088672553        1 2024-01-17 17:13:31.000000 metDataModel-0.6.0/metDataModel.egg-info/dependency_links.txt
--rw-r--r--   0 lish     (195676001) 1088672553        1 2024-01-17 17:13:31.000000 metDataModel-0.6.0/metDataModel.egg-info/not-zip-safe
--rw-r--r--   0 lish     (195676001) 1088672553       19 2024-01-17 17:13:31.000000 metDataModel-0.6.0/metDataModel.egg-info/top_level.txt
--rw-r--r--   0 lish     (195676001) 1088672553      103 2024-01-04 16:52:35.000000 metDataModel-0.6.0/pyproject.toml
--rw-r--r--   0 lish     (195676001) 1088672553       38 2024-01-17 17:13:31.981557 metDataModel-0.6.0/setup.cfg
--rwxr-xr-x   0 lish     (195676001) 1088672553     1425 2024-01-04 16:52:35.000000 metDataModel-0.6.0/setup.py
-drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-01-17 17:13:31.979640 metDataModel-0.6.0/tests/
--rwxr-xr-x   0 lish     (195676001) 1088672553       50 2024-01-04 16:52:35.000000 metDataModel-0.6.0/tests/__init__.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:46:18.644928 metdatamodel-0.6.1/
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)     1508 2024-01-04 16:54:10.000000 metdatamodel-0.6.1/LICENSE
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9407 2024-04-15 19:46:18.644149 metdatamodel-0.6.1/PKG-INFO
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)     8644 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/README.md
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:46:18.633310 metdatamodel-0.6.1/metDataModel/
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)       87 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/metDataModel/__init__.py
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)    25985 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/metDataModel/core.py
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)    27392 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/metDataModel/core_simple.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:46:18.640520 metdatamodel-0.6.1/metDataModel/data/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-01-04 17:07:12.000000 metdatamodel-0.6.1/metDataModel/data/__init__.py
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)     4147 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/metDataModel/derived.py
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)     2965 2024-04-15 19:44:44.000000 metdatamodel-0.6.1/metDataModel/derived_simple.py
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      785 2024-01-04 16:52:35.000000 metdatamodel-0.6.1/metDataModel/simpleTuples.py
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)      838 2024-01-04 17:06:52.000000 metdatamodel-0.6.1/metDataModel/util.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:46:18.643288 metdatamodel-0.6.1/metDataModel.egg-info/
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)     9407 2024-04-15 19:46:18.000000 metdatamodel-0.6.1/metDataModel.egg-info/PKG-INFO
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      447 2024-04-15 19:46:18.000000 metdatamodel-0.6.1/metDataModel.egg-info/SOURCES.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-04-15 19:46:18.000000 metdatamodel-0.6.1/metDataModel.egg-info/dependency_links.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)        1 2024-04-15 19:46:18.000000 metdatamodel-0.6.1/metDataModel.egg-info/not-zip-safe
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       19 2024-04-15 19:46:18.000000 metdatamodel-0.6.1/metDataModel.egg-info/top_level.txt
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)      103 2024-01-04 16:52:35.000000 metdatamodel-0.6.1/pyproject.toml
+-rw-r--r--   0 lish     (195676001) JAX\Domain Users (1088672553)       38 2024-04-15 19:46:18.644994 metdatamodel-0.6.1/setup.cfg
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)     1425 2024-01-04 16:52:35.000000 metdatamodel-0.6.1/setup.py
+drwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)        0 2024-04-15 19:46:18.642648 metdatamodel-0.6.1/tests/
+-rwxr-xr-x   0 lish     (195676001) JAX\Domain Users (1088672553)       50 2024-01-04 16:52:35.000000 metdatamodel-0.6.1/tests/__init__.py
```

### Comparing `metDataModel-0.6.0/LICENSE` & `metdatamodel-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metDataModel-0.6.0/PKG-INFO` & `metdatamodel-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metDataModel
-Version: 0.6.0
+Version: 0.6.1
 Summary: Data models for metabolomics
 Home-page: https://github.com/shuzhao-li/metDataModel
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD license
 Keywords: metDataModel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -127,25 +127,34 @@
 
 
 ## For developers
 
 The data structures should be language neutral. 
 
 We edit primarily in the Python code, as JSON and YAML can be exported automatically.
-Each Python class has a serialization function to export JSON, which is selective.
+Each Python class has a serialization function to export JSON.
+
 I.e., concise information for users' need is exported, but not all class details.
 
 Adaptation/update/extension is encouraged in other languages. 
 
 We strive for the right level of abstraction.
 For the core classes, it's more important to have transparent, extensible structure.
 Therefore, it's a design decision not to have getter or setter functions. 
 Shallow data structures are more portable.
 MetDataModel provides a template, and application projects can extend it to fit their specific needs.
 
+There are two flavors of the metDataModel provided. The default version uses Python Dataclasses to 
+enforce weak static typing. These types are recommended and not enforced at runtime, but should provide
+users details to implement methods that use them in statically typed languages. The other is 
+dictionary based and has no suggested types. This is the minimal model. 
+
+Note that while metDataModel objects can have other metDataObjects as data members, this can cause 
+issues if there are circular references. 
+
 Please feel free to submit issues, and write Wiki pages for discussions.
 
 Pypi install: https://pypi.org/project/metDataModel/
 
 
 ### Related community resources
 While we focus on the application of mass spectrometry data,
```

### Comparing `metDataModel-0.6.0/README.md` & `metdatamodel-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -105,25 +105,34 @@
 
 
 ## For developers
 
 The data structures should be language neutral. 
 
 We edit primarily in the Python code, as JSON and YAML can be exported automatically.
-Each Python class has a serialization function to export JSON, which is selective.
+Each Python class has a serialization function to export JSON.
+
 I.e., concise information for users' need is exported, but not all class details.
 
 Adaptation/update/extension is encouraged in other languages. 
 
 We strive for the right level of abstraction.
 For the core classes, it's more important to have transparent, extensible structure.
 Therefore, it's a design decision not to have getter or setter functions. 
 Shallow data structures are more portable.
 MetDataModel provides a template, and application projects can extend it to fit their specific needs.
 
+There are two flavors of the metDataModel provided. The default version uses Python Dataclasses to 
+enforce weak static typing. These types are recommended and not enforced at runtime, but should provide
+users details to implement methods that use them in statically typed languages. The other is 
+dictionary based and has no suggested types. This is the minimal model. 
+
+Note that while metDataModel objects can have other metDataObjects as data members, this can cause 
+issues if there are circular references. 
+
 Please feel free to submit issues, and write Wiki pages for discussions.
 
 Pypi install: https://pypi.org/project/metDataModel/
 
 
 ### Related community resources
 While we focus on the application of mass spectrometry data, 
@@ -144,8 +153,8 @@
 To learn about genome scale metabolic models:
 
 - review by Gu et al, 2019 (https://link.springer.com/article/10.1186/s13059-019-1730-3)
 
 - our book chapter to explain metabolic models in the context of metabolomic pathway analysis (https://link.springer.com/protocol/10.1007/978-1-0716-0239-3_19)
 
 ### Citation
-Mitchell et al, Common data models to streamline metabolomics processing and annotation, and implementation in a Python pipeline  (to come).
+Mitchell et al, Common data models to streamline metabolomics processing and annotation, and implementation in a Python pipeline  (to come).
```

### Comparing `metDataModel-0.6.0/metDataModel/core.py` & `metdatamodel-0.6.1/metDataModel/core_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     def __init__(self, id=''):
         '''
         Default to mass spectrum level 2, but easy to be used for level 1 and other data types.
         '''
         self.id = id
         self.ms_level = 2
         self.precursor_ion = self.precursor_ion_mz = 0
-
+        self.ionization = "pos"
         self.list_mz = []
         self.list_intensity = []
         self.retention_time = self.rtime = 0
 
     def serialize(self):
         '''
         return dictionary of key variables.
```

### Comparing `metDataModel-0.6.0/metDataModel/derived.py` & `metdatamodel-0.6.1/metDataModel/derived_simple.py`

 * *Files identical despite different names*

### Comparing `metDataModel-0.6.0/metDataModel/simpleTuples.py` & `metdatamodel-0.6.1/metDataModel/simpleTuples.py`

 * *Files identical despite different names*

### Comparing `metDataModel-0.6.0/metDataModel/util.py` & `metdatamodel-0.6.1/metDataModel/util.py`

 * *Files identical despite different names*

### Comparing `metDataModel-0.6.0/metDataModel.egg-info/PKG-INFO` & `metdatamodel-0.6.1/metDataModel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metDataModel
-Version: 0.6.0
+Version: 0.6.1
 Summary: Data models for metabolomics
 Home-page: https://github.com/shuzhao-li/metDataModel
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: BSD license
 Keywords: metDataModel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -127,25 +127,34 @@
 
 
 ## For developers
 
 The data structures should be language neutral. 
 
 We edit primarily in the Python code, as JSON and YAML can be exported automatically.
-Each Python class has a serialization function to export JSON, which is selective.
+Each Python class has a serialization function to export JSON.
+
 I.e., concise information for users' need is exported, but not all class details.
 
 Adaptation/update/extension is encouraged in other languages. 
 
 We strive for the right level of abstraction.
 For the core classes, it's more important to have transparent, extensible structure.
 Therefore, it's a design decision not to have getter or setter functions. 
 Shallow data structures are more portable.
 MetDataModel provides a template, and application projects can extend it to fit their specific needs.
 
+There are two flavors of the metDataModel provided. The default version uses Python Dataclasses to 
+enforce weak static typing. These types are recommended and not enforced at runtime, but should provide
+users details to implement methods that use them in statically typed languages. The other is 
+dictionary based and has no suggested types. This is the minimal model. 
+
+Note that while metDataModel objects can have other metDataObjects as data members, this can cause 
+issues if there are circular references. 
+
 Please feel free to submit issues, and write Wiki pages for discussions.
 
 Pypi install: https://pypi.org/project/metDataModel/
 
 
 ### Related community resources
 While we focus on the application of mass spectrometry data,
```

### Comparing `metDataModel-0.6.0/setup.py` & `metdatamodel-0.6.1/setup.py`

 * *Files identical despite different names*

