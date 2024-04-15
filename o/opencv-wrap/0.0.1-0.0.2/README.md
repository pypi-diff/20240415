# Comparing `tmp/opencv_wrap-0.0.1.tar.gz` & `tmp/opencv_wrap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_wrap-0.0.1.tar", last modified: Mon Apr 15 16:38:32 2024, max compression
+gzip compressed data, was "opencv_wrap-0.0.2.tar", last modified: Mon Apr 15 16:41:40 2024, max compression
```

## Comparing `opencv_wrap-0.0.1.tar` & `opencv_wrap-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:38:32.152529 opencv_wrap-0.0.1/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv_wrap-0.0.1/LICENSE
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 16:38:32.152095 opencv_wrap-0.0.1/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1370 2024-04-15 16:38:31.000000 opencv_wrap-0.0.1/README.rst
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:38:32.138215 opencv_wrap-0.0.1/opencv_wrap/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       69 2024-04-15 16:15:05.000000 opencv_wrap-0.0.1/opencv_wrap/__init__.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13648 2024-04-13 15:13:15.000000 opencv_wrap-0.0.1/opencv_wrap/cv2Decorator.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:38:32.147287 opencv_wrap-0.0.1/opencv_wrap/detectors/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     6338 2024-04-15 16:29:27.000000 opencv_wrap-0.0.1/opencv_wrap/detectors/Face.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     8187 2024-02-15 15:33:42.000000 opencv_wrap-0.0.1/opencv_wrap/detectors/Hand.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       78 2024-04-15 16:24:08.000000 opencv_wrap-0.0.1/opencv_wrap/detectors/__init__.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:38:32.150977 opencv_wrap-0.0.1/opencv_wrap/utils/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       19 2024-04-15 16:13:38.000000 opencv_wrap-0.0.1/opencv_wrap/utils/__init__.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2202 2024-04-14 13:38:36.000000 opencv_wrap-0.0.1/opencv_wrap/utils/base.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13004 2024-04-15 16:23:08.000000 opencv_wrap-0.0.1/opencv_wrap/utils/helper.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:38:32.143291 opencv_wrap-0.0.1/opencv_wrap.egg-info/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      503 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/SOURCES.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/dependency_links.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       63 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/entry_points.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 16:36:21.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/not-zip-safe
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      434 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/requires.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       12 2024-04-15 16:38:32.000000 opencv_wrap-0.0.1/opencv_wrap.egg-info/top_level.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-04-15 16:38:32.152688 opencv_wrap-0.0.1/setup.cfg
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1658 2024-04-15 16:38:31.000000 opencv_wrap-0.0.1/setup.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:41:40.785535 opencv_wrap-0.0.2/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv_wrap-0.0.2/LICENSE
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 16:41:40.785164 opencv_wrap-0.0.2/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1370 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/README.rst
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:41:40.771740 opencv_wrap-0.0.2/opencv_wrap/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       69 2024-04-15 16:15:05.000000 opencv_wrap-0.0.2/opencv_wrap/__init__.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13648 2024-04-13 15:13:15.000000 opencv_wrap-0.0.2/opencv_wrap/cv2Decorator.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:41:40.780570 opencv_wrap-0.0.2/opencv_wrap/detectors/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     6338 2024-04-15 16:29:27.000000 opencv_wrap-0.0.2/opencv_wrap/detectors/Face.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     8187 2024-02-15 15:33:42.000000 opencv_wrap-0.0.2/opencv_wrap/detectors/Hand.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       78 2024-04-15 16:24:08.000000 opencv_wrap-0.0.2/opencv_wrap/detectors/__init__.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:41:40.784126 opencv_wrap-0.0.2/opencv_wrap/utils/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       19 2024-04-15 16:13:38.000000 opencv_wrap-0.0.2/opencv_wrap/utils/__init__.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2202 2024-04-14 13:38:36.000000 opencv_wrap-0.0.2/opencv_wrap/utils/base.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13004 2024-04-15 16:41:22.000000 opencv_wrap-0.0.2/opencv_wrap/utils/helper.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-15 16:41:40.777696 opencv_wrap-0.0.2/opencv_wrap.egg-info/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2154 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      503 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       63 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/entry_points.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/not-zip-safe
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      434 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/requires.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       12 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/opencv_wrap.egg-info/top_level.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-04-15 16:41:40.785681 opencv_wrap-0.0.2/setup.cfg
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1658 2024-04-15 16:41:40.000000 opencv_wrap-0.0.2/setup.py
```

### Comparing `opencv_wrap-0.0.1/LICENSE` & `opencv_wrap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/PKG-INFO` & `opencv_wrap-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: opencv_wrap
-Version: 0.0.1
+Version: 0.0.2
 Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand.
-Home-page: https://github.com/rishi23root/opencv.util
+Home-page: https://github.com/rishi23root/opencv_wrap
 Author: rishi23root
 Author-email: rishi23root@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencv_wrap-0.0.1/README.rst` & `opencv_wrap-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap/cv2Decorator.py` & `opencv_wrap-0.0.2/opencv_wrap/cv2Decorator.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap/detectors/Face.py` & `opencv_wrap-0.0.2/opencv_wrap/detectors/Face.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap/detectors/Hand.py` & `opencv_wrap-0.0.2/opencv_wrap/detectors/Hand.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap/utils/base.py` & `opencv_wrap-0.0.2/opencv_wrap/utils/base.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap/utils/helper.py` & `opencv_wrap-0.0.2/opencv_wrap/utils/helper.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.0.1/opencv_wrap.egg-info/PKG-INFO` & `opencv_wrap-0.0.2/opencv_wrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: opencv-wrap
-Version: 0.0.1
+Version: 0.0.2
 Summary: working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand.
-Home-page: https://github.com/rishi23root/opencv.util
+Home-page: https://github.com/rishi23root/opencv_wrap
 Author: rishi23root
 Author-email: rishi23root@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencv_wrap-0.0.1/setup.py` & `opencv_wrap-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # flake8: noqa: E501
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand."
 
 setup(
     name="opencv_wrap",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.rst").read(),
-    url="https://github.com/rishi23root/opencv.util",
+    url="https://github.com/rishi23root/opencv_wrap",
     author="rishi23root",
     author_email="rishi23root@gmail.com",
     license="MIT",
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

