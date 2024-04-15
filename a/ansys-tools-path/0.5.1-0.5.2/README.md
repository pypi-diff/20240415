# Comparing `tmp/ansys_tools_path-0.5.1.tar.gz` & `tmp/ansys_tools_path-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.5.1.tar` & `ansys_tools_path-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1089 2024-04-02 16:18:20.462743 ansys_tools_path-0.5.1/LICENSE
--rw-r--r--   0        0        0     4692 2024-04-02 16:18:20.462743 ansys_tools_path-0.5.1/README.rst
--rw-r--r--   0        0        0     1981 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1697 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      297 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/applications/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/applications/dyna.py
--rw-r--r--   0        0        0     1417 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/applications/mapdl.py
--rw-r--r--   0        0        0     1726 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/applications/mechanical.py
--rw-r--r--   0        0        0      677 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    38025 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0        0 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/py.typed
--rw-r--r--   0        0        0     1971 2024-04-02 16:18:20.466743 ansys_tools_path-0.5.1/src/ansys/tools/path/save.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-15 19:06:49.783151 ansys_tools_path-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4692 2024-04-15 19:06:49.783151 ansys_tools_path-0.5.2/README.rst
+-rw-r--r--   0        0        0     2027 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1697 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/dyna.py
+-rw-r--r--   0        0        0     1417 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mapdl.py
+-rw-r--r--   0        0        0     1726 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mechanical.py
+-rw-r--r--   0        0        0      677 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    38410 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/py.typed
+-rw-r--r--   0        0        0     1971 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/save.py
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 ansys_tools_path-0.5.2/PKG-INFO
```

### Comparing `ansys_tools_path-0.5.1/LICENSE` & `ansys_tools_path-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/README.rst` & `ansys_tools_path-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/pyproject.toml` & `ansys_tools_path-0.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.5.1"
+version = "0.5.2"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "platformdirs>=3.6.0",
     "click>=8.1.3",        # for CLI interface
 ]
 
 
 [project.optional-dependencies]
-tests = ["pytest==8.1.1", "pytest-cov==5.0.0", "pyfakefs==5.3.5"]
+tests = ["pytest==8.1.1", "pytest-cov==5.0.0", "pyfakefs==5.4.1"]
 
 doc = [
     "Sphinx==7.2.6",
     "numpydoc==1.7.0",
-    "ansys-sphinx-theme==0.15.0",
+    "ansys-sphinx-theme==0.15.2",
     "sphinx-copybutton==0.5.2",
 ]
 
 build = ["build==1.2.1", "twine==5.0.0"]
 
 [tool.flit.module]
 name = "ansys.tools.path"
```

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/applications/dyna.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/dyna.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/applications/mapdl.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mapdl.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/applications/mechanical.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/path.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -939,18 +939,27 @@
 
 def _get_application_path(
     product: str,
     allow_input: bool = True,
     version: Optional[float] = None,
     find: bool = True,
 ) -> Optional[str]:
-    if version is None:
-        exe_loc = _read_executable_path_from_config_file(product)
-        if exe_loc is not None:
-            return exe_loc
+    _exe_loc = _read_executable_path_from_config_file(product)
+    if _exe_loc is not None:
+        if version is None:
+            return _exe_loc
+        else:
+            _version = version_from_path(product, _exe_loc)
+            if _version == version:
+                return _exe_loc
+            else:
+                LOG.debug(
+                    f"Application {product} requested version {version} does not match with {_version} "
+                    f"in config file. Trying to find version {version} ..."
+                )
 
     LOG.debug(f"{product} path not found in config file")
     if not _has_plugin(product):
         raise Exception(f"Application {product} not registered.")
 
     if find:
         try:
```

### Comparing `ansys_tools_path-0.5.1/src/ansys/tools/path/save.py` & `ansys_tools_path-0.5.2/src/ansys/tools/path/save.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.1/PKG-INFO` & `ansys_tools_path-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.5.1
+Version: 0.5.2
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: platformdirs>=3.6.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: build==1.2.1 ; extra == "build"
 Requires-Dist: twine==5.0.0 ; extra == "build"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.15.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==8.1.1 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
-Requires-Dist: pyfakefs==5.3.5 ; extra == "tests"
+Requires-Dist: pyfakefs==5.4.1 ; extra == "tests"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
 Project-URL: Source, https://github.com/ansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: tests
```

