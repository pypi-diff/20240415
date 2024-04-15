# Comparing `tmp/matsubplots-1.0.3.tar.gz` & `tmp/matsubplots-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matsubplots-1.0.3.tar", last modified: Tue Nov 21 19:28:15 2023, max compression
+gzip compressed data, was "matsubplots-1.1.0.tar", last modified: Mon Apr 15 16:10:12 2024, max compression
```

## Comparing `matsubplots-1.0.3.tar` & `matsubplots-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 19:28:15.880309 matsubplots-1.0.3/
--rw-rw-rw-   0        0        0     1099 2023-11-21 19:27:36.000000 matsubplots-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0     1247 2023-11-21 19:28:15.881308 matsubplots-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      786 2023-11-21 19:27:36.000000 matsubplots-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-11-21 19:28:15.820190 matsubplots-1.0.3/matsubplots/
--rw-rw-rw-   0        0        0      168 2023-11-21 19:27:36.000000 matsubplots-1.0.3/matsubplots/__init__.py
--rw-rw-rw-   0        0        0     5009 2023-11-21 19:27:36.000000 matsubplots-1.0.3/matsubplots/matsubplots.py
--rw-rw-rw-   0        0        0     7514 2023-11-21 19:27:36.000000 matsubplots-1.0.3/matsubplots/orthoview.py
--rw-rw-rw-   0        0        0       23 2023-11-21 19:27:36.000000 matsubplots-1.0.3/matsubplots/version.py
-drwxrwxrwx   0        0        0        0 2023-11-21 19:28:15.878310 matsubplots-1.0.3/matsubplots.egg-info/
--rw-rw-rw-   0        0        0     1247 2023-11-21 19:28:15.000000 matsubplots-1.0.3/matsubplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-11-21 19:28:15.000000 matsubplots-1.0.3/matsubplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 19:28:15.000000 matsubplots-1.0.3/matsubplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-11-21 19:28:15.000000 matsubplots-1.0.3/matsubplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-11-21 19:28:15.000000 matsubplots-1.0.3/matsubplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      312 2023-11-21 19:28:15.884308 matsubplots-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-11-21 19:27:36.000000 matsubplots-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.519089 matsubplots-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-15 16:09:00.000000 matsubplots-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1274 2024-04-15 16:10:12.518092 matsubplots-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-04-15 16:09:00.000000 matsubplots-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.475412 matsubplots-1.1.0/matsubplots/
+-rw-rw-rw-   0        0        0      168 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/matsubplots.py
+-rw-rw-rw-   0        0        0     7514 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/orthoview.py
+-rw-rw-rw-   0        0        0       23 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.515350 matsubplots-1.1.0/matsubplots.egg-info/
+-rw-rw-rw-   0        0        0     1274 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      312 2024-04-15 16:10:12.522087 matsubplots-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-15 16:09:00.000000 matsubplots-1.1.0/setup.py
```

### Comparing `matsubplots-1.0.3/LICENSE.md` & `matsubplots-1.1.0/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-The MIT License (MIT)
+# MIT License
 
 Copyright (c) 2022 Ali Uneri
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `matsubplots-1.0.3/PKG-INFO` & `matsubplots-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.0.3
+Version: 1.1.0
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib
 
 # matsubplots
 
 Better subplots for [matplotlib](https://matplotlib.org).
 
 [![license](https://img.shields.io/github/license/auneri/matsubplots)](https://github.com/auneri/matsubplots/blob/main/LICENSE.md)
 [![build](https://img.shields.io/github/actions/workflow/status/auneri/matsubplots/main.yml)](https://github.com/auneri/matsubplots/actions)
```

### Comparing `matsubplots-1.0.3/README.md` & `matsubplots-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.0.3/matsubplots/matsubplots.py` & `matsubplots-1.1.0/matsubplots/matsubplots.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,20 +40,22 @@
     width /= figsize[0]
     height /= figsize[1]
     return fig.add_axes((left, bottom, width, height), **kwargs)
 
 
 def grid(shape=1, size=3, pad=0, close=False, ioff=False, image_grid=False, return_grid=False, **kwargs):
     """Extend mpl_toolkits.axes_grid1.Grid."""
-    if np.isscalar(shape):
-        shape = shape, 1
+    shape_scalar = np.isscalar(shape)
+    if shape_scalar:
+        shape = 1, shape
     if np.isscalar(size):
         size = np.repeat(size, 2)
     if np.isscalar(pad):
         pad = np.repeat(pad, 2)
+    shape, size, pad = shape[::-1], size[::-1], pad[::-1]
     xticks = kwargs.pop('xticks', None)
     yticks = kwargs.pop('yticks', None)
     frameon = kwargs.pop('frameon', None)
     if image_grid:
         kwargs.setdefault('cbar_pad', pad[0])
         kwargs.setdefault('cbar_size', size[0] * 0.1)
         if kwargs.get('cbar_mode') == 'each':
@@ -73,36 +75,40 @@
     for ax in axs.ravel():
         if xticks is not None:
             ax.set_xticks(xticks)
         if yticks is not None:
             ax.set_yticks(yticks)
         if frameon is not None:
             ax.set_frame_on(frameon)
+    if shape_scalar:
+        axs = axs[0,0] if axs.size == 1 else np.squeeze(axs)
     returned = fig, axs
     if return_grid:
         returned += grid,
     return returned
 
 
 def imagegrid(*args, **kwargs):
     """Extend mpl_toolkits.axes_grid1.ImageGrid."""
     kwargs['image_grid'] = True
     kwargs.setdefault('xticks', ())
     kwargs.setdefault('yticks', ())
     return grid(*args, **kwargs)
 
 
-def subplots(shape=1, size=3, pad=0, close=False, ioff=False, label_mode='L', squeeze=True, **kwargs):
+def subplots(shape=1, size=3, pad=0, close=False, ioff=False, label_mode='L', **kwargs):
     """Extend matplotlib.pyplot.subplots."""
-    if np.isscalar(shape):
-        shape = shape, 1
+    shape_scalar = np.isscalar(shape)
+    if shape_scalar:
+        shape = 1, shape
     if np.isscalar(size):
         size = np.repeat(size, 2)
     if np.isscalar(pad):
         pad = np.repeat(pad, 2)
+    shape, size, pad = shape[::-1], size[::-1], pad[::-1]
     cbar_mode = kwargs.pop('cbar_mode', None)
     cbar_size = kwargs.pop('cbar_size', size[0] * 0.1)
     if cbar_mode == 'edge':
         shape = shape[0] + 1, shape[1]
     figsize = [size[x] * shape[x] + pad[x] * (shape[x] + 1) for x in range(2)]
     with plt.ioff() if ioff else contextlib.nullcontext():
         fig = plt.figure(figsize=figsize)
@@ -124,10 +130,10 @@
         axs, caxs = axs[:,:-1], axs[:,-1]
         for ax1, cax in zip(axs, caxs):
             cax.set_position([cbar_size / figsize[0] if i == 2 else x for i, x in enumerate(cax.get_position().bounds)])
             for ax2 in ax1:
                 ax2.cax = cax
     elif cbar_mode:
         raise NotImplementedError(cbar_mode)
-    if squeeze:
+    if shape_scalar:
         axs = axs[0,0] if axs.size == 1 else np.squeeze(axs)
     return fig, axs
```

### Comparing `matsubplots-1.0.3/matsubplots/orthoview.py` & `matsubplots-1.1.0/matsubplots/orthoview.py`

 * *Files identical despite different names*

### Comparing `matsubplots-1.0.3/matsubplots.egg-info/PKG-INFO` & `matsubplots-1.1.0/matsubplots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.0.3
+Version: 1.1.0
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib
 
 # matsubplots
 
 Better subplots for [matplotlib](https://matplotlib.org).
 
 [![license](https://img.shields.io/github/license/auneri/matsubplots)](https://github.com/auneri/matsubplots/blob/main/LICENSE.md)
 [![build](https://img.shields.io/github/actions/workflow/status/auneri/matsubplots/main.yml)](https://github.com/auneri/matsubplots/actions)
```

### Comparing `matsubplots-1.0.3/setup.py` & `matsubplots-1.1.0/setup.py`

 * *Files identical despite different names*

