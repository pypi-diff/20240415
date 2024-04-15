# Comparing `tmp/gerber_writer-0.4.3.tar.gz` & `tmp/gerber_writer-0.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerber_writer-0.4.3.tar", last modified: Fri Apr 12 18:40:05 2024, max compression
+gzip compressed data, was "gerber_writer-0.4.3.1.tar", last modified: Mon Apr 15 10:11:15 2024, max compression
```

## Comparing `gerber_writer-0.4.3.tar` & `gerber_writer-0.4.3.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2024-04-09 14:53:35.000000 gerber_writer-0.4.3/LICENSE
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2533 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/PKG-INFO
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/doc/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1738 2024-04-12 18:24:55.000000 gerber_writer-0.4.3/doc/README.rst
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      990 2024-04-12 14:57:21.000000 gerber_writer-0.4.3/pyproject.toml
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/setup.cfg
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/gerber_writer/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       75 2024-04-12 09:41:07.000000 gerber_writer-0.4.3/src/gerber_writer/__init__.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.3/src/gerber_writer/lutils.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/src/gerber_writer/macros.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.3/src/gerber_writer/padmasters.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.3/src/gerber_writer/writer.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.3/src/gerber_writer/writer_test.py
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/gerber_writer.egg-info/
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2533 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      422 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/SOURCES.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/dependency_links.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/top_level.txt
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/tests/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/tests/test_arcs.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/tests/test_contours.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.121472 gerber_writer-0.4.3.1/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2024-04-09 14:53:35.000000 gerber_writer-0.4.3.1/LICENSE
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2535 2024-04-15 10:11:15.121472 gerber_writer-0.4.3.1/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1738 2024-04-12 18:24:55.000000 gerber_writer-0.4.3.1/README.rst
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.117472 gerber_writer-0.4.3.1/doc/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1738 2024-04-15 10:07:14.000000 gerber_writer-0.4.3.1/doc/README.rst
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      992 2024-04-15 10:06:51.000000 gerber_writer-0.4.3.1/pyproject.toml
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-15 10:11:15.121472 gerber_writer-0.4.3.1/setup.cfg
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.117472 gerber_writer-0.4.3.1/src/
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.117472 gerber_writer-0.4.3.1/src/gerber_writer/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       77 2024-04-15 10:06:51.000000 gerber_writer-0.4.3.1/src/gerber_writer/__init__.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.3.1/src/gerber_writer/lutils.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.3.1/src/gerber_writer/macros.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.3.1/src/gerber_writer/padmasters.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.3.1/src/gerber_writer/writer.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.3.1/src/gerber_writer/writer_test.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.121472 gerber_writer-0.4.3.1/src/gerber_writer.egg-info/
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2535 2024-04-15 10:11:15.000000 gerber_writer-0.4.3.1/src/gerber_writer.egg-info/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      433 2024-04-15 10:11:15.000000 gerber_writer-0.4.3.1/src/gerber_writer.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-15 10:11:15.000000 gerber_writer-0.4.3.1/src/gerber_writer.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-15 10:11:15.000000 gerber_writer-0.4.3.1/src/gerber_writer.egg-info/top_level.txt
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-15 10:11:15.121472 gerber_writer-0.4.3.1/tests/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.3.1/tests/test_arcs.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.3.1/tests/test_contours.py
```

### Comparing `gerber_writer-0.4.3/LICENSE` & `gerber_writer-0.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/PKG-INFO` & `gerber_writer-0.4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.3
+Version: 0.4.3.1
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
 Project-URL: Repository, https://github.com/karel-tavernier/gerber_writer
 Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/html
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gerber_writer-0.4.3/doc/README.rst` & `gerber_writer-0.4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/pyproject.toml` & `gerber_writer-0.4.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "gerber_writer"
-version = "0.4.3"
+version = "0.4.3.1"
 authors = [
   { name="Karel Tavernier", email="karel_tavernier@hotmail.com" },
 ]
 description = "A library to write Gerber files"
 readme = "doc/README.rst"
 license = { text ="Apache 2.0 License" }
 requires-python = ">=3.9"
```

### Comparing `gerber_writer-0.4.3/src/gerber_writer/macros.py` & `gerber_writer-0.4.3.1/src/gerber_writer/macros.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/src/gerber_writer/padmasters.py` & `gerber_writer-0.4.3.1/src/gerber_writer/padmasters.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/src/gerber_writer/writer.py` & `gerber_writer-0.4.3.1/src/gerber_writer/writer.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/src/gerber_writer/writer_test.py` & `gerber_writer-0.4.3.1/src/gerber_writer/writer_test.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/src/gerber_writer.egg-info/PKG-INFO` & `gerber_writer-0.4.3.1/src/gerber_writer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.3
+Version: 0.4.3.1
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
 Project-URL: Repository, https://github.com/karel-tavernier/gerber_writer
 Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/html
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gerber_writer-0.4.3/tests/test_arcs.py` & `gerber_writer-0.4.3.1/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.3/tests/test_contours.py` & `gerber_writer-0.4.3.1/tests/test_contours.py`

 * *Files identical despite different names*

