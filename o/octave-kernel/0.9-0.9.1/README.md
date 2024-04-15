# Comparing `tmp/octave_kernel-0.9.zip` & `tmp/octave_kernel-0.9.1.zip`

## zipinfo {}

```diff
@@ -1,5 +1,8 @@
-Zip file size: 3643 bytes, number of entries: 3
--rw-rw-r--  2.0 unx     5044 b- defN 15-Feb-04 08:46 octave_kernel-0.9/octave_kernel.py
--rw-rw-r--  2.0 unx     2259 b- defN 15-Feb-04 07:24 octave_kernel-0.9/setup.py
--rw-rw-r--  2.0 unx     1150 b- defN 15-Feb-04 08:48 octave_kernel-0.9/PKG-INFO
-3 files, 8453 bytes uncompressed, 3221 bytes compressed:  61.9%
+Zip file size: 5395 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      883 b- defN 15-Feb-01 15:17 octave_kernel-0.9.1/HISTORY.rst
+-rw-r--r--  2.0 unx      486 b- defN 15-Feb-01 11:14 octave_kernel-0.9.1/README.rst
+-rw-r--r--  2.0 unx     1274 b- defN 15-Feb-01 10:58 octave_kernel-0.9.1/Makefile
+-rw-r--r--  2.0 unx     5177 b- defN 15-Feb-04 16:14 octave_kernel-0.9.1/octave_kernel.py
+-rw-r--r--  2.0 unx     1152 b- defN 15-Feb-04 16:14 octave_kernel-0.9.1/PKG-INFO
+-rw-r--r--  2.0 unx     2259 b- defN 15-Feb-02 19:26 octave_kernel-0.9.1/setup.py
+6 files, 11231 bytes uncompressed, 4555 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,10 +1,19 @@
-Filename: octave_kernel-0.9/octave_kernel.py
+Filename: octave_kernel-0.9.1/HISTORY.rst
 Comment: 
 
-Filename: octave_kernel-0.9/setup.py
+Filename: octave_kernel-0.9.1/README.rst
 Comment: 
 
-Filename: octave_kernel-0.9/PKG-INFO
+Filename: octave_kernel-0.9.1/Makefile
+Comment: 
+
+Filename: octave_kernel-0.9.1/octave_kernel.py
+Comment: 
+
+Filename: octave_kernel-0.9.1/PKG-INFO
+Comment: 
+
+Filename: octave_kernel-0.9.1/setup.py
 Comment: 
 
 Zip file comment:
```

## Comparing `octave_kernel-0.9/octave_kernel.py` & `octave_kernel-0.9.1/octave_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from IPython.display import Image
 from subprocess import check_output
 import os
 import tempfile
 from shutil import rmtree
 
 
-__version__ = '0.9'
+__version__ = '0.9.1'
 
 
 class OctaveKernel(ProcessMetaKernel):
     implementation = 'Octave Kernel'
     implementation_version = __version__,
     language = 'octave'
     language_version = '0.1',
@@ -111,20 +111,23 @@
         if settings['backend'] == 'inline':
             cmds.append("set(0, 'defaultfigurevisible', 'off');")
             cmds.append("graphics_toolkit('gnuplot');")
         else:
             cmds.append("set(0, 'defaultfigurevisible', 'on');")
             cmds.append("graphics_toolkit('%s');" % settings['backend'])
 
-        try:
-            width, height = settings['size'].split(',')
-            width, height = int(width), int(height)
-        except Exception as e:
-            self.Error(e)
-            width, height = 560, 420
+        if isinstance(settings['size'], tuple):
+            width, height = settings['size']
+        else:
+            try:
+                width, height = settings['size'].split(',')
+                width, height = int(width), int(height)
+            except Exception as e:
+                self.Error(e)
+                width, height = 560, 420
 
         cmds.append("""
         function make_figs(figdir)
             figHandles = get(0, 'children');
             for fig=1:length(figHandles)
                 f = figHandles(fig);
                 p = get(f, 'position');
```

## Comparing `octave_kernel-0.9/setup.py` & `octave_kernel-0.9.1/setup.py`

 * *Files identical despite different names*

## Comparing `octave_kernel-0.9/PKG-INFO` & `octave_kernel-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: octave_kernel
-Version: 0.9
+Version: 0.9.1
 Summary: An Octave kernel for Jupyter/IPython
 Home-page: https://github.com/calysto/octave_kernel
 Author: Steven Silvester
 Author-email: steven.silvester@ieee.org
 License: MIT
 Description: A Jupyter/IPython kernel for Octave
```

