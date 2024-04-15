# Comparing `tmp/silicon_analyser-1.0.5.tar.gz` & `tmp/silicon_analyser-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon_analyser-1.0.5.tar", last modified: Sun Apr 14 11:47:14 2024, max compression
+gzip compressed data, was "silicon_analyser-1.0.6.tar", last modified: Mon Apr 15 16:13:13 2024, max compression
```

## Comparing `silicon_analyser-1.0.5.tar` & `silicon_analyser-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2770 2024-04-14 11:47:14.000000 silicon_analyser-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1989 2024-04-14 09:44:53.000000 silicon_analyser-1.0.5/README.md
--rw-rw-rw-   0        0        0     1141 2024-04-14 09:48:03.000000 silicon_analyser-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 11:47:14.000000 silicon_analyser-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.5/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.5/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.5/silicon_analyser/dialogs/pixel_image.py
--rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.5/silicon_analyser/dialogs/pixel_image.ui
--rw-rw-rw-   0        0        0     3052 2024-04-14 07:08:53.000000 silicon_analyser-1.0.5/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2313 2024-04-13 13:47:07.000000 silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2771 2024-04-14 06:57:02.000000 silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.5/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.5/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1354 2024-04-14 11:44:59.000000 silicon_analyser-1.0.5/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    14402 2024-04-13 13:49:48.000000 silicon_analyser-1.0.5/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    20548 2024-04-14 09:34:44.000000 silicon_analyser-1.0.5/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.5/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3499 2024-04-13 13:39:46.000000 silicon_analyser-1.0.5/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    18798 2024-04-14 08:01:35.000000 silicon_analyser-1.0.5/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.5/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     6663 2024-04-14 06:53:38.000000 silicon_analyser-1.0.5/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0     8907 2024-04-14 06:57:21.000000 silicon_analyser-1.0.5/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.5/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2053 2024-04-13 13:22:20.000000 silicon_analyser-1.0.5/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.5/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     2770 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-14 11:47:13.000000 silicon_analyser-1.0.5/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3242 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2024-04-14 16:45:54.000000 silicon_analyser-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1141 2024-04-15 15:27:19.000000 silicon_analyser-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     3096 2024-04-15 15:27:03.000000 silicon_analyser-1.0.6/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2313 2024-04-13 13:47:07.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     2771 2024-04-14 06:57:02.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.6/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.6/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1354 2024-04-14 11:44:59.000000 silicon_analyser-1.0.6/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    14402 2024-04-14 16:49:50.000000 silicon_analyser-1.0.6/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    20772 2024-04-15 15:38:08.000000 silicon_analyser-1.0.6/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.6/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     3499 2024-04-13 13:39:46.000000 silicon_analyser-1.0.6/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    18962 2024-04-15 15:54:55.000000 silicon_analyser-1.0.6/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.6/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     6698 2024-04-15 15:57:44.000000 silicon_analyser-1.0.6/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0     9837 2024-04-15 16:00:59.000000 silicon_analyser-1.0.6/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.6/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2053 2024-04-13 13:22:20.000000 silicon_analyser-1.0.6/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.6/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     3242 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon_analyser-1.0.5/LICENSE` & `silicon_analyser-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/PKG-INFO` & `silicon_analyser-1.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.5
+Version: 1.0.6
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Install from pip:
 
 `pip install silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
+(but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
 * [Keras](https://keras.io/)
 * [PyQtGraph](https://www.pyqtgraph.org/)
 
@@ -61,22 +62,29 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Additional info
+
+* you might need to install cuda-specific [PyTorch](https://pytorch.org/get-started/previous-versions/#linux-and-windows-4) for accelerated computing
+    * check your graphic driver version for compatible cuda version!
+
 # Keys
 
 * Use up/down/left/right to navigate
 * Hold shift to move faster
 * Scroll-wheel to zoom out
 * Click on minimap to get directly to a position
+* Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
+* show loading screen on start (pytorch with cuda support takes a bit to load)
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.5/README.md` & `silicon_analyser-1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Install from pip:
 
 `pip install silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
+(but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
 * [Keras](https://keras.io/)
 * [PyQtGraph](https://www.pyqtgraph.org/)
 
@@ -40,22 +41,29 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Additional info
+
+* you might need to install cuda-specific [PyTorch](https://pytorch.org/get-started/previous-versions/#linux-and-windows-4) for accelerated computing
+    * check your graphic driver version for compatible cuda version!
+
 # Keys
 
 * Use up/down/left/right to navigate
 * Hold shift to move faster
 * Scroll-wheel to zoom out
 * Click on minimap to get directly to a position
+* Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
+* show loading screen on start (pytorch with cuda support takes a bit to load)
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.5/pyproject.toml` & `silicon_analyser-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/dialogs/pixel_image.py` & `silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/dialogs/pixel_image.ui` & `silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/grid.py` & `silicon_analyser-1.0.6/silicon_analyser/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,17 @@
                 self._rects[label][i] = [col, row+1]
     
     def setRect(self, col, row, label):
         #print(f"setRect {col} {row} {label}")
         r = [col, row]
         if label not in self._rects:
             self._rects[label] = []
-        if r in self._rects[label]:
-            self._rects[label].remove(r)
+        for lbl in self._rects.keys():
+            if r in self._rects[lbl]:
+                self._rects[lbl].remove(r)
         self._rects[label].append(r)
         
     def unsetRect(self, col, row, label):
         print(f"unsetRect {col} {row}")
         r = [col, row]
         if r in self._rects[label]:
             self._rects[label].remove(r)
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/addgridbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/addlabelbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/ai.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/ai.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/computebtn.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/computebtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/fullimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,40 +370,47 @@
         sposX, sposY = posX*scale, posY*scale
         for k in grids.keys():
             if gridsActive[k]:
                 grid: Grid = grids[k]
                 cellWidth = grid.width / grid.cols
                 cellHeight = grid.height / grid.rows
                 startCol, startRow, endCol, endRow = self.calcGridCellsVisibleRange(grid)
-                #for col in range(0,grid.cols):
-                #    for row in range(0,grid.rows):
-                for col in range(startCol,endCol):
-                    for row in range(startRow,endRow):
-                        ox = grid.x + col * cellWidth
-                        oy = grid.y + row * cellHeight
-                        ex = ox + cellWidth
-                        ey = oy + cellHeight
-                        x = int(self._translatePixelToScaled(ox)-sposX)
-                        y = int(self._translatePixelToScaled(oy)-sposY)
-                        ex = int(self._translatePixelToScaled(ex)-sposX)
-                        ey = int(self._translatePixelToScaled(ey)-sposY)
-                        w = ex - x
-                        h = ey - y
-                        if x>=0 and y>=0 and x<=self.width() and y<=self.height():
-                            if grid.isRectSet(col,row):
-                                rectLabel = grid.rectLabel(col, row)
-                                if self._myWindow.getTree().isItemSelected(rectLabel, grid.name, gridItemType):
-                                    brush = QBrush(rectSetActiveColor)
-                                else:
-                                    brush = QBrush(rectSetColor)
-                                qp.setBrush(brush)
-                            else:
-                                brush = QBrush(rectUnsetColor)
-                                qp.setBrush(brush)
-                            qp.drawRect(x,y,w,h)
+                for row in range(startRow,endRow):
+                    if not self._drawGridOnScaledImgRow(qp, gridItemType, rectSetColor, rectSetActiveColor, rectUnsetColor, sposX, sposY, grid, cellWidth, cellHeight, startCol, endCol, row):
+                        break
+
+    def _drawGridOnScaledImgRow(self, qp:QPainter, gridItemType:str, rectSetColor:QColor, rectSetActiveColor:QColor, rectUnsetColor:QColor, sposX:float, sposY:float, grid:Grid, cellWidth:float, cellHeight:float, startCol:int, endCol:int, row:int):
+        oy = grid.y + row * cellHeight
+        y = int(self._translatePixelToScaled(oy)-sposY)
+        if y >= self.height():
+            return False
+        for col in range(startCol,endCol):
+            ox = grid.x + col * cellWidth
+            ex = ox + cellWidth
+            ey = oy + cellHeight
+            x = int(self._translatePixelToScaled(ox)-sposX)
+            if x > self.width():
+                break
+            ex = int(self._translatePixelToScaled(ex)-sposX)
+            ey = int(self._translatePixelToScaled(ey)-sposY)
+            w = ex - x
+            h = ey - y
+            if x>=0 and y>=0 and x<=self.width() and y<=self.height():
+                if grid.isRectSet(col,row):
+                    rectLabel = grid.rectLabel(col, row)
+                    if self._myWindow.getTree().isItemSelected(rectLabel, grid.name, gridItemType):
+                        brush = QBrush(rectSetActiveColor)
+                    else:
+                        brush = QBrush(rectSetColor)
+                    qp.setBrush(brush)
+                else:
+                    brush = QBrush(rectUnsetColor)
+                    qp.setBrush(brush)
+                qp.drawRect(x,y,w,h)
+        return True
                         
     def _drawRectOnScaledImg(self, rects, rectActive, qp:QPainter):
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         sposX, sposY = posX*scale, posY*scale
         for k in rects.keys():
             if rectActive[k]:
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/minimap.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/properties.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/properties.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/helper/tree.py` & `silicon_analyser-1.0.6/silicon_analyser/helper/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,18 @@
         if type == TreeItem.TYPE_GRID:
             treeItem: QStandardItem = myWindow.getManualItem()
         if type == TreeItem.TYPE_AI_GRID:
             treeItem: QStandardItem = myWindow.getAIItem()
         if type == TreeItem.TYPE_GRID_ITEM:
             selectedItem = self.getSelectedItem()
             if selectedItem is not None:
-                treeItem: QStandardItem = selectedItem.parent()
+                if selectedItem.data(TreeItem.TYPE) == TreeItem.TYPE_GRID:
+                    treeItem: QStandardItem = selectedItem 
+                else:
+                    treeItem: QStandardItem = selectedItem.parent()
         if type == TreeItem.TYPE_AI_GRID_ITEM:
             selectedItem = self.getSelectedItem()
             if selectedItem is not None:
                 treeItem: QStandardItem = selectedItem.parent()
         if parent_item is not None:
             treeItem: QStandardItem = parent_item
         tree: Tree = self
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.6/silicon_analyser/main_window.ui`

 * *Files 1% similar despite different names*

#### Comparing `silicon_analyser-1.0.5/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.6/silicon_analyser/main_window.ui`

```diff
@@ -144,14 +144,15 @@
       </property>
       <widget class="QMenu" name="menuInfo">
         <property name="title">
           <string>Info</string>
         </property>
         <addaction name="_actionMade_by_TheCrazyT"/>
         <addaction name="_actionUrl"/>
+        <addaction name="separator"/>
       </widget>
       <addaction name="menuInfo"/>
     </widget>
     <action name="_actionGridAddRowTop">
       <property name="text">
         <string>Add row to top</string>
       </property>
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/mywindow.py` & `silicon_analyser-1.0.6/silicon_analyser/mywindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import torch
+import importlib.metadata
 from PyQt5 import QtCore, QtGui, uic
 from PyQt5.QtCore import Qt, QItemSelection
-from PyQt5.QtWidgets import QFileDialog, QTableView, QStatusBar, QAction, QPushButton
+from PyQt5.QtWidgets import QFileDialog, QMenu, QTableView, QStatusBar, QAction
 from PyQt5.QtGui import QPixmap, QStandardItem, QStandardItemModel
 from os import path as p
 import sys
 
 import silicon_analyser.savefiles
 from silicon_analyser.savefiles import loadGrids, loadRects
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
@@ -37,14 +39,15 @@
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     autosave: bool
+    menuBar: QMenu
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
         path: str = p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui'
         uic.loadUi(path, self)
         tree: Tree = self._tree
         properties: QTableView = self._properties
@@ -66,15 +69,15 @@
         self._treeModel.appendRow(self._treeAIItem)
         tree.setModel(self._treeModel)
         self._models = {}
         self._actionUrl.triggered.connect(self.openMainUrl)
 
         if(len(sys.argv) < 2):
             dlg = QFileDialog()
-            filenames = dlg.getOpenFileName(caption="Load image",filter="Image (*.png;*.jpg;*.bmp;*.gif)",initialFilter="Trained model (*.h5)")
+            filenames = dlg.getOpenFileName(caption="Load image",filter="Image (*.png;*.jpg;*.bmp;*.gif)",initialFilter="Image (*.png;*.jpg;*.bmp;*.gif)")
             if(len(filenames) >= 1):
                 self._pixmap = QPixmap(filenames[0])
         else:
             self._pixmap = QPixmap(sys.argv[1])
         
         computeBtn: ComputeBtn = self._computeBtn
         addGridBtn: AddGridBtn = self._addGridBtn
@@ -116,14 +119,24 @@
                     text = treeItem.data(TreeItem.TEXT)
                     if(not grids[gridKey]._rectsActive[text]):
                         treeItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
             image.loadGrids(grids)
         
         image.drawImage()
         self.autosave = True
+        if(torch.cuda.is_available()):
+            self.setSuccessStatus("CUDA successfully initialized")
+        else:
+            self.setSuccessStatus("CUDA not found")
+        
+        menuBar: QMenu = self.menuBar    
+
+        version = importlib.metadata.version("silicon-analyser")
+        action = menuBar.addAction(f"Version: {version}")
+        action.triggered.connect(self.openMainUrl)
         
     def treeSelectionChanged(self, selection: QItemSelection):
         tree: Tree = self._tree
         selectedType: str|None = tree.selectedType()
         computeBtn: ComputeBtn = self._computeBtn
         addLabelBtn: AddLabelBtn = self._addLabelBtn
         if((selectedType == TreeItem.TYPE_GRID_ITEM)
@@ -161,17 +174,29 @@
         return self._minimap
 
     def imageWidth(self):
         return self.getImage().width()
 
     def imageHeight(self):
         return self.getImage().height()
+
+    def setSuccessStatus(self, text):
+        statusBar: QStatusBar = self._statusBar
+        statusBar.setStyleSheet('background-color: #0ff000')
+        statusBar.showMessage(text)
+
+    def setErrorStatus(self, text):
+        statusBar: QStatusBar = self._statusBar
+        statusBar.setStyleSheet('background-color: #ff0000')
+        statusBar.showMessage(text)
             
     def setStatusText(self, text):
-        self._statusBar.showMessage(text)
+        statusBar: QStatusBar = self._statusBar
+        statusBar.setStyleSheet('')
+        statusBar.showMessage(text)
         
     def getTree(self) -> AbstractTreeHelper:
         return self._tree
     
     def getManualItem(self) -> QStandardItem:
         return self._treeManualItem
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser/savefiles.py` & `silicon_analyser-1.0.6/silicon_analyser/savefiles.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser/treeitem.py` & `silicon_analyser-1.0.6/silicon_analyser/treeitem.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.5/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.0.6/silicon_analyser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.5
+Version: 1.0.6
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Install from pip:
 
 `pip install silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
+(but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
 * [Keras](https://keras.io/)
 * [PyQtGraph](https://www.pyqtgraph.org/)
 
@@ -61,22 +62,29 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Additional info
+
+* you might need to install cuda-specific [PyTorch](https://pytorch.org/get-started/previous-versions/#linux-and-windows-4) for accelerated computing
+    * check your graphic driver version for compatible cuda version!
+
 # Keys
 
 * Use up/down/left/right to navigate
 * Hold shift to move faster
 * Scroll-wheel to zoom out
 * Click on minimap to get directly to a position
+* Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
+* show loading screen on start (pytorch with cuda support takes a bit to load)
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.5/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.0.6/silicon_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

