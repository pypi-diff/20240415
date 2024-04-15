# Comparing `tmp/prusek_spheroid-5.1.tar.gz` & `tmp/prusek_spheroid-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.1.tar", last modified: Fri Apr 12 12:15:01 2024, max compression
+gzip compressed data, was "prusek_spheroid-5.2.tar", last modified: Mon Apr 15 12:20:37 2024, max compression
```

## Comparing `prusek_spheroid-5.1.tar` & `prusek_spheroid-5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.394313 prusek_spheroid-5.1/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-12 12:15:01.394056 prusek_spheroid-5.1/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.1/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.393015 prusek_spheroid-5.1/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.1/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52507 2024-04-12 12:01:36.000000 prusek_spheroid-5.1/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.1/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.1/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.1/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-5.1/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.1/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.1/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.1/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.1/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.1/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-12 12:15:01.393821 prusek_spheroid-5.1/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-12 12:15:01.000000 prusek_spheroid-5.1/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-12 12:15:01.394372 prusek_spheroid-5.1/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-12 12:14:58.000000 prusek_spheroid-5.1/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.390362 prusek_spheroid-5.2/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 12:20:37.390063 prusek_spheroid-5.2/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.2/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.388720 prusek_spheroid-5.2/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.2/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    52507 2024-04-12 12:01:36.000000 prusek_spheroid-5.2/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.2/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.2/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.2/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-5.2/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.2/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.2/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.2/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.2/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.2/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.389810 prusek_spheroid-5.2/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 12:20:37.390408 prusek_spheroid-5.2/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 12:20:28.000000 prusek_spheroid-5.2/setup.py
```

### Comparing `prusek_spheroid-5.1/PKG-INFO` & `prusek_spheroid-5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.1
+Version: 5.2
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.1/README.md` & `prusek_spheroid-5.2/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-5.2/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/GUI.py` & `prusek_spheroid-5.2/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-5.2/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-5.2/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/conversion.py` & `prusek_spheroid-5.2/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/file_management.py` & `prusek_spheroid-5.2/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/image_processing.py` & `prusek_spheroid-5.2/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/merge_directories.py` & `prusek_spheroid-5.2/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/methods.py` & `prusek_spheroid-5.2/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/metrics.py` & `prusek_spheroid-5.2/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-5.2/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-5.2/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.1
+Version: 5.2
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.1/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-5.2/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.1/setup.py` & `prusek_spheroid-5.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.1",
+    version="5.2",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

