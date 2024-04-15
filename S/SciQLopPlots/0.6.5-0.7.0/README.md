# Comparing `tmp/sciqlopplots-0.6.5-cp39-cp39-win_amd64.whl.zip` & `tmp/sciqlopplots-0.7.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 965206 bytes, number of entries: 6
-?rw-rw-r--  2.0 fat     3166 b- defN 24-Mar-13 17:29 sciqlopplots-0.6.5.dist-info/METADATA
-?rw-rw-r--  2.0 fat       83 b- defN 24-Mar-13 17:29 sciqlopplots-0.6.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1585 b- defN 24-Mar-13 16:40 sciqlopplots-0.6.5.dist-info/COPYING
--rw-rw-rw-  2.0 fat  2726912 b- defN 24-Mar-13 17:29 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      204 b- defN 24-Mar-13 16:40 SciQLopPlots/__init__.py
-?rw-rw-r--  2.0 fat      506 b- defN 24-Mar-13 17:29 sciqlopplots-0.6.5.dist-info/RECORD
-6 files, 2732456 bytes uncompressed, 964292 bytes compressed:  64.7%
+Zip file size: 973239 bytes, number of entries: 6
+?rw-rw-r--  2.0 fat     3166 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/METADATA
+?rw-rw-r--  2.0 fat       83 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1585 b- defN 24-Apr-15 20:47 sciqlopplots-0.7.0.dist-info/COPYING
+-rw-rw-rw-  2.0 fat  2752000 b- defN 24-Apr-15 21:00 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      204 b- defN 24-Apr-15 20:47 SciQLopPlots/__init__.py
+?rw-rw-r--  2.0 fat      506 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/RECORD
+6 files, 2757544 bytes uncompressed, 972325 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: sciqlopplots-0.6.5.dist-info/METADATA
+Filename: sciqlopplots-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: sciqlopplots-0.6.5.dist-info/WHEEL
+Filename: sciqlopplots-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: sciqlopplots-0.6.5.dist-info/COPYING
+Filename: sciqlopplots-0.7.0.dist-info/COPYING
 Comment: 
 
 Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
 Comment: 
 
 Filename: SciQLopPlots/__init__.py
 Comment: 
 
-Filename: sciqlopplots-0.6.5.dist-info/RECORD
+Filename: sciqlopplots-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SciQLopPlots/__init__.py

```diff
@@ -1,5 +1,5 @@
 from PySide6 import QtCore, QtGui, QtWidgets, QtOpenGL, QtPrintSupport, QtSvg
 from .SciQLopPlotsBindings import *
 from .SciQLopPlotsBindings import _QCustomPlot as QCustomPlot
 
-__version__ = '0.6.5'
+__version__ = '0.7.0'
```

## Comparing `sciqlopplots-0.6.5.dist-info/METADATA` & `sciqlopplots-0.7.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciQLopPlots
-Version: 0.6.5
+Version: 0.7.0
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

## Comparing `sciqlopplots-0.6.5.dist-info/COPYING` & `sciqlopplots-0.7.0.dist-info/COPYING`

 * *Files identical despite different names*

