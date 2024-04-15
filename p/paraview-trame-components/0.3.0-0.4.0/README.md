# Comparing `tmp/paraview_trame_components-0.3.0.tar.gz` & `tmp/paraview_trame_components-0.4.0.tar.gz`

## Comparing `paraview_trame_components-0.3.0.tar` & `paraview_trame_components-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/cone-with-slider.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/cone.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/pipeline.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/state-loader-slider.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/state-loader.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/test-cols.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/examples/wavelet-contour-state.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/__init__.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/core.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/pipeline.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/vcr.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/assets/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/layouts/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/layouts/col.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/layouts/factory.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/ptc/layouts/side.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/.gitignore
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/LICENSE
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/README.md
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 paraview_trame_components-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/all.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/cone-with-slider.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/cone.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/pipeline.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/state-loader-slider.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/state-loader.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/test-cols.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/examples/wavelet-contour-state.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/__init__.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/colors.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/core.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/pipeline.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/utils.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/vcr.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/assets/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/layouts/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/layouts/col.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/layouts/factory.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/ptc/layouts/side.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/.gitignore
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/README.md
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 paraview_trame_components-0.4.0/PKG-INFO
```

### Comparing `paraview_trame_components-0.3.0/examples/cone-with-slider.py` & `paraview_trame_components-0.4.0/examples/cone-with-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/examples/state-loader-slider.py` & `paraview_trame_components-0.4.0/examples/state-loader-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/examples/test-cols.py` & `paraview_trame_components-0.4.0/examples/test-cols.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/examples/wavelet-contour-state.py` & `paraview_trame_components-0.4.0/examples/wavelet-contour-state.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/ptc/core.py` & `paraview_trame_components-0.4.0/ptc/core.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/ptc/pipeline.py` & `paraview_trame_components-0.4.0/ptc/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,22 @@
             width=width,
             # Events
             actives_change=(self.on_active_change, "[$event]"),
             visibility_change=(
                 self.on_visibility_change,
                 "[$event.id, $event.visible]",
             ),
-            **kwargs,
+            **{
+                **kwargs,
+                "classes": kwargs.get("classes", "elevation-5 rounded-lg"),
+                "style": kwargs.get(
+                    "style",
+                    "pointer-events: auto; user-select: none; background: rgba(255, 255, 255, 0.5);",
+                ),
+            },
         )
         self._deleted_ids = set()
         self.update()
 
     def on_active_change(self, active_ids, **_):
         current_active = simple.GetActiveSource()
         proxy = None
```

### Comparing `paraview_trame_components-0.3.0/ptc/utils.py` & `paraview_trame_components-0.4.0/ptc/utils.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/ptc/layouts/col.py` & `paraview_trame_components-0.4.0/ptc/layouts/col.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/ptc/layouts/side.py` & `paraview_trame_components-0.4.0/ptc/layouts/side.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/LICENSE` & `paraview_trame_components-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.3.0/README.md` & `paraview_trame_components-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 ```bash
 # Create and activate venv
 python3.10 -m venv .venv
 source .venv/bin/activate
 
 # Install published package
-pip install ptc
+pip install paraview-trame-components
 
 # Let ParaView know about the location of that venv
 export PV_VENV=$PWD/.venv
 ```
 
 ## Running examples
 
 ```bash
-# Adjust path to point to your executable
+# Adjust path to point to your ParaView executable
 export PVPYTHON=/Applications/ParaView-5.12.0.app/Contents/bin/pvpython
 
 # Run the scripts
 $PVPYTHON --force-offscreen-rendering ./examples/cone.py
 $PVPYTHON --force-offscreen-rendering ./examples/cone_width_slider.py
 $PVPYTHON --force-offscreen-rendering ./examples/wavelet-contour-state.py
 $PVPYTHON --force-offscreen-rendering ./examples/pipeline.py
```

### Comparing `paraview_trame_components-0.3.0/pyproject.toml` & `paraview_trame_components-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paraview-trame-components"
-version = "0.3.0"
+version = "0.4.0"
 requires-python = ">= 3.10"
 dependencies = [
   "trame",
   "trame-vtk",
   "trame-vuetify",
   "trame-components",
 ]
@@ -75,15 +75,16 @@
 line-ending = "auto"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
   # ok
   "C408",
-
+  "PLR2004",
+  
   # need cleanup
   "ARG001",
   "ANN001",
   "ANN002",
   "ANN003",
   "ANN101",
   "ANN201",
```

### Comparing `paraview_trame_components-0.3.0/PKG-INFO` & `paraview_trame_components-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: paraview-trame-components
-Version: 0.3.0
+Version: 0.4.0
 Summary: Macro components for ParaView
 Author-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 Maintainer-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 License: Copyright 2024 Kitware Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -52,24 +52,24 @@
 
 ```bash
 # Create and activate venv
 python3.10 -m venv .venv
 source .venv/bin/activate
 
 # Install published package
-pip install ptc
+pip install paraview-trame-components
 
 # Let ParaView know about the location of that venv
 export PV_VENV=$PWD/.venv
 ```
 
 ## Running examples
 
 ```bash
-# Adjust path to point to your executable
+# Adjust path to point to your ParaView executable
 export PVPYTHON=/Applications/ParaView-5.12.0.app/Contents/bin/pvpython
 
 # Run the scripts
 $PVPYTHON --force-offscreen-rendering ./examples/cone.py
 $PVPYTHON --force-offscreen-rendering ./examples/cone_width_slider.py
 $PVPYTHON --force-offscreen-rendering ./examples/wavelet-contour-state.py
 $PVPYTHON --force-offscreen-rendering ./examples/pipeline.py
```

