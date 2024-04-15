# Comparing `tmp/napari-tomotwin-0.4.0b3.tar.gz` & `tmp/napari-tomotwin-0.4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomotwin-0.4.0b3.tar", last modified: Thu Jan 25 08:54:48 2024, max compression
+gzip compressed data, was "napari-tomotwin-0.4.0b4.tar", last modified: Wed Mar  6 14:17:04 2024, max compression
```

## Comparing `napari-tomotwin-0.4.0b3.tar` & `napari-tomotwin-0.4.0b4.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.594673 napari-tomotwin-0.4.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.586673 napari-tomotwin-0.4.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-25 08:54:48.594673 napari-tomotwin-0.4.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/conda_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/notebooks/test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-25 08:54:48.594673 napari-tomotwin-0.4.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/src/napari_tomotwin/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.590673 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_qt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_qt/labeled_progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.594673 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/test_load_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/test_make_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/anchor_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/load_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/make_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin/umap_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:54:48.594673 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-25 08:54:48.000000 napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-25 08:54:32.000000 napari-tomotwin-0.4.0b3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.155358 napari-tomotwin-0.4.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.159358 napari-tomotwin-0.4.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.159358 napari-tomotwin-0.4.0b4/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/conda_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.159358 napari-tomotwin-0.4.0b4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/notebooks/test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.159358 napari-tomotwin-0.4.0b4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.159358 napari-tomotwin-0.4.0b4/src/napari_tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_qt/labeled_progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/test_load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/test_make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/anchor_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/cluster_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/load_umap_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/target_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin/umap_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:17:04.163359 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 14:17:04.000000 napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-06 14:16:52.000000 napari-tomotwin-0.4.0b4/tox.ini
```

### Comparing `napari-tomotwin-0.4.0b3/.github/workflows/test_and_deploy.yml` & `napari-tomotwin-0.4.0b4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/.gitignore` & `napari-tomotwin-0.4.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/.napari-hub/config.yml` & `napari-tomotwin-0.4.0b4/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/.pre-commit-config.yaml` & `napari-tomotwin-0.4.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/LICENSE` & `napari-tomotwin-0.4.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/PKG-INFO` & `napari-tomotwin-0.4.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.4.0b3
+Version: 0.4.0b4
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.4.0b3/README.md` & `napari-tomotwin-0.4.0b4/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/notebooks/test.ipynb` & `napari-tomotwin-0.4.0b4/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/setup.cfg` & `napari-tomotwin-0.4.0b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/test_load_umap.py` & `napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/test_load_umap.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             umap_df.attrs['embeddings_attrs'] = {
                 "stride": (1,1,1),
                 "tomogram_input_shape": (100,100,100)
             }
             umap_df.attrs['embeddings_path'] = ""
             umap_df.to_pickle(f"{tmpdirname}/umap.tumap")
 
-            widget, _ = viewer.window.add_plugin_dock_widget('napari-tomotwin', widget_name='Cluster UMAP embeddings')
+            widget, _ = viewer.window.add_plugin_dock_widget('napari-tomotwin', widget_name='TomoTwin clustering workflow')
             lyr = tool.load_umap(filename=f"{tmpdirname}/umap.tumap")
             viewer.add_layer(lyr)
 
             assert True # just make sure that now exception is raised
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `napari-tomotwin-0.4.0b3/src/napari_tomotwin/_tests/test_make_targets.py` & `napari-tomotwin-0.4.0b4/src/napari_tomotwin/_tests/test_make_targets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tempfile
 import unittest
 
 import numpy as np
 import pandas as pd
-from napari_tomotwin.make_targets import _run
+from napari_tomotwin.make_targets import _make_targets, _get_medoid_embedding
 
 from glob import glob
 
 class MyTestCase(unittest.TestCase):
     def test_make_targets_single_cluster_medoid(self):
         fake_embedding = {
             "X": [0, 1, 2],
@@ -16,113 +16,68 @@
             "Z": [0, 1, 2],
             "1": [5, 6, 7],
             "2": [5, 6, 7],
             "filepath": ["a.mrc","b.mrc","c.mrc"]
         }
         cluster = pd.Series(np.array([1,1,1]))
         with tempfile.TemporaryDirectory() as tmpdirname:
-            _run(clusters=cluster,
-                 embeddings=pd.DataFrame(fake_embedding),
-                 average_method_name="Medoid",
-                 output_folder=tmpdirname)
-
-            box_data: pd.DataFrame = pd.read_csv(
-                os.path.join(tmpdirname,"cluster_1_medoid.coords"),
-                delim_whitespace=True,
-                index_col=False,
-                header=None,
-                dtype=float,
-                names=["X","Y","Z"]
-            ).astype(np.int32)  # type: ignore
-            self.assertEqual(box_data.iloc[0, 0], 1)
-            self.assertEqual(box_data.iloc[0, 1], 1)
-            self.assertEqual(box_data.iloc[0, 2], 1)
+            _, _, target_locations = _make_targets(embeddings=pd.DataFrame(fake_embedding),
+                          clusters=cluster,
+                          avg_func=_get_medoid_embedding,
+                          target_cluster= None)
+
+
+            self.assertEqual(target_locations[1].iloc[0, 0], 1)
+            self.assertEqual(target_locations[1].iloc[0, 1], 1)
+            self.assertEqual(target_locations[1].iloc[0, 2], 1)
 
     def test_make_targets_two_clusters_medoid(self):
         range(6)
         fake_embedding = {
             "X": [0, 1, 2, 8, 9, 10],
             "Y": [0, 1, 2, 8, 9, 10],
             "Z": [0, 1, 2, 8, 9, 10],
             "1": [-1, 0, 1, -1, 0, 1],
             "2": [1, 1, 1, 2, 2, 2],
         }
         fake_embedding['filepath'] = [f"{i}.mrc" for i in range(len(fake_embedding["X"]))]
         cluster = pd.Series(np.array([1,1,1,2,2,2]))
         with tempfile.TemporaryDirectory() as tmpdirname:
-            _run(clusters=cluster,
-                 embeddings=pd.DataFrame(fake_embedding),
-                 average_method_name="Medoid",
-                 output_folder=tmpdirname)
-
-            box_data: pd.DataFrame = pd.read_csv(
-                os.path.join(tmpdirname,"cluster_1_medoid.coords"),
-                delim_whitespace=True,
-                index_col=False,
-                header=None,
-                dtype=float,
-                names=["X","Y","Z"]
-            ).astype(np.int32)  # type: ignore
+            _, _, target_locations = _make_targets(embeddings=pd.DataFrame(fake_embedding),
+                                                   clusters=cluster,
+                                                   avg_func=_get_medoid_embedding,
+                                                   target_cluster=None)
+
+            box_data: pd.DataFrame = target_locations[1]
             self.assertEqual(box_data.iloc[0, 0], 1)
             self.assertEqual(box_data.iloc[0, 1], 1)
             self.assertEqual(box_data.iloc[0, 2], 1)
 
-            box_data: pd.DataFrame = pd.read_csv(
-                os.path.join(tmpdirname, "cluster_2_medoid.coords"),
-                delim_whitespace=True,
-                index_col=False,
-                header=None,
-                dtype=float,
-                names=["X", "Y", "Z"]
-            ).astype(np.int32)  # type: ignore
+            box_data: pd.DataFrame = target_locations[2]
             self.assertEqual(box_data.iloc[0, 0], 9)
             self.assertEqual(box_data.iloc[0, 1], 9)
             self.assertEqual(box_data.iloc[0, 2], 9)
 
     def test_make_targets_single_cluster_average(self):
         fake_embedding = {
             "X": [0, 1, 2],
             "Y": [0, 1, 2],
             "Z": [0, 1, 2],
             "1": [5, 6, 7],
             "2": [5, 6, 7],
             "filepath": ["a.mrc","b.mrc","c.mrc"]
         }
         cluster = pd.Series(np.array([1,1,1]))
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            _run(clusters=cluster,
-                 embeddings=pd.DataFrame(fake_embedding),
-                 average_method_name="Average",
-                 output_folder=tmpdirname)
-
-            targets_emb: pd.DataFrame = pd.read_pickle(
-                os.path.join(tmpdirname,"cluster_targets.temb"),
-            )
-            self.assertEqual(targets_emb["1"].iloc[0],6)
-            self.assertEqual(targets_emb["2"].iloc[0],6)
+        targets_emb, _, _ = _make_targets(embeddings=pd.DataFrame(fake_embedding),
+                                               clusters=cluster,
+                                               avg_func=_get_medoid_embedding,
+                                               target_cluster=None)
 
-    def test_make_targets_single_cluster_no_coords_written(self):
-        fake_embedding = {
-            "X": [0, 1, 2],
-            "Y": [0, 1, 2],
-            "Z": [0, 1, 2],
-            "1": [5, 6, 7],
-            "2": [5, 6, 7],
-            "filepath": ["a.mrc","b.mrc","c.mrc"]
-        }
-        cluster = pd.Series(np.array([1,1,1]))
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            _run(clusters=cluster,
-                 embeddings=pd.DataFrame(fake_embedding),
-                 average_method_name="Average",
-                 output_folder=tmpdirname)
-
-            r = glob(os.path.join(tmpdirname,"*.coords"))
-            print(r)
-            self.assertEqual(len(r),0)
+        self.assertEqual(targets_emb["1"].iloc[0],6)
+        self.assertEqual(targets_emb["2"].iloc[0],6)
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `napari-tomotwin-0.4.0b3/src/napari_tomotwin/anchor_tool.py` & `napari-tomotwin-0.4.0b4/src/napari_tomotwin/anchor_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,57 @@
 from matplotlib.patches import Circle
 from napari_clusters_plotter._plotter import PlotterWidget
 from qtpy.QtCore import Qt
 from qtpy.QtGui import QGuiApplication
 
 circles: List[Circle] = []
 
+
 def _draw_circle(
-        plotter_widget: PlotterWidget,
-        data_coordinates,
-        label_layer,
-        umap):
+    plotter_widget: PlotterWidget, data_coordinates, label_layer, umap
+):
     global circles
-    '''
+    """
     Adds a circle on the umap when you click on the image
-    '''
+    """
     label_layer.visible = True
     val = label_layer._get_value(data_coordinates)
 
     umap_coordinates = umap.loc[
-        umap['label'] == val, [plotter_widget.plot_x_axis.currentText(), plotter_widget.plot_y_axis.currentText()]]
+        umap["label"] == val,
+        [
+            plotter_widget.plot_x_axis.currentText(),
+            plotter_widget.plot_y_axis.currentText(),
+        ],
+    ]
 
     try:
         center = umap_coordinates.values.tolist()[0]
     except IndexError:
         print("ERROR!!! UAMP")
         return
     modifiers = QGuiApplication.keyboardModifiers()
     if modifiers == Qt.ShiftModifier:
         pass
     else:
         for c in circles[::-1]:
             c.remove()
         circles = []
-    col = '#40d5aa'
+    col = "#40d5aa"
     if plotter_widget.log_scale.isChecked():
-        col = '#79abfd'
+        col = "#79abfd"
     circle = Circle(tuple(center), 0.5, fill=False, color=col)
     circles.append(circle)
     plotter_widget.graphics_widget.axes.add_patch(circle)
     plotter_widget.graphics_widget.draw_idle()
 
+
 def drag_circle_callback(plotter_widget, viewer, event):
-    data_coordinates = plotter_widget.layer_select.value.world_to_data(event.position)
-    _draw_circle(plotter_widget, data_coordinates, plotter_widget.layer_select.value, plotter_widget.layer_select.value.features)
+    data_coordinates = plotter_widget.layer_select.value.world_to_data(
+        event.position
+    )
+    _draw_circle(
+        plotter_widget,
+        data_coordinates,
+        plotter_widget.layer_select.value,
+        plotter_widget.layer_select.value.features,
+    )
```

### Comparing `napari-tomotwin-0.4.0b3/src/napari_tomotwin/load_umap.py` & `napari-tomotwin-0.4.0b4/src/napari_tomotwin/load_umap.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,88 +7,102 @@
 import numpy as np
 import pandas as pd
 from magicgui.tqdm import tqdm as mtqdm
 from matplotlib.patches import Circle
 from napari.qt.threading import thread_worker
 from napari.utils import notifications
 from napari_clusters_plotter._plotter_utilities import estimate_number_bins
-from napari_tomotwin._qt.labeled_progress_bar import LabeledProgressBar
 from napari_tomotwin.anchor_tool import drag_circle_callback
 from qtpy.QtWidgets import (
     QFileDialog,
     QMessageBox,
-
 )
 
 
 class LoadUmapTool:
 
-    def __init__(self, pbar: LabeledProgressBar, plotter_widget = None):
+    def __init__(self, plotter_widget=None):
 
         self.umap = None
         self.plotter_widget = plotter_widget
-        self.pbar = pbar
+        self.pbar = None
         self.circles: List[Circle] = []
         self.viewer = napari.current_viewer()
         self.label_layer_name: str = "Label layer"
-        self.viewer.mouse_drag_callbacks.append(partial(drag_circle_callback, self.plotter_widget))
+        self.viewer.mouse_drag_callbacks.append(
+            partial(drag_circle_callback, self.plotter_widget)
+        )
         self.created_layers = []
 
+    def set_progressbar(self, pbar):
+        self.pbar = pbar
+
     def set_new_label_layer_name(self, name: str):
         self.label_layer_name = name
 
-    def update_progress_bar(self,text: str) -> None:
+    def update_progress_bar(self, text: str) -> None:
         try:
             if self.pbar is not None:
                 self.pbar.set_label_text(text)
         except AttributeError:
             print("Can't initialize progress bar")
 
     def hide_progress_bar(self) -> None:
         try:
             self.pbar.setHidden(True)
         except AttributeError:
             print("Can't hide progress bar. Not initialized")
 
-
-
     @thread_worker()
-    def run_clusters_plotter(self, plotter_widget,
-                             features,
-                             plot_x_axis_name,
-                             plot_y_axis_name,
-                             plot_cluster_name,
-                             force_redraw):
-        '''
+    def run_clusters_plotter(
+        self,
+        plotter_widget,
+        features,
+        plot_x_axis_name,
+        plot_y_axis_name,
+        plot_cluster_name,
+        force_redraw,
+    ):
+        """
         Wrapper function to run clusters plotter in a seperate thead.
-        '''
-        plotter_widget.run(features=features, plot_x_axis_name=plot_x_axis_name, plot_y_axis_name=plot_y_axis_name,
-                           plot_cluster_name=plot_cluster_name, force_redraw=force_redraw)
-
+        """
+        plotter_widget.run(
+            features=features,
+            plot_x_axis_name=plot_x_axis_name,
+            plot_y_axis_name=plot_y_axis_name,
+            plot_cluster_name=plot_cluster_name,
+            force_redraw=force_redraw,
+        )
 
     def show_umap(self, label_layer):
 
+        if label_layer is None:
+            self.viewer.window._qt_window.setEnabled(True)
+
+            notifications.show_error("Can't load umap")
+
         valid = self.check_umap_metadata()
 
         if not valid:
             if self.pbar is not None:
                 self.pbar.hide()
             self.viewer.window._qt_window.setEnabled(True)
             return
 
-        label_layer.metadata['tomotwin']["embeddings_path"] = self.umap.attrs['embeddings_path'] #might have been updated while checking umap metadata
+        label_layer.metadata["tomotwin"]["embeddings_path"] = self.umap.attrs[
+            "embeddings_path"
+        ]  # might have been updated while checking umap metadata
 
         self.update_progress_bar("Visualize umap")
         self.viewer.add_layer(label_layer)
 
         label_layer.opacity = 0
         label_layer.visible = True
         self.created_layers.append(label_layer)
 
-
         try:
             # napari-clusters-plotter > 0.7.4
             self.plotter_widget.layer_select.value = label_layer
         except:
             # napari-clusters-plotter < 0.7.4
             pass
 
@@ -97,37 +111,53 @@
         self.plotter_widget.bin_auto.setChecked(True)
         self.plotter_widget.plotting_type.setCurrentIndex(1)
         self.plotter_widget.plot_hide_non_selected.setChecked(True)
         self.plotter_widget.setDisabled(True)
 
         try:
             # Needs to run in a separate thread, otherwise it freezes when it is loading the umap
-            worker = self.run_clusters_plotter(self.plotter_widget, features=self.umap, plot_x_axis_name="umap_0",
-                                          plot_y_axis_name="umap_1", plot_cluster_name=None,
-                                          force_redraw=True)  # create "worker" object
-            worker.returned.connect(lambda x: self.plotter_widget.setEnabled(True))
+            worker = self.run_clusters_plotter(
+                self.plotter_widget,
+                features=self.umap,
+                plot_x_axis_name="umap_0",
+                plot_y_axis_name="umap_1",
+                plot_cluster_name=None,
+                force_redraw=True,
+            )  # create "worker" object
+            worker.returned.connect(
+                lambda x: self.plotter_widget.setEnabled(True)
+            )
             worker.finished.connect(self.hide_progress_bar)
-            worker.finished.connect(lambda: napari.current_viewer().window._qt_window.setEnabled(True))
+            worker.finished.connect(
+                lambda: napari.current_viewer().window._qt_window.setEnabled(
+                    True
+                )
+            )
             worker.start()
 
         except:
+            notifications.show_error("Can't load umap")
+            self.hide_progress_bar()
+            napari.current_viewer().window._qt_window.setEnabled(True)
             pass
 
     def get_created_layers(self) -> List[any]:
         return self.created_layers
 
-    def create_embedding_mask(self, umap: pd.DataFrame, values: np.array) -> np.array:
+    def create_embedding_mask(
+        self, umap: pd.DataFrame, values: np.array
+    ) -> np.array:
         """
         Creates mask where each individual subvolume of the running windows gets an individual ID
         """
         print("Create embedding mask")
-        Z = umap.attrs['embeddings_attrs']["tomogram_input_shape"][0]
-        Y = umap.attrs['embeddings_attrs']["tomogram_input_shape"][1]
-        X = umap.attrs['embeddings_attrs']["tomogram_input_shape"][2]
-        stride = umap.attrs['embeddings_attrs']["stride"][0]
+        Z = umap.attrs["embeddings_attrs"]["tomogram_input_shape"][0]
+        Y = umap.attrs["embeddings_attrs"]["tomogram_input_shape"][1]
+        X = umap.attrs["embeddings_attrs"]["tomogram_input_shape"][2]
+        stride = umap.attrs["embeddings_attrs"]["stride"][0]
         segmentation_array = np.zeros(shape=(Z, Y, X), dtype=np.float32)
         z = np.array(umap["Z"], dtype=int)
         y = np.array(umap["Y"], dtype=int)
         x = np.array(umap["X"], dtype=int)
 
         # values = np.array(range(1, len(x) + 1))
         for stride_x in mtqdm(list(range(stride))):
@@ -135,95 +165,105 @@
                 for stride_z in range(stride):
                     index = (z + stride_z, y + stride_y, x + stride_x)
                     segmentation_array[index] = values
 
         return segmentation_array
 
     def relabel_and_update(self):
-        '''
+        """
         Here I reduce the number of labels according the histogram bins. This is only for speed reasons.
-        '''
+        """
         print("Relabel")
-        nbins = np.max([estimate_number_bins(self.umap['umap_0']), estimate_number_bins(self.umap['umap_1'])])
-        h, xedges, yedges = np.histogram2d(self.umap['umap_0'], self.umap['umap_1'], bins=nbins)
-        xbins = np.digitize(self.umap['umap_0'], xedges)
-        ybins = np.digitize(self.umap['umap_1'], yedges)
+        nbins = np.max(
+            [
+                estimate_number_bins(self.umap["umap_0"]),
+                estimate_number_bins(self.umap["umap_1"]),
+            ]
+        )
+        h, xedges, yedges = np.histogram2d(
+            self.umap["umap_0"], self.umap["umap_1"], bins=nbins
+        )
+        xbins = np.digitize(self.umap["umap_0"], xedges)
+        ybins = np.digitize(self.umap["umap_1"], yedges)
         new_lbl = xbins * h.shape[0] + ybins
         if "label" not in self.umap.keys().tolist():
-            self.umap['label'] = new_lbl
-        lbl_data = self.create_embedding_mask(self.umap, new_lbl).astype(np.int64)
+            self.umap["label"] = new_lbl
+        lbl_data = self.create_embedding_mask(self.umap, new_lbl).astype(
+            np.int64
+        )
         return lbl_data
 
     def check_umap_metadata(self) -> bool:
         def get_embedding_path(pth: str) -> str:
-            '''
+            """
             Checks if the embedding path exists. If it does not exist, it opens a file selection dialogue. Otherwise, it returns the path.
-            '''
+            """
             if not os.path.exists(pth):
                 msg = QMessageBox()
                 msg.setIcon(QMessageBox.Critical)
                 msg.setWindowTitle("Can't open embedding file")
                 msg.setText("Can't open embedding file")
                 msg.setInformativeText(
-                    "The embedding path in the metadata (see below) doesn't exist or can't be accessed, click OK and select the path to the embedding file.")
+                    "The embedding path in the metadata (see below) doesn't exist or can't be accessed, click OK and select the path to the embedding file."
+                )
                 msg.setDetailedText(pth)
                 msg.setStandardButtons(QMessageBox.Ok)
                 msg.exec_()
-                pth = QFileDialog.getOpenFileName(napari.current_viewer().window._qt_window, 'Open embedding file',
-                                                  os.getcwd(),
-                                                  "Embedding file (*.temb)")[0]
+                pth = QFileDialog.getOpenFileName(
+                    napari.current_viewer().window._qt_window,
+                    "Open embedding file",
+                    os.getcwd(),
+                    "Embedding file (*.temb)",
+                )[0]
 
             return pth
 
-        if 'embeddings_attrs' not in self.umap.attrs:
+        if "embeddings_attrs" not in self.umap.attrs:
             napari.utils.notifications.show_error(
-                "The umap was calculated with an old version of TomoTwin. Please update TomoTwin and re-estimate the umap.")
+                "The umap was calculated with an old version of TomoTwin. Please update TomoTwin and re-estimate the umap."
+            )
             return False
 
-        emb_path = get_embedding_path(self.umap.attrs['embeddings_path'])
+        emb_path = get_embedding_path(self.umap.attrs["embeddings_path"])
 
         if emb_path == "":
             return False
 
-        self.umap.attrs['embeddings_path'] = emb_path # overwrite in case it was updated
+        self.umap.attrs["embeddings_path"] = (
+            emb_path  # overwrite in case it was updated
+        )
 
         return True
 
-
     def load_umap(self, filename: pathlib.Path):
         self.update_progress_bar("Read umap")
         self.umap = pd.read_pickle(filename)
         self.update_progress_bar("Generate label layer")
 
+        if "umap_0" not in self.umap:
+            return None
 
         lbl_data = self.relabel_and_update()
         from napari.layers import Layer
-        lbl_layer = Layer.create(lbl_data, {
-            "name": self.label_layer_name}, layer_type="Labels")
+
+        lbl_layer = Layer.create(
+            lbl_data, {"name": self.label_layer_name}, layer_type="Labels"
+        )
         lbl_layer.features = self.umap
         lbl_layer.properties = self.umap
-        lbl_layer.metadata['tomotwin'] = {
+        lbl_layer.metadata["tomotwin"] = {
             "umap_path": filename,
-            "embeddings_path": self.umap.attrs['embeddings_path']
+            "embeddings_path": self.umap.attrs["embeddings_path"],
         }
 
         return lbl_layer
 
     @thread_worker
     def _load_umap_worker(self, filename: pathlib.Path):
         return self.load_umap(filename)
 
     def start_umap_worker(self, filename: pathlib.Path):
         napari.current_viewer().window._qt_window.setEnabled(False)
         worker = self._load_umap_worker(filename)
         worker.returned.connect(self.show_umap)
 
         return worker
-
-
-
-
-
-
-
-
-
```

### Comparing `napari-tomotwin-0.4.0b3/src/napari_tomotwin.egg-info/PKG-INFO` & `napari-tomotwin-0.4.0b4/src/napari_tomotwin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.4.0b3
+Version: 0.4.0b4
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.4.0b3/tox.ini` & `napari-tomotwin-0.4.0b4/tox.ini`

 * *Files identical despite different names*

