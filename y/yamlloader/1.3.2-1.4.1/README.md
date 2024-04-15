# Comparing `tmp/yamlloader-1.3.2.tar.gz` & `tmp/yamlloader-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlloader-1.3.2.tar", last modified: Wed Aug  2 12:46:34 2023, max compression
+gzip compressed data, was "yamlloader-1.4.1.tar", last modified: Mon Apr 15 05:18:19 2024, max compression
```

## Comparing `yamlloader-1.3.2.tar` & `yamlloader-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-02 12:46:25.000000 yamlloader-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 12:46:25.000000 yamlloader-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-02 12:46:34.660501 yamlloader-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-02 12:46:25.000000 yamlloader-1.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 12:46:25.000000 yamlloader-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 12:46:25.000000 yamlloader-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:46:34.660501 yamlloader-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-02 12:46:25.000000 yamlloader-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.656501 yamlloader-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    71023 2023-08-02 12:46:25.000000 yamlloader-1.3.2/tests/test_ext_anatools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-08-02 12:46:25.000000 yamlloader-1.3.2/tests/test_ordereddict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.656501 yamlloader-1.3.2/yamlloader/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/yamlloader/ordereddict/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/yamlloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader.egg-info/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:18:19.461322 yamlloader-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-15 05:18:16.000000 yamlloader-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 05:18:16.000000 yamlloader-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-15 05:18:19.461322 yamlloader-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-15 05:18:16.000000 yamlloader-1.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-15 05:18:16.000000 yamlloader-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 05:18:16.000000 yamlloader-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 05:18:19.461322 yamlloader-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-15 05:18:16.000000 yamlloader-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:18:19.457322 yamlloader-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    71023 2024-04-15 05:18:16.000000 yamlloader-1.4.1/tests/test_ext_anatools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-15 05:18:16.000000 yamlloader-1.4.1/tests/test_ordereddict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:18:19.457322 yamlloader-1.4.1/yamlloader/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:18:19.461322 yamlloader-1.4.1/yamlloader/ordereddict/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader/ordereddict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader/ordereddict/dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader/ordereddict/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:18:19.461322 yamlloader-1.4.1/yamlloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 05:18:16.000000 yamlloader-1.4.1/yamlloader.egg-info/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 05:18:19.000000 yamlloader-1.4.1/yamlloader.egg-info/top_level.txt
```

### Comparing `yamlloader-1.3.2/LICENSE` & `yamlloader-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlloader-1.3.2/PKG-INFO` & `yamlloader-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlloader
-Version: 1.3.2
+Version: 1.4.1
 Summary: Ordered YAML loader and dumper for PyYAML.
 Home-page: https://github.com/Phynix/yamlloader
 Download-URL: https://github.com/Phynix/yamlloader
 Author: Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"
 Author-email: jonas.eschle@phynix.science, johannes.lade@phynix.science
 Maintainer: Jonas Eschle "Mayou36"
 Maintainer-email: jonas.eschle@phynix.science
@@ -18,18 +18,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyyaml
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
 
 
 .. image:: https://github.com/Phynix/yamlloader/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Phynix/yamlloader/actions
 .. image:: https://img.shields.io/pypi/pyversions/yamlloader.svg
     :target: https://pypi.org/project/yamlloader/
 .. image:: https://badge.fury.io/py/yamlloader.svg
```

### Comparing `yamlloader-1.3.2/README.rst` & `yamlloader-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `yamlloader-1.3.2/setup.py` & `yamlloader-1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import os
+from __future__ import annotations
+
+from pathlib import Path
 
 from setuptools import setup
 
-here = os.path.abspath(os.path.dirname(__file__))
+here = Path(__file__).resolve().parent
 
-with open(os.path.join(here, "requirements.txt")) as f:
+with (here / "requirements.txt").open() as f:
     requirements = f.read().split("\n")
 
 
 def long_description():
     """Load README.rst."""
-    with open("README.rst", encoding="utf-8") as f:
+    with Path("README.rst").open(encoding="utf-8") as f:
         return f.read()
 
 
 dev_requiremnets = ["pytest", "hypothesis"]
 setup(
     name="yamlloader",
-    version="1.3.2",
+    version="1.4.1",
     author='Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"',
     author_email="jonas.eschle@phynix.science, johannes.lade@phynix.science",
     maintainer='Jonas Eschle "Mayou36"',
     maintainer_email="jonas.eschle@phynix.science",
     url="https://github.com/Phynix/yamlloader",
     download_url="https://github.com/Phynix/yamlloader",
     license="MIT License",
@@ -37,14 +39,16 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
     packages=["yamlloader", "yamlloader.ordereddict"],
     python_requires=">=3.7",
     install_requires=requirements,
     tests_require=dev_requiremnets,
     extras_require={"dev": dev_requiremnets},
```

### Comparing `yamlloader-1.3.2/tests/test_ext_anatools.py` & `yamlloader-1.4.1/tests/test_ext_anatools.py`

 * *Files identical despite different names*

### Comparing `yamlloader-1.3.2/tests/test_ordereddict.py` & `yamlloader-1.4.1/tests/test_ordereddict.py`

 * *Files identical despite different names*

### Comparing `yamlloader-1.3.2/yamlloader/__init__.py` & `yamlloader-1.4.1/yamlloader/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 
 if sys.version_info[:2] < (2, 7):
     raise RuntimeError(
         "You are using Python < 2.7. This is not supported. "
         "Please upgrade your distribution and/or packages."
     )
 
-__version__ = "1.2.2"
+__version__ = "1.4.1"
 __author__ = 'Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"'
 __email__ = "jonas.eschle@phynix.science, johannes.lade@phynix.science"
 
 __all__ = ["ordereddict"]
```

### Comparing `yamlloader-1.3.2/yamlloader/ordereddict/dumpers.py` & `yamlloader-1.4.1/yamlloader/ordereddict/dumpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Dumpers for `:py:class:~collections.OrderedDict`."""
 
+from __future__ import annotations
+
 from collections import OrderedDict
 
 import yaml
 
 from .. import settings
 
 __all__ = []
```

### Comparing `yamlloader-1.3.2/yamlloader/ordereddict/loaders.py` & `yamlloader-1.4.1/yamlloader/ordereddict/loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Loaders for `:py:class:~collections.OrderedDict`."""
 
+from __future__ import annotations
+
 from collections import OrderedDict
 
 import yaml
 
 from .. import settings
 
 __all__ = []
@@ -17,29 +19,30 @@
 
 
 def construct_mapping(self, node, deep=False):
     if isinstance(node, yaml.MappingNode):
         self.flatten_mapping(node)
     else:
         msg = f"Expected a mapping node, but found {node.id}"
-        raise yaml.constructor.ConstructError(None, None, msg, node.start_mark)
+        raise yaml.constructor.ConstructorError(None, None, msg, node.start_mark)
 
     mapping = OrderedDict()
 
     for key_node, value_node in node.value:
         key = self.construct_object(key_node, deep=deep)
         try:
             hash(key)
         except TypeError as err:
-            raise yaml.constructor.ConstructError(
-                "while constructing a mapping",
+            msg = "while constructing a mapping"
+            raise yaml.constructor.ConstructorError(
+                msg,
                 node.start_mark,
                 f"found unacceptable key ({err})",
                 key_node.start_mark,
-            )
+            ) from err
         value = self.construct_object(value_node, deep=deep)
         mapping[key] = value
     return mapping
 
 
 class OrderedLoaderMixin:
     def __init__(self, *args, **kwargs):
```

### Comparing `yamlloader-1.3.2/yamlloader.egg-info/PKG-INFO` & `yamlloader-1.4.1/yamlloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlloader
-Version: 1.3.2
+Version: 1.4.1
 Summary: Ordered YAML loader and dumper for PyYAML.
 Home-page: https://github.com/Phynix/yamlloader
 Download-URL: https://github.com/Phynix/yamlloader
 Author: Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"
 Author-email: jonas.eschle@phynix.science, johannes.lade@phynix.science
 Maintainer: Jonas Eschle "Mayou36"
 Maintainer-email: jonas.eschle@phynix.science
@@ -18,18 +18,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyyaml
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
 
 
 .. image:: https://github.com/Phynix/yamlloader/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Phynix/yamlloader/actions
 .. image:: https://img.shields.io/pypi/pyversions/yamlloader.svg
     :target: https://pypi.org/project/yamlloader/
 .. image:: https://badge.fury.io/py/yamlloader.svg
```

