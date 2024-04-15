# Comparing `tmp/opencv.wrap-0.0.3.tar.gz` & `tmp/opencv.wrap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv.wrap-0.0.3.tar", last modified: Sat Feb 24 10:02:24 2024, max compression
+gzip compressed data, was "opencv.wrap-0.0.4.tar", last modified: Mon Apr 15 15:26:02 2024, max compression
```

## Comparing `opencv.wrap-0.0.3.tar` & `opencv.wrap-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-02-24 10:02:24.655267 opencv.wrap-0.0.3/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv.wrap-0.0.3/LICENSE
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2011 2024-02-24 10:02:24.654745 opencv.wrap-0.0.3/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1040 2024-02-24 05:44:05.000000 opencv.wrap-0.0.3/README.md
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1232 2024-02-24 10:02:23.000000 opencv.wrap-0.0.3/README.rst
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-02-24 10:02:24.653166 opencv.wrap-0.0.3/opencv.wrap.egg-info/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2011 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      283 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/SOURCES.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/dependency_links.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       63 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/entry_points.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-02-24 08:30:15.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/not-zip-safe
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      434 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/requires.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-02-24 10:02:24.000000 opencv.wrap-0.0.3/opencv.wrap.egg-info/top_level.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-02-24 10:02:24.655520 opencv.wrap-0.0.3/setup.cfg
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     3440 2024-02-24 10:02:23.000000 opencv.wrap-0.0.3/setup.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 15:26:02.225690 opencv.wrap-0.0.4/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv.wrap-0.0.4/LICENSE
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 15:26:02.224995 opencv.wrap-0.0.4/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1162 2024-04-13 15:21:30.000000 opencv.wrap-0.0.4/README.md
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1370 2024-04-15 15:26:01.000000 opencv.wrap-0.0.4/README.rst
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 15:26:02.223527 opencv.wrap-0.0.4/opencv.wrap.egg-info/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      283 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       63 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/entry_points.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-02-24 08:30:15.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/not-zip-safe
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      434 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/requires.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 15:26:02.000000 opencv.wrap-0.0.4/opencv.wrap.egg-info/top_level.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-04-15 15:26:02.226228 opencv.wrap-0.0.4/setup.cfg
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1658 2024-04-15 15:26:01.000000 opencv.wrap-0.0.4/setup.py
```

### Comparing `opencv.wrap-0.0.3/LICENSE` & `opencv.wrap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv.wrap-0.0.3/PKG-INFO` & `opencv.wrap-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: opencv.wrap
-Version: 0.0.3
-Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, etc, this package is designed to make it easier to work with opencv while focusing on the main task
+Version: 0.0.4
+Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand.
 Home-page: https://github.com/rishi23root/opencv.util
 Author: rishi23root
 Author-email: rishi23root@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -39,18 +39,27 @@
 -  ReadCamAndShowFrames
 -  ReadCamAddDetectShowFrames
 -  ReadCamAddDetectShowFrames_video
 
 additional Utils
 ================
 
+-  saveFrames
+-  detectionBox
+-  show_all_frames
+
+Detection Utils
+===============
+
 -  face detection
 -  hand detection
 -  eye detection (yet to be added)
 
+add code examples here for each feature and utilities
+
 .. |GitHub stars| image:: https://img.shields.io/github/stars/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/stargazers
 .. |PyPI| image:: https://img.shields.io/pypi/v/opencv.wrap.svg
    :target: https://pypi.org/project/opencv.wrap/
 .. |GitHub| image:: https://img.shields.io/github/license/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/blob/master/LICENSE
 .. |PyPI - Python Version| image:: https://img.shields.io/pypi/pyversions/Django.svg
```

### Comparing `opencv.wrap-0.0.3/README.md` & `opencv.wrap-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -20,10 +20,19 @@
 - ConvertCOLOR
 - ReadCamAndShowFrames
 - ReadCamAddDetectShowFrames
 - ReadCamAddDetectShowFrames_video
 
 # additional Utils
 
+- saveFrames
+- detectionBox
+- show_all_frames
+
+# Detection Utils
+
 - face detection
 - hand detection
 - eye detection (yet to be added)
+
+
+add code examples here for each feature and utilities
```

### Comparing `opencv.wrap-0.0.3/README.rst` & `opencv.wrap-0.0.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,27 @@
 -  ReadCamAndShowFrames
 -  ReadCamAddDetectShowFrames
 -  ReadCamAddDetectShowFrames_video
 
 additional Utils
 ================
 
+-  saveFrames
+-  detectionBox
+-  show_all_frames
+
+Detection Utils
+===============
+
 -  face detection
 -  hand detection
 -  eye detection (yet to be added)
 
+add code examples here for each feature and utilities
+
 .. |GitHub stars| image:: https://img.shields.io/github/stars/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/stargazers
 .. |PyPI| image:: https://img.shields.io/pypi/v/opencv.wrap.svg
    :target: https://pypi.org/project/opencv.wrap/
 .. |GitHub| image:: https://img.shields.io/github/license/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/blob/master/LICENSE
 .. |PyPI - Python Version| image:: https://img.shields.io/pypi/pyversions/Django.svg
```

### Comparing `opencv.wrap-0.0.3/opencv.wrap.egg-info/PKG-INFO` & `opencv.wrap-0.0.4/opencv.wrap.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: opencv.wrap
-Version: 0.0.3
-Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, etc, this package is designed to make it easier to work with opencv while focusing on the main task
+Version: 0.0.4
+Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand.
 Home-page: https://github.com/rishi23root/opencv.util
 Author: rishi23root
 Author-email: rishi23root@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -39,18 +39,27 @@
 -  ReadCamAndShowFrames
 -  ReadCamAddDetectShowFrames
 -  ReadCamAddDetectShowFrames_video
 
 additional Utils
 ================
 
+-  saveFrames
+-  detectionBox
+-  show_all_frames
+
+Detection Utils
+===============
+
 -  face detection
 -  hand detection
 -  eye detection (yet to be added)
 
+add code examples here for each feature and utilities
+
 .. |GitHub stars| image:: https://img.shields.io/github/stars/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/stargazers
 .. |PyPI| image:: https://img.shields.io/pypi/v/opencv.wrap.svg
    :target: https://pypi.org/project/opencv.wrap/
 .. |GitHub| image:: https://img.shields.io/github/license/rishi23root/opencv.wrap.svg
    :target: https://github.com/rishi23root/opencv.wrap/blob/master/LICENSE
 .. |PyPI - Python Version| image:: https://img.shields.io/pypi/pyversions/Django.svg
```

