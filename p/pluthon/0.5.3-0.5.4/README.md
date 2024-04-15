# Comparing `tmp/pluthon-0.5.3.tar.gz` & `tmp/pluthon-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluthon-0.5.3.tar", last modified: Tue Apr  2 13:52:22 2024, max compression
+gzip compressed data, was "pluthon-0.5.4.tar", last modified: Mon Apr 15 11:22:17 2024, max compression
```

## Comparing `pluthon-0.5.3.tar` & `pluthon-0.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:52:22.303259 pluthon-0.5.3/
--rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-02 13:52:22.303259 pluthon-0.5.3/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1001 2024-04-02 13:51:16.000000 pluthon-0.5.3/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:52:22.299260 pluthon-0.5.3/pluthon/
--rw-r--r--   0 travis    (1000) travis    (1000)      647 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1937 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/compiler_config.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:52:22.303259 pluthon-0.5.3/pluthon/optimize/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/optimize/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1147 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/optimize/constant_index_access_list.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9675 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/optimize/patterns.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5398 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/pluthon_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2694 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/pluthon_functional_data.py
--rw-r--r--   0 travis    (1000) travis    (1000)    31767 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/pluthon_sugar.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1215 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/tools.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5041 2024-04-02 13:51:16.000000 pluthon-0.5.3/pluthon/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:52:22.303259 pluthon-0.5.3/pluthon.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-02 13:52:22.000000 pluthon-0.5.3/pluthon.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      440 2024-04-02 13:52:22.000000 pluthon-0.5.3/pluthon.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2024-04-02 13:52:22.000000 pluthon-0.5.3/pluthon.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      112 2024-04-02 13:52:22.000000 pluthon-0.5.3/pluthon.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2024-04-02 13:52:22.000000 pluthon-0.5.3/pluthon.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2024-04-02 13:52:22.303259 pluthon-0.5.3/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1842 2024-04-02 13:51:16.000000 pluthon-0.5.3/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-15 11:22:17.675140 pluthon-0.5.4/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-15 11:22:17.675140 pluthon-0.5.4/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1001 2024-04-15 11:21:09.000000 pluthon-0.5.4/README.md
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-15 11:22:17.671141 pluthon-0.5.4/pluthon/
+-rw-r--r--   0 travis    (1000) travis    (1000)      647 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1974 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/compiler_config.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-15 11:22:17.671141 pluthon-0.5.4/pluthon/optimize/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/optimize/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1147 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/optimize/constant_index_access_list.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9675 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/optimize/patterns.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5398 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/pluthon_ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2694 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/pluthon_functional_data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    31767 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/pluthon_sugar.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1215 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/tools.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5041 2024-04-15 11:21:09.000000 pluthon-0.5.4/pluthon/util.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-15 11:22:17.671141 pluthon-0.5.4/pluthon.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-15 11:22:17.000000 pluthon-0.5.4/pluthon.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      440 2024-04-15 11:22:17.000000 pluthon-0.5.4/pluthon.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2024-04-15 11:22:17.000000 pluthon-0.5.4/pluthon.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      112 2024-04-15 11:22:17.000000 pluthon-0.5.4/pluthon.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       13 2024-04-15 11:22:17.000000 pluthon-0.5.4/pluthon.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2024-04-15 11:22:17.675140 pluthon-0.5.4/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1842 2024-04-15 11:21:09.000000 pluthon-0.5.4/setup.py
```

### Comparing `pluthon-0.5.3/PKG-INFO` & `pluthon-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.5.3
+Version: 0.5.4
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/opshin/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.5.3/README.md` & `pluthon-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/__init__.py` & `pluthon-0.5.4/pluthon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from .compiler_config import *
 except ImportError as e:
     logging.error(
         "Error, trying to import dependencies. Should only occur upon package installation",
         exc_info=e,
     )
 
-VERSION = (0, 5, 3)
+VERSION = (0, 5, 4)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/opshin/pluthon"
```

### Comparing `pluthon-0.5.3/pluthon/compiler_config.py` & `pluthon-0.5.4/pluthon/compiler_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self, other: Optional["CompilationConfig"] = None, **kwargs
     ) -> "CompilationConfig":
         own_dict = self.__dict__
         other_dict = other.__dict__ if isinstance(other, CompilationConfig) else kwargs
         return self.__class__(
             **{
                 k: other_dict.get(k) if other_dict.get(k) is not None else own_dict[k]
-                for k in own_dict
+                for k in set(own_dict.keys()) | set(other_dict.keys())
             }
         )
 
 
 # The default configuration for the compiler
 OPT_O0_CONFIG = CompilationConfig(
     compress_patterns=False,
```

### Comparing `pluthon-0.5.3/pluthon/optimize/constant_index_access_list.py` & `pluthon-0.5.4/pluthon/optimize/constant_index_access_list.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/optimize/patterns.py` & `pluthon-0.5.4/pluthon/optimize/patterns.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/pluthon_ast.py` & `pluthon-0.5.4/pluthon/pluthon_ast.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/pluthon_functional_data.py` & `pluthon-0.5.4/pluthon/pluthon_functional_data.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/pluthon_sugar.py` & `pluthon-0.5.4/pluthon/pluthon_sugar.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/tools.py` & `pluthon-0.5.4/pluthon/tools.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon/util.py` & `pluthon-0.5.4/pluthon/util.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.3/pluthon.egg-info/PKG-INFO` & `pluthon-0.5.4/pluthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.5.3
+Version: 0.5.4
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/opshin/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.5.3/setup.py` & `pluthon-0.5.4/setup.py`

 * *Files identical despite different names*

