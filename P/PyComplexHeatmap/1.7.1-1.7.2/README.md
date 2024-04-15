# Comparing `tmp/PyComplexHeatmap-1.7.1.tar.gz` & `tmp/pycomplexheatmap-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.7.1.tar", last modified: Wed Apr 10 19:15:48 2024, max compression
+gzip compressed data, was "pycomplexheatmap-1.7.2.tar", last modified: Mon Apr 15 20:36:49 2024, max compression
```

## Comparing `PyComplexHeatmap-1.7.1.tar` & `pycomplexheatmap-1.7.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.043738 PyComplexHeatmap-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.011738 PyComplexHeatmap-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.015738 PyComplexHeatmap-1.7.1/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 19:15:46.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    63152 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21507 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-10 19:15:48.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:15:47.000000 PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:48.039738 PyComplexHeatmap-1.7.1/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 19:15:13.000000 PyComplexHeatmap-1.7.1/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 19:15:14.000000 PyComplexHeatmap-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:15:48.043738 PyComplexHeatmap-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-10 19:15:14.000000 PyComplexHeatmap-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63152 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80279 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 20:36:49.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-15 20:36:28.000000 pycomplexheatmap-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-15 20:36:28.000000 pycomplexheatmap-1.7.2/setup.py
```

### Comparing `PyComplexHeatmap-1.7.1/.github/FUNDING.yml` & `pycomplexheatmap-1.7.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/.github/workflows/python-publish.yml` & `pycomplexheatmap-1.7.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/CITATION.cff` & `pycomplexheatmap-1.7.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/LICENSE` & `pycomplexheatmap-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PKG-INFO` & `pycomplexheatmap-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.1
+Version: 1.7.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
@@ -101,16 +101,16 @@
 ### [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/get_started.html)
 ### Example output
 Click picture to view the source code
 
 <table>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
-                <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Control-gap-&-pad-in-heatmap">
+                <img src="docs/images/gallery1.png" title="kwargs, gap and pad" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Modifying-xlabel-and-ylabel-using-xlabel_kws-and-ylabel_kws">
                 <img src="docs/images/gallery11.png" title="Modify labels" align="center" width="250px">
             </a>
         </td>
```

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/annotations.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/annotations.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/clustermap.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/clustermap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1131,26 +1131,29 @@
 		default is None (no xlabel would be shown).
 	ylabel: str
 		default is None (no ylabel would be shown).
 	xlabel_kws: dict
 		alpha,color,fontfamily,fontname,fontproperties,fontsize,fontstyle,
 		fontweight,label,rasterized,rotation,rotation_mode(default,anchor),visible,
 		zorder,verticalalignment,horizontalalignment.
-		See ax.xaxis.label.properties()
+		See ax.xaxis.label.properties(), for example:
+				cm=ClusterMapPlotter(***), print(cm.ax.xaxis.label.properties())
 		or matplotlib.axis.XAxis.label.properties() for detail.
 	ylabel_kws: dict
 		sams as xlabel_kws
 	xlabel_side: str
 		bottom or top, default is bottom,
 	ylabel_side: str
 		left or right, default is left
 	xlabel_bbox_kws: dict
 		alpha,clip_box, clip_on,edgecolor,facecolor,fill,height,in_layout,label,
 		linestyle, linewidth,rasterized,visible,width.
 		See ax.xaxis.label.get_bbox_patch().properties() for more information.
+		For example:
+			cm=ClusterMapPlotter(***), print(cm.ax.xaxis.label.get_bbox_patch().properties())
 	ylabel_bbox_kws: dict
 		same as xlabel_bbox_kws
 	rasterized :bool
 		default is auto, when the number of rows or number of cols > 5000,
 		rasterized would be automatically set to True to speed up the plotting.
 	kwargs :kws passed to plot_heatmap, including vmin, vmax,center,robust,
 		annot, annot_kws, fmt, mask, linewidths linecolor, na_col, cbar,cbar_kwss
@@ -2148,14 +2151,20 @@
 				)  # unit is pixel
 			else:
 				xticklabel_h = 0
 			if 'labelpad' not in self.xlabel_kws:
 				labelpad = xticklabel_h * 72 / self.ax.figure.dpi  # points; pixel to points: 1 point == fig.dpi/72. pixels
 			else:
 				labelpad = self.xlabel_kws.pop('labelpad')
+			if 'position' not in self.xlabel_kws:
+				ax_heatmap_box = self.ax_heatmap.get_window_extent()
+				ax_box = self.ax.get_window_extent()
+				pos_x=(np.mean([ax_heatmap_box.x0,ax_heatmap_box.x1])-ax_box.x0) / ax_box.width
+				self.xlabel_kws.setdefault('position',(pos_x,0))
+
 			self.xlabel_kws.setdefault("verticalalignment", "center")
 			self.ax.set_xlabel(self.xlabel, labelpad=labelpad + self.ax.xaxis.labelpad)
 			self.ax.xaxis.label.update(self.xlabel_kws)
 			self.ax.xaxis.set_label_position(self.xlabel_side)
 			if not self.xlabel_bbox_kws is None:
 				self.ax.xaxis.label.set_bbox(
 					self.xlabel_bbox_kws
@@ -2167,14 +2176,19 @@
 				)  # unit is pixel
 			else:
 				yticklabel_w = 0
 			if 'labelpad' not in self.ylabel_kws:
 				labelpad = yticklabel_w * 72 / self.ax.figure.dpi  # points; pixel to points: 1 point == fig.dpi/72. pixels
 			else:
 				labelpad = self.ylabel_kws.pop('labelpad')
+			if 'position' not in self.xlabel_kws:
+				ax_heatmap_box = self.ax_heatmap.get_window_extent()
+				ax_box = self.ax.get_window_extent()
+				pos_y=(np.mean([ax_heatmap_box.y0,ax_heatmap_box.y1])-ax_box.y0) / ax_box.height
+				self.ylabel_kws.setdefault('position',(0,pos_y))
 			self.ylabel_kws.setdefault("horizontalalignment", "center")
 			self.ax.set_ylabel(self.ylabel, labelpad=labelpad + self.ax.yaxis.labelpad)
 			self.ax.yaxis.label.update(self.ylabel_kws)
 			self.ax.yaxis.set_label_position(self.ylabel_side)
 			if not self.ylabel_bbox_kws is None:
 				self.ax.yaxis.label.set_bbox(
 					self.ylabel_bbox_kws
```

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/colors.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/dotHeatmap.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/dotHeatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,21 +100,19 @@
 		max_s = r**2
 	# s
 	s = kwargs.pop("s", None)
 	# print(s is None,vmin,vmax)
 	if s is None:
 		df["S"] = scale(df["Value"].abs().values,vmin=vmin, vmax=vmax)
 	else:
-		if isinstance(s, pd.DataFrame):
+		if isinstance(s, pd.DataFrame): # s is already normalized globally
 			s = s.reindex(index=row_labels, columns=col_labels).stack().reset_index()
 			s.columns = ["Row", "Col", "Value"]
-			# print(s.shape)
-			# print(s.head())
-			df["S"] = scale(s.Value.abs().values) #scale to 0-1
-			# df['S'] = s.Value.values
+			# df["S"] = scale(s.Value.abs().values) #scale to 0-1
+			df['S'] = s.Value.values
 		elif isinstance(s, (int, float)):
 			df["S"] = s
 
 	# hue
 	if not hue is None:  # hue is a dataframe
 		hue = hue.reindex(index=row_labels, columns=col_labels).stack().reset_index()
 		hue.columns = ["Row", "Col", "Value"]
@@ -360,29 +358,34 @@
 				index=self.y, columns=self.x, values=self.hue
 			).fillna(self.hue_na)
 		# s
 		if not self.s is None:
 			if isinstance(self.s, (int, float)):
 				self.kwargs["s"] = self.s
 				self.smax=self.s
-				self.smin=self.s
+				self.smin=None
 			elif isinstance(self.s, str):
 				self.kwargs["s"] = data.pivot_table(
 					index=self.y, columns=self.x, values=self.s, aggfunc=self.aggfunc
 				).fillna(self.s_na)
 				self.smin = np.nanmin(self.kwargs["s"].values)
 				self.smax = np.nanmax(self.kwargs["s"].values)
 			elif isinstance(self.s,pd.Series):
 				self.kwargs["s"] = data.assign(GivenS=self.s).pivot_table(
 					index=self.y, columns=self.x, values='GivenS', aggfunc=self.aggfunc
 				).fillna(self.s_na)
 				self.smin = np.nanmin(self.kwargs["s"].values)
 				self.smax = np.nanmax(self.kwargs["s"].values)
 			else:
 				raise ValueError("s must be a str, int or float!")
+
+			if not self.smin is None: #s is a dataframe, perform standard normalization.
+				delta=self.smax-self.smin
+				self.kwargs["s"]=self.kwargs["s"].applymap(lambda x:(x-self.smin)/delta)
+
 		# c
 		if not self.c is None:
 			if isinstance(self.c,pd.Series):
 				self.kwargs["s"] = data.assign(GivenC=self.s).pivot_table(
 					index=self.y, columns=self.x, values='GivenC', aggfunc=self.aggfunc
 				).fillna(self.c_na)
```

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/example.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/oncoPrint.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap/utils.py` & `pycomplexheatmap-1.7.2/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/PKG-INFO` & `pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.1
+Version: 1.7.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
@@ -101,16 +101,16 @@
 ### [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/get_started.html)
 ### Example output
 Click picture to view the source code
 
 <table>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
-                <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Control-gap-&-pad-in-heatmap">
+                <img src="docs/images/gallery1.png" title="kwargs, gap and pad" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Modifying-xlabel-and-ylabel-using-xlabel_kws-and-ylabel_kws">
                 <img src="docs/images/gallery11.png" title="Modify labels" align="center" width="250px">
             </a>
         </td>
```

### Comparing `PyComplexHeatmap-1.7.1/PyComplexHeatmap.egg-info/SOURCES.txt` & `pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/README.md` & `pycomplexheatmap-1.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 ### [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/get_started.html)
 ### Example output
 Click picture to view the source code
 
 <table>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
-                <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Control-gap-&-pad-in-heatmap">
+                <img src="docs/images/gallery1.png" title="kwargs, gap and pad" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/kwargs.html#Modifying-xlabel-and-ylabel-using-xlabel_kws-and-ylabel_kws">
                 <img src="docs/images/gallery11.png" title="Modify labels" align="center" width="250px">
             </a>
         </td>
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 want to update it, please run `pip uninstall PyComplexHeatmap` and install from
 github again OR ```shell git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap python setup.py install ``` ## [**Usage**](https://
 dingwb.github.io/PyComplexHeatmap) ---------------------- ### [Simple Guide To
 Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/
 get_started.html) ### Example output Click picture to view the source code
 _[_d_o_c_s_/_i_m_a_g_e_s_/          _[_d_o_c_s_/_i_m_a_g_e_s_/     _[_d_o_c_s_/_i_m_a_g_e_s_/_g_a_l_l_e_r_y_3_._j_p_g_]
-_g_a_l_l_e_r_y_1_._j_p_g_]          _g_a_l_l_e_r_y_1_1_._p_n_g_]
+_g_a_l_l_e_r_y_1_._p_n_g_]          _g_a_l_l_e_r_y_1_1_._p_n_g_]
 _[_d_o_c_s_/_i_m_a_g_e_s_/ _[_d_o_c_s_/_i_m_a_g_e_s_/_g_a_l_l_e_r_y_6_._p_n_g_] _[_d_o_c_s_/_i_m_a_g_e_s_/_g_a_l_l_e_r_y_9_._p_n_g_]
 _g_a_l_l_e_r_y_5_._p_n_g_]
 _[_d_o_c_s_/_i_m_a_g_e_s_/ _[_d_o_c_s_/_i_m_a_g_e_s_/_g_a_l_l_e_r_y_7_._p_n_g_] _[_d_o_c_s_/_i_m_a_g_e_s_/_g_a_l_l_e_r_y_4_._p_n_g_]
 _g_a_l_l_e_r_y_8_._p_n_g_]
 _[_d_o_c_s_/_i_m_a_g_e_s_/          _[_d_o_c_s_/_i_m_a_g_e_s_/              _[_d_o_c_s_/_i_m_a_g_e_s_/
 _g_a_l_l_e_r_y_2_._p_n_g_]          _g_a_l_l_e_r_y_1_0_._p_n_g_]             _g_a_l_l_e_r_y_1_2_._p_n_g_]
 ### [Advanced Usage](https://dingwb.github.io/PyComplexHeatmap/build/html/
```

### Comparing `PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.pdf` & `pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/ComplexHeatmap.png` & `pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.pdf` & `pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/PyComplexHeatmap.png` & `pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/README.md` & `pycomplexheatmap-1.7.2/comparison/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/beta.csv` & `pycomplexheatmap-1.7.2/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/df_col.csv` & `pycomplexheatmap-1.7.2/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/df_row.csv` & `pycomplexheatmap-1.7.2/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/heatmap.R` & `pycomplexheatmap-1.7.2/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/heatmap.ipynb` & `pycomplexheatmap-1.7.2/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/comparison/heatmap.py` & `pycomplexheatmap-1.7.2/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/pyproject.toml` & `pycomplexheatmap-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.7.1/setup.py` & `pycomplexheatmap-1.7.2/setup.py`

 * *Files identical despite different names*

