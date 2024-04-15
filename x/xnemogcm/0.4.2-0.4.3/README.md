# Comparing `tmp/xnemogcm-0.4.2.tar.gz` & `tmp/xnemogcm-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnemogcm-0.4.2.tar", max compression
+gzip compressed data, was "xnemogcm-0.4.3.tar", max compression
```

## Comparing `xnemogcm-0.4.2.tar` & `xnemogcm-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-08-07 10:10:50.714835 xnemogcm-0.4.2/LICENSE
--rw-r--r--   0        0        0     4097 2023-08-07 10:10:50.714835 xnemogcm-0.4.2/README.md
--rw-r--r--   0        0        0      982 2023-08-07 10:10:50.718835 xnemogcm-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      242 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/__init__.py
--rw-r--r--   0        0        0     1300 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/arakawa_points.py
--rw-r--r--   0        0        0     7473 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/domcfg.py
--rw-r--r--   0        0        0     4454 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/merge.py
--rw-r--r--   0        0        0     4520 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/metrics.py
--rw-r--r--   0        0        0     1112 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/namelist.py
--rw-r--r--   0        0        0     8852 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/nemo.py
--rw-r--r--   0        0        0      468 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/test/conftest.py
--rw-r--r--   0        0        0     1195 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_dask.py
--rw-r--r--   0        0        0     4148 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_domcfg.py
--rw-r--r--   0        0        0     1856 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_merge.py
--rw-r--r--   0        0        0     2316 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_metrics.py
--rw-r--r--   0        0        0     1198 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_namelist.py
--rw-r--r--   0        0        0     5317 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_nemo.py
--rw-r--r--   0        0        0      764 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_surface.py
--rw-r--r--   0        0        0      461 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_version.py
--rw-r--r--   0        0        0     3361 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/tools.py
--rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 xnemogcm-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-15 12:48:39.347794 xnemogcm-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2735 2024-04-15 12:48:39.347794 xnemogcm-0.4.3/README.md
+-rw-r--r--   0        0        0     1241 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/__init__.py
+-rw-r--r--   0        0        0     1357 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/arakawa_points.py
+-rw-r--r--   0        0        0     7448 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/domcfg.py
+-rw-r--r--   0        0        0     4454 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/merge.py
+-rw-r--r--   0        0        0     4544 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/metrics.py
+-rw-r--r--   0        0        0     1094 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/namelist.py
+-rw-r--r--   0        0        0     8782 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/nemo.py
+-rw-r--r--   0        0        0      468 2024-04-15 12:48:39.351794 xnemogcm-0.4.3/xnemogcm/test/conftest.py
+-rw-r--r--   0        0        0     1195 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_dask.py
+-rw-r--r--   0        0        0     4148 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_domcfg.py
+-rw-r--r--   0        0        0     1856 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_merge.py
+-rw-r--r--   0        0        0     2316 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_metrics.py
+-rw-r--r--   0        0        0     1198 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_namelist.py
+-rw-r--r--   0        0        0     5317 2024-04-15 12:48:39.363794 xnemogcm-0.4.3/xnemogcm/test/test_nemo.py
+-rw-r--r--   0        0        0      764 2024-04-15 12:48:39.367794 xnemogcm-0.4.3/xnemogcm/test/test_surface.py
+-rw-r--r--   0        0        0      461 2024-04-15 12:48:39.367794 xnemogcm-0.4.3/xnemogcm/test/test_version.py
+-rw-r--r--   0        0        0     3361 2024-04-15 12:48:39.367794 xnemogcm-0.4.3/xnemogcm/tools.py
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 xnemogcm-0.4.3/PKG-INFO
```

### Comparing `xnemogcm-0.4.2/LICENSE` & `xnemogcm-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/pyproject.toml` & `xnemogcm-0.4.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "xnemogcm"
-version = "0.4.2"
+version = "0.4.3"
 description = "Interface to open NEMO global circulation model output dataset and create a xgcm grid."
 license = "MIT"
 homepage = "https://github.com/rcaneill/xnemogcm"
-authors = ["Romain Caneill <romain.caneill@gu.se>"]
+authors = ["Romain Caneill <romain.caneill@ens-lyon.org>"]
 readme = "README.md"
 exclude = ["xnemogcm/test/data"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9"
 dask = {extras = ["array"], version = "*"}
 netcdf4 = ">=1.5.8"
 xarray = ">=0.21.1"
 xgcm = {optional = true, version = ">=0.6.0"}
 f90nml = {optional = true, version = ">=1.3.1"}
+pre-commit = {optional = true, version = "^3.6.2"}
 
 [tool.poetry.extras]
 namelist = ["f90nml"]
 metrics = ["xgcm"]
 
 [tool.poetry.group.test]
 optional = true
@@ -31,11 +32,22 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 jupyterlab = ">=3.5.1"
+pre-commit = "^3.6.2"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.3"
+mkdocs-jupyter = "^0.24.6"
+mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core>=1",
+]
```

### Comparing `xnemogcm-0.4.2/xnemogcm/arakawa_points.py` & `xnemogcm-0.4.3/xnemogcm/arakawa_points.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Needs to start with variables that have 2 letters for regex
 ALL_POINTS = ["UW", "VW", "FW", "T", "U", "V", "F", "W"]
 
 
 class Point:
     """
-    Point types
-
-    TODO
+    Class that represents the Arakawa points (i.e. center point, face, edge, etc).
     """
 
     def __init__(self, point_type):
         """
         point_type : 'T', 'U', 'V', 'F', 'W', 'UW', 'VW', 'FW'
         """
         if point_type not in ALL_POINTS:
```

### Comparing `xnemogcm-0.4.2/xnemogcm/domcfg.py` & `xnemogcm-0.4.3/xnemogcm/domcfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pathlib import Path
 import numpy as np
 import xarray as xr
 
 from . import arakawa_points as akp
 from .tools import get_domcfg_points, _dir_or_files_to_files
 
 
@@ -45,15 +44,15 @@
         (x0, y0) = ds.attrs["DOMAIN_position_first"]
         ds = ds.assign_coords({"x": ds.x + x0 - 1, "y": ds.y + y0 - 1})
     else:
         # This means that we are not merging multiple outputs from processors but e.g. a domain_cfg and a mesh_mask
         ds.coords["x"] = ds.x
         ds.coords["y"] = ds.y
     # We need to add "nav_lev" in the coordinates if not present
-    if (not "nav_lev" in ds.coords) and ("nav_lev" in ds):
+    if ("nav_lev" not in ds.coords) and ("nav_lev" in ds):
         ds.coords["nav_lev"] = ds["nav_lev"]
     return ds
 
 
 def open_file_multi(files):
     """
     Open and merge netcdf file created on each processor by NEMO (e.g. domain_cfg of mesh_mask).
```

### Comparing `xnemogcm-0.4.2/xnemogcm/merge.py` & `xnemogcm-0.4.3/xnemogcm/merge.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/metrics.py` & `xnemogcm-0.4.3/xnemogcm/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,24 @@
         "e3uw": {"e3w": ["X"]},
         "e3vw": {"e3w": ["Y"]},
         "e3fw": {"e3w": ["X", "Y"]},
     }
 )
 
 
-def compute_missing_metrics(
-    ds, all_scale_factors=all_scale_factors, time_varying=True, periodic=False
-):
+def compute_missing_metrics(ds, all_scale_factors=all_scale_factors, time_varying=True):
     """
     Add all possible scale factors to the dataset.
 
     For the moment, e3t (or e3t_0) at least needs to be present in the dataset
     for the time_varying=True (time_varying=False) case.
     If e3t_0 is not found (e.g. for nemo 3.6), it will raise a warning and use e3t_1d
     (this will lead to wrong results if terrain-following coordinates are used).
 
-    May have some boundary issues.
+    May have some boundary issues, and only non-periodic boundaries are implemented.
 
     Will add the metrics to the given dataset. To avoid this, use a ds.copy()
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset containing the scale factors. Must be xgcm compatible (e.g. opened with xnemogcm)
@@ -50,15 +48,15 @@
 
     Returns
     -------
     the new dataset with the scale factors added
     """
     try:
         import xgcm
-    except ModuleNotFoundError as e:
+    except ModuleNotFoundError:
         raise ModuleNotFoundError(
             "xgcm is not installed, you need xgcm for this function"
         )
     from warnings import warn
 
     warn(
         "This function is in pre-phase. Do not expect a high precision, but a good estimate. Some boundary issues may arise."
@@ -108,15 +106,15 @@
 
     Parameters
     ----------
     ds : xarray.Dataset
         domain_cfg
         or DataSet returned by xnemogcm._merge_nemo_and_domain_cfg
         or Dataset returned by xnemogcm.open_nemo_and_domain_cfg
-        Should contain the outputed metrics, in a standard format 'e3x'
+        Should contain the outputted metrics, in a standard format 'e3x'
         with x an arakawa point in lower case
 
     Returns
     -------
     metrics : dict
         dict understood by xgcm.Grid, metrics argument
     """
```

### Comparing `xnemogcm-0.4.2/xnemogcm/namelist.py` & `xnemogcm-0.4.3/xnemogcm/namelist.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,21 @@
     files = _dir_or_files_to_files(datadir, files, patterns=["namelist*"])
 
     if len(files) > 2:
         raise ValueError(
             f"Too many files given for the namelists, please check. Got {files}"
         )
 
-    namcfg = {}
-    namref = {}
     ds = xr.Dataset()
 
-    for (load, name) in [[ref, "ref"], [cfg, "cfg"]]:
+    for load, name in [[ref, "ref"], [cfg, "cfg"]]:
         if load:
             try:
                 namelist = f90nml.read(*[i for i in files if name in str(i)])
-                for nam in namelist.keys():
-                    for i in namelist[nam]:
-                        ds[i] = namelist[nam][i]
-                        ds[i].attrs["namelist"] = nam
+                for nam_key in namelist.keys():
+                    for i in namelist[nam_key]:
+                        ds[i] = namelist[nam_key][i]
+                        ds[i].attrs["namelist"] = nam_key
             except (FileNotFoundError, TypeError):
                 _warn_namelist_not_found(name)
 
     return ds
```

### Comparing `xnemogcm-0.4.2/xnemogcm/nemo.py` & `xnemogcm-0.4.3/xnemogcm/nemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from functools import partial
 import re
-from pathlib import Path
 import xarray as xr
 
 from . import arakawa_points as akp
 from .tools import _dir_or_files_to_files
 
 
 def _get_point_type(filename, description):
     """
     Infers point type from filename and/or description
     """
     point_type_fn = None
     point_type_desc = None
 
     # Try with filename
-    all_points_str = a = "|".join(akp.ALL_POINTS)
+    a = "|".join(akp.ALL_POINTS)
     m = re.search(f"grid_({a})", filename)
     if m:
         point_type_fn = m.groups()[0]
 
     # try with description
     m = re.search(f"ocean ({a}) grid", description)
     if m:
@@ -161,15 +159,15 @@
         the domcfg dataset
     parallel : bool, default False
         whether to use dask.delayed to process tasks in parallel
 
     Returns
     -------
     nemo_ds : xarray.Dataset
-        Dataset containing all outputed variables, set on the proper
+        Dataset containing all outputted variables, set on the proper
         grid points (center, face, etc).
     """
     if parallel:
         import dask
 
         # wrap preprocess with delayed
         preprocess = dask.delayed(nemo_preprocess)
@@ -222,15 +220,15 @@
         i.e. 'time_counter', 'x', etc
         For more complex chunking, you may want to open without any chunks and set them up afterward.
     kwargs_open : any other argument given to the xarray.open_dataset function
 
     Returns
     -------
     nemo_ds : xarray.Dataset
-        Dataset containing all outputed variables, set on the proper
+        Dataset containing all outputted variables, set on the proper
         grid points (center, face, etc).
     """
     files = _dir_or_files_to_files(datadir, files, patterns=["*grid_*.nc"])
     if not files:
         raise FileNotFoundError("No output files are provided")
     #
     if parallel:
```

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_dask.py` & `xnemogcm-0.4.3/xnemogcm/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_domcfg.py` & `xnemogcm-0.4.3/xnemogcm/test/test_domcfg.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_merge.py` & `xnemogcm-0.4.3/xnemogcm/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_metrics.py` & `xnemogcm-0.4.3/xnemogcm/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_namelist.py` & `xnemogcm-0.4.3/xnemogcm/test/test_namelist.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_nemo.py` & `xnemogcm-0.4.3/xnemogcm/test/test_nemo.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/test/test_surface.py` & `xnemogcm-0.4.3/xnemogcm/test/test_surface.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.2/xnemogcm/tools.py` & `xnemogcm-0.4.3/xnemogcm/tools.py`

 * *Files identical despite different names*

