# Comparing `tmp/foamlib-0.2.8.tar.gz` & `tmp/foamlib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.8.tar", last modified: Thu Apr 11 16:25:11 2024, max compression
+gzip compressed data, was "foamlib-0.2.9.tar", last modified: Fri Apr 12 18:57:56 2024, max compression
```

## Comparing `foamlib-0.2.8.tar` & `foamlib-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.893628 foamlib-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-11 16:25:07.000000 foamlib-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-11 16:25:11.893628 foamlib-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-11 16:25:07.000000 foamlib-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib/_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-11 16:25:07.000000 foamlib-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:25:11.893628 foamlib-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:57:56.162921 foamlib-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-12 18:57:48.000000 foamlib-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 18:57:56.162921 foamlib-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-12 18:57:48.000000 foamlib-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:57:56.158921 foamlib-0.2.9/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:57:56.162921 foamlib-0.2.9/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:57:48.000000 foamlib-0.2.9/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:57:56.162921 foamlib-0.2.9/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 18:57:56.000000 foamlib-0.2.9/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-12 18:57:56.000000 foamlib-0.2.9/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:57:56.000000 foamlib-0.2.9/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 18:57:56.000000 foamlib-0.2.9/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 18:57:56.000000 foamlib-0.2.9/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-12 18:57:48.000000 foamlib-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:57:56.162921 foamlib-0.2.9/setup.cfg
```

### Comparing `foamlib-0.2.8/LICENSE.txt` & `foamlib-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/PKG-INFO` & `foamlib-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.8/README.md` & `foamlib-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib/_cases.py` & `foamlib-0.2.9/foamlib/_cases.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib/_dictionaries/_base.py` & `foamlib-0.2.9/foamlib/_dictionaries/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib/_dictionaries/_files.py` & `foamlib-0.2.9/foamlib/_dictionaries/_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from copy import deepcopy
 from pathlib import Path
 from types import TracebackType
 from typing import (
     Any,
     Optional,
     Tuple,
     Type,
@@ -68,17 +69,20 @@
             if contents != self.__contents:
                 self.__contents = contents
                 self.__parsed = None
 
         assert self.__contents is not None
 
         if self.__parsed is None:
-            self.__parsed = parse(self.__contents)
+            parsed = parse(self.__contents)
+            self.__parsed = parsed
+        else:
+            parsed = deepcopy(self.__parsed)
 
-        return self.__contents, self.__parsed
+        return self.__contents, parsed
 
     def _write(self, contents: str) -> None:
         self.__contents = contents
         self.__parsed = None
         if not self.__defer_io:
             self.path.write_text(contents)
             self.__dirty = False
```

### Comparing `foamlib-0.2.8/foamlib/_dictionaries/_parsing.py` & `foamlib-0.2.9/foamlib/_dictionaries/_parsing.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib/_dictionaries/_serialization.py` & `foamlib-0.2.9/foamlib/_dictionaries/_serialization.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib/_util.py` & `foamlib-0.2.9/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.8/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.9/foamlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.8/pyproject.toml` & `foamlib-0.2.9/pyproject.toml`

 * *Files identical despite different names*

