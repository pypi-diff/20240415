# Comparing `tmp/ducktools-pythonfinder-0.1.0.tar.gz` & `tmp/ducktools_pythonfinder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools-pythonfinder-0.1.0.tar", last modified: Thu Feb 15 13:07:15 2024, max compression
+gzip compressed data, was "ducktools_pythonfinder-0.1.1.tar", last modified: Mon Apr 15 13:58:34 2024, max compression
```

## Comparing `ducktools-pythonfinder-0.1.0.tar` & `ducktools_pythonfinder-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.937160 ducktools-pythonfinder-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.937160 ducktools-pythonfinder-0.1.0/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.937160 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.937160 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/darwin/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/details_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.937160 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/linux/pyenv_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/pyenv_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/registry_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-02-15 13:07:15.000000 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-15 13:07:15.000000 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 13:07:15.000000 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-15 13:07:15.000000 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 13:07:15.000000 ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:07:15.941160 ducktools-pythonfinder-0.1.0/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/tests/sources/python_versions.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/tests/test_details_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/tests/test_foldersearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/tests/test_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-02-15 13:07:03.000000 ducktools-pythonfinder-0.1.0/tests/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.268868 ducktools_pythonfinder-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:58:34.268868 ducktools_pythonfinder-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.260868 ducktools_pythonfinder-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.260868 ducktools_pythonfinder-0.1.1/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/darwin/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/details_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/linux/pyenv_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/pyenv_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/registry_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-15 13:58:34.000000 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 13:58:34.000000 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:58:34.000000 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 13:58:34.000000 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:58:34.000000 ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:58:34.264868 ducktools_pythonfinder-0.1.1/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/tests/sources/python_versions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/tests/test_details_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/tests/test_foldersearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/tests/test_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-15 13:58:30.000000 ducktools_pythonfinder-0.1.1/tests/test_shared.py
```

### Comparing `ducktools-pythonfinder-0.1.0/COPYING` & `ducktools_pythonfinder-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/COPYING.LESSER` & `ducktools_pythonfinder-0.1.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/PKG-INFO` & `ducktools_pythonfinder-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-pythonfinder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cross platform tool to find available python installations
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/ducktools-pythonfinder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: ducktools-lazyimporter
-Requires-Dist: prefab-classes
+Requires-Dist: ducktools-classbuilder
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pyfakefs; extra == "testing"
 
 # ducktools: pythonfinder #
```

### Comparing `ducktools-pythonfinder-0.1.0/README.md` & `ducktools_pythonfinder-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/pyproject.toml` & `ducktools_pythonfinder-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 authors = [
     { name = "David C Ellis" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "ducktools-lazyimporter",
-    "prefab-classes",
+    "ducktools-classbuilder",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
```

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/__init__.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # Find platform python versions
 
-__version__ = "v0.1.0"
+__version__ = "v0.1.1"
 
 __all__ = [
     "get_python_installs",
     "list_python_installs",
     "PythonInstall",
 ]
```

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/__main__.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/__main__.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/darwin/__init__.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/darwin/__init__.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/details_script.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/details_script.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/linux/__init__.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/linux/pyenv_search.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/linux/pyenv_search.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/shared.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/shared.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import sys
 import os
 import os.path
 
-from prefab_classes import prefab, attribute
+from ducktools.classbuilder import slotclass, Field, SlotFields
 from ducktools.lazyimporter import LazyImporter, ModuleImport, FromImport
 
 from . import details_script
 
 _laz = LazyImporter(
     [
         ModuleImport("re"),
@@ -33,21 +33,28 @@
     ]
 )
 
 
 FULL_PY_VER_RE = r"(?P<major>\d+)\.(?P<minor>\d+)\.?(?P<micro>\d*)(?P<releaselevel>[a-zA-Z]*)(?P<serial>\d*)"
 
 
-@prefab
+@slotclass
 class PythonInstall:
+    __slots__ = SlotFields(
+        version=Field(),
+        executable=Field(),
+        architecture="64bit",
+        implementation="cpython",
+        metadata=Field(default_factory=dict),
+    )
     version: tuple[int, int, int, str, int]
     executable: str
-    architecture: str = "64bit"
-    implementation: str = "cpython"
-    metadata: dict = attribute(default_factory=dict)
+    architecture: str
+    implementation: str
+    metadata: dict
 
     @property
     def version_str(self) -> str:
         major, minor, micro, releaselevel, serial = self.version
 
         match releaselevel:
             case "alpha":
```

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/pyenv_search.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/pyenv_search.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools/pythonfinder/win32/registry_search.py` & `ducktools_pythonfinder-0.1.1/src/ducktools/pythonfinder/win32/registry_search.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/PKG-INFO` & `ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-pythonfinder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cross platform tool to find available python installations
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/ducktools-pythonfinder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: ducktools-lazyimporter
-Requires-Dist: prefab-classes
+Requires-Dist: ducktools-classbuilder
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pyfakefs; extra == "testing"
 
 # ducktools: pythonfinder #
```

### Comparing `ducktools-pythonfinder-0.1.0/src/ducktools_pythonfinder.egg-info/SOURCES.txt` & `ducktools_pythonfinder-0.1.1/src/ducktools_pythonfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/tests/sources/python_versions.txt` & `ducktools_pythonfinder-0.1.1/tests/sources/python_versions.txt`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/tests/test_details_script.py` & `ducktools_pythonfinder-0.1.1/tests/test_details_script.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/tests/test_foldersearch.py` & `ducktools_pythonfinder-0.1.1/tests/test_foldersearch.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/tests/test_pyenv.py` & `ducktools_pythonfinder-0.1.1/tests/test_pyenv.py`

 * *Files identical despite different names*

### Comparing `ducktools-pythonfinder-0.1.0/tests/test_shared.py` & `ducktools_pythonfinder-0.1.1/tests/test_shared.py`

 * *Files identical despite different names*

