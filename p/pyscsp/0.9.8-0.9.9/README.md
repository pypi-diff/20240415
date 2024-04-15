# Comparing `tmp/pyscsp-0.9.8.tar.gz` & `tmp/pyscsp-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscsp-0.9.8.tar", max compression
+gzip compressed data, was "pyscsp-0.9.9.tar", max compression
```

## Comparing `pyscsp-0.9.8.tar` & `pyscsp-0.9.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      750 2023-10-02 10:54:01.268119 pyscsp-0.9.8/LICENSE.md
--rw-r--r--   0        0        0     7656 2023-10-11 04:49:06.962721 pyscsp-0.9.8/README.md
--rw-r--r--   0        0        0     1592 2023-10-11 04:50:12.818501 pyscsp-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      284 2023-10-10 13:31:29.845153 pyscsp-0.9.8/pyscsp/__init__.py
--rw-r--r--   0        0        0    64814 2023-10-04 09:04:52.622575 pyscsp-0.9.8/pyscsp/discscsp.py
--rw-r--r--   0        0        0    11972 2023-10-04 09:49:41.613785 pyscsp-0.9.8/pyscsp/torchscsp.py
--rw-r--r--   0        0        0     8384 1970-01-01 00:00:00.000000 pyscsp-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-10-02 10:54:01.268119 pyscsp-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0     7656 2023-10-11 04:49:06.962721 pyscsp-0.9.9/README.md
+-rw-r--r--   0        0        0     1592 2023-10-13 15:16:17.887790 pyscsp-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-10-10 13:31:29.845153 pyscsp-0.9.9/pyscsp/__init__.py
+-rw-r--r--   0        0        0    64814 2023-10-04 09:04:52.622575 pyscsp-0.9.9/pyscsp/discscsp.py
+-rw-r--r--   0        0        0    11972 2023-10-04 09:49:41.613785 pyscsp-0.9.9/pyscsp/torchscsp.py
+-rw-r--r--   0        0        0     8384 1970-01-01 00:00:00.000000 pyscsp-0.9.9/PKG-INFO
```

### Comparing `pyscsp-0.9.8/LICENSE.md` & `pyscsp-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyscsp-0.9.8/README.md` & `pyscsp-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscsp-0.9.8/pyproject.toml` & `pyscsp-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyscsp"
-version = "0.9.8"
+version = "0.9.9"
 description = "Scale-Space Toolbox for Python."
 authors = ["Tony Lindeberg <tony@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tonylindeberg/pyscsp"
 
 [tool.poetry.dependencies]
```

### Comparing `pyscsp-0.9.8/pyscsp/discscsp.py` & `pyscsp-0.9.9/pyscsp/discscsp.py`

 * *Files identical despite different names*

### Comparing `pyscsp-0.9.8/pyscsp/torchscsp.py` & `pyscsp-0.9.9/pyscsp/torchscsp.py`

 * *Files identical despite different names*

### Comparing `pyscsp-0.9.8/PKG-INFO` & `pyscsp-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscsp
-Version: 0.9.8
+Version: 0.9.9
 Summary: Scale-Space Toolbox for Python.
 Home-page: https://github.com/tonylindeberg/pyscsp
 License: MIT
 Author: Tony Lindeberg
 Author-email: tony@kth.se
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

