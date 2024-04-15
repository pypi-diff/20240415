# Comparing `tmp/pana-0.2.0.tar.gz` & `tmp/pana-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pana-0.2.0.tar", last modified: Sun Aug  6 21:37:23 2023, max compression
+gzip compressed data, was "pana-0.2.1.tar", last modified: Mon Apr 15 06:20:00 2024, max compression
```

## Comparing `pana-0.2.0.tar` & `pana-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-08-06 21:37:23.459187 pana-0.2.0/
--rw-r--r--   0 azazel     (501) staff       (20)     1301 2023-07-11 00:01:43.000000 pana-0.2.0/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)     1659 2023-08-06 21:37:23.459026 pana-0.2.0/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     1188 2023-08-06 21:34:13.000000 pana-0.2.0/README.md
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-08-06 21:37:23.458840 pana-0.2.0/pana.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     1659 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      204 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       40 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)       18 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)        5 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/top_level.txt
--rw-r--r--   0 azazel     (501) staff       (20)     2944 2023-08-06 21:13:52.000000 pana-0.2.0/pana.py
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-08-06 21:37:23.459229 pana-0.2.0/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     1024 2023-08-06 21:18:01.000000 pana-0.2.0/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 06:20:00.996050 pana-0.2.1/
+-rw-r--r--   0 azazel     (501) staff       (20)     1308 2024-04-15 06:18:06.000000 pana-0.2.1/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1715 2024-04-15 06:20:00.995774 pana-0.2.1/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     1192 2024-04-15 06:18:22.000000 pana-0.2.1/README.md
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 06:20:00.995529 pana-0.2.1/pana.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1715 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      204 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       40 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       18 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        5 2024-04-15 06:20:00.000000 pana-0.2.1/pana.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     2952 2024-04-15 06:18:39.000000 pana-0.2.1/pana.py
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 06:20:00.996096 pana-0.2.1/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1034 2024-04-15 06:18:48.000000 pana-0.2.1/setup.py
```

### Comparing `pana-0.2.0/LICENSE` & `pana-0.2.1/LICENSE`

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

### Comparing `pana-0.2.0/PKG-INFO` & `pana-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pana
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pana is a CLI and module built to check if a package name or username is available from common package managers.
-Home-page: https://github.com/azazelm3dj3d/pana
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/pana
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: colorama
 
 <h2 align="center">Pana - Pick a Name Already</h2>
 
 <p align="center">
   Check if a package or username is available from some of the most popular package managers.
 </p>
 
@@ -39,15 +41,15 @@
 
 ### Module
 ```python
 from pana import Pana
 
 # Print both lists to stdout
 print(Pana.check_pkg("pana"))
-print(Pana.check_user("azazelm3dj3d"))
+print(Pana.check_user("battleoverflow"))
 
 # Example output
 """
 [
   ['pypi', False],
   ['npm', False],
   ['nuget', True],
@@ -63,9 +65,9 @@
 ```bash
 pana -p pana
 ```
 
 Search for a username
 
 ```bash
-pana -u azazelm3dj3d
+pana -u battleoverflow
 ```
```

### Comparing `pana-0.2.0/README.md` & `pana-0.2.1/pana.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pana
+Version: 0.2.1
+Summary: Pana is a CLI and module built to check if a package name or username is available from common package managers.
+Home-page: https://github.com/battleoverflow/pana
+Author: battleoverflow
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: colorama
+
 <h2 align="center">Pana - Pick a Name Already</h2>
 
 <p align="center">
   Check if a package or username is available from some of the most popular package managers.
 </p>
 
 
@@ -26,15 +41,15 @@
 
 ### Module
 ```python
 from pana import Pana
 
 # Print both lists to stdout
 print(Pana.check_pkg("pana"))
-print(Pana.check_user("azazelm3dj3d"))
+print(Pana.check_user("battleoverflow"))
 
 # Example output
 """
 [
   ['pypi', False],
   ['npm', False],
   ['nuget', True],
@@ -50,9 +65,9 @@
 ```bash
 pana -p pana
 ```
 
 Search for a username
 
 ```bash
-pana -u azazelm3dj3d
+pana -u battleoverflow
 ```
```

### Comparing `pana-0.2.0/pana.py` & `pana-0.2.1/pana.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
-    Project: Pana (https://github.com/azazelm3dj3d/pana)
-    Author: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: Pana (https://github.com/battleoverflow/pana)
+    Author: battleoverflow (https://github.com/battleoverflow)
     License: BSD 2-Clause
 """
 
 import requests
 import argparse
 from colorama import Fore, Style
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-p', '--pkg', help="Name of the package", default=None, required=False)
 parser.add_argument('-u', '--user', help="Name of the username", default=None, required=False)
 args = parser.parse_args()
 
-version = "0.2.0"
+version = "0.2.1"
 
 banner = \
 f"""
  ____  _____ ____  _____ 
 |  _ \(____ |  _ \(____ |
 | |_| / ___ | | | / ___ |
 |  __/\_____|_| |_\_____|
 |_|
 
-   azazelm3dj3d | v{version}
+   battleoverflow | v{version}
 """
 
 class Pana:
 
     def check_pkg(pkg_name: str) -> list:
 
         pkg_config = {
```

### Comparing `pana-0.2.0/setup.py` & `pana-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-    Project: Pana (https://github.com/azazelm3dj3d/pana)
-    Author: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: Pana (https://github.com/battleoverflow/pana)
+    Author: battleoverflow (https://github.com/battleoverflow)
     License: BSD 2-Clause
 """
 
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pana",
-    version = "0.2.0",
-    author = "azazelm3dj3d",
+    version = "0.2.1",
+    author = "battleoverflow",
     description = "Pana is a CLI and module built to check if a package name or username is available from common package managers.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/azazelm3dj3d/pana",
+    url = "https://github.com/battleoverflow/pana",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     py_modules=['pana'],
     install_requires=[
```

