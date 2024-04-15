# Comparing `tmp/pyprjbtstrptst-0.1.7-py3-none-any.whl.zip` & `tmp/pyprjbtstrptst-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9090 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3513 b- defN 24-Apr-13 01:58 BuildBinary.py
--rw-r--r--  2.0 unx     2552 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/EntryPoint.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/Math.py
--rw-r--r--  2.0 unx      612 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 24-Apr-13 01:58 pyprjbtstrptst/EntryPoint.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-13 01:58 pyprjbtstrptst/Math.py
--rw-r--r--  2.0 unx      598 b- defN 24-Apr-13 01:58 pyprjbtstrptst/__init__.py
--rw-r--r--  2.0 unx     1091 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5770 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       60 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1142 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/RECORD
-13 files, 19699 bytes uncompressed, 7150 bytes compressed:  63.7%
+Zip file size: 9131 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3513 b- defN 24-Apr-15 13:31 BuildBinary.py
+-rw-r--r--  2.0 unx     2552 b- defN 24-Apr-15 13:31 PythonProjectBootstrapperTesting/EntryPoint.py
+-rw-r--r--  2.0 unx      947 b- defN 24-Apr-15 13:31 PythonProjectBootstrapperTesting/Math.py
+-rw-r--r--  2.0 unx      612 b- defN 24-Apr-15 13:31 PythonProjectBootstrapperTesting/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 24-Apr-15 13:31 pyprjbtstrptst/EntryPoint.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-15 13:31 pyprjbtstrptst/Math.py
+-rw-r--r--  2.0 unx      598 b- defN 24-Apr-15 13:32 pyprjbtstrptst/__init__.py
+-rw-r--r--  2.0 unx     1091 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5770 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1142 b- defN 24-Apr-15 13:32 pyprjbtstrptst-0.1.8.dist-info/RECORD
+13 files, 19811 bytes uncompressed, 7191 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pyprjbtstrptst/Math.py
 Comment: 
 
 Filename: pyprjbtstrptst/__init__.py
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt
+Filename: pyprjbtstrptst-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/METADATA
+Filename: pyprjbtstrptst-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/WHEEL
+Filename: pyprjbtstrptst-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/entry_points.txt
+Filename: pyprjbtstrptst-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/top_level.txt
+Filename: pyprjbtstrptst-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.7.dist-info/RECORD
+Filename: pyprjbtstrptst-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PythonProjectBootstrapperTesting/Math.py

```diff
@@ -21,7 +21,12 @@
 def Mult(x, y):
     return x * y
 
 
 # ----------------------------------------------------------------------
 def Div(x, y):
     return x / y
+
+
+# ----------------------------------------------------------------------
+def Mod(x, y):
+    return x % y
```

## pyprjbtstrptst/__init__.py

```diff
@@ -5,10 +5,10 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 from .Math import Add, Sub, Mult, Div
```

## Comparing `pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt` & `pyprjbtstrptst-0.1.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pyprjbtstrptst-0.1.7.dist-info/METADATA` & `pyprjbtstrptst-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprjbtstrptst
-Version: 0.1.7
+Version: 0.1.8
 Summary: python proj btstrp test
 Author-email: Varun Narayan <varun646@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Documentation, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Repository, https://github.com/varun646/PythonProjectBootstrapperTest
 Classifier: License :: OSI Approved :: MIT License
```

