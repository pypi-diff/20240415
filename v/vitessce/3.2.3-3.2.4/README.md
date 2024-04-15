# Comparing `tmp/vitessce-3.2.3.tar.gz` & `tmp/vitessce-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitessce-3.2.3.tar", last modified: Thu Feb 29 19:23:39 2024, max compression
+gzip compressed data, was "vitessce-3.2.4.tar", last modified: Mon Apr 15 16:14:25 2024, max compression
```

## Comparing `vitessce-3.2.3.tar` & `vitessce-3.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:23:39.262063 vitessce-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-29 19:21:47.000000 vitessce-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-29 19:21:47.000000 vitessce-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-02-29 19:23:39.262063 vitessce-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-02-29 19:21:47.000000 vitessce-3.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-29 19:21:47.000000 vitessce-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-29 19:23:39.262063 vitessce-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 19:21:47.000000 vitessce-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:23:39.254063 vitessce-3.2.3/vitessce/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75366 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/config_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:23:39.258063 vitessce-3.2.3/vitessce/data_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/data_utils/anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/data_utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/data_utils/multivec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/data_utils/ome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20415 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    53729 2024-02-29 19:21:47.000000 vitessce-3.2.3/vitessce/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:23:39.258063 vitessce-3.2.3/vitessce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-02-29 19:23:39.000000 vitessce-3.2.3/vitessce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-29 19:23:39.000000 vitessce-3.2.3/vitessce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 19:23:39.000000 vitessce-3.2.3/vitessce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-29 19:23:39.000000 vitessce-3.2.3/vitessce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-29 19:23:39.000000 vitessce-3.2.3/vitessce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.962208 vitessce-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:12:24.000000 vitessce-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 16:12:24.000000 vitessce-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-15 16:14:25.962208 vitessce-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-15 16:12:24.000000 vitessce-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-15 16:12:24.000000 vitessce-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 16:14:25.962208 vitessce-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:12:24.000000 vitessce-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.954208 vitessce-3.2.4/vitessce/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75366 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.958208 vitessce-3.2.4/vitessce/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/multivec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/ome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53910 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.958208 vitessce-3.2.4/vitessce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/top_level.txt
```

### Comparing `vitessce-3.2.3/LICENSE` & `vitessce-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/PKG-INFO` & `vitessce-3.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.3
+Version: 3.2.4
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,19 +42,20 @@
 Requires-Dist: zarr>=2.5.0
 Requires-Dist: numcodecs>=0.5.7
 Requires-Dist: scipy>=1.2.1
 Requires-Dist: negspy>=0.2.24
 Requires-Dist: pandas>=1.1.2
 Requires-Dist: black>=21.11b1
 Requires-Dist: numpy>=1.21.2
-Requires-Dist: anndata<0.9,>=0.7.8
+Requires-Dist: anndata<0.11,>=0.7.8
 Requires-Dist: scanpy>=1.9.3
 Requires-Dist: ome-zarr==0.8.3
 Requires-Dist: tifffile>=2020.10.1
 Requires-Dist: jsonschema>=3.2
+Requires-Dist: tqdm>=4.1.0
 Provides-Extra: dev
 Requires-Dist: build==0.1.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: loompy>=3.0.6; extra == "dev"
 Requires-Dist: coverage>=6.3.2; extra == "dev"
 Requires-Dist: flake8==3.8.4; extra == "dev"
 Provides-Extra: docs
@@ -69,15 +70,15 @@
 Requires-Dist: nbsphinx==0.8.8; extra == "docs"
 Requires-Dist: nbclean==0.3.2; extra == "docs"
 Requires-Dist: sqlalchemy==1.3.24; extra == "docs"
 Requires-Dist: nbconvert==5.6.1; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Provides-Extra: all
 Requires-Dist: jupyter-server-proxy>=1.5.2; extra == "all"
-Requires-Dist: anywidget==0.4.2; extra == "all"
+Requires-Dist: anywidget>=0.9.3; extra == "all"
 Requires-Dist: uvicorn>=0.17.0; extra == "all"
 Requires-Dist: ujson>=4.0.1; extra == "all"
 Requires-Dist: starlette==0.14.0; extra == "all"
 Requires-Dist: generate-tiff-offsets>=0.1.7; extra == "all"
 Requires-Dist: aiofiles>=0.6.0; extra == "all"
 Provides-Extra: building
 Provides-Extra: testing
```

### Comparing `vitessce-3.2.3/README.md` & `vitessce-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/pyproject.toml` & `vitessce-3.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel>=0.38.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vitessce"
-version = "3.2.3"
+version = "3.2.4"
 authors = [
   { name="Mark Keller", email="mark_keller@hms.harvard.edu" },
 ]
 description = "Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -28,19 +28,20 @@
   'zarr>=2.5.0',
   'numcodecs>=0.5.7',
   'scipy>=1.2.1',
   'negspy>=0.2.24',
   'pandas>=1.1.2',
   'black>=21.11b1',
   'numpy>=1.21.2',
-  'anndata>=0.7.8,<0.9',
+  'anndata>=0.7.8,<0.11',
   'scanpy>=1.9.3',
   'ome-zarr==0.8.3',
   'tifffile>=2020.10.1',
-  'jsonschema>=3.2'
+  'jsonschema>=3.2',
+  'tqdm>=4.1.0'
 ]
 
 [project.optional-dependencies]
 dev = [
   'build==0.1.0',
   'pytest>=6.2.4',
   'loompy>=3.0.6',
@@ -68,15 +69,15 @@
   # nbconvert and jinja2 versions need to be pinned.
   # Reference: https://github.com/vitessce/vitessce-python/issues/152
   'nbconvert==5.6.1',
   'jinja2==3.0.3',
 ]
 all = [
   'jupyter-server-proxy>=1.5.2',
-  'anywidget==0.4.2',
+  'anywidget>=0.9.3',
   'uvicorn>=0.17.0',
   'ujson>=4.0.1',
   'starlette==0.14.0',
   'generate-tiff-offsets>=0.1.7',
 
   # aiofiles is not explicitly referenced in our code,
   # but it is an implicit dependency of starlette==0.14.0.
```

### Comparing `vitessce-3.2.3/setup.cfg` & `vitessce-3.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/__init__.py` & `vitessce-3.2.4/vitessce/__init__.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/config.py` & `vitessce-3.2.4/vitessce/config.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/config_converter.py` & `vitessce-3.2.4/vitessce/config_converter.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/constants.py` & `vitessce-3.2.4/vitessce/constants.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/data_utils/anndata.py` & `vitessce-3.2.4/vitessce/data_utils/anndata.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/data_utils/entities.py` & `vitessce-3.2.4/vitessce/data_utils/entities.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/data_utils/multivec.py` & `vitessce-3.2.4/vitessce/data_utils/multivec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,49 @@
 import math
 import zarr
 import numpy as np
 import pandas as pd
+from tqdm import tqdm
 
 from .anndata import to_dense
 from .entities import GenomicProfiles
 
 
-def adata_to_multivec_zarr(adata, output_path, obs_set_col, obs_set_name, obs_set_vals=None, var_interval_col="interval", layer_key=None, assembly="hg38", starting_resolution=5000):
+def adata_to_multivec_zarr(adata, output_path, obs_set_col, obs_set_name, obs_set_vals=None, var_interval_col="interval", layer_key=None, assembly="hg38", starting_resolution=5000, chr_subset=None):
+    """
+    Convert an AnnData object containing a cell-by-bin matrix to a Multivec-Zarr store.
+
+    :param adata: The object to convert.
+    :type adata: anndata.AnnData
+    :param output_path: The path to the output Zarr store.
+    :type output_path: str
+    :param obs_set_col: The name of the column in adata.obs that contains the cluster IDs.
+    :type obs_set_col: str
+    :param obs_set_name: The name of the cluster set.
+    :type obs_set_name: str
+    :param obs_set_vals: The cluster IDs to include in the output. If None, all cluster IDs will be included. This can be used to override the order of the cluster IDs.
+    :type obs_set_vals: list[str] or None
+    :param var_interval_col: The name of the column in adata.var that contains the bin interval strings. By default, "interval".
+    :type var_interval_col: str
+    :param layer_key: The name of the layer in adata.layers to use. If None, adata.X will be used. By default, None.
+    :type layer_key: str or None
+    :param assembly: The name of the genome assembly. By default, "hg38".
+    :type assembly: str
+    :param starting_resolution: The starting resolution of the data. By default, 5000.
+    :type starting_resolution: int
+    :param chr_subset: For debugging purposes, a subset of chromosomes to process. If None, all chromosomes in the assembly will be processed. By default, None.
+    :type chr_subset: list[str] or None
+    """
     in_mtx = adata.layers[layer_key] if layer_key is not None else adata.X
     in_barcodes_df = adata.obs
     in_bins_df = adata.var
 
+    # Ensure that in_bins_df has a sequential integer index
+    in_bins_df = in_bins_df.reset_index()
+
     in_mtx = to_dense(in_mtx)  # TODO: is this necessary?
 
     # The bin datafram consists of one column like chrName:binStart-binEnd
     def convert_bin_name_to_chr_name(bin_name):
         try:
             return bin_name[:bin_name.index(':')]
         except ValueError:
@@ -80,28 +108,34 @@
     out_f = zarr.open(output_path, mode='w')
 
     genomic_profiles = GenomicProfiles(
         out_f, profile_paths=cluster_paths, assembly=assembly, starting_resolution=starting_resolution
     )
     chrom_name_to_length = genomic_profiles.chrom_name_to_length
 
+    # For debugging purposes, allow the user to specify a subset of chromosomes to process.
+    chrom_names = chr_subset if chr_subset is not None else list(chrom_name_to_length.keys())
+
     # Create each chromosome dataset.
-    for chr_name, chr_len in chrom_name_to_length.items():
+    for chr_name in tqdm(chrom_names):
+        chr_len = chrom_name_to_length[chr_name]
         # The bins dataframe frustratingly does not contain every bin.
         # We need to figure out which bins are missing.
 
         # We want to check for missing bins in each chromosome separately,
         # otherwise too much memory is used during the join step.
         chr_bins_in_df = in_bins_df.loc[in_bins_df["chr_name"] == chr_name]
         if chr_bins_in_df.shape[0] == 0:
+            print("Warning: No bins found for chromosome", chr_name)
             # No processing or output is necessary if there is no data for this chromosome.
             # Continue on through all resolutions of this chromosome to the next chromosome.
             continue
         # Determine the indices of the matrix at which the bins for this chromosome start and end.
         chr_bin_i_start = int(chr_bins_in_df.head(1).iloc[0].name)
+        # +1 because the end index is exclusive.
         chr_bin_i_end = int(chr_bins_in_df.tail(1).iloc[0].name) + 1
 
         # Extract the part of the matrix corresponding to the current chromosome.
         chr_mtx = in_mtx[:, chr_bin_i_start:chr_bin_i_end]
 
         # Create a list of the "ground truth" bins (all bins from position 0 to the end of the chromosome).
         # We will join the input bins onto this dataframe to determine which bins are missing.
```

### Comparing `vitessce-3.2.3/vitessce/data_utils/ome.py` & `vitessce-3.2.4/vitessce/data_utils/ome.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/export.py` & `vitessce-3.2.4/vitessce/export.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/repr.py` & `vitessce-3.2.4/vitessce/repr.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/routes.py` & `vitessce-3.2.4/vitessce/routes.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/utils.py` & `vitessce-3.2.4/vitessce/utils.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce/widget.py` & `vitessce-3.2.4/vitessce/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         ...f,
         url: `${origin}${baseUrl}${f.url}`,
       })),
     })),
   };
 }
 
-export async function render(view) {
+async function render(view) {
     const cssUid = view.model.get('uid');
     const jsDevMode = view.model.get('js_dev_mode');
     const jsPackageVersion = view.model.get('js_package_version');
     const customJsUrl = view.model.get('custom_js_url');
     const pluginEsm = view.model.get('plugin_esm');
     const remountOnUidChange = view.model.get('remount_on_uid_change');
 
@@ -335,14 +335,15 @@
         // Clean up React and DOM state.
         root.unmount();
         if(view._isFromDisplay) {
             view.el.remove();
         }
     };
 }
+export default { render };
 """
 
 DEFAULT_PLUGIN_ESM = """
 function createPlugins(utilsForPlugins) {
     const {
         React,
         PluginFileType,
@@ -378,21 +379,21 @@
     theme = Unicode('auto').tag(sync=True)
     proxy = Bool(False).tag(sync=True)
     uid = Unicode('').tag(sync=True)
     has_host_name = Bool(False).tag(sync=True)
 
     next_port = DEFAULT_PORT
 
-    js_package_version = Unicode('3.3.6').tag(sync=True)
+    js_package_version = Unicode('3.3.7').tag(sync=True)
     js_dev_mode = Bool(False).tag(sync=True)
     custom_js_url = Unicode('').tag(sync=True)
     plugin_esm = Unicode(DEFAULT_PLUGIN_ESM).tag(sync=True)
     remount_on_uid_change = Bool(True).tag(sync=True)
 
-    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='3.3.6', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
+    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='3.3.7', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
         """
         Construct a new Vitessce widget.
 
         :param config: A view config instance.
         :type config: VitessceConfig
         :param str theme: The theme name, either "light" or "dark". By default, "auto", which selects light or dark based on operating system preferences.
         :param int height: The height of the widget, in pixels. By default, 600.
@@ -458,15 +459,15 @@
     def close(self):
         self.config_obj.stop_server(self.port)
         super().close()
 
 # Launch Vitessce using plain HTML representation (no ipywidgets)
 
 
-def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='3.3.6', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
+def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='3.3.7', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
     from IPython.display import display, HTML
     uid_str = "vitessce" + get_uid_str(uid)
 
     base_url, use_port, _ = get_base_url_and_port(
         port, DEFAULT_PORT, proxy=proxy, base_url=base_url, host_name=host_name)
     config_dict = config.to_dict(base_url=base_url)
     routes = config.get_routes()
```

### Comparing `vitessce-3.2.3/vitessce/wrappers.py` & `vitessce-3.2.4/vitessce/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,23 @@
     """
 
     def __init__(self, **kwargs):
         """
         Abstract constructor to be inherited by dataset wrapper classes.
 
         :param str out_dir: The path to a local directory used for data processing outputs. By default, uses a temp. directory.
+        :param dict request_init: options to be passed along with every fetch request from the browser, like `{ "header": { "Authorization": "Bearer dsfjalsdfa1431" } }`
         """
         self.out_dir = kwargs['out_dir'] if 'out_dir' in kwargs else tempfile.mkdtemp(
         )
         self.routes = []
         self.is_remote = False
         self.file_def_creators = []
         self.base_dir = None
+        self._request_init = kwargs['request_init'] if 'request_init' in kwargs else None
 
     def __repr__(self):
         return self._repr
 
     def convert_and_save(self, dataset_uid, obj_i, base_dir=None):
         """
         Fill in the file_def_creators array.
@@ -890,15 +892,15 @@
                 file_def["coordinationValues"] = self._coordination_values
             return file_def
 
         return image_file_def_creator
 
 
 class AnnDataWrapper(AbstractWrapper):
-    def __init__(self, adata_path=None, adata_url=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, obs_spots_path=None, obs_points_path=None, request_init=None, feature_labels_path=None, obs_labels_path=None, convert_to_dense=True, coordination_values=None, obs_labels_paths=None, obs_labels_names=None, **kwargs):
+    def __init__(self, adata_path=None, adata_url=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, obs_spots_path=None, obs_points_path=None, feature_labels_path=None, obs_labels_path=None, convert_to_dense=True, coordination_values=None, obs_labels_paths=None, obs_labels_names=None, **kwargs):
         """
         Wrap an AnnData object by creating an instance of the ``AnnDataWrapper`` class.
 
         :param str adata_path: A path to an AnnData object written to a Zarr store containing single-cell experiment data.
         :param str adata_url: A remote url pointing to a zarr-backed AnnData store.
         :param str obs_feature_matrix_path: Location of the expression (cell x gene) matrix, like `X` or `obsm/highly_variable_genes_subset`
         :param str feature_filter_path: A string like `var/highly_variable` used in conjunction with `obs_feature_matrix_path` if obs_feature_matrix_path points to a subset of `X` of the full `var` list.
@@ -908,15 +910,14 @@
         :param str obs_locations_path: Column name in `obsm` that contains centroid coordinates for displaying centroids in the spatial viewer
         :param str obs_segmentations_path: Column name in `obsm` that contains polygonal coordinates for displaying outlines in the spatial viewer
         :param list[str] obs_embedding_paths: Column names like `['obsm/X_umap', 'obsm/X_pca']` for showing scatterplots
         :param list[str] obs_embedding_names: Overriding names like `['UMAP', 'PCA']` for displaying above scatterplots
         :param list[str] obs_embedding_dims: Dimensions along which to get data for the scatterplot, like `[[0, 1], [4, 5]]` where `[0, 1]` is just the normal x and y but `[4, 5]` could be comparing the third and fourth principal components, for example.
         :param str obs_spots_path: Column name in `obsm` that contains centroid coordinates for displaying spots in the spatial viewer
         :param str obs_points_path: Column name in `obsm` that contains centroid coordinates for displaying points in the spatial viewer
-        :param dict request_init: options to be passed along with every fetch request from the browser, like `{ "header": { "Authorization": "Bearer dsfjalsdfa1431" } }`
         :param str feature_labels_path: The name of a column containing feature labels (e.g., alternate gene symbols), instead of the default index in `var` of the AnnData store.
         :param str obs_labels_path: (DEPRECATED) The name of a column containing observation labels (e.g., alternate cell IDs), instead of the default index in `obs` of the AnnData store. Use `obs_labels_paths` and `obs_labels_names` instead. This arg will be removed in a future release.
         :param list[str] obs_labels_paths: The names of columns containing observation labels (e.g., alternate cell IDs), instead of the default index in `obs` of the AnnData store.
         :param list[str] obs_labels_names: The optional display names of columns containing observation labels (e.g., alternate cell IDs), instead of the default index in `obs` of the AnnData store.
         :param bool convert_to_dense: Whether or not to convert `X` to dense the zarr store (dense is faster but takes more disk space).
         :param coordination_values: Coordination values for the file definition.
         :type coordination_values: dict or None
@@ -947,15 +948,14 @@
         self._cell_set_obs = obs_set_paths
         self._spatial_centroid_obsm = obs_locations_path
         self._spatial_polygon_obsm = obs_segmentations_path
         self._mappings_obsm = obs_embedding_paths
         self._mappings_obsm_dims = obs_embedding_dims
         self._spatial_spots_obsm = obs_spots_path
         self._spatial_points_obsm = obs_points_path
-        self._request_init = request_init
         self._gene_alias = feature_labels_path
         # Support legacy provision of single obs labels path
         if (obs_labels_path is not None):
             self._obs_labels_paths = [obs_labels_path]
             self._obs_labels_names = [obs_labels_path.split('/')[-1]]
         else:
             self._obs_labels_paths = obs_labels_paths
@@ -1134,12 +1134,15 @@
     def get_zarr_url(self, base_url="", dataset_uid="", obj_i=""):
         if self.is_remote:
             return self._zarr_url
         return self.get_local_dir_url(base_url, dataset_uid, obj_i, self._zarr_path, self.local_dir_uid)
 
     def make_genomic_profiles_file_def_creator(self, dataset_uid, obj_i):
         def genomic_profiles_file_def_creator(base_url):
-            return {
+            obj_file_def = {
                 "fileType": "genomic-profiles.zarr",
                 "url": self.get_zarr_url(base_url, dataset_uid, obj_i)
             }
+            if self._request_init is not None:
+                obj_file_def['requestInit'] = self._request_init
+            return obj_file_def
         return genomic_profiles_file_def_creator
```

### Comparing `vitessce-3.2.3/vitessce.egg-info/PKG-INFO` & `vitessce-3.2.4/vitessce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.3
+Version: 3.2.4
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,19 +42,20 @@
 Requires-Dist: zarr>=2.5.0
 Requires-Dist: numcodecs>=0.5.7
 Requires-Dist: scipy>=1.2.1
 Requires-Dist: negspy>=0.2.24
 Requires-Dist: pandas>=1.1.2
 Requires-Dist: black>=21.11b1
 Requires-Dist: numpy>=1.21.2
-Requires-Dist: anndata<0.9,>=0.7.8
+Requires-Dist: anndata<0.11,>=0.7.8
 Requires-Dist: scanpy>=1.9.3
 Requires-Dist: ome-zarr==0.8.3
 Requires-Dist: tifffile>=2020.10.1
 Requires-Dist: jsonschema>=3.2
+Requires-Dist: tqdm>=4.1.0
 Provides-Extra: dev
 Requires-Dist: build==0.1.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: loompy>=3.0.6; extra == "dev"
 Requires-Dist: coverage>=6.3.2; extra == "dev"
 Requires-Dist: flake8==3.8.4; extra == "dev"
 Provides-Extra: docs
@@ -69,15 +70,15 @@
 Requires-Dist: nbsphinx==0.8.8; extra == "docs"
 Requires-Dist: nbclean==0.3.2; extra == "docs"
 Requires-Dist: sqlalchemy==1.3.24; extra == "docs"
 Requires-Dist: nbconvert==5.6.1; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Provides-Extra: all
 Requires-Dist: jupyter-server-proxy>=1.5.2; extra == "all"
-Requires-Dist: anywidget==0.4.2; extra == "all"
+Requires-Dist: anywidget>=0.9.3; extra == "all"
 Requires-Dist: uvicorn>=0.17.0; extra == "all"
 Requires-Dist: ujson>=4.0.1; extra == "all"
 Requires-Dist: starlette==0.14.0; extra == "all"
 Requires-Dist: generate-tiff-offsets>=0.1.7; extra == "all"
 Requires-Dist: aiofiles>=0.6.0; extra == "all"
 Provides-Extra: building
 Provides-Extra: testing
```

### Comparing `vitessce-3.2.3/vitessce.egg-info/SOURCES.txt` & `vitessce-3.2.4/vitessce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.3/vitessce.egg-info/requires.txt` & `vitessce-3.2.4/vitessce.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 zarr>=2.5.0
 numcodecs>=0.5.7
 scipy>=1.2.1
 negspy>=0.2.24
 pandas>=1.1.2
 black>=21.11b1
 numpy>=1.21.2
-anndata<0.9,>=0.7.8
+anndata<0.11,>=0.7.8
 scanpy>=1.9.3
 ome-zarr==0.8.3
 tifffile>=2020.10.1
 jsonschema>=3.2
+tqdm>=4.1.0
 
 [all]
 jupyter-server-proxy>=1.5.2
-anywidget==0.4.2
+anywidget>=0.9.3
 uvicorn>=0.17.0
 ujson>=4.0.1
 starlette==0.14.0
 generate-tiff-offsets>=0.1.7
 aiofiles>=0.6.0
 
 [building]
```

