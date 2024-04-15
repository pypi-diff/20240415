# Comparing `tmp/objx-70.tar.gz` & `tmp/objx-80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objx-70.tar", last modified: Fri Apr 12 14:06:45 2024, max compression
+gzip compressed data, was "objx-80.tar", last modified: Mon Apr 15 12:21:15 2024, max compression
```

## Comparing `objx-70.tar` & `objx-80.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/
--rw-r--r--   0 bart      (1000) bart      (1000)     1406 2024-04-12 14:06:45.108174 objx-70/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      880 2024-04-06 11:08:24.000000 objx-70/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/objx/
--rw-r--r--   0 bart      (1000) bart      (1000)      664 2024-04-12 14:05:42.000000 objx-70/objx/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-12 14:05:42.000000 objx-70/objx/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-12 14:05:42.000000 objx-70/objx/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3261 2024-04-12 14:05:42.000000 objx-70/objx/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      731 2024-04-12 14:05:42.000000 objx-70/objx/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/objx.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     1406 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      249 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-12 14:06:38.000000 objx-70/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 14:06:45.108174 objx-70/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-06 11:08:24.000000 objx-70/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:21:15.266739 objx-80/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1391 2024-04-15 12:21:15.266739 objx-80/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      873 2024-04-15 12:20:05.000000 objx-80/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:21:15.266739 objx-80/objx/
+-rw-r--r--   0 bart      (1000) bart      (1000)      495 2024-04-15 12:18:24.000000 objx-80/objx/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-15 12:18:24.000000 objx-80/objx/object.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-15 12:21:15.266739 objx-80/objx.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1391 2024-04-15 12:21:15.000000 objx-80/objx.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      201 2024-04-15 12:21:15.000000 objx-80/objx.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-15 12:21:15.000000 objx-80/objx.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-15 12:21:15.000000 objx-80/objx.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-15 12:21:15.000000 objx-80/objx.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      868 2024-04-15 12:19:40.000000 objx-80/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-15 12:21:15.266739 objx-80/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-15 12:17:55.000000 objx-80/setup.py
```

### Comparing `objx-70/PKG-INFO` & `objx-80/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: objx
-Version: 70
-Summary: objects library
+Version: 80
+Summary: objects
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objx
 Project-URL: bugs, https://github.com/xobjectz/objx/issues
 Project-URL: source, https://github.com/xobjectz/objx
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
 NAME
 
 ::
 
-    OBJX - objects library
+    OBJX - objects
 
 
 SYNOPSIS
 
 ::
 
     >>> from objx import Object, dumps, loads
@@ -49,15 +49,15 @@
     OBJX is Public Domain.
 
 
 AUTHOR
 
 ::
 
-    xobjectz <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
 
 ::
 
     OBJX is Public Domain.
```

### Comparing `objx-70/README.rst` & `objx-80/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 NAME
 
 ::
 
-    OBJX - objects library
+    OBJX - objects
 
 
 SYNOPSIS
 
 ::
 
     >>> from objx import Object, dumps, loads
@@ -33,15 +33,15 @@
     OBJX is Public Domain.
 
 
 AUTHOR
 
 ::
 
-    xobjectz <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
 
 ::
 
     OBJX is Public Domain.
```

### Comparing `objx-70/objx/object.py` & `objx-80/objx/object.py`

 * *Files identical despite different names*

### Comparing `objx-70/objx.egg-info/PKG-INFO` & `objx-80/objx.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: objx
-Version: 70
-Summary: objects library
+Version: 80
+Summary: objects
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objx
 Project-URL: bugs, https://github.com/xobjectz/objx/issues
 Project-URL: source, https://github.com/xobjectz/objx
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
 NAME
 
 ::
 
-    OBJX - objects library
+    OBJX - objects
 
 
 SYNOPSIS
 
 ::
 
     >>> from objx import Object, dumps, loads
@@ -49,15 +49,15 @@
     OBJX is Public Domain.
 
 
 AUTHOR
 
 ::
 
-    xobjectz <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
 
 ::
 
     OBJX is Public Domain.
```

### Comparing `objx-70/pyproject.toml` & `objx-80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "objx"
-description = "objects library"
-version = "70"
+description = "objects"
+version = "80"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

