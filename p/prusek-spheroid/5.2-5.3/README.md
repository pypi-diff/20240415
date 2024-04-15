# Comparing `tmp/prusek_spheroid-5.2.tar.gz` & `tmp/prusek_spheroid-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.2.tar", last modified: Mon Apr 15 12:20:37 2024, max compression
+gzip compressed data, was "prusek_spheroid-5.3.tar", last modified: Mon Apr 15 16:22:06 2024, max compression
```

## Comparing `prusek_spheroid-5.2.tar` & `prusek_spheroid-5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.390362 prusek_spheroid-5.2/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 12:20:37.390063 prusek_spheroid-5.2/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.2/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.388720 prusek_spheroid-5.2/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.2/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52507 2024-04-12 12:01:36.000000 prusek_spheroid-5.2/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.2/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.2/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.2/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-5.2/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.2/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.2/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.2/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.2/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.2/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 12:20:37.389810 prusek_spheroid-5.2/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 12:20:37.000000 prusek_spheroid-5.2/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 12:20:37.390408 prusek_spheroid-5.2/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 12:20:28.000000 prusek_spheroid-5.2/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:22:06.968797 prusek_spheroid-5.3/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 16:22:06.968487 prusek_spheroid-5.3/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.3/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:22:06.967334 prusek_spheroid-5.3/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.3/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51962 2024-04-15 13:05:48.000000 prusek_spheroid-5.3/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.3/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.3/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.3/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7174 2024-04-15 13:24:40.000000 prusek_spheroid-5.3/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.3/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.3/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.3/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.3/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.3/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 16:22:06.968234 prusek_spheroid-5.3/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 16:22:06.000000 prusek_spheroid-5.3/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 16:22:06.000000 prusek_spheroid-5.3/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 16:22:06.000000 prusek_spheroid-5.3/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 16:22:06.000000 prusek_spheroid-5.3/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 16:22:06.000000 prusek_spheroid-5.3/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 16:22:06.968848 prusek_spheroid-5.3/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 16:22:03.000000 prusek_spheroid-5.3/setup.py
```

### Comparing `prusek_spheroid-5.2/PKG-INFO` & `prusek_spheroid-5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.2
+Version: 5.3
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.2/README.md` & `prusek_spheroid-5.3/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-5.3/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/GUI.py` & `prusek_spheroid-5.3/prusek_spheroid/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,72 +20,70 @@
 class SelectionDialog:
     def __init__(self, root):
         self.root = root
         self.dialog = tk.Toplevel(root)
         self.dialog.title("Software Selection")
         self.dialog.geometry("600x200")
 
-        self.main_section_label = tk.Label(self.dialog, text="Main software", font=("Helvetica", 12, "bold"))
-        self.main_section_label.pack()
+        tk.Label(self.dialog, text="Main software", font=("Helvetica", 12, "bold")).pack()
+        tk.Button(self.dialog, text="Spheroids Segmentation", command=self.open_segmentation_gui).pack(pady=10)
+        tk.Button(self.dialog, text="Spheroids Quantification", command=self.open_quantification_gui).pack(pady=10)
 
-        seg_button = tk.Button(self.dialog, text="Spheroids Segmentation", command=self.open_segmentation_gui)
-        seg_button.pack(pady=10)
-
-        quant_button = tk.Button(self.dialog, text="Spheroids Quantification", command=self.open_quantification_gui)
-        quant_button.pack(pady=10)
-
-        self.address_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
-        self.address_separator.pack(fill=tk.X, padx=5, pady=5)
-
-        self.utils_section_label = tk.Label(self.dialog, text="Utils", font=("Helvetica", 12, "bold"))
-        self.utils_section_label.pack()
+        tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN).pack(fill=tk.X, padx=5, pady=5)
+        tk.Label(self.dialog, text="Utils", font=("Helvetica", 12, "bold")).pack()
 
         button_frame = tk.Frame(self.dialog)
         button_frame.pack(pady=10)
+        tk.Button(button_frame, text="Convert between COCO 1.0 and Masks", command=self.open_conversion_gui).grid(row=0, column=0, padx=(0, 10))
+        tk.Button(button_frame, text="Create dataset folder (merge directories)", command=self.open_image_processing_dialog).grid(row=0, column=1, padx=(10, 0))
 
-        convert_button = tk.Button(button_frame, text="Convert between COCO 1.0 and Masks",
-                                   command=self.open_conversion_gui)
-        image_processing_btn = tk.Button(button_frame, text="Create dataset folder (merge directories)",
-                                         command=self.open_image_processing_dialog)
-
-        # Place buttons in the frame using grid
-        convert_button.grid(row=0, column=0, padx=(0, 10))  # Padding to the right
-        image_processing_btn.grid(row=0, column=1, padx=(10, 0))  # Padding to the left
-
-        # Adjust the frame's column configuration to center the buttons
         button_frame.grid_columnconfigure(0, weight=1)
         button_frame.grid_columnconfigure(1, weight=1)
-
         self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
 
-    def show(self):
-        self.dialog.deiconify()
-
-    def hide(self):
-        self.dialog.withdraw()
-
     def open_segmentation_gui(self):
         self.hide()
         SpheroidSegmentationGUI(self)
 
     def open_quantification_gui(self):
         self.hide()
         SpheroidQuantificationGUI(self)
 
     def open_conversion_gui(self):
         self.hide()
         ConversionDialog(self)
 
     def open_image_processing_dialog(self):
-        self.hide()  # Optionally hide the selection dialog
+        self.hide()
         ImageProcessingDialog(self)
 
+    def show(self):
+        self.dialog.deiconify()
+
+    def hide(self):
+        self.dialog.withdraw()
+
     def on_close(self):
         self.root.quit()
 
+def browse_directory(var, title, label):
+    directory_path = filedialog.askdirectory()
+    # Normalize the path to ensure consistency across different OS
+    directory_path = os.path.normpath(directory_path)
+    var.set(directory_path)
+    label.config(text=f"{title}: {shorten_path(directory_path)}")
+
+def shorten_path(path, max_length=40):
+    if len(path) > max_length:
+        return '...' + path[-max_length + 3:]
+    return path
+
+def update_addresses(annotations_address):
+    return os.path.join(annotations_address, "annotations"), os.path.join(annotations_address, "images")
+
 
 class ImageProcessingDialog:
     def __init__(self, selection_dialog):
         self.done_dialog = None
         self.progress_label = None
         self.progress_dialog = None
         self.output_dir_label = None
@@ -344,21 +342,14 @@
     @staticmethod
     def shorten_path(path, max_length=40):
         if len(path) > max_length:
             return '...' + path[-max_length + 3:]
         return path
 
 
-def update_addresses(annotationsAddress):
-    annotation_address = os.path.join(annotationsAddress, "annotations")
-    images_address = os.path.join(annotationsAddress, "images")
-
-    return annotation_address, images_address
-
-
 class ProcessingProgressWindow(tk.Toplevel):
     def __init__(self, master):
         tk.Toplevel.__init__(self, master)
         self.title("Processing Progress")
 
         self.geometry("500x250")
         self.resizable(width=False, height=False)
@@ -465,34 +456,23 @@
                 self.entries[param].insert(0, str(value))
 
     def update_parameters(self, new_parameters):
         # Update parameters in the main application when entering them manually
         self.parameters = new_parameters
 
 
-def shorten_path(path, max_length=40):
-    if len(path) > max_length:
-        return '...' + path[-max_length + 3:]
-    return path
-
-
 def browse_file(var, title, label):
     file_path = filedialog.askopenfilename()
+    # Normalize the file path
+    file_path = os.path.normpath(file_path)
     var.set(file_path)
     shortened_path = shorten_path(file_path)
     label.config(text=f"{title}: {shortened_path}")
 
 
-def browse_directory(var, title, label):
-    directory_path = filedialog.askdirectory()
-    var.set(directory_path)
-    shortened_path = shorten_path(directory_path)
-    label.config(text=f"{title}: {shortened_path}")
-
-
 class SpheroidQuantificationGUI:
     def __init__(self, selection_dialog):
         self.selection_dialog = selection_dialog
         self.dialog = tk.Toplevel(selection_dialog.root)
         self.dialog.title("Spheroid Quantification")
 
         back_button = tk.Button(self.dialog, text="Back", command=self.go_back)
```

### Comparing `prusek_spheroid-5.2/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-5.3/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-5.3/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/conversion.py` & `prusek_spheroid-5.3/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/file_management.py` & `prusek_spheroid-5.3/prusek_spheroid/file_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import os
 import shutil
-import zipfile
 import cv2 as cv
 import numpy as np
 import json as js
 from tkinter import messagebox
 
 
 import zipfile
```

### Comparing `prusek_spheroid-5.2/prusek_spheroid/image_processing.py` & `prusek_spheroid-5.3/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/merge_directories.py` & `prusek_spheroid-5.3/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/methods.py` & `prusek_spheroid-5.3/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/metrics.py` & `prusek_spheroid-5.3/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-5.3/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-5.3/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.2
+Version: 5.3
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.2/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-5.3/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.2/setup.py` & `prusek_spheroid-5.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.2",
+    version="5.3",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

