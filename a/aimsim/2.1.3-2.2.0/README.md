# Comparing `tmp/aimsim-2.1.3.tar.gz` & `tmp/aimsim-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsim-2.1.3.tar", last modified: Fri Feb  2 22:30:19 2024, max compression
+gzip compressed data, was "aimsim-2.2.0.tar", last modified: Mon Apr 15 16:35:26 2024, max compression
```

## Comparing `aimsim-2.1.3.tar` & `aimsim-2.2.0.tar`

### file list

```diff
@@ -1,87 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.376478 aimsim-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-02-02 22:30:11.000000 aimsim-2.1.3/AIMSim-GUI.png
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-02 22:30:11.000000 aimsim-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-02 22:30:11.000000 aimsim-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-02-02 22:30:19.376478 aimsim-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-02-02 22:30:11.000000 aimsim-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.364478 aimsim-2.1.3/aimsim/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-02 22:30:11.000000 aimsim-2.1.3/aimsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-02 22:30:11.000000 aimsim-2.1.3/aimsim/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.368478 aimsim-2.1.3/aimsim/chemical_datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-02 22:30:11.000000 aimsim-2.1.3/aimsim/chemical_datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-02-02 22:30:11.000000 aimsim-2.1.3/aimsim/chemical_datastructures/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    49022 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/chemical_datastructures/molecule_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.368478 aimsim-2.1.3/aimsim/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/ops/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    76163 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/ops/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/ops/similarity_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.368478 aimsim-2.1.3/aimsim/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/cluster_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/compare_target_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/extended_similarity_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/identify_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/measure_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/see_property_variation_with_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/tasks/visualize_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.368478 aimsim-2.1.3/aimsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/utils/ccbmlib_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/utils/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-02-02 22:30:12.000000 aimsim-2.1.3/aimsim/utils/plotting_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.376478 aimsim-2.1.3/aimsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-02 22:30:19.000000 aimsim-2.1.3/aimsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-02 22:30:12.000000 aimsim-2.1.3/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.360478 aimsim-2.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/_images/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/_images/sulfonamide-substrate-scope.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/_static/plus.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.360478 aimsim-2.1.3/docs/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/docs/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/interfaces/UI/AIMSim-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-02-02 22:30:12.000000 aimsim-2.1.3/docs/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-02 22:30:12.000000 aimsim-2.1.3/implemented_metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/UI/AIMSim-GUI-corner-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/UI/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/UI/AIMSim_ui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/UI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.372478 aimsim-2.1.3/interfaces/UI/libraries/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/UI/libraries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-02 22:30:12.000000 aimsim-2.1.3/interfaces/config_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-02 22:30:12.000000 aimsim-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 22:30:19.376478 aimsim-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-02 22:30:12.000000 aimsim-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.376478 aimsim-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:30:19.376478 aimsim-2.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/sulfonamide-substrate-scope-PDF.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_CompareTargetMolecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_Descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_LoadingErrorException.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_MeasureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_Molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    52827 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_MoleculeSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_SimilarityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_SimilarityMeasureValueErrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_ToolTip.py
--rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-02-02 22:30:12.000000 aimsim-2.1.3/tests/test_multithreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-04-15 16:35:23.000000 aimsim-2.2.0/AIMSim-GUI.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 16:35:23.000000 aimsim-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 16:35:23.000000 aimsim-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-15 16:35:26.919880 aimsim-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-15 16:35:23.000000 aimsim-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/chemical_datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48544 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/molecule_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75466 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/similarity_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/aimsim/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/cluster_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/compare_target_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/extended_similarity_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/identify_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/measure_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/see_property_variation_with_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/visualize_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/aimsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/ccbmlib_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/plotting_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/aimsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:35:23.000000 aimsim-2.2.0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.903880 aimsim-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_images/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_images/sulfonamide-substrate-scope.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.903880 aimsim-2.2.0/docs/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/interfaces/UI/AIMSim-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 16:35:23.000000 aimsim-2.2.0/implemented_metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim_ui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/UI/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/libraries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/config_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 16:35:23.000000 aimsim-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 16:35:23.000000 aimsim-2.2.0/requirements_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:35:26.919880 aimsim-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-15 16:35:23.000000 aimsim-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/sulfonamide-substrate-scope-PDF.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_CompareTargetMolecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_Descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_LoadingErrorException.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_MeasureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52891 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_MoleculeSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_SimilarityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_SimilarityMeasureValueErrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_ToolTip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_multithreading.py
```

### Comparing `aimsim-2.1.3/AIMSim-GUI.png` & `aimsim-2.2.0/AIMSim-GUI.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/LICENSE` & `aimsim-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/PKG-INFO` & `aimsim-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aimsim
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python command line and GUI tool to analyze molecular similarity.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: numpy
 Requires-Dist: multiprocess>=0.70
-Requires-Dist: scikit_learn_extra
 Requires-Dist: pandas
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: scikit_learn
 Requires-Dist: rdkit
 Requires-Dist: psutil
 Requires-Dist: padelpy
 Requires-Dist: plotly
@@ -30,22 +29,24 @@
 
 <h1 align="center">AIMSim README</h1> 
 <h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
 
 ![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
   <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/ci.yml/badge.svg?event=schedule">
 </p>
 
+Downloads Stats:
+ - `aimsim`: [![Downloads](https://static.pepy.tech/badge/aimsim)](https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+ - `aimsim_core`: [![Downloads](https://static.pepy.tech/badge/aimsim_core)](https://pepy.tech/project/aimsim_core?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+
 ## Documentation and Tutorial
 [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the _AIMSim_ comprehensive tutorial in your browser:
 <a target="_blank" href="https://colab.research.google.com/github/VlachosGroup/AIMSim/blob/master/AIMSim-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Purpose
@@ -81,14 +82,18 @@
 
 ## Installing AIMSim
 It is recommended to install `AIMSim` in a virtual environment with [`conda`](https://docs.conda.io/en/latest/) or Python's [`venv`](https://docs.python.org/3/library/venv.html).
 ### `pip`
 `AIMSim` can be installed with a single command using Python's package manager `pip`:
 `pip install aimsim`
 This command also installs the required dependencies.
+
+> [!NOTE]
+> Looking to use AIMSim for descriptor calculation or extend its functionality? `AIMSim`'s core modules for creating molecules, calculating descriptors, and comparing the results are available without support for plotting or visualization in the PyPI package `aimsim_core`.
+
 ### `conda`
 `AIMSim` is also available with the `conda` package manager via:
 `conda install -c conda-forge aimsim`
 This will install all dependencies from `conda-forge`.
 
 ### Note for mordred-descriptor
 AIMSim v1 provided direct support for the descriptors provided in the `mordred` package but unfortunately the original `mordred` is now abandonware.
```

### Comparing `aimsim-2.1.3/README.md` & `aimsim-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 <h1 align="center">AIMSim README</h1> 
 <h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
 
 ![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
   <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/ci.yml/badge.svg?event=schedule">
 </p>
 
+Downloads Stats:
+ - `aimsim`: [![Downloads](https://static.pepy.tech/badge/aimsim)](https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+ - `aimsim_core`: [![Downloads](https://static.pepy.tech/badge/aimsim_core)](https://pepy.tech/project/aimsim_core?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+
 ## Documentation and Tutorial
 [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the _AIMSim_ comprehensive tutorial in your browser:
 <a target="_blank" href="https://colab.research.google.com/github/VlachosGroup/AIMSim/blob/master/AIMSim-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Purpose
@@ -51,14 +53,18 @@
 
 ## Installing AIMSim
 It is recommended to install `AIMSim` in a virtual environment with [`conda`](https://docs.conda.io/en/latest/) or Python's [`venv`](https://docs.python.org/3/library/venv.html).
 ### `pip`
 `AIMSim` can be installed with a single command using Python's package manager `pip`:
 `pip install aimsim`
 This command also installs the required dependencies.
+
+> [!NOTE]
+> Looking to use AIMSim for descriptor calculation or extend its functionality? `AIMSim`'s core modules for creating molecules, calculating descriptors, and comparing the results are available without support for plotting or visualization in the PyPI package `aimsim_core`.
+
 ### `conda`
 `AIMSim` is also available with the `conda` package manager via:
 `conda install -c conda-forge aimsim`
 This will install all dependencies from `conda-forge`.
 
 ### Note for mordred-descriptor
 AIMSim v1 provided direct support for the descriptors provided in the `mordred` package but unfortunately the original `mordred` is now abandonware.
```

### Comparing `aimsim-2.1.3/aimsim/chemical_datastructures/molecule.py` & `aimsim-2.2.0/aimsim/chemical_datastructures/molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/chemical_datastructures/molecule_set.py` & `aimsim-2.2.0/aimsim/chemical_datastructures/molecule_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         get_pairwise_similarities(): Get an array of pairwise similarities
             of molecules in the set.
         get_mol_names(): Get names of the molecules in the set.
         get_mol_properties(): Get properties of all the molecules
             in the dataset.
         cluster(n_clusters=8, clustering_method=None, **kwargs): Cluster
             the molecules of the MoleculeSet. Implemented methods.
-                'kmedoids': for the K-Medoids algorithm.
                 'complete_linkage', 'complete':
                     Complete linkage agglomerative hierarchical
                     clustering.
                 'average_linkage', 'average':
                     average linkage agglomerative hierarchical clustering.
                 'single_linkage', 'single':
                     single linkage agglomerative hierarchical clustering.
@@ -993,31 +992,26 @@
         """Cluster the molecules of the MoleculeSet.
 
         Args:
             n_clusters (int): Number of clusters. Default is 8.
             clustering_method (str): Clustering algorithm to use. Default is
                 None in which case the algorithm is chosen from the
                 similarity measure in use. Implemented clustering_methods are:
-                'kmedoids': for the K-Medoids algorithm [1].
-                    This method is useful
-                    when the molecular descriptors are continuous / Euclidean
-                    since it relies on the existence of a sensible medoid.
                 'complete_linkage', 'complete':
                     Complete linkage agglomerative hierarchical clustering [2].
                 'average_linkage', 'average':
                     average linkage agglomerative hierarchical clustering [2].
                 'single_linkage', 'single':
                     single linkage agglomerative hierarchical clustering [2].
                 'ward':
                     for Ward's algorithm [2]. This method is useful for
                     Euclidean descriptors.
             kwargs (keyword args): Key word arguments to supply to clustering
                 algorithm. See the documentation pages
                 listed below for these arguments:
-                'kmedoids': https://scikit-learn-extra.readthedocs.io/en/stable/generated/sklearn_extra.cluster.KMedoids.html
                 'complete_linkage', 'average_linkage', 'single_linkage', 'ward'
                     : https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html
 
         Returns:
             cluster_grouped_mol_names (dict): Dictionary of cluster id
                 (key) --> Names of molecules in cluster.
 
@@ -1033,25 +1027,25 @@
         if not self.similarity_measure.is_distance_metric():
             raise InvalidConfigurationError(
                 str(self.similarity_measure) + " is not a distance metric. "
                 "Clustering will not yield "
                 "meaningful results."
             )
         if (
-            clustering_method == "kmedoids" or clustering_method == "ward"
+            clustering_method == "ward"
         ) and self.similarity_measure.type_ == "discrete":
             print(
                 f"{clustering_method} cannot be used with "
                 f"{self.similarity_measure.type_} "
                 f"similarity measure. Changing."
             )
             clustering_method = None
         if clustering_method is None:
             if self.similarity_measure.type_ == "continuous":
-                clustering_method = "kmedoids"
+                clustering_method = "ward"
             else:
                 clustering_method = "complete_linkage"
         self.clusters_ = Cluster(
             n_clusters=n_clusters, clustering_method=clustering_method, **kwargs
         ).fit(self.get_distance_matrix())
 
     def get_cluster_labels(self):
```

### Comparing `aimsim-2.1.3/aimsim/exceptions.py` & `aimsim-2.2.0/aimsim/exceptions.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/ops/clustering.py` & `aimsim-2.2.0/aimsim/ops/clustering.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 """Operation for clustering molecules"""
 import sklearn.exceptions
 from sklearn.cluster import AgglomerativeClustering
-from sklearn_extra.cluster import KMedoids as SklearnExtraKMedoids
 
 
 class Cluster:
     """
     Wrapper class for different clustering algorithms.
     Attributes:
         clustering_method (str):
             Label for the specific algorithm used.
-            'kmedoids':
-                for the K-Medoids algorithm [1]. This method is useful
-                when the molecular descriptors are continuous / Euclidean
-                since it relies on the existence of a sensible medoid.
             'complete_linkage', 'complete':
                 Complete linkage agglomerative hierarchical clustering [2].
             'average_linkage', 'average':
                 average linkage agglomerative hierarchical clustering [2].
             'single_linkage', 'single':
                 single linkage agglomerative hierarchical clustering [2].
             'ward':
                 for Ward's algorithm [2]. This method is useful for
                 Euclidean descriptors.
         n_clusters (int):
             Number of clusters.
-        model_ (sklearn.cluster.AgglomerativeClustering or sklearn_extra.cluster.KMedoids):
+        model_ (sklearn.cluster.AgglomerativeClustering):
             The clustering estimator.
         labels_ (np.ndarray of shape (n_samples,)):
             cluster labels of the training set samples.
 
     Methods:
         fit(X): Fit the estimator.
         predict(X): Get prediction from the estimator.
@@ -46,77 +41,51 @@
     """
     def __init__(self, n_clusters, clustering_method, **kwargs):
         """
         Constructor for the Cluster class.
         Args:
             n_clusters (int): Number of clusters.
             clustering_method(str): Label for the specific algorithm used.
-                Supported methods are:
-                'kmedoids' for the K-Medoids algorithm [1]. This method is
-                    useful when the molecular descriptors are continuous
-                    / Euclidean since it relies on the existence of a
-                    sensible medoid.
                 'complete_linkage', 'complete' for complete linkage
                     agglomerative hierarchical clustering [2].
                 'average_linkage', 'average' for average linkage agglomerative
                     hierarchical clustering [2].
                 'single_linkage', 'single' for single linkage agglomerative
                     hierarchical clustering [2].
                 'ward' for Ward's algorithm [2]. This method is useful for
                     Euclidean descriptors.
             kwargs (dict): Keyword arguments. These are passed to the
                 estimators. Refer to the following documentation page for
-                kmedoids: https://scikit-learn-extra.readthedocs.io/en/stable/generated/sklearn_extra.cluster.KMedoids.html
                 agglomerative hierarchical clustering: https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html
 
         References:
         [1] Hastie, T., Tibshirani R. and Friedman J.,
             The Elements of statistical Learning: Data Mining, Inference,
             and Prediction, 2nd Ed., Springer Series in Statistics (2009).
         [2] Murtagh, F. and Contreras, P., Algorithms for hierarchical
             clustering: an overview. WIREs Data Mining Knowl Discov
             (2011). https://doi.org/10.1002/widm.53
         """
         self.clustering_method = clustering_method
         self.n_clusters = n_clusters
-        if self.clustering_method == "kmedoids":
-            self.model_ = self._get_kmedoids_model_(**kwargs)
-        elif clustering_method in ["complete_linkage", "complete"]:
+        if clustering_method in ["complete_linkage", "complete"]:
             self.model_ = self._get_linkage_model(linkage_method="complete",
                                                   **kwargs)
         elif clustering_method in ["average", "average_linkage"]:
             self.model_ = self._get_linkage_model(linkage_method="average",
                                                   **kwargs)
         elif clustering_method in ["single", "single_linkage"]:
             self.model_ = self._get_linkage_model(linkage_method="single",
                                                   **kwargs)
         elif clustering_method == "ward":
             self.model_ = self._get_linkage_model(linkage_method="ward",
                                                   **kwargs)
         else:
             raise ValueError(f"{clustering_method} not implemented")
 
-    def _get_kmedoids_model_(self, **kwargs):
-        """
-        Initialize a k-medoids model.
-
-        Args:
-        kwargs (dict): Keyword arguments. These are passed to the
-                estimators. Refer to the following documentation page for
-                kmedoids:
-                [https://scikit-learn-extra.readthedocs.io/en/stable/generated/sklearn_extra.cluster.KMedoids.html]
-
-        """
-        _ = kwargs.pop('metric', None)
-        return SklearnExtraKMedoids(
-            n_clusters=self.n_clusters,
-            metric="precomputed",
-            **kwargs
-        )
-
     def _get_linkage_model(self, linkage_method, **kwargs):
         _ = kwargs.pop('affinity', None)
         try:
             return AgglomerativeClustering(
                 n_clusters=self.n_clusters,
                 affinity="precomputed",
                 linkage=linkage_method,
```

### Comparing `aimsim-2.1.3/aimsim/ops/descriptor.py` & `aimsim-2.2.0/aimsim/ops/descriptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """This module contains methods to featurize molecules."""
+
 import numpy as np
 from rdkit.Chem import rdmolops
 from rdkit import Chem
 from rdkit import DataStructs
 from rdkit.Chem import AllChem
 from rdkit.Chem.Fingerprints import FingerprintMols
 from rdkit.Chem import MACCSkeys
 from rdkit.Chem.AtomPairs import Pairs, Torsions
 from rdkit.DataStructs import cDataStructs
 from aimsim.utils.ccbmlib_fingerprints import generate_fingerprints
 from padelpy import from_smiles
-from aimsim.utils.extras import requires_mordred
 from mhfp.encoder import MHFPEncoder
-
-try:
-    from mordred import Calculator, descriptors
-except ImportError:
-    NO_MORDRED = True
+from mordred import Calculator, descriptors
 
 
 from ..exceptions import (
     InvalidConfigurationError,
     NotInitializedError,
     MordredCalculatorError,
 )
@@ -55,18 +51,15 @@
         Attribute will be initialized if not present.
 
         Returns:
             (np.array): Numpy vector of descriptor.
 
         """
         if self.check_init() is False:
-            raise NotInitializedError(
-                "Descriptor value not generated. Use "
-                "make_fingerprint() to initialize it."
-            )
+            raise NotInitializedError("Descriptor value not generated. Use " "make_fingerprint() to initialize it.")
         if not hasattr(self, "numpy_"):
             self.numpy_ = np.zeros((0,), dtype=np.int8)
             DataStructs.ConvertToNumpyArray(self.rdkit_, self.numpy_)
         self.numpy_ = self.numpy_.ravel()
         return self.numpy_
 
     def to_rdkit(self):
@@ -78,58 +71,45 @@
         Raises:
             (NotInitializedError): If object not initialized with a fingerprint.
             (ValueError): If only arbitrary numpy descriptor is used to
                 initialize the object. This cannot be converted to bit vectors.
 
         """
         if self.check_init() is False:
-            raise NotInitializedError(
-                "Descriptor value not generated. Use "
-                "make_fingerprint() to initialize it."
-            )
+            raise NotInitializedError("Descriptor value not generated. Use " "make_fingerprint() to initialize it.")
         if not hasattr(self, "rdkit_"):
-            raise ValueError(
-                "Attempting to convert arbitrary numpy array "
-                "to rdkit bit vector is not supported"
-            )
+            raise ValueError("Attempting to convert arbitrary numpy array " "to rdkit bit vector is not supported")
         return self.rdkit_
 
     def check_init(self):
         """Check initialization status of the Descriptor object.
 
         Returns:
             (bool): True if object is initialized.
 
         """
-        return (
-            getattr(self, "numpy_", None) is not None
-            or getattr(self, "rdkit_", None) is not None
-        )
+        return getattr(self, "numpy_", None) is not None or getattr(self, "rdkit_", None) is not None
 
     def _set_morgan_fingerprint(self, molecule_graph, radius, n_bits, **kwargs):
         """Set the descriptor to a morgan fingerprint.
 
         Args:
             molecule_graph (RDKIT object): Graph of molecule to be
                 fingerprinted.
             radius (int): Radius of fingerprint, 3 corresponds to ECFP6.
             n_bits (int):Number of bits to use if Morgan Fingerprint wanted as
                 a bit vector. If set to None, Morgan fingerprint returned
                 as count.
 
         """
-        self.rdkit_ = AllChem.GetMorganFingerprintAsBitVect(
-            molecule_graph, radius, nBits=n_bits, **kwargs
-        )
+        self.rdkit_ = AllChem.GetMorganFingerprintAsBitVect(molecule_graph, radius, nBits=n_bits, **kwargs)
         self.label_ = "morgan_fingerprint"
         self.params_ = {"radius": radius, "n_bits": n_bits}
 
-    def _set_rdkit_topological_fingerprint(
-        self, molecule_graph, min_path, max_path, **kwargs
-    ):
+    def _set_rdkit_topological_fingerprint(self, molecule_graph, min_path, max_path, **kwargs):
         """Set the descriptor to a topological fingerprint.
 
         Args:
             molecule_graph (RDKIT object): Graph of molecule to be
                 fingerprinted.
             min_path (int): Minimum path used to generate the
                 topological fingerprint.
@@ -143,17 +123,15 @@
                 f"{molecule_graph.GetNumAtoms()}, "
                 f"min_path: {min_path}. "
                 f"For topological fingerprint, "
                 f"the number of atoms has to be "
                 f"greater than the minimum path "
                 f"used for fingerprint."
             )
-        self.rdkit_ = rdmolops.RDKFingerprint(
-            molecule_graph, minPath=min_path, maxPath=max_path
-        )
+        self.rdkit_ = rdmolops.RDKFingerprint(molecule_graph, minPath=min_path, maxPath=max_path)
         self.label_ = "topological_fingerprint"
         self.params_ = {"min_path": min_path, "max_path": max_path}
 
     def _set_padelpy_descriptor(self, molecule_graph, descriptor, **kwargs):
         """Set the value of numpy_ to the descriptor as indicated by descriptor.
 
         Args:
@@ -163,19 +141,16 @@
         """
         try:
             local_smi = Chem.MolToSmiles(molecule_graph)
             all_desc = from_smiles(local_smi, timeout=kwargs.get("timeout", 60))
             self.numpy_ = np.array(all_desc[descriptor])
             self.label_ = descriptor
         except Exception as e:
-            raise RuntimeError(
-                f"Unable to retrieve PaDELPy Descriptor '{descriptor}'. Is it a valid descriptor?"
-            )
+            raise RuntimeError(f"Unable to retrieve PaDELPy Descriptor '{descriptor}'. Is it a valid descriptor?")
 
-    @requires_mordred
     def _set_mordred_descriptor(self, molecule_graph, descriptor, **kwargs):
         """Set the value of numpy_ to the descriptor as indicated by descriptor.
 
         Args:
             molecule_graph (RDKit object): Graph of the molecule of interest.
             descriptor (string): Name of descriptor, as implemented in Mordred.
 
@@ -188,15 +163,15 @@
             res = calc(molecule_graph)
             res.drop_missing()
             self.numpy_ = np.array(res[descriptor])
             self.label_ = descriptor
         except KeyError:
             raise MordredCalculatorError(
                 """Mordred descriptor calculator unable to calculate descriptor \"{}\",
-                ensure correct name is used (https://mordred-descriptor.github.io/documentation/master/descriptors.html).""".format(
+                ensure correct name is used (https://jacksonburns.github.io/mordred-community/descriptors.html).""".format(
                     descriptor
                 )
             )
 
     def _set_daylight_fingerprint(self, molecule_graph, **kwargs):
         """Set the descriptor to a daylight fingerprint.
 
@@ -282,17 +257,15 @@
             rings=kwargs["rings"],
             kekulize=kwargs["kekulize"],
         )
         self.numpy_ = fp
         self.label_ = "minhash_fingerprint"
         self.params_ = kwargs
 
-    def make_fingerprint(
-        self, molecule_graph, fingerprint_type, fingerprint_params=None
-    ):
+    def make_fingerprint(self, molecule_graph, fingerprint_type, fingerprint_params=None):
         """Make fingerprint of a molecule based on a graph representation.
         Set the state of the descriptor to this fingerprint.
 
         Args:
             molecule_graph (RDKIT object): The graph object used to make a
                 fingerprint.
             fingerprint_type (str): label for the type of fingerprint.
@@ -312,53 +285,43 @@
                 "n_permutations": 2048,
                 "seed": 42,
                 "radius": 3,
                 "rings": True,
                 "kekulize": True,
             }
             minhash_params.update(fingerprint_params)
-            self._set_minhash_fingerprint(
-                molecule_graph=molecule_graph, **minhash_params
-            )
+            self._set_minhash_fingerprint(molecule_graph=molecule_graph, **minhash_params)
         elif fingerprint_type == "topological_fingerprint":
             topological_params = {"min_path": 1, "max_path": 7}
             topological_params.update(fingerprint_params)
-            self._set_rdkit_topological_fingerprint(
-                molecule_graph=molecule_graph, **topological_params
-            )
+            self._set_rdkit_topological_fingerprint(molecule_graph=molecule_graph, **topological_params)
         elif fingerprint_type == "daylight_fingerprint":
             daylight_params = {
                 "minPath": 1,
                 "maxPath": 7,
                 "fpSize": 2048,
                 "bitsPerHash": 2,
                 "useHs": 0,
                 "tgtDensity": 0.3,
                 "minSize": 64,
             }
             daylight_params.update(fingerprint_params)
-            self._set_daylight_fingerprint(
-                molecule_graph=molecule_graph, **daylight_params
-            )
+            self._set_daylight_fingerprint(molecule_graph=molecule_graph, **daylight_params)
         elif fingerprint_type == "maccs_keys":
             maccs_params = {}
             maccs_params.update(fingerprint_params)
             self._set_maccs_keys(molecule_graph=molecule_graph, **maccs_params)
         elif fingerprint_type == "atom-pair_fingerprint":
             atom_pair_fp_params = {}
             atom_pair_fp_params.update(fingerprint_params)
-            self._set_atom_pair_fingerprint(
-                molecule_graph=molecule_graph, **atom_pair_fp_params
-            )
+            self._set_atom_pair_fingerprint(molecule_graph=molecule_graph, **atom_pair_fp_params)
         elif fingerprint_type == "torsion_fingerprint":
             torsion_params = {}
             torsion_params.update(fingerprint_params)
-            self._set_torsion_fingerprint(
-                molecule_graph=molecule_graph, **torsion_params
-            )
+            self._set_torsion_fingerprint(molecule_graph=molecule_graph, **torsion_params)
         elif fingerprint_type.split(":")[0] == "mordred":
             mordred_params = {}
             self._set_mordred_descriptor(
                 molecule_graph=molecule_graph,
                 descriptor=fingerprint_type.split(":")[1],
                 **mordred_params,
             )
@@ -414,26 +377,19 @@
         Returns:
             (np.ndarray): Folded fingerprint.
         """
         if not self.is_fingerprint():
             raise ValueError("Can only fold fingerprints")
         fingerprint = self.to_numpy()
         if len(fingerprint) < fold_to_length:
-            raise InvalidConfigurationError(
-                f"Cannot fold fingerprint of "
-                f"length {len(fingerprint)}to a "
-                f"higher length {fold_to_length}"
-            )
+            raise InvalidConfigurationError(f"Cannot fold fingerprint of " f"length {len(fingerprint)}to a " f"higher length {fold_to_length}")
         n_folds = np.log2(len(fingerprint) / fold_to_length)
         if n_folds - int(n_folds) > 0.0:
             raise InvalidConfigurationError(
-                f"Fingerprint length "
-                f"{len(fingerprint)} not "
-                f"a 2-multiple of required "
-                f"folded length {fold_to_length}"
+                f"Fingerprint length " f"{len(fingerprint)} not " f"a 2-multiple of required " f"folded length {fold_to_length}"
             )
         for _ in range(int(n_folds)):
             mid_point = int(len(fingerprint) / 2)
             assert mid_point - (len(fingerprint) / 2) == 0.0
             fingerprint = fingerprint[:mid_point] | fingerprint[mid_point:]
         assert len(fingerprint) == fold_to_length
         return fingerprint
@@ -480,17 +436,15 @@
         fprint2_arr = fingerprint2.to_numpy()
         if len(fprint1_arr) > len(fprint2_arr):
             return (
                 fingerprint1.get_folded_fprint(fold_to_length=len(fprint2_arr)),
                 fprint2_arr,
             )
         else:
-            return fprint1_arr, fingerprint2.get_folded_fprint(
-                fold_to_length=len(fprint1_arr)
-            )
+            return fprint1_arr, fingerprint2.get_folded_fprint(fold_to_length=len(fprint1_arr))
 
     @staticmethod
     def get_supported_fprints():
         """Return a list of strings for the currently implemented
         molecular fingerprints.
         Returns:
             List: List of strings.
```

### Comparing `aimsim-2.1.3/aimsim/ops/similarity_measures.py` & `aimsim-2.2.0/aimsim/ops/similarity_measures.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/cluster_data.py` & `aimsim-2.2.0/aimsim/tasks/cluster_data.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/compare_target_molecule.py` & `aimsim-2.2.0/aimsim/tasks/compare_target_molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/extended_similarity_indices.py` & `aimsim-2.2.0/aimsim/tasks/extended_similarity_indices.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/identify_outliers.py` & `aimsim-2.2.0/aimsim/tasks/identify_outliers.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/measure_search.py` & `aimsim-2.2.0/aimsim/tasks/measure_search.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/see_property_variation_with_similarity.py` & `aimsim-2.2.0/aimsim/tasks/see_property_variation_with_similarity.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/task_manager.py` & `aimsim-2.2.0/aimsim/tasks/task_manager.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/tasks/visualize_dataset.py` & `aimsim-2.2.0/aimsim/tasks/visualize_dataset.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/utils/ccbmlib_fingerprints.py` & `aimsim-2.2.0/aimsim/utils/ccbmlib_fingerprints.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/aimsim/utils/plotting_scripts.py` & `aimsim-2.2.0/aimsim/utils/plotting_scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 """Plotting functions"""
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
-import numpy as np
-import pandas as pd
-import plotly.express as px
-import plotly.graph_objects as go
-from seaborn import kdeplot, heatmap
 
-from aimsim.exceptions import InvalidConfigurationError
+NO_PLOT = False
+try:
+    import matplotlib.pyplot as plt
+    import matplotlib.ticker as ticker
+    import numpy as np
+    import pandas as pd
+    import plotly.express as px
+    import plotly.graph_objects as go
+    from seaborn import heatmap, kdeplot
+except ImportError:
+    NO_PLOT = True
+
+from aimsim.exceptions import InvalidConfigurationError  # noqa: E402
+
+
+def check_plot(func):
+    def wrapper(*args, **kwargs):
+        if NO_PLOT:
+            raise RuntimeError("Missing plotting dependencies.")
+        return func(*args, **kwargs)
 
+    return wrapper
 
+
+@check_plot
 def plot_density(densities, n_densities=1, legends=None, **kwargs):
     """Plot the similarity density.
 
     Args:
         densities (list or numpy ndarray): Vector(s) of densities to plot.
             Shape (n_densities, n_points_per_density). n_densities can be 1.
         n_densities (int): Number of densities.
@@ -52,49 +67,39 @@
     shade = kwargs.pop("shade", False)
 
     if n_densities == 1:
         valid_number_types = (float, np.int64, int, float)
         for density in densities:
             is_number = isinstance(density, valid_number_types)
             if not is_number:
-                raise InvalidConfigurationError(f'Element of type '
-                                                f'{type(density)} passed when '
-                                                f'expecting types '
-                                                f'{valid_number_types}')
+                raise InvalidConfigurationError(f"Element of type " f"{type(density)} passed when " f"expecting types " f"{valid_number_types}")
         # converting to 2D array for uniform processing
         densities = [densities]
     if color is None or isinstance(color, str):
         color = [color] * n_densities
     if legends is None:
         legends = [None] * n_densities
     if len(color) < n_densities:
-        raise InvalidConfigurationError(f'{len(color)} colors supplied '
-                                        f'for {n_densities} '
-                                        f'densities')
+        raise InvalidConfigurationError(f"{len(color)} colors supplied " f"for {n_densities} " f"densities")
     if len(legends) < n_densities:
-        raise InvalidConfigurationError(f'{len(legends)} colors supplied '
-                                        f'for {n_densities} '
-                                        f'densities')
+        raise InvalidConfigurationError(f"{len(legends)} colors supplied " f"for {n_densities} " f"densities")
 
     plt.figure()
     plt.rcParams["svg.fonttype"] = "none"
     for density_id, density in enumerate(densities):
-        kdeplot(density,
-                color=color[density_id],
-                label=legends[density_id],
-                shade=shade,
-                **kwargs)
+        kdeplot(density, color=color[density_id], label=legends[density_id], shade=shade, **kwargs)
     plt.xlabel(xlabel, fontsize=xlabel_fontsize)
     plt.ylabel(ylabel, fontsize=ylabel_fontsize)
     if not legends == [None] * n_densities:
         plt.legend(fontsize=legend_fontsize)
     if plot_title is not None:
         plt.title(plot_title, fontsize=plot_title_fontsize)
 
 
+@check_plot
 def plot_heatmap(input_matrix, **kwargs):
     """Plot a heatmap representing the input matrix.
 
     Args:
         input_matrix (np.ndarray): Matrix to be plotted.
 
     kwargs: dict
@@ -138,14 +143,15 @@
         cmap=parameters["cmap"],
         mask=mask,
         annot=parameters["annotate"],
     )
     plt.title(parameters["plot_title"], fontsize=24)
 
 
+@check_plot
 def plot_parity(x, y, **kwargs):
     """Plot parity plot of x vs y.
 
     Args:
         x (n x 1 np.ndarray): values plotted along x axis
         y (n x 1 np.ndarray): values plotted along y axis
 
@@ -175,26 +181,17 @@
     axes.set_xlim([min_entry, max_entry])
     axes.set_ylim([min_entry, max_entry])
     plt.plot(
         [min_entry, max_entry],
         [min_entry, max_entry],
         color=plot_params.get("linecolor", "black"),
     )
-    plt.title(
-        plot_params.get("title", ""),
-        fontsize=plot_params.get("title_fontsize", 24)
-    )
-    plt.xlabel(
-        plot_params.get("xlabel", ""),
-        fontsize=plot_params.get("xlabel_fontsize", 20)
-    )
-    plt.ylabel(
-        plot_params.get("ylabel", ""),
-        fontsize=plot_params.get("ylabel_fontsize", 20)
-    )
+    plt.title(plot_params.get("title", ""), fontsize=plot_params.get("title_fontsize", 24))
+    plt.xlabel(plot_params.get("xlabel", ""), fontsize=plot_params.get("xlabel_fontsize", 20))
+    plt.ylabel(plot_params.get("ylabel", ""), fontsize=plot_params.get("ylabel_fontsize", 20))
     plt.xticks(fontsize=plot_params.get("xticksize", 24))
     plt.yticks(fontsize=plot_params.get("yticksize", 24))
     start, end = axes.get_xlim()
     stepsize = (end - start) / 5
     axes.xaxis.set_ticks(np.arange(start, end, stepsize))
     axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
     # set y tick stepsize
@@ -211,14 +208,15 @@
     )
     if kwargs.get("show_plot", True):
         pass
     else:
         return axes
 
 
+@check_plot
 def plot_barchart(x, heights, colors, xtick_labels=None, **kwargs):
     """Plot a bar chart
 
     Args:
         x (list or numpy array): X axis grid.
         heights (list or numpy array): Height of the bars.
         colors (list or str): Plot colors.
@@ -244,20 +242,16 @@
     plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
     plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
     plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
     plt.xticks(fontsize=plot_params["xticksize"])
     plt.yticks(fontsize=plot_params["yticksize"])
 
 
-def plot_multiple_barchart(x,
-                           heights,
-                           colors,
-                           legend_labels=None,
-                           xtick_labels=None,
-                           **kwargs):
+@check_plot
+def plot_multiple_barchart(x, heights, colors, legend_labels=None, xtick_labels=None, **kwargs):
     """Plot a bar chart with multiplears per category.
 
     Args:
         x (list or numpy array): X axis grid.
         heights (list or numpy array): Heights of the sets of bars.
             Size of the array is (n_bars_per_xtick, n_xticks),
         colors (list or str): Plot colors. If list supplied,
@@ -281,50 +275,41 @@
         "ylabel": kwargs.pop("ylabel", ""),
         "ylabel_fontsize": kwargs.pop("ylabel_fontsize", 20),
         "xticksize": kwargs.pop("xticksize", 24),
         "yticksize": kwargs.pop("yticksize", 24),
     }
     x = np.array(x)
     heights = np.array(heights)
-    bar_width = kwargs.pop('bar_width', 0.2)
+    bar_width = kwargs.pop("bar_width", 0.2)
     n_bars_per_xtick = heights.shape[0]
     if isinstance(colors, str):
         colors = [colors] * n_bars_per_xtick
     if len(colors) < n_bars_per_xtick:
-        raise InvalidConfigurationError(f'{len(colors)} colors supplied '
-                                        f'insufficient for '
-                                        f'{n_bars_per_xtick} bars')
+        raise InvalidConfigurationError(f"{len(colors)} colors supplied " f"insufficient for " f"{n_bars_per_xtick} bars")
     plt.figure()
     plt.tight_layout()
     plt.rcParams["svg.fonttype"] = "none"
     if xtick_labels is None:
         xtick_labels = x
     bars = []
     for bar_id in range(n_bars_per_xtick):
-        bars.append(plt.bar(x + bar_id*bar_width,
-                            heights[bar_id],
-                            bar_width,
-                            color=colors[bar_id],
-                            **kwargs))
+        bars.append(plt.bar(x + bar_id * bar_width, heights[bar_id], bar_width, color=colors[bar_id], **kwargs))
 
     plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
     plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
     plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
-    plt.xticks(x + bar_width * ((n_bars_per_xtick-1)/2),
-               xtick_labels,
-               fontsize=plot_params["xticksize"])
+    plt.xticks(x + bar_width * ((n_bars_per_xtick - 1) / 2), xtick_labels, fontsize=plot_params["xticksize"])
     plt.yticks(fontsize=plot_params["yticksize"])
     if legend_labels is not None:
         if len(legend_labels) != n_bars_per_xtick:
-            raise InvalidConfigurationError(f'{len(legend_labels)} legend '
-                                            f'labels not sufficient for '
-                                            f'{n_bars_per_xtick} bars')
+            raise InvalidConfigurationError(f"{len(legend_labels)} legend " f"labels not sufficient for " f"{n_bars_per_xtick} bars")
         plt.legend(bars, legend_labels)
 
 
+@check_plot
 def plot_scatter(x, y, outlier_idxs=None, **kwargs):
     """Plot scatter plot of x vs y.
 
     Args:
         x(np.ndarray or list): Values plotted along x axis.
         y(np.ndarray or list): Values plotted along y axis.
 
@@ -357,23 +342,17 @@
             c="r",
         )
     max_entry = max(max(x), max(y)) + plot_params.get("offset", 5.0)
     min_entry = min(min(x), min(y)) - plot_params.get("offset", 5.0)
     axes = plt.gca()
     axes.set_xlim([min_entry, max_entry])
     axes.set_ylim([min_entry, max_entry])
-    plt.title(
-        plot_params.get("title", ""), fontsize=plot_params.get("title_fontsize", 24)
-    )
-    plt.xlabel(
-        plot_params.get("xlabel", ""), fontsize=plot_params.get("xlabel_fontsize", 20)
-    )
-    plt.ylabel(
-        plot_params.get("ylabel", ""), fontsize=plot_params.get("ylabel_fontsize", 20)
-    )
+    plt.title(plot_params.get("title", ""), fontsize=plot_params.get("title_fontsize", 24))
+    plt.xlabel(plot_params.get("xlabel", ""), fontsize=plot_params.get("xlabel_fontsize", 20))
+    plt.ylabel(plot_params.get("ylabel", ""), fontsize=plot_params.get("ylabel_fontsize", 20))
     plt.xticks(fontsize=plot_params.get("xticksize", 24))
     plt.yticks(fontsize=plot_params.get("yticksize", 24))
     start, end = axes.get_xlim()
     stepsize = (end - start) / 5
     axes.xaxis.set_ticks(np.arange(start, end, stepsize))
     axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
     # set y tick stepsize
@@ -383,22 +362,16 @@
     axes.yaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
     if kwargs.get("show_plot", True):
         pass
     else:
         return axes
 
 
-def plot_scatter_interactive(
-    x,
-    y,
-    hover_names=None,
-    outlier_idxs=None,
-    cluster_memberships=None,
-    **kwargs
-):
+@check_plot
+def plot_scatter_interactive(x, y, hover_names=None, outlier_idxs=None, cluster_memberships=None, **kwargs):
     """Plot interactive scatter plot of x vs y.
 
     Args:
         x (np.ndarray or list): Values plotted along x axis.
         y (np.ndarray or list): Values plotted along y axis.
         hover_names (n x 1 np.ndarray): Names of points that will appear
             when cursor is hovered around. Default is None in which case
@@ -406,97 +379,88 @@
         outlier_idxs (list or np.ndarray): List of idx of points which
             corresponds to outliers.
         cluster_memberships (list or np.ndarray): List of cluster
             memberships of all the points.
             Should be the same shape as x or y.
 
     """
-    opacity = kwargs.get('alpha', 0.7)
-    marker_size = kwargs.get('s', 20)
-    plot_color = kwargs.get('plot_color', 'green')
-    outlier_color = kwargs.get('outlier_color', 'red')
-    cluster_colors = kwargs.get('cluster_colors', None)
-    title = kwargs.get('title', None)
-    xlabel = kwargs.get('xlabel', 'Dimension 1')
-    ylabel = kwargs.get('ylabel', 'Dimension 2')
+    opacity = kwargs.get("alpha", 0.7)
+    marker_size = kwargs.get("s", 20)
+    plot_color = kwargs.get("plot_color", "green")
+    outlier_color = kwargs.get("outlier_color", "red")
+    cluster_colors = kwargs.get("cluster_colors", None)
+    title = kwargs.get("title", None)
+    xlabel = kwargs.get("xlabel", "Dimension 1")
+    ylabel = kwargs.get("ylabel", "Dimension 2")
 
     if cluster_memberships is not None:
-        df = pd.DataFrame({
-            'x': x,
-            'y': y,
-            'cluster_memberships': cluster_memberships,
-            'hover_names': hover_names
-        })
+        df = pd.DataFrame({"x": x, "y": y, "cluster_memberships": cluster_memberships, "hover_names": hover_names})
         fig = go.Figure()
         all_cluster_idx = np.unique(cluster_memberships)
-        if cluster_colors is None \
-                or len(cluster_colors) < len(all_cluster_idx):
+        if cluster_colors is None or len(cluster_colors) < len(all_cluster_idx):
             cluster_colors = [None] * len(all_cluster_idx)
 
         for idx, cluster_id in enumerate(all_cluster_idx):
-            cluster_df = df.loc[df['cluster_memberships'] == cluster_id]
-            fig.add_trace(go.Scatter(x=cluster_df['x'].values,
-                                     y=cluster_df['y'].values,
-                                     name=f'cluster {cluster_id}',
-                                     text=cluster_df['hover_names'].values,
-                                     mode='markers',
-                                     marker_size=marker_size,
-                                     marker_color=cluster_colors[idx],
-                                     opacity=opacity,
-                                     marker_symbol='circle',
-                                     marker_line_width=0))
+            cluster_df = df.loc[df["cluster_memberships"] == cluster_id]
+            fig.add_trace(
+                go.Scatter(
+                    x=cluster_df["x"].values,
+                    y=cluster_df["y"].values,
+                    name=f"cluster {cluster_id}",
+                    text=cluster_df["hover_names"].values,
+                    mode="markers",
+                    marker_size=marker_size,
+                    marker_color=cluster_colors[idx],
+                    opacity=opacity,
+                    marker_symbol="circle",
+                    marker_line_width=0,
+                )
+            )
 
     else:
         is_outlier = [0] * len(x)
         if outlier_idxs is not None:
             for id in outlier_idxs:
                 is_outlier[id] = 1
-        df = pd.DataFrame({
-            'x': x,
-            'y': y,
-            'is_outlier': is_outlier,
-            'hover_names': hover_names
-        })
+        df = pd.DataFrame({"x": x, "y": y, "is_outlier": is_outlier, "hover_names": hover_names})
 
         fig = go.Figure()
-        non_outliers = df.loc[df['is_outlier'] == 0]
-        fig.add_trace(go.Scatter(x=non_outliers['x'].values,
-                                 y=non_outliers['y'].values,
-                                 name='molecule',
-                                 text=non_outliers['hover_names'].values,
-                                 mode='markers',
-                                 marker_size=marker_size,
-                                 opacity=opacity,
-                                 marker_color=plot_color,
-                                 marker_symbol='circle',
-                                 marker_line_width=0))
+        non_outliers = df.loc[df["is_outlier"] == 0]
+        fig.add_trace(
+            go.Scatter(
+                x=non_outliers["x"].values,
+                y=non_outliers["y"].values,
+                name="molecule",
+                text=non_outliers["hover_names"].values,
+                mode="markers",
+                marker_size=marker_size,
+                opacity=opacity,
+                marker_color=plot_color,
+                marker_symbol="circle",
+                marker_line_width=0,
+            )
+        )
         if outlier_idxs is not None:
-            outliers = df.loc[df['is_outlier'] == 1]
-            fig.add_trace(go.Scatter(x=outliers['x'].values,
-                                     y=outliers['y'].values,
-                                     name='outlier',
-                                     text=outliers['hover_names'].values,
-                                     mode='markers',
-                                     marker_size=marker_size,
-                                     opacity=opacity,
-                                     marker_color=outlier_color,
-                                     marker_symbol='x',
-                                     marker_line_width=int(marker_size/10),
-                                     marker_line_color='black'))
-    fig.update_layout(
-        xaxis_title=xlabel,
-        yaxis_title=ylabel,
-        font=dict(
-            family="Courier New, monospace",
-            size=40))
+            outliers = df.loc[df["is_outlier"] == 1]
+            fig.add_trace(
+                go.Scatter(
+                    x=outliers["x"].values,
+                    y=outliers["y"].values,
+                    name="outlier",
+                    text=outliers["hover_names"].values,
+                    mode="markers",
+                    marker_size=marker_size,
+                    opacity=opacity,
+                    marker_color=outlier_color,
+                    marker_symbol="x",
+                    marker_line_width=int(marker_size / 10),
+                    marker_line_color="black",
+                )
+            )
+    fig.update_layout(xaxis_title=xlabel, yaxis_title=ylabel, font=dict(family="Courier New, monospace", size=40))
 
     if title is not None:
-        fig.update_layout(title={'text': title,
-                                 'y': 0.9,
-                                 'x': 0.5,
-                                 'xanchor': 'center',
-                                 'yanchor': 'top',
-                                 'font_size': 40})
+        fig.update_layout(title={"text": title, "y": 0.9, "x": 0.5, "xanchor": "center", "yanchor": "top", "font_size": 40})
 
     if hover_names is not None:
         fig.update_traces(hovertemplate="<b>%{text}</b><br><br>")
     fig.show()
```

### Comparing `aimsim-2.1.3/aimsim.egg-info/PKG-INFO` & `aimsim-2.2.0/aimsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aimsim
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python command line and GUI tool to analyze molecular similarity.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: numpy
 Requires-Dist: multiprocess>=0.70
-Requires-Dist: scikit_learn_extra
 Requires-Dist: pandas
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: scikit_learn
 Requires-Dist: rdkit
 Requires-Dist: psutil
 Requires-Dist: padelpy
 Requires-Dist: plotly
@@ -30,22 +29,24 @@
 
 <h1 align="center">AIMSim README</h1> 
 <h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
 
 ![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
   <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/ci.yml/badge.svg?event=schedule">
 </p>
 
+Downloads Stats:
+ - `aimsim`: [![Downloads](https://static.pepy.tech/badge/aimsim)](https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+ - `aimsim_core`: [![Downloads](https://static.pepy.tech/badge/aimsim_core)](https://pepy.tech/project/aimsim_core?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads)
+
 ## Documentation and Tutorial
 [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the _AIMSim_ comprehensive tutorial in your browser:
 <a target="_blank" href="https://colab.research.google.com/github/VlachosGroup/AIMSim/blob/master/AIMSim-demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Purpose
@@ -81,14 +82,18 @@
 
 ## Installing AIMSim
 It is recommended to install `AIMSim` in a virtual environment with [`conda`](https://docs.conda.io/en/latest/) or Python's [`venv`](https://docs.python.org/3/library/venv.html).
 ### `pip`
 `AIMSim` can be installed with a single command using Python's package manager `pip`:
 `pip install aimsim`
 This command also installs the required dependencies.
+
+> [!NOTE]
+> Looking to use AIMSim for descriptor calculation or extend its functionality? `AIMSim`'s core modules for creating molecules, calculating descriptors, and comparing the results are available without support for plotting or visualization in the PyPI package `aimsim_core`.
+
 ### `conda`
 `AIMSim` is also available with the `conda` package manager via:
 `conda install -c conda-forge aimsim`
 This will install all dependencies from `conda-forge`.
 
 ### Note for mordred-descriptor
 AIMSim v1 provided direct support for the descriptors provided in the `mordred` package but unfortunately the original `mordred` is now abandonware.
```

### Comparing `aimsim-2.1.3/aimsim.egg-info/SOURCES.txt` & `aimsim-2.2.0/aimsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AIMSim-GUI.png
 LICENSE
 MANIFEST.in
 README.md
 config.yaml
 implemented_metrics.md
 requirements.txt
+requirements_core.txt
 setup.py
 aimsim/__init__.py
 aimsim/__main__.py
 aimsim/exceptions.py
 aimsim.egg-info/PKG-INFO
 aimsim.egg-info/SOURCES.txt
 aimsim.egg-info/dependency_links.txt
@@ -30,15 +31,14 @@
 aimsim/tasks/measure_search.py
 aimsim/tasks/see_property_variation_with_similarity.py
 aimsim/tasks/task.py
 aimsim/tasks/task_manager.py
 aimsim/tasks/visualize_dataset.py
 aimsim/utils/__init__.py
 aimsim/utils/ccbmlib_fingerprints.py
-aimsim/utils/extras.py
 aimsim/utils/plotting_scripts.py
 docs/_images/AIMSim-logo.png
 docs/_images/sulfonamide-substrate-scope.png
 docs/_static/file.png
 docs/_static/minus.png
 docs/_static/plus.png
 docs/interfaces/UI/AIMSim-logo.png
@@ -46,15 +46,14 @@
 interfaces/__init__.py
 interfaces/config_reader.py
 interfaces/UI/AIMSim-GUI-corner-logo.png
 interfaces/UI/AIMSim-logo.png
 interfaces/UI/AIMSim_ui_main.py
 interfaces/UI/__init__.py
 interfaces/UI/libraries/README.md
-tests/__init__.py
 tests/sulfonamide-substrate-scope-PDF.png
 tests/sulfonamide-substrate-scope.png
 tests/test_CompareTargetMolecule.py
 tests/test_Descriptor.py
 tests/test_LoadingErrorException.py
 tests/test_MeasureSearch.py
 tests/test_Molecule.py
```

### Comparing `aimsim-2.1.3/config.yaml` & `aimsim-2.2.0/config.yaml`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/docs/_images/AIMSim-logo.png` & `aimsim-2.2.0/docs/_images/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/docs/_images/sulfonamide-substrate-scope.png` & `aimsim-2.2.0/docs/_images/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/docs/interfaces/UI/AIMSim-logo.png` & `aimsim-2.2.0/docs/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/docs/tests/sulfonamide-substrate-scope.png` & `aimsim-2.2.0/docs/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/implemented_metrics.md` & `aimsim-2.2.0/implemented_metrics.md`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/interfaces/UI/AIMSim-GUI-corner-logo.png` & `aimsim-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/interfaces/UI/AIMSim-logo.png` & `aimsim-2.2.0/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/interfaces/UI/AIMSim_ui_main.py` & `aimsim-2.2.0/interfaces/UI/AIMSim_ui_main.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/interfaces/config_reader.py` & `aimsim-2.2.0/interfaces/config_reader.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/sulfonamide-substrate-scope-PDF.png` & `aimsim-2.2.0/tests/sulfonamide-substrate-scope-PDF.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/sulfonamide-substrate-scope.png` & `aimsim-2.2.0/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_CompareTargetMolecule.py` & `aimsim-2.2.0/tests/test_CompareTargetMolecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_Descriptor.py` & `aimsim-2.2.0/tests/test_Descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the Descriptor class"""
+
 import unittest
 import numpy as np
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect
 from rdkit.Chem import MolFromSmiles
 from aimsim.ops import Descriptor
 from aimsim.exceptions import MordredCalculatorError, InvalidConfigurationError
-from aimsim.utils.extras import requires_mordred
 
 SUPPORTED_FPRINTS = Descriptor.get_supported_fprints()
 
 
 class TestDescriptor(unittest.TestCase):
     """Tests for methods of the Descriptor class.
 
@@ -39,16 +39,15 @@
         self.assertTrue(
             descriptor.check_init(),
             "Expected Descriptor object to be initialized",
         )
         self.assertEqual(
             descriptor.label_,
             "arbitrary",
-            "Expected label of descriptor initialized with "
-            'arbitrary vector to be "arbitrary"',
+            "Expected label of descriptor initialized with " 'arbitrary vector to be "arbitrary"',
         )
         self.assertIsInstance(
             descriptor.to_numpy(),
             np.ndarray,
             "Expected numpy.ndarray value from to_numpy()",
         )
         self.assertEqual(
@@ -70,33 +69,28 @@
         self.assertTrue(
             descriptor.check_init(),
             "Expected Descriptor object to be initialized",
         )
         self.assertEqual(
             descriptor.label_,
             "arbitrary",
-            "Expected label of descriptor initialized with "
-            'arbitrary vector to be "arbitrary"',
-        )
-        self.assertIsInstance(
-            descriptor.to_numpy(), np.ndarray, "Expected numpy.ndarray from to_numpy()"
+            "Expected label of descriptor initialized with " 'arbitrary vector to be "arbitrary"',
         )
+        self.assertIsInstance(descriptor.to_numpy(), np.ndarray, "Expected numpy.ndarray from to_numpy()")
         self.assertTrue(
             (descriptor.to_numpy() == descriptor_value).all(),
             "Expected descriptor value to match init value",
         )
         with self.assertRaises(ValueError):
             descriptor.to_rdkit()
 
     def test_topological_fprint_min_path_lesser_than_atoms(self):
         atomic_mols = [MolFromSmiles(smiles) for smiles in ["C", "O", "N", "P"]]
         diatomic_mols = [MolFromSmiles(smiles) for smiles in ["CC", "CO", "CN", "CP"]]
-        triatomic_mols = [
-            MolFromSmiles(smiles) for smiles in ["CCC", "COO", "CCN", "CCP"]
-        ]
+        triatomic_mols = [MolFromSmiles(smiles) for smiles in ["CCC", "COO", "CCN", "CCP"]]
         min_path = 1
         for mol in atomic_mols:
             with self.assertRaises(InvalidConfigurationError):
                 descriptor = Descriptor()
                 descriptor.make_fingerprint(
                     molecule_graph=mol,
                     fingerprint_type="topological_fingerprint",
@@ -107,29 +101,25 @@
             try:
                 descriptor.make_fingerprint(
                     molecule_graph=diatomic_mol,
                     fingerprint_type="topological_fingerprint",
                     fingerprint_params={"min_path": min_path},
                 )
             except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
+                self.fail("Did not expect Descriptor to raise " "InvalidConfigurationError")
         for triatomic_mol in triatomic_mols:
             descriptor = Descriptor()
             try:
                 descriptor.make_fingerprint(
                     molecule_graph=triatomic_mol,
                     fingerprint_type="topological_fingerprint",
                     fingerprint_params={"min_path": min_path},
                 )
             except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
+                self.fail("Did not expect Descriptor to raise " "InvalidConfigurationError")
 
         min_path = 2
         for mol in atomic_mols:
             with self.assertRaises(InvalidConfigurationError):
                 descriptor = Descriptor()
                 descriptor.make_fingerprint(
                     molecule_graph=mol,
@@ -149,17 +139,15 @@
             try:
                 descriptor.make_fingerprint(
                     molecule_graph=triatomic_mol,
                     fingerprint_type="topological_fingerprint",
                     fingerprint_params={"min_path": min_path},
                 )
             except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
+                self.fail("Did not expect Descriptor to raise " "InvalidConfigurationError")
 
         min_path = 3
         for mol in atomic_mols:
             with self.assertRaises(InvalidConfigurationError):
                 descriptor = Descriptor()
                 descriptor.make_fingerprint(
                     molecule_graph=mol,
@@ -188,111 +176,94 @@
         Test to verify creation of Descriptor object by
         creating molecular fingerprints from the molecule graph.
 
         """
         mol_graph = MolFromSmiles("CCC")
         for fprint in SUPPORTED_FPRINTS:
             descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type=fprint
-            )
+            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type=fprint)
             self.assertTrue(
                 descriptor.check_init(),
                 "Expected Descriptor object to be initialized",
             )
             self.assertEqual(
                 descriptor.label_,
                 fprint,
-                "Expected label of descriptor initialized with "
-                "fingerprint to match the fingerprint",
+                "Expected label of descriptor initialized with " "fingerprint to match the fingerprint",
             )
             self.assertIsInstance(
                 descriptor.to_numpy(),
                 np.ndarray,
                 "Expected numpy.ndarray from to_numpy()",
             )
             self.assertIsInstance(
                 descriptor.to_rdkit(),
                 ExplicitBitVect,
-                "Expected to_rdkit() to return "
-                "ExplicitBitVect representation "
-                f"of {fprint} fingerprint",
+                "Expected to_rdkit() to return " "ExplicitBitVect representation " f"of {fprint} fingerprint",
             )
 
-    @requires_mordred
     def test_mordred_descriptors(self):
         """Test ability to passthrough descriptors to Mordred."""
-        mol_graph = MolFromSmiles(
-            "CC(C)C1=CC(=C(C(=C1)C(C)C)C2=CC=CC=C2P(C3CCCCC3)C4CCCCC4)C(C)C"
-        )
+        mol_graph = MolFromSmiles("CC(C)C1=CC(=C(C(=C1)C(C)C)C2=CC=CC=C2P(C3CCCCC3)C4CCCCC4)C(C)C")
         for desc in ["MW", "LogEE_Dt", "BalabanJ"]:
             descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="mordred:" + desc
-            )
+            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type="mordred:" + desc)
             self.assertTrue(
                 descriptor.check_init(),
                 "Expected Descriptor object to be initialized",
             )
             self.assertEqual(
                 descriptor.label_,
                 desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
+                "Expected label of descriptor initialized with " "{} to match the fingerprint".format(desc),
             )
             self.assertIsInstance(
                 descriptor.to_numpy(),
                 np.ndarray,
                 "Expected numpy.ndarray from to_numpy()",
             )
             with self.assertRaises(ValueError):
                 descriptor.to_rdkit()
 
     def test_padelpy_descriptors(self):
         """Test ability to passthrough descriptors to PadelPy."""
         mol_graph = MolFromSmiles("CCOCC")
         for desc in ["MATS7e", "Ti", "ATSC6p"]:
             descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="padelpy:" + desc
-            )
+            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type="padelpy:" + desc)
             self.assertTrue(
                 descriptor.check_init(),
                 "Expected Descriptor object to be initialized",
             )
             self.assertEqual(
                 descriptor.label_,
                 desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
+                "Expected label of descriptor initialized with " "{} to match the fingerprint".format(desc),
             )
             self.assertIsInstance(
                 descriptor.to_numpy(),
                 np.ndarray,
                 "Expected numpy.ndarray from to_numpy()",
             )
             with self.assertRaises(ValueError):
                 descriptor.to_rdkit()
 
     def test_minhash_fingerprint(self):
         """Test creation of minhash fingerprint"""
         mol_graph = MolFromSmiles("CCOCC")
         descriptor = Descriptor()
-        descriptor.make_fingerprint(
-            molecule_graph=mol_graph, fingerprint_type="minhash_fingerprint"
-        )
+        descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type="minhash_fingerprint")
         self.assertTrue(
             descriptor.check_init(),
             "Expected Descriptor object to be initialized",
         )
         self.assertEqual(
             descriptor.label_,
             "minhash_fingerprint",
-            "Expected label of descriptor initialized with "
-            "{} to match the fingerprint".format("minhash_fingerprint"),
+            "Expected label of descriptor initialized with " "{} to match the fingerprint".format("minhash_fingerprint"),
         )
         self.assertIsInstance(
             descriptor.to_numpy(),
             np.ndarray,
             "Expected numpy.ndarray from to_numpy()",
         )
         with self.assertRaises(ValueError):
@@ -310,26 +281,23 @@
             "hashed_morgan",
             "rdkit_fingerprint",
             "torsions",
             "hashed_torsions",
         ]
         for desc in fprint_list:
             descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="ccbmlib:" + desc
-            )
+            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type="ccbmlib:" + desc)
             self.assertTrue(
                 descriptor.check_init(),
                 "Expected Descriptor object to be initialized",
             )
             self.assertEqual(
                 descriptor.label_,
                 desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
+                "Expected label of descriptor initialized with " "{} to match the fingerprint".format(desc),
             )
 
     def test_exptl_descriptors(self):
         """Test ability to use experimental descriptors."""
         mol_graph = MolFromSmiles("CCOCC")
         fprint_list = [
             "maccs_keys",
@@ -343,19 +311,17 @@
             self.assertTrue(
                 descriptor.check_init(),
                 "Expected Descriptor object to be initialized",
             )
             self.assertEqual(
                 descriptor.label_,
                 desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
+                "Expected label of descriptor initialized with " "{} to match the fingerprint".format(desc),
             )
 
-    @requires_mordred
     def test_nonexistent_mordred_descriptors(self):
         """Test ability to pass through descriptors to Mordred."""
         mol_graph = MolFromSmiles("C")
         for desc in ["", "ReallyInvalidDescriptorName"]:
             descriptor = Descriptor()
             with self.assertRaises(MordredCalculatorError):
                 descriptor.make_fingerprint(
@@ -393,71 +359,57 @@
         desc = Descriptor()
         desc.label_ = arbit_label
         desc.numpy_ = arbit_vector
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=4)
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=3) == folded_vector).all())
-        )
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=3) == folded_vector).all()))
 
         # Case 3
         arbit_vector = np.array([1, 0, 1, 0, 0, 0, 0, 0])
         folded_once_vector = np.array([1, 0, 1, 0])
         folded_twice_vector = np.array([1, 0])
         arbit_label = "arbitrary_fingerprint"
         desc = Descriptor()
         desc.label_ = arbit_label
         desc.numpy_ = arbit_vector
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=3)
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all()))
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all()))
 
         # Case 3
         arbit_vector = np.array([0, 0, 0, 0, 0, 0, 0, 0])
         folded_once_vector = np.array([0, 0, 0, 0])
         folded_twice_vector = np.array([0, 0])
         arbit_label = "arbitrary_fingerprint"
         desc = Descriptor()
         desc.label_ = arbit_label
         desc.numpy_ = arbit_vector
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=3)
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all()))
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all()))
 
         # Case 4
         arbit_vector = np.array([1, 1, 1, 1, 1, 1, 1, 1])
         folded_once_vector = np.array([1, 1, 1, 1])
         folded_twice_vector = np.array([1, 1])
         arbit_label = "arbitrary_fingerprint"
         desc = Descriptor()
         desc.label_ = arbit_label
         desc.numpy_ = arbit_vector
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=3)
         with self.assertRaises(InvalidConfigurationError):
             desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all()))
+        self.assertTrue(((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all()))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aimsim-2.1.3/tests/test_LoadingErrorException.py` & `aimsim-2.2.0/tests/test_LoadingErrorException.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_MeasureSearch.py` & `aimsim-2.2.0/tests/test_MeasureSearch.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_Molecule.py` & `aimsim-2.2.0/tests/test_Molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_MoleculeSet.py` & `aimsim-2.2.0/tests/test_MoleculeSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1257,14 +1257,15 @@
         features = TSNE(perplexity=len(self.test_smiles) / 2).fit_transform(features)
         with self.assertRaises(InvalidConfigurationError):
             error_matrix = features - molecule_set.get_transformed_descriptors(
                 method_="not a real method"
             )
         remove(csv_fpath)
 
+    @unittest.skip(reason="kmedoids was removed, obsoleting this test")
     def test_clustering_fingerprints(self):
         """
         Test the clustering of molecules featurized by their fingerprints.
 
         """
         csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
         n_clusters = 3
@@ -1286,16 +1287,16 @@
                         n_clusters,
                         "Expected number of cluster labels to be "
                         "less than equal to number of clusters",
                     )
                     if molecule_set.similarity_measure.type_ == "continuous":
                         self.assertEqual(
                             str(molecule_set.clusters_),
-                            "kmedoids",
-                            f"Expected kmedoids clustering for "
+                            "ward",
+                            f"Expected ward clustering for "
                             f"similarity: {similarity_measure}",
                         )
                     else:
                         self.assertEqual(
                             str(molecule_set.clusters_),
                             "complete_linkage",
                             f"Expected complete_linkage clustering"
```

### Comparing `aimsim-2.1.3/tests/test_SimilarityMeasure.py` & `aimsim-2.2.0/tests/test_SimilarityMeasure.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_SimilarityMeasureValueErrors.py` & `aimsim-2.2.0/tests/test_SimilarityMeasureValueErrors.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_TaskManager.py` & `aimsim-2.2.0/tests/test_TaskManager.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_ToolTip.py` & `aimsim-2.2.0/tests/test_ToolTip.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.1.3/tests/test_multithreading.py` & `aimsim-2.2.0/tests/test_multithreading.py`

 * *Files identical despite different names*

