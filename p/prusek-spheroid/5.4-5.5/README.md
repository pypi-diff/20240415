# Comparing `tmp/prusek_spheroid-5.4.tar.gz` & `tmp/prusek_spheroid-5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.4.tar", last modified: Mon Apr 15 16:36:36 2024, max compression
+gzip compressed data, was "prusek_spheroid-5.5.tar", last modified: Mon Apr 15 17:00:16 2024, max compression
```

## Comparing `prusek_spheroid-5.4.tar` & `prusek_spheroid-5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:36:36.669180 prusek_spheroid-5.4/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 16:36:36.668589 prusek_spheroid-5.4/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.4/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:36:36.667112 prusek_spheroid-5.4/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.4/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52048 2024-04-15 16:36:29.000000 prusek_spheroid-5.4/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.4/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.4/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.4/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7174 2024-04-15 13:24:40.000000 prusek_spheroid-5.4/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.4/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.4/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.4/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.4/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.4/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:36:36.668283 prusek_spheroid-5.4/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 16:36:36.000000 prusek_spheroid-5.4/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 16:36:36.000000 prusek_spheroid-5.4/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 16:36:36.000000 prusek_spheroid-5.4/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 16:36:36.000000 prusek_spheroid-5.4/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 16:36:36.000000 prusek_spheroid-5.4/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 16:36:36.669233 prusek_spheroid-5.4/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 16:36:34.000000 prusek_spheroid-5.4/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.194156 prusek_spheroid-5.5/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 17:00:16.193865 prusek_spheroid-5.5/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.5/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.192698 prusek_spheroid-5.5/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.5/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51985 2024-04-15 16:54:02.000000 prusek_spheroid-5.5/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.5/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.5/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.5/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7196 2024-04-15 16:59:57.000000 prusek_spheroid-5.5/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.5/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.5/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.5/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.5/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.5/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.193635 prusek_spheroid-5.5/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 17:00:16.194205 prusek_spheroid-5.5/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 17:00:11.000000 prusek_spheroid-5.5/setup.py
```

### Comparing `prusek_spheroid-5.4/PKG-INFO` & `prusek_spheroid-5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.4
+Version: 5.5
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.4/README.md` & `prusek_spheroid-5.5/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-5.5/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/GUI.py` & `prusek_spheroid-5.5/prusek_spheroid/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import tkinter as tk
 from tkinter import filedialog
 from tkinter import messagebox
 from prusek_spheroid import GradientDescentGUI as g
 from prusek_spheroid import ContoursClassGUI as F
 import threading
 import time
@@ -12,15 +13,14 @@
 from prusek_spheroid import conversion as c
 from prusek_spheroid import merge_directories as md
 import pandas as pd
 import cv2 as cv
 from tkinter import Toplevel, Label
 from tkinter import ttk
 
-
 class SelectionDialog:
     def __init__(self, root):
         self.root = root
         self.dialog = tk.Toplevel(root)
         self.dialog.title("Software Selection")
         self.dialog.geometry("600x200")
 
@@ -64,17 +64,15 @@
 
     def on_close(self):
         self.root.quit()
 
 def browse_directory(var, title, label):
     directory_path = filedialog.askdirectory()
     # Normalize the path to ensure consistency across different OS
-    print(f"adresa pred: {directory_path}")
     directory_path = os.path.normpath(directory_path)
-    print(f"adresa po: {directory_path}")
     var.set(directory_path)
     label.config(text=f"{title}: {shorten_path(directory_path)}")
 
 def shorten_path(path, max_length=40):
     if len(path) > max_length:
         return '...' + path[-max_length + 3:]
     return path
```

### Comparing `prusek_spheroid-5.4/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-5.5/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-5.5/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/conversion.py` & `prusek_spheroid-5.5/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/file_management.py` & `prusek_spheroid-5.5/prusek_spheroid/file_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+# -*- coding: utf-8 -*-
 import shutil
 import cv2 as cv
 import numpy as np
 import json as js
 from tkinter import messagebox
-
-
 import zipfile
 import os
 
 
 def unzip(zip_file_path):
     # Odstranění přípony '.zip' a vytvoření cesty pro cílovou složku
     base_path = os.path.splitext(zip_file_path)[0]
```

### Comparing `prusek_spheroid-5.4/prusek_spheroid/image_processing.py` & `prusek_spheroid-5.5/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/merge_directories.py` & `prusek_spheroid-5.5/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/methods.py` & `prusek_spheroid-5.5/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/metrics.py` & `prusek_spheroid-5.5/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-5.5/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-5.5/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.4
+Version: 5.5
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.4/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-5.5/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.4/setup.py` & `prusek_spheroid-5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.4",
+    version="5.5",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

