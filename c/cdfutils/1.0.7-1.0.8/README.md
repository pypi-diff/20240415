# Comparing `tmp/cdfutils-1.0.7-py3-none-any.whl.zip` & `tmp/cdfutils-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14383 bytes, number of entries: 9
+Zip file size: 14410 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     3085 b- defN 23-Apr-11 00:24 cdfutils/Config.py
--rw-rw-rw-  2.0 fat     4750 b- defN 24-Mar-13 01:49 cdfutils/DotNet.py
+-rw-rw-rw-  2.0 fat     4823 b- defN 24-Apr-15 02:31 cdfutils/DotNet.py
 -rw-rw-rw-  2.0 fat     1061 b- defN 22-Jun-27 06:25 cdfutils/Textfile.py
--rw-rw-rw-  2.0 fat      341 b- defN 24-Feb-21 02:17 cdfutils/__init__.py
--rw-rw-rw-  2.0 fat    25589 b- defN 24-Mar-13 01:50 cdfutils-1.0.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1597 b- defN 24-Mar-13 01:50 cdfutils-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-13 01:50 cdfutils-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Mar-13 01:50 cdfutils-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      698 b- defN 24-Mar-13 01:50 cdfutils-1.0.7.dist-info/RECORD
-9 files, 37222 bytes uncompressed, 13189 bytes compressed:  64.6%
+-rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-15 02:28 cdfutils/__init__.py
+-rw-rw-rw-  2.0 fat    25589 b- defN 24-Apr-15 04:19 cdfutils-1.0.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1597 b- defN 24-Apr-15 04:19 cdfutils-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 04:19 cdfutils-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-15 04:19 cdfutils-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      698 b- defN 24-Apr-15 04:19 cdfutils-1.0.8.dist-info/RECORD
+9 files, 37295 bytes uncompressed, 13216 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: cdfutils/Textfile.py
 Comment: 
 
 Filename: cdfutils/__init__.py
 Comment: 
 
-Filename: cdfutils-1.0.7.dist-info/LICENSE.txt
+Filename: cdfutils-1.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cdfutils-1.0.7.dist-info/METADATA
+Filename: cdfutils-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: cdfutils-1.0.7.dist-info/WHEEL
+Filename: cdfutils-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: cdfutils-1.0.7.dist-info/top_level.txt
+Filename: cdfutils-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cdfutils-1.0.7.dist-info/RECORD
+Filename: cdfutils-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cdfutils/DotNet.py

```diff
@@ -15,14 +15,16 @@
 #
 #   Copyright Craig Farrow, 2010 - 2024
 #
 
 import clr
 clr.AddReference("System.Windows.Forms")
 
+import os
+
 from System.Windows.Forms import (
     MainMenu, MenuItem, Shortcut,
     ToolBar, ToolBarButton, ToolBarButtonStyle, ToolBarAppearance,
     ToolStrip, ToolStripContainer, ToolStripSeparator,
     ContextMenu,
     ImageList, 
     ColorDepth,
@@ -86,17 +88,17 @@
         self.ImageList = ImageList()
         self.ImageList.ColorDepth = ColorDepth.Depth32Bit
 
         for bParams in buttonList:
             button = ToolBarButton()
             if bParams:
                 handler, button.Text, imageName, button.ToolTipText = bParams
-                
-                self.ImageList.Images.Add(
-                    Bitmap.FromFile(imageName.join(imagePathTuple)))
+                path, suffix = imagePathTuple
+                imagePathName = os.path.join(path, imageName+suffix)
+                self.ImageList.Images.Add(Bitmap.FromFile(imagePathName))
                 button.ImageIndex = self.ImageList.Images.Count-1
                 self.HandlerList.append(handler)
                 if not handler:
                     button.Enabled = False
             else:
                 button.Style = ToolBarButtonStyle.Separator
                 self.HandlerList.append(None)   # Place-holder in handler list
```

## cdfutils/__init__.py

```diff
@@ -1,8 +1,8 @@
 #----------------------------------------------------------------------------
 # Name:         __init__.py
 # Purpose:      cdfutils provides a Python library of various functions 
 #               and classes that I use in my projects.
 #
 #----------------------------------------------------------------------------
 
-version = "1.0.7"
+version = "1.0.8"
```

## Comparing `cdfutils-1.0.7.dist-info/LICENSE.txt` & `cdfutils-1.0.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cdfutils-1.0.7.dist-info/METADATA` & `cdfutils-1.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdfutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: A general utility library of miscellaneous functions and classes
 Home-page: https://github.com/cdfarrow/cdfutils/wiki
 Author: Craig Farrow
 Platform: Windows
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

