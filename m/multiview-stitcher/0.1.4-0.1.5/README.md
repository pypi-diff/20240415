# Comparing `tmp/multiview-stitcher-0.1.4.tar.gz` & `tmp/multiview_stitcher-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiview-stitcher-0.1.4.tar", last modified: Wed Mar 20 15:14:11 2024, max compression
+gzip compressed data, was "multiview_stitcher-0.1.5.tar", last modified: Mon Apr 15 14:12:59 2024, max compression
```

## Comparing `multiview-stitcher-0.1.4.tar` & `multiview_stitcher-0.1.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.639467 multiview-stitcher-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.619467 multiview-stitcher-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.619467 multiview-stitcher-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/.github/workflows/documentation_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/.github/workflows/documentation_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-03-20 15:14:11.639467 multiview-stitcher-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.623467 multiview-stitcher-0.1.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.623467 multiview-stitcher-0.1.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/api/fusion.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/api/registration.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/api/transformation.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/data_formats.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/docs_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/features.md
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.623467 multiview-stitcher-0.1.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)  1615078 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/images/20230929_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/napari_stitcher.md
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/objects.md
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/docs/related_projects.md
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.627467 multiview-stitcher-0.1.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/notebooks/stitching_bigstitcher_grid_2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   114440 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/notebooks/stitching_multi_view.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/notebooks/stitching_multipos_2D_czi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-20 15:14:11.639467 multiview-stitcher-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.619467 multiview-stitcher-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.627467 multiview-stitcher-0.1.4/src/multiview_stitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.631467 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_mv_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_spatial_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_vis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    29677 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/msi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/mv_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/ngff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37052 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/spatial_image_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.631467 multiview-stitcher-0.1.4/src/multiview_stitcher/test-datasets/
--rw-r--r--   0 runner    (1001) docker     (127)  2791008 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/test-datasets/mosaic_test.czi
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/vis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/src/multiview_stitcher/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:14:11.635467 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 15:14:11.000000 multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-20 15:13:59.000000 multiview-stitcher-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.698665 multiview_stitcher-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.702665 multiview_stitcher-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/documentation_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/documentation_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/fusion.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/registration.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/api/transformation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/data_formats.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/docs_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/features.md
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  1615078 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/images/20230929_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/napari_stitcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/objects.md
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/docs/related_projects.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.706665 multiview_stitcher-0.1.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_2d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   114440 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_multi_view.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/notebooks/stitching_multipos_2D_czi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-15 14:12:59.722665 multiview_stitcher-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.702665 multiview_stitcher-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.710665 multiview_stitcher-0.1.5/src/multiview_stitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.714665 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_mv_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_spatial_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_vis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29677 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/msi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/mv_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/ngff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59895 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/spatial_image_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.714665 multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)  2791008 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/mosaic_test.czi
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/vis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/src/multiview_stitcher/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:12:59.718665 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 14:12:59.000000 multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 14:12:48.000000 multiview_stitcher-0.1.5/tox.ini
```

### Comparing `multiview-stitcher-0.1.4/.github/workflows/documentation_main.yml` & `multiview_stitcher-0.1.5/.github/workflows/documentation_main.yml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/.github/workflows/documentation_release.yml` & `multiview_stitcher-0.1.5/.github/workflows/documentation_release.yml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/.github/workflows/test_and_deploy.yml` & `multiview_stitcher-0.1.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/.gitignore` & `multiview_stitcher-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/.pre-commit-config.yaml` & `multiview_stitcher-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/LICENSE` & `multiview_stitcher-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/PKG-INFO` & `multiview_stitcher-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiview-stitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: Registration and fusion of large imaging datasets in 2D and 3D.
 Home-page: https://github.com/multiview-stitcher/multiview-stitcher
 Author: Marvin Albert
 Author-email: marvin.albert@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/multiview-stitcher/multiview-stitcher/issues
 Project-URL: Documentation, https://github.com/multiview-stitcher/multiview-stitcher#README.md
```

### Comparing `multiview-stitcher-0.1.4/README.md` & `multiview_stitcher-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/data_formats.md` & `multiview_stitcher-0.1.5/docs/data_formats.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/docs_requirements.txt` & `multiview_stitcher-0.1.5/docs/docs_requirements.txt`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/features.md` & `multiview_stitcher-0.1.5/docs/features.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/images/20230929_screenshot.png` & `multiview_stitcher-0.1.5/docs/images/20230929_screenshot.png`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/implementation_details.md` & `multiview_stitcher-0.1.5/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/index.md` & `multiview_stitcher-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/docs/objects.md` & `multiview_stitcher-0.1.5/docs/objects.md`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/mkdocs.yml` & `multiview_stitcher-0.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/notebooks/stitching_bigstitcher_grid_2d.ipynb` & `multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_2d.ipynb`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb` & `multiview_stitcher-0.1.5/notebooks/stitching_bigstitcher_grid_3d_ngff.ipynb`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/notebooks/stitching_multi_view.ipynb` & `multiview_stitcher-0.1.5/notebooks/stitching_multi_view.ipynb`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/notebooks/stitching_multipos_2D_czi.ipynb` & `multiview_stitcher-0.1.5/notebooks/stitching_multipos_2D_czi.ipynb`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/pyproject.toml` & `multiview_stitcher-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/setup.cfg` & `multiview_stitcher-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_fusion.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_integration.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_io.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_io.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_mv_graph.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_mv_graph.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_sample_data.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_sample_data.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_spatial_image_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_spatial_image_utils.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/_tests/test_vis_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/_tests/test_vis_utils.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/fusion.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/fusion.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/io.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/io.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/msi_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/msi_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,41 @@
     """
     for scale_key in get_sorted_scale_keys(msim):
         if "chunks" in msim[scale_key]["image"].encoding:
             del msim[scale_key]["image"].encoding["chunks"]
     msim.to_zarr(path)
 
 
+def complete_msim_zarr(msim, path):
+    """
+    Complete zarr store with data from msim that doesn't exist in store.
+    """
+
+    path = Path(path)
+
+    if not path.exists():
+        raise ValueError("Path does not exist")
+        # multiscale_spatial_image_to_zarr(msim, path)
+        # return
+
+    msim_disk = multiscale_spatial_image_from_zarr(path)
+
+    for scale_key in get_sorted_scale_keys(msim):
+        if scale_key in msim_disk:
+            ds = xr.open_zarr(path, group=scale_key)
+            ds_diff = xr.Dataset(msim[scale_key].drop_vars(ds.data_vars))
+            ds_diff.to_zarr(path, group=scale_key, mode="a")
+
+        else:
+            ds.to_zarr(
+                path,
+                group=scale_key,
+            )
+
+
 def get_optimal_multi_scale_factors_from_sim(sim, min_size=512):
     """
     This is currently simply downscaling z and xy until a minimum size is reached.
     Probably it'd make more sense to downscale considering the dims spacing.
     """
 
     spatial_dims = si_utils.get_spatial_dims_from_sim(sim)
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/mv_graph.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/mv_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import copy
 import warnings
 from collections.abc import Iterable
 from itertools import chain
 
 import networkx as nx
 import numpy as np
 import xarray as xr
 from dask import compute, delayed
 from scipy.spatial import cKDTree
 from skimage.filters import threshold_otsu
 
-from multiview_stitcher import msi_utils, spatial_image_utils
+from multiview_stitcher import msi_utils, spatial_image_utils, transformation
 from multiview_stitcher.fusion import fuse
 from multiview_stitcher.misc_utils import DisableLogger
 
 with DisableLogger():
     from Geometry3D import (
         ConvexPolygon,
         ConvexPolyhedron,
@@ -261,15 +262,15 @@
             n: g.nodes[n][node_attribute]
             for n in g.nodes
             if node_attribute in g.nodes[n]
         }
     )
 
 
-def get_vertices_from_stack_props(stack_props):
+def get_faces_from_stack_props(stack_props):
     """
     Get sim stack corners in world coordinates.
     """
     ndim = len(stack_props["origin"])
     sdims = ["z", "y", "x"][-ndim:]
 
     gv = np.array(list(np.ndindex(tuple([2] * ndim))))
@@ -298,14 +299,37 @@
         ).T[:, :-1]
 
         faces = faces.reshape(orig_shape)
 
     return faces
 
 
+def get_vertices_from_stack_props(stack_props):
+    """
+    Get sim stack corners in world coordinates.
+    """
+    ndim = len(stack_props["origin"])
+    sdims = ["z", "y", "x"][-ndim:]
+
+    gv = np.array(list(np.ndindex(tuple([2] * ndim))))
+
+    vertices = gv * (
+        np.array([stack_props["shape"][dim] for dim in sdims]) - 1
+    ) * np.array([stack_props["spacing"][dim] for dim in sdims]) + np.array(
+        [stack_props["origin"][dim] for dim in sdims]
+    )
+
+    if "transform" in stack_props:
+        vertices = transformation.transform_pts(
+            vertices, stack_props["transform"]
+        )
+
+    return vertices
+
+
 def sims_are_far_apart(sim1, sim2, transform_key):
     """ """
 
     centers = [
         spatial_image_utils.get_center_of_sim(sim, transform_key=transform_key)
         for sim in [sim1, sim2]
     ]
@@ -364,15 +388,16 @@
         return None
 
     ndim = len(stack_props_1["origin"])
 
     cphs = []
     facess = []
     for stack_props in [stack_props_1, stack_props_2]:
-        faces = get_vertices_from_stack_props(stack_props)
+        # faces = get_vertices_from_stack_props(stack_props)
+        faces = get_faces_from_stack_props(stack_props)
         cps = get_poly_from_stack_props(stack_props)
 
         facess.append(faces.reshape((-1, ndim)))
         cphs.append(cps)
 
     if ndim == 3 and (
         min([any((f == facess[0]).all(1)) for f in facess[1]])
@@ -416,27 +441,78 @@
         corners = np.unique(
             get_vertices_from_stack_props(stack_props).reshape((-1, 2)),
             axis=0,
         )
         sim_domain = ConvexPolygon([Point([0] + list(c)) for c in corners])
 
     elif ndim == 3:
-        faces = get_vertices_from_stack_props(stack_props)
+        # faces = get_vertices_from_stack_props(stack_props)
+        faces = get_faces_from_stack_props(stack_props)
         sim_domain = ConvexPolyhedron(
             [ConvexPolygon([Point(c) for c in face]) for face in faces]
         )
 
     return sim_domain
 
 
+# def get_greedy_colors(sims, n_colors=2, transform_key=None):
+#     """
+#     Get colors (indices) from view adjacency graph analysis
+
+#     Idea: use the same logic to determine relevant registration edges
+#     """
+
+#     view_adj_graph = build_view_adjacency_graph_from_msims(
+#         [msi_utils.get_msim_from_sim(sim, scale_factors=[]) for sim in sims],
+#         expand=True,
+#         transform_key=transform_key,
+#     )
+
+#     # thresholds = threshold_multiotsu(overlaps)
+
+#     # strategy: remove edges with overlap values of increasing thresholds until
+#     # the graph division into n_colors is successful
+
+#     # modify overlap values
+#     # strategy: add a small amount to edge overlap depending on how many edges the nodes it connects have (betweenness?)
+
+#     edge_vals = nx.edge_betweenness_centrality(view_adj_graph)
+
+#     edges = list(view_adj_graph.edges(data=True))
+#     for e in edges:
+#         edge_vals[tuple(e[:2])] = edge_vals[tuple(e[:2])] + e[2]["overlap"]
+
+#     sorted_unique_vals = sorted(np.unique(list(edge_vals.values())))
+
+#     nx.set_edge_attributes(view_adj_graph, edge_vals, name="edge_val")
+
+#     thresh_ind = 0
+#     while 1:
+#         colors = nx.coloring.greedy_color(view_adj_graph)
+#         if (
+#             len(set(colors.values())) <= n_colors
+#         ):  # and nx.coloring.equitable_coloring.is_equitable(view_adj_graph, colors):
+#             break
+#         view_adj_graph.remove_edges_from(
+#             [
+#                 (a, b)
+#                 for a, b, attrs in view_adj_graph.edges(data=True)
+#                 if attrs["edge_val"] <= sorted_unique_vals[thresh_ind]
+#             ]
+#         )
+#         thresh_ind += 1
+
+#     greedy_colors = dict(colors.items())
+
+#     return greedy_colors
+
+
 def get_greedy_colors(sims, n_colors=2, transform_key=None):
     """
     Get colors (indices) from view adjacency graph analysis
-
-    Idea: use the same logic to determine relevant registration edges
     """
 
     view_adj_graph = build_view_adjacency_graph_from_msims(
         [msi_utils.get_msim_from_sim(sim, scale_factors=[]) for sim in sims],
         expand=True,
         transform_key=transform_key,
     )
@@ -445,43 +521,76 @@
 
     # strategy: remove edges with overlap values of increasing thresholds until
     # the graph division into n_colors is successful
 
     # modify overlap values
     # strategy: add a small amount to edge overlap depending on how many edges the nodes it connects have (betweenness?)
 
-    edge_vals = nx.edge_betweenness_centrality(view_adj_graph)
+    view_adj_graph_pruned, greedy_colors = prune_graph_to_alternating_colors(
+        view_adj_graph, n_colors=n_colors
+    )
+
+    return greedy_colors
+
+
+def prune_graph_to_alternating_colors(g, n_colors=2, return_colors=True):
+    """
+    Prune a graph
+
+    Parameters
+    ----------
+    g : nx.Graph
+        Graph containing edges with overlap values
+    n_colors : int, optional
+    return_colors : bool, optional
+
+    Returns
+    -------
+    nx.Graph
+        Pruned graph
+    """
+
+    # strategy: remove edges with overlap values of increasing thresholds until
+    # the graph division into n_colors is successful
+
+    # modify overlap values
+    # strategy: add a small amount to edge overlap depending on how many edges the nodes it connects have (betweenness?)
+
+    g_pruned = copy.deepcopy(g)
+
+    edge_vals = nx.edge_betweenness_centrality(g)
 
-    edges = list(view_adj_graph.edges(data=True))
+    edges = list(g_pruned.edges(data=True))
     for e in edges:
         edge_vals[tuple(e[:2])] = edge_vals[tuple(e[:2])] + e[2]["overlap"]
 
     sorted_unique_vals = sorted(np.unique(list(edge_vals.values())))
 
-    nx.set_edge_attributes(view_adj_graph, edge_vals, name="edge_val")
+    # nx.set_edge_attributes(g, edge_vals, name="edge_val")
 
     thresh_ind = 0
     while 1:
-        colors = nx.coloring.greedy_color(view_adj_graph)
+        colors = nx.coloring.greedy_color(g_pruned)
         if (
             len(set(colors.values())) <= n_colors
-        ):  # and nx.coloring.equitable_coloring.is_equitable(view_adj_graph, colors):
+        ):  # and nx.coloring.equitable_coloring.is_equitable(g_pruned, colors):
             break
-        view_adj_graph.remove_edges_from(
+        g_pruned.remove_edges_from(
             [
                 (a, b)
-                for a, b, attrs in view_adj_graph.edges(data=True)
-                if attrs["edge_val"] <= sorted_unique_vals[thresh_ind]
+                for a, b, attrs in g_pruned.edges(data=True)
+                if edge_vals[(a, b)] <= sorted_unique_vals[thresh_ind]
             ]
         )
         thresh_ind += 1
 
-    greedy_colors = dict(colors.items())
-
-    return greedy_colors
+    if return_colors:
+        return g_pruned, colors
+    else:
+        return g_pruned
 
 
 def prune_to_shortest_weighted_paths(g):
     """
     g contains the overlap between views as edge weights
 
     Strategy:
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/ngff_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/ngff_utils.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/param_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/param_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,28 @@
     M = np.eye(ndim + 1)
     M[:ndim, :ndim] = linear_affine[: ndim**2].reshape((ndim, ndim))
     M[:ndim, ndim] = linear_affine[-ndim:]
 
     return M
 
 
+def linear_affine_from_affine(affine):
+    """
+    Return linear representation of affine matrix from affine matrix.
+    """
+    ndim = affine.shape[-1] - 1
+
+    linear_affine = np.zeros(ndim**2 + ndim, dtype=float)
+
+    linear_affine[: ndim**2] = affine[:ndim, :ndim].flatten()
+    linear_affine[-ndim:] = affine[:ndim, ndim]
+
+    return linear_affine
+
+
 def translation_from_affine(affine):
     """
     Return matrix in homogeneous coords representing a translation.
     """
     ndim = len(affine) - 1
     t = affine[:ndim, ndim]
     return t
@@ -105,15 +119,24 @@
 
 
 def get_xparam_from_param(params):
     """
     Homogeneous matrix to xparams
     """
 
-    xparam = xr.DataArray(params, dims=["x_in", "x_out"])
+    ndim = params.shape[-1] - 1
+
+    xparam = xr.DataArray(
+        params,
+        dims=["x_in", "x_out"],
+        coords={
+            "x_in": ["z", "y", "x"][-ndim:] + ["1"],
+            "x_out": ["z", "y", "x"][-ndim:] + ["1"],
+        },
+    )
 
     return xparam
 
 
 def rebase_affine(xaffine, base_affine):
     """
     Take two xr.DataArrays of affine transforms and
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/sample_data.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/sample_data.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/spatial_image_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/spatial_image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,18 @@
     Returns
     -------
     spatial_image.SpatialImage
         spatial-image with multiview-stitcher flavor
         (SpatialImage + affine transform attributes)
     """
 
-    assert len(dims) == array.ndim
+    if dims is None:
+        dims = ["t", "c", "z", "y", "x"][-array.ndim :]
+    else:
+        assert len(dims) == array.ndim
 
     xim = xr.DataArray(
         array,
         dims=dims,
     )
 
     nsdims = ["c", "t"]
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/test-datasets/mosaic_test.czi` & `multiview_stitcher-0.1.5/src/multiview_stitcher/test-datasets/mosaic_test.czi`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/transformation.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/transformation.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/vis_utils.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/vis_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     sims = [msi_utils.get_sim_from_msim(msim) for msim in msims]
 
     # select a single position for non-spatial dimensions
     for isim, sim in enumerate(sims):
         sdims = spatial_image_utils.get_spatial_dims_from_sim(sim)
         nsdims = [dim for dim in sim.dims if dim not in sdims]
         for nsdim in nsdims:
-            if nsdim in sim.dims and len(sim.coords[nsdim]) > 1:
+            # if nsdim in sim.dims and len(sim.coords[nsdim]) > 1:
+            if nsdim in sim.dims:
                 if nsdim not in nscoord:
                     nscoord[nsdim] = sim.coords[nsdim][0]
                 sims[isim] = spatial_image_utils.sim_sel_coords(sim, nscoord)
 
     if use_positional_colors:
         pos_colors = ["red", "green", "blue", "yellow"]
         greedy_colors = mv_graph.get_greedy_colors(
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher/weights.py` & `multiview_stitcher-0.1.5/src/multiview_stitcher/weights.py`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/PKG-INFO` & `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiview-stitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: Registration and fusion of large imaging datasets in 2D and 3D.
 Home-page: https://github.com/multiview-stitcher/multiview-stitcher
 Author: Marvin Albert
 Author-email: marvin.albert@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/multiview-stitcher/multiview-stitcher/issues
 Project-URL: Documentation, https://github.com/multiview-stitcher/multiview-stitcher#README.md
```

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/SOURCES.txt` & `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/src/multiview_stitcher.egg-info/requires.txt` & `multiview_stitcher-0.1.5/src/multiview_stitcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `multiview-stitcher-0.1.4/tox.ini` & `multiview_stitcher-0.1.5/tox.ini`

 * *Files identical despite different names*

