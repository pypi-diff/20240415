# Comparing `tmp/dysys-0.1.5.tar.gz` & `tmp/dysys-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysys-0.1.5.tar", max compression
+gzip compressed data, was "dysys-0.1.6.tar", max compression
```

## Comparing `dysys-0.1.5.tar` & `dysys-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1498 2024-02-01 09:26:06.877114 dysys-0.1.5/LICENSE
--rw-r--r--   0        0        0     1854 2024-03-20 06:27:39.755678 dysys-0.1.5/README.md
--rw-r--r--   0        0        0      120 2024-03-25 20:14:23.763429 dysys-0.1.5/dysys/__init__.py
--rw-r--r--   0        0        0     3710 2024-03-20 05:56:14.267785 dysys-0.1.5/dysys/controltf.py
--rw-r--r--   0        0        0     5469 2024-03-05 00:21:11.701919 dysys-0.1.5/dysys/statespacesymbolic.py
--rw-r--r--   0        0        0     1189 2024-03-04 21:43:00.231686 dysys-0.1.5/dysys/sysdyn.py
--rw-r--r--   0        0        0     2222 2024-03-11 20:05:48.865404 dysys-0.1.5/dysys/transferfunctions.py
--rw-r--r--   0        0        0     5724 2024-03-26 07:22:17.047525 dysys-0.1.5/dysys/transferfunctionsymbolic.py
--rw-r--r--   0        0        0      595 2024-03-26 07:27:04.649506 dysys-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dysys-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-02-01 09:26:06.877114 dysys-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1854 2024-03-20 06:27:39.755678 dysys-0.1.6/README.md
+-rw-r--r--   0        0        0      120 2024-03-25 20:14:23.763429 dysys-0.1.6/dysys/__init__.py
+-rw-r--r--   0        0        0     3710 2024-03-20 05:56:14.267785 dysys-0.1.6/dysys/controltf.py
+-rw-r--r--   0        0        0     5469 2024-03-05 00:21:11.701919 dysys-0.1.6/dysys/statespacesymbolic.py
+-rw-r--r--   0        0        0     1189 2024-03-04 21:43:00.231686 dysys-0.1.6/dysys/sysdyn.py
+-rw-r--r--   0        0        0     2222 2024-03-11 20:05:48.865404 dysys-0.1.6/dysys/transferfunctions.py
+-rw-r--r--   0        0        0     5830 2024-04-15 04:26:14.953037 dysys-0.1.6/dysys/transferfunctionsymbolic.py
+-rw-r--r--   0        0        0      595 2024-04-15 05:54:14.765611 dysys-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dysys-0.1.6/PKG-INFO
```

### Comparing `dysys-0.1.5/LICENSE` & `dysys-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/README.md` & `dysys-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/dysys/controltf.py` & `dysys-0.1.6/dysys/controltf.py`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/dysys/statespacesymbolic.py` & `dysys-0.1.6/dysys/statespacesymbolic.py`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/dysys/sysdyn.py` & `dysys-0.1.6/dysys/sysdyn.py`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/dysys/transferfunctions.py` & `dysys-0.1.6/dysys/transferfunctions.py`

 * *Files identical despite different names*

### Comparing `dysys-0.1.5/dysys/transferfunctionsymbolic.py` & `dysys-0.1.6/dysys/transferfunctionsymbolic.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class TransferFunctionSymbolic:
     """Represents a SISO continuous LTI transfer function model in symbolic form"""
 
     def __init__(self, H, s=None):
         if s is not None:
             self.s = s
         else:
-            self.s = sp.symbols("s", complex=True)
-            # self.s = list(H.free_symbols)[0]  # Don't need this because sp.symbols("s") is unique
+            # self.s = sp.symbols("s", complex=True)  # Should be able to but had issues
+            self.s = list(H.free_symbols)[0]  # Shouldn't need this because sp.symbols("s") is supposed to be unique. This doesn't work if there are other symbols in H
         num, den = sp.fraction(H)
         self.num = num.collect(self.s)
         self.den = den.collect(self.s)
         self.H = self.num/self.den
         sp.init_printing(order='grevlex')
         
     def __call__(self, s):
```

### Comparing `dysys-0.1.5/pyproject.toml` & `dysys-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dysys"
-version = "0.1.5"
+version = "0.1.6"
 description = "A package for working with system dynamics symbolically and numerically"
 authors = ["Rico Picone <rpicone@stmartin.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dysys-0.1.5/PKG-INFO` & `dysys-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysys
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for working with system dynamics symbolically and numerically
 License: MIT
 Author: Rico Picone
 Author-email: rpicone@stmartin.edu
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

