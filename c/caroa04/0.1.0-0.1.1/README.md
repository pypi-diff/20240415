# Comparing `tmp/caroa04-0.1.0.tar.gz` & `tmp/caroa04-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caroa04-0.1.0.tar", last modified: Sun Apr 14 18:41:21 2024, max compression
+gzip compressed data, was "caroa04-0.1.1.tar", last modified: Sun Apr 14 19:02:31 2024, max compression
```

## Comparing `caroa04-0.1.0.tar` & `caroa04-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.947184 caroa04-0.1.0/
--rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2637 2024-04-14 18:41:21.945125 caroa04-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1793 2024-04-14 18:23:02.000000 caroa04-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.922525 caroa04-0.1.0/docs/
--rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4967 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-0.1.0/docs/usage.rst
--rw-rw-rw-   0        0        0     1323 2024-04-14 18:35:05.000000 caroa04-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 18:41:21.947184 caroa04-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.886101 caroa04-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.927296 caroa04-0.1.0/src/caroa04/
--rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-0.1.0/src/caroa04/__init__.py
--rw-rw-rw-   0        0        0     8958 2024-04-14 17:26:49.000000 caroa04-0.1.0/src/caroa04/canmessage.py
--rw-rw-rw-   0        0        0    10501 2024-04-14 18:33:21.000000 caroa04-0.1.0/src/caroa04/caroa04.py
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.943124 caroa04-0.1.0/src/caroa04.egg-info/
--rw-rw-rw-   0        0        0     2637 2024-04-14 18:41:21.000000 caroa04-0.1.0/src/caroa04.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-14 18:41:21.000000 caroa04-0.1.0/src/caroa04.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 18:41:21.000000 caroa04-0.1.0/src/caroa04.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-14 18:41:21.000000 caroa04-0.1.0/src/caroa04.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 18:41:21.000000 caroa04-0.1.0/src/caroa04.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 18:41:21.942124 caroa04-0.1.0/tests/
--rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     7403 2024-04-14 18:30:50.000000 caroa04-0.1.0/tests/test_caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.869630 caroa04-0.1.1/
+-rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2637 2024-04-14 19:02:31.867629 caroa04-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1793 2024-04-14 18:51:13.000000 caroa04-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.839784 caroa04-0.1.1/docs/
+-rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-0.1.1/docs/usage.rst
+-rw-rw-rw-   0        0        0     1323 2024-04-14 19:01:53.000000 caroa04-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:02:31.869630 caroa04-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.800227 caroa04-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.850174 caroa04-0.1.1/src/caroa04/
+-rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-0.1.1/src/caroa04/__init__.py
+-rw-rw-rw-   0        0        0     8958 2024-04-14 17:26:49.000000 caroa04-0.1.1/src/caroa04/canmessage.py
+-rw-rw-rw-   0        0        0    10524 2024-04-14 19:02:02.000000 caroa04-0.1.1/src/caroa04/caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.865632 caroa04-0.1.1/src/caroa04.egg-info/
+-rw-rw-rw-   0        0        0     2637 2024-04-14 19:02:31.000000 caroa04-0.1.1/src/caroa04.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-14 19:02:31.000000 caroa04-0.1.1/src/caroa04.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 19:02:31.000000 caroa04-0.1.1/src/caroa04.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-14 19:02:31.000000 caroa04-0.1.1/src/caroa04.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 19:02:31.000000 caroa04-0.1.1/src/caroa04.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 19:02:31.863637 caroa04-0.1.1/tests/
+-rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     7403 2024-04-14 18:51:13.000000 caroa04-0.1.1/tests/test_caroa04.py
```

### Comparing `caroa04-0.1.0/CONTRIBUTING.rst` & `caroa04-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/LICENSE` & `caroa04-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/PKG-INFO` & `caroa04-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
```

### Comparing `caroa04-0.1.0/README.rst` & `caroa04-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/docs/Makefile` & `caroa04-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/docs/conf.py` & `caroa04-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
-import caroa04
+import src.caroa04.caroa04 as caroa04
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `caroa04-0.1.0/docs/installation.rst` & `caroa04-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/docs/make.bat` & `caroa04-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/pyproject.toml` & `caroa04-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caroa04"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library to control the CAROA04 CAN-IO expander device from eletechsup."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
   {name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com"}
 ]
 maintainers = [
```

### Comparing `caroa04-0.1.0/src/caroa04/canmessage.py` & `caroa04-0.1.1/src/caroa04/canmessage.py`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/src/caroa04/caroa04.py` & `caroa04-0.1.1/src/caroa04/caroa04.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 sys.path.append(str(pathlib.Path(__file__).parent))
 
 from canmessage import *
 
 logging.basicConfig(level=logging.INFO)
 
 __author__ = "R. Soyding"
+__version__ = "0.1.1"
 
 MSGID_DO_WRITE = 0x100
 MSGID_DO_READ = 0x200
 MSGID_DI_READ = 0x300
 MSGID_PARAM = 0x700
 DEFAULT_NODEID = 0xE0
```

### Comparing `caroa04-0.1.0/src/caroa04.egg-info/PKG-INFO` & `caroa04-0.1.1/src/caroa04.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
```

### Comparing `caroa04-0.1.0/src/caroa04.egg-info/SOURCES.txt` & `caroa04-0.1.1/src/caroa04.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.0/tests/test_caroa04.py` & `caroa04-0.1.1/tests/test_caroa04.py`

 * *Files identical despite different names*

