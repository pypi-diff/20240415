# Comparing `tmp/shhistory-0.1.8.tar.gz` & `tmp/shhistory-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shhistory-0.1.8.tar", last modified: Sun Jan 15 04:41:20 2023, max compression
+gzip compressed data, was "shhistory-0.1.9.tar", last modified: Mon Apr 15 04:21:33 2024, max compression
```

## Comparing `shhistory-0.1.8.tar` & `shhistory-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-01-15 04:41:20.160854 shhistory-0.1.8/
--rw-r--r--   0 azazel     (501) staff       (20)     1301 2023-01-15 04:38:34.000000 shhistory-0.1.8/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)     1170 2023-01-15 04:41:20.160646 shhistory-0.1.8/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      709 2023-01-15 04:39:09.000000 shhistory-0.1.8/README.md
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-01-15 04:41:20.160907 shhistory-0.1.8/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)      887 2023-01-15 04:39:19.000000 shhistory-0.1.8/setup.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-01-15 04:41:20.160400 shhistory-0.1.8/shhistory.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     1170 2023-01-15 04:41:20.000000 shhistory-0.1.8/shhistory.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      171 2023-01-15 04:41:20.000000 shhistory-0.1.8/shhistory.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-01-15 04:41:20.000000 shhistory-0.1.8/shhistory.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       10 2023-01-15 04:41:20.000000 shhistory-0.1.8/shhistory.egg-info/top_level.txt
--rw-r--r--   0 azazel     (501) staff       (20)     1835 2023-01-15 04:39:41.000000 shhistory-0.1.8/shhistory.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:21:33.397171 shhistory-0.1.9/
+-rw-r--r--   0 azazel     (501) staff       (20)     1308 2024-04-15 04:20:04.000000 shhistory-0.1.9/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1174 2024-04-15 04:21:33.396953 shhistory-0.1.9/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      709 2024-04-15 04:19:48.000000 shhistory-0.1.9/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 04:21:33.397211 shhistory-0.1.9/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)      898 2024-04-15 04:20:37.000000 shhistory-0.1.9/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:21:33.396704 shhistory-0.1.9/shhistory.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1174 2024-04-15 04:21:33.000000 shhistory-0.1.9/shhistory.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      171 2024-04-15 04:21:33.000000 shhistory-0.1.9/shhistory.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 04:21:33.000000 shhistory-0.1.9/shhistory.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       10 2024-04-15 04:21:33.000000 shhistory-0.1.9/shhistory.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     1841 2024-04-15 04:20:26.000000 shhistory-0.1.9/shhistory.py
```

### Comparing `shhistory-0.1.8/LICENSE` & `shhistory-0.1.9/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2023, azazelm3dj3d
+Copyright (c) 2023-2024, battleoverflow
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `shhistory-0.1.8/PKG-INFO` & `shhistory-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shhistory
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple Python library to return your shell history or dump to a nicely formatted JSON file.
-Home-page: https://github.com/azazelm3dj3d/shhistory
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/shhistory
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `shhistory-0.1.8/README.md` & `shhistory-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `shhistory-0.1.8/setup.py` & `shhistory-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-    Project: shhistory (https://github.com/azazelm3dj3d/shhistory)
-    Author: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: shhistory (https://github.com/battleoverflow/shhistory)
+    Author: battleoverflow (https://github.com/battleoverflow)
     License: BSD 2-Clause
 """
 
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "shhistory",
-    version = "0.1.8",
-    author = "azazelm3dj3d",
+    version = "0.1.9",
+    author = "battleoverflow",
     description = "Simple Python library to return your shell history or dump to a nicely formatted JSON file.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/azazelm3dj3d/shhistory",
+    url = "https://github.com/battleoverflow/shhistory",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
     py_modules=["shhistory"],
     python_requires = ">=3.6"
-)
+)
```

### Comparing `shhistory-0.1.8/shhistory.egg-info/PKG-INFO` & `shhistory-0.1.9/shhistory.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shhistory
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple Python library to return your shell history or dump to a nicely formatted JSON file.
-Home-page: https://github.com/azazelm3dj3d/shhistory
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/shhistory
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `shhistory-0.1.8/shhistory.py` & `shhistory-0.1.9/shhistory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-    Project: shhistory (https://github.com/azazelm3dj3d/shhistory)
-    Author: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: shhistory (https://github.com/battleoverflow/shhistory)
+    Author: battleoverflow (https://github.com/battleoverflow)
     License: BSD 2-Clause
 """
 
 import platform, os, json
 
 # Accepted platforms
 platform_type = [
```

