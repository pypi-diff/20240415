# Comparing `tmp/liveplotlib-0.3.1.tar.gz` & `tmp/liveplotlib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveplotlib-0.3.1.tar", last modified: Sat Apr 13 01:25:28 2024, max compression
+gzip compressed data, was "liveplotlib-0.3.2.tar", last modified: Mon Apr 15 16:26:32 2024, max compression
```

## Comparing `liveplotlib-0.3.1.tar` & `liveplotlib-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 01:25:28.170035 liveplotlib-0.3.1/
--rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6074 2024-04-13 01:25:28.169036 liveplotlib-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5444 2024-04-13 01:05:28.000000 liveplotlib-0.3.1/README.md
--rw-rw-rw-   0        0        0      108 2024-04-13 00:24:49.000000 liveplotlib-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      760 2024-04-13 01:25:28.171035 liveplotlib-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 01:25:28.143037 liveplotlib-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:25:28.151036 liveplotlib-0.3.1/src/liveplotlib/
--rw-rw-rw-   0        0        0      351 2024-04-13 01:15:51.000000 liveplotlib-0.3.1/src/liveplotlib/__init__.py
--rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.3.1/src/liveplotlib/get_file_format.py
--rw-rw-rw-   0        0        0     1226 2024-04-12 21:49:28.000000 liveplotlib-0.3.1/src/liveplotlib/if_ipynb.py
--rw-rw-rw-   0        0        0     2863 2024-04-12 23:21:47.000000 liveplotlib-0.3.1/src/liveplotlib/live_plot_only_train.py
--rw-rw-rw-   0        0        0     4732 2024-04-12 23:25:03.000000 liveplotlib-0.3.1/src/liveplotlib/live_plot_train_and_val.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:25:28.168036 liveplotlib-0.3.1/src/liveplotlib.egg-info/
--rw-rw-rw-   0        0        0     6074 2024-04-13 01:25:28.000000 liveplotlib-0.3.1/src/liveplotlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-04-13 01:25:28.000000 liveplotlib-0.3.1/src/liveplotlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 01:25:28.000000 liveplotlib-0.3.1/src/liveplotlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-13 01:25:28.000000 liveplotlib-0.3.1/src/liveplotlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 01:25:28.000000 liveplotlib-0.3.1/src/liveplotlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 16:26:32.826328 liveplotlib-0.3.2/
+-rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     6074 2024-04-15 16:26:32.826328 liveplotlib-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5444 2024-04-13 01:05:28.000000 liveplotlib-0.3.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-13 00:24:49.000000 liveplotlib-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2024-04-15 16:26:32.830326 liveplotlib-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 16:26:32.794708 liveplotlib-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:26:32.807328 liveplotlib-0.3.2/src/liveplotlib/
+-rw-rw-rw-   0        0        0      351 2024-04-13 01:15:51.000000 liveplotlib-0.3.2/src/liveplotlib/__init__.py
+-rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.3.2/src/liveplotlib/get_file_format.py
+-rw-rw-rw-   0        0        0     1235 2024-04-15 15:50:11.000000 liveplotlib-0.3.2/src/liveplotlib/if_ipynb.py
+-rw-rw-rw-   0        0        0     3100 2024-04-15 15:56:03.000000 liveplotlib-0.3.2/src/liveplotlib/live_plot_only_train.py
+-rw-rw-rw-   0        0        0     4943 2024-04-15 15:56:21.000000 liveplotlib-0.3.2/src/liveplotlib/live_plot_train_and_val.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:26:32.825328 liveplotlib-0.3.2/src/liveplotlib.egg-info/
+-rw-rw-rw-   0        0        0     6074 2024-04-15 16:26:32.000000 liveplotlib-0.3.2/src/liveplotlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-15 16:26:32.000000 liveplotlib-0.3.2/src/liveplotlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:26:32.000000 liveplotlib-0.3.2/src/liveplotlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 16:26:32.000000 liveplotlib-0.3.2/src/liveplotlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 16:26:32.000000 liveplotlib-0.3.2/src/liveplotlib.egg-info/top_level.txt
```

### Comparing `liveplotlib-0.3.1/LICENSE` & `liveplotlib-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.3.1/PKG-INFO` & `liveplotlib-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyQt6
+Requires-Dist: PyQt5
 Requires-Dist: matplotlib
 
 # LIVE PLOT LIBrary (liveplotlib)
 - Library for plotting (visualizing) cost function changes during model training (in real time)
 
 
 # Notations
```

### Comparing `liveplotlib-0.3.1/README.md` & `liveplotlib-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.3.1/setup.cfg` & `liveplotlib-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6976 6570 6c6f 746c 6962 0d0a   = liveplotlib..
-00000020: 7665 7273 696f 6e20 3d20 302e 332e 310d  version = 0.3.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 332e 320d  version = 0.3.2.
 00000030: 0a61 7574 686f 7220 3d20 706f 7a68 6172  .author = pozhar
 00000040: 736b 7945 0d0a 6175 7468 6f72 5f65 6d61  skyE..author_ema
 00000050: 696c 203d 2065 7667 656e 792e 706f 7a68  il = evgeny.pozh
 00000060: 6172 736b 7940 676d 6169 6c2e 636f 6d0d  arsky@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 204c  .description = L
 00000080: 6962 7261 7279 2066 6f72 2070 6c6f 7474  ibrary for plott
 00000090: 696e 6720 2876 6973 7561 6c69 7a69 6e67  ing (visualizing
@@ -35,14 +35,14 @@
 00000220: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
 00000230: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
 00000240: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
 00000250: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
 00000260: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
 00000270: 203d 203e 3d33 2e37 0d0a 696e 7374 616c   = >=3.7..instal
 00000280: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000290: 5079 5174 360d 0a09 6d61 7470 6c6f 746c  PyQt6...matplotl
+00000290: 5079 5174 350d 0a09 6d61 7470 6c6f 746c  PyQt5...matplotl
 000002a0: 6962 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ib....[options.p
 000002b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
 000002c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
 000002d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
 000002e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
 000002f0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `liveplotlib-0.3.1/src/liveplotlib/get_file_format.py` & `liveplotlib-0.3.2/src/liveplotlib/get_file_format.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.3.1/src/liveplotlib/if_ipynb.py` & `liveplotlib-0.3.2/src/liveplotlib/if_ipynb.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         self.file_format = get_file_format()
         if self.print_reports:
             print('Detected file format: ', self.file_format)
 
         if self.file_format == 'ipynb':
             import IPython
 
-            IPython.get_ipython().run_line_magic('matplotlib', 'qt')
+            IPython.get_ipython().run_line_magic('matplotlib', 'qt5')
 
             if self.print_reports:
-                print('matplotlib is in "separated window" mode now')
+                print('matplotlib is in "separated window" (PyQt5) mode now')
                 print('To return to "inline" mode later, just run live_plot.close()')
 
     def end(self):
         if self.file_format == 'ipynb':
             import IPython
 
             IPython.get_ipython().run_line_magic('matplotlib', 'inline')
```

### Comparing `liveplotlib-0.3.1/src/liveplotlib/live_plot_only_train.py` & `liveplotlib-0.3.2/src/liveplotlib/live_plot_only_train.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 class LivePlotOnlyTrain():
     """
     `J - cost/loss function` \n
 
     Renders 2 subplots:
     -------------------
-    1) J_history
-    2) J_history slice (last {slice_size} steps)
+    1) J_train_history
+    2) J_train_history slice (last {slice_size} steps)
         `slice_size = slice_fraction * len(J_history) + slice_bias`
 
     Usage
     -------------------
     ```python
     
     # STEP 1: IMPORT
@@ -66,14 +66,20 @@
     ```
     """
 
     def __init__(self, 
                  slice_bias: int = 10,
                  slice_fraction: float = 0,
                  print_reports: bool = True): 
+        
+
+        # Parameters checking 
+        if not ( 0 <= slice_fraction < 1 ):
+            raise ValueError(f"Slice fraction should be: 0 <= slice_fraction < 1  (in [0, 1)), but you gave {slice_fraction}")
+
 
         self.slice_bias = slice_bias
         self.slice_fraction = slice_fraction
 
 
         self.if_ipynb_handler = IfIPYNBHandler(print_reports=print_reports)
         self.if_ipynb_handler.start()
@@ -98,15 +104,15 @@
 
 
     def update(self, J_history: list):
         slice_size = int(len(J_history) * self.slice_fraction) + self.slice_bias
 
         slice = J_history[-slice_size:]
 
-        self.ax2.set_title(f"J_train_history - last {len(slice)}")
+        self.ax2.set_title(f"J_train_history - last {len(slice)} steps")
 
         self.line1.set_data(range(len(J_history)), J_history)
         self.line2.set_data(range(len(J_history) - len(slice), len(J_history)), slice)
 
 
         for ax in [self.ax1, self.ax2]:
             ax.relim()
```

### Comparing `liveplotlib-0.3.1/src/liveplotlib/live_plot_train_and_val.py` & `liveplotlib-0.3.2/src/liveplotlib/live_plot_train_and_val.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,20 @@
 
     
     def __init__(self, 
                  slice_bias: int = 10,
                  slice_fraction: float = 0, 
                  print_reports: bool = True):
         
+
+        # Parameters checking 
+        if not ( 0 <= slice_fraction < 1 ):
+            raise ValueError(f"Slice fraction should be: 0 <= slice_fraction < 1  (in [0, 1)), but you gave {slice_fraction}")
+
+
         self.slice_bias = slice_bias
         self.slice_fraction = slice_fraction
 
 
 
         self.if_ipynb_handler = IfIPYNBHandler(print_reports=print_reports)
         self.if_ipynb_handler.start()
```

### Comparing `liveplotlib-0.3.1/src/liveplotlib.egg-info/PKG-INFO` & `liveplotlib-0.3.2/src/liveplotlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyQt6
+Requires-Dist: PyQt5
 Requires-Dist: matplotlib
 
 # LIVE PLOT LIBrary (liveplotlib)
 - Library for plotting (visualizing) cost function changes during model training (in real time)
 
 
 # Notations
```

