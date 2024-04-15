# Comparing `tmp/paicos-0.1.8.tar.gz` & `tmp/paicos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicos-0.1.8.tar", last modified: Sun Jan 21 15:25:20 2024, max compression
+gzip compressed data, was "paicos-0.1.9.tar", last modified: Wed Apr 10 08:54:52 2024, max compression
```

## Comparing `paicos-0.1.8.tar` & `paicos-0.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.247889 paicos-0.1.8/
--rw-r--r--   0 berlok     (501) staff       (20)     1528 2023-11-01 15:21:45.000000 paicos-0.1.8/LICENSE.txt
--rw-r--r--   0 berlok     (501) staff       (20)       40 2024-01-21 15:16:27.000000 paicos-0.1.8/MANIFEST.in
--rw-r--r--   0 berlok     (501) staff       (20)     1638 2024-01-21 15:25:20.247724 paicos-0.1.8/PKG-INFO
--rw-r--r--   0 berlok     (501) staff       (20)     1138 2024-01-19 15:45:58.000000 paicos-0.1.8/README.md
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.242831 paicos-0.1.8/paicos/
--rw-r--r--   0 berlok     (501) staff       (20)     7548 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/__init__.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.244398 paicos-0.1.8/paicos/cython/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-11-02 13:10:45.000000 paicos-0.1.8/paicos/cython/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)     4623 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/cython/get_derived_variables.pyx
--rw-r--r--   0 berlok     (501) staff       (20)     7847 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/cython/get_index_of_region.pyx
--rw-r--r--   0 berlok     (501) staff       (20)     5231 2023-11-01 15:21:45.000000 paicos-0.1.8/paicos/cython/histogram.pyx
--rw-r--r--   0 berlok     (501) staff       (20)      876 2023-02-09 10:55:33.000000 paicos-0.1.8/paicos/cython/openmp_info.pyx
--rw-r--r--   0 berlok     (501) staff       (20)    15853 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/cython/sph_projectors.pyx
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.244757 paicos-0.1.8/paicos/derived_variables/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/derived_variables/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)      323 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/derived_variables/derived_variables.py
--rw-r--r--   0 berlok     (501) staff       (20)     9346 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/derived_variables/derived_variables_gas.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.245047 paicos-0.1.8/paicos/histograms/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/histograms/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)     3579 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/histograms/histogram.py
--rw-r--r--   0 berlok     (501) staff       (20)    10283 2023-11-01 15:21:45.000000 paicos-0.1.8/paicos/histograms/histogram2D.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.246182 paicos-0.1.8/paicos/image_creators/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/image_creators/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)    12920 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/gpu_ray_projector.py
--rw-r--r--   0 berlok     (501) staff       (20)    15751 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/gpu_sph_projector.py
--rw-r--r--   0 berlok     (501) staff       (20)    13436 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/image_creator.py
--rw-r--r--   0 berlok     (501) staff       (20)     9058 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/nested_projector.py
--rw-r--r--   0 berlok     (501) staff       (20)     9097 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/projector.py
--rw-r--r--   0 berlok     (501) staff       (20)     7412 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/slicer.py
--rw-r--r--   0 berlok     (501) staff       (20)    11660 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/image_creators/tree_projector.py
--rw-r--r--   0 berlok     (501) staff       (20)    10979 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/orientation.py
--rw-r--r--   0 berlok     (501) staff       (20)      592 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/paicos_user_settings.py
--rw-r--r--   0 berlok     (501) staff       (20)     1100 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/paicos_user_settings_template.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.246663 paicos-0.1.8/paicos/readers/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/readers/__init__.py
--rwxr-xr-x   0 berlok     (501) staff       (20)     6471 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/readers/arepo_catalog.py
--rwxr-xr-x   0 berlok     (501) staff       (20)    39307 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/readers/arepo_snap.py
--rw-r--r--   0 berlok     (501) staff       (20)    25712 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/readers/paicos_readers.py
--rw-r--r--   0 berlok     (501) staff       (20)      813 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/settings.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.247119 paicos-0.1.8/paicos/trees/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/trees/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)    17935 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/trees/bvh_cpu.py
--rw-r--r--   0 berlok     (501) staff       (20)    17194 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/trees/bvh_gpu.py
--rw-r--r--   0 berlok     (501) staff       (20)      536 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/trees/bvh_tree.pyx
--rw-r--r--   0 berlok     (501) staff       (20)     7053 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/unit_specifications.py
--rw-r--r--   0 berlok     (501) staff       (20)    26319 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/units.py
--rw-r--r--   0 berlok     (501) staff       (20)    13926 2024-01-21 15:16:27.000000 paicos-0.1.8/paicos/util.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.247469 paicos-0.1.8/paicos/writers/
--rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.8/paicos/writers/__init__.py
--rw-r--r--   0 berlok     (501) staff       (20)     4811 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/writers/arepo_image.py
--rw-r--r--   0 berlok     (501) staff       (20)     5988 2024-01-19 15:45:58.000000 paicos-0.1.8/paicos/writers/paicos_writer.py
-drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-01-21 15:25:20.243544 paicos-0.1.8/paicos.egg-info/
--rw-r--r--   0 berlok     (501) staff       (20)     1638 2024-01-21 15:25:20.000000 paicos-0.1.8/paicos.egg-info/PKG-INFO
--rw-r--r--   0 berlok     (501) staff       (20)     1437 2024-01-21 15:25:20.000000 paicos-0.1.8/paicos.egg-info/SOURCES.txt
--rw-r--r--   0 berlok     (501) staff       (20)        1 2024-01-21 15:25:20.000000 paicos-0.1.8/paicos.egg-info/dependency_links.txt
--rw-r--r--   0 berlok     (501) staff       (20)       31 2024-01-21 15:25:20.000000 paicos-0.1.8/paicos.egg-info/requires.txt
--rw-r--r--   0 berlok     (501) staff       (20)        7 2024-01-21 15:25:20.000000 paicos-0.1.8/paicos.egg-info/top_level.txt
--rw-r--r--   0 berlok     (501) staff       (20)      120 2023-12-15 18:48:12.000000 paicos-0.1.8/pyproject.toml
--rw-r--r--   0 berlok     (501) staff       (20)       38 2024-01-21 15:25:20.247927 paicos-0.1.8/setup.cfg
--rw-r--r--   0 berlok     (501) staff       (20)     3355 2024-01-21 15:16:27.000000 paicos-0.1.8/setup.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.870746 paicos-0.1.9/
+-rw-r--r--   0 berlok     (501) staff       (20)    35149 2024-04-10 08:41:37.000000 paicos-0.1.9/LICENSE.txt
+-rw-r--r--   0 berlok     (501) staff       (20)       40 2024-01-21 15:16:27.000000 paicos-0.1.9/MANIFEST.in
+-rw-r--r--   0 berlok     (501) staff       (20)     2183 2024-04-10 08:54:52.870562 paicos-0.1.9/PKG-INFO
+-rw-r--r--   0 berlok     (501) staff       (20)     1561 2024-04-10 08:41:37.000000 paicos-0.1.9/README.md
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.862332 paicos-0.1.9/paicos/
+-rw-r--r--   0 berlok     (501) staff       (20)     9311 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/__init__.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.863733 paicos-0.1.9/paicos/cython/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-11-02 13:10:45.000000 paicos-0.1.9/paicos/cython/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)     4874 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/cython/get_derived_variables.pyx
+-rw-r--r--   0 berlok     (501) staff       (20)    12355 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/cython/get_index_of_region.pyx
+-rw-r--r--   0 berlok     (501) staff       (20)     5616 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/cython/histogram.pyx
+-rw-r--r--   0 berlok     (501) staff       (20)     1207 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/cython/openmp_info.pyx
+-rw-r--r--   0 berlok     (501) staff       (20)    16581 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/cython/sph_projectors.pyx
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.864163 paicos-0.1.9/paicos/derived_variables/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/derived_variables/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)      323 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/derived_variables/derived_variables.py
+-rw-r--r--   0 berlok     (501) staff       (20)     9384 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/derived_variables/derived_variables_gas.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.864639 paicos-0.1.9/paicos/histograms/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/histograms/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)     3583 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/histograms/histogram.py
+-rw-r--r--   0 berlok     (501) staff       (20)    10710 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/histograms/histogram2D.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.866711 paicos-0.1.9/paicos/image_creators/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/image_creators/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)    12920 2024-03-13 08:54:10.000000 paicos-0.1.9/paicos/image_creators/gpu_ray_projector.py
+-rw-r--r--   0 berlok     (501) staff       (20)    15751 2024-03-09 19:32:19.000000 paicos-0.1.9/paicos/image_creators/gpu_sph_projector.py
+-rw-r--r--   0 berlok     (501) staff       (20)    15900 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/image_creators/image_creator.py
+-rw-r--r--   0 berlok     (501) staff       (20)     9271 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/image_creators/nested_projector.py
+-rw-r--r--   0 berlok     (501) staff       (20)     9198 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/image_creators/projector.py
+-rw-r--r--   0 berlok     (501) staff       (20)     7632 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/image_creators/slicer.py
+-rw-r--r--   0 berlok     (501) staff       (20)    12329 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/image_creators/tree_projector.py
+-rw-r--r--   0 berlok     (501) staff       (20)    11772 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/orientation.py
+-rw-r--r--   0 berlok     (501) staff       (20)     1159 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/paicos_user_settings_template.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.868436 paicos-0.1.9/paicos/readers/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/readers/__init__.py
+-rwxr-xr-x   0 berlok     (501) staff       (20)     9173 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/readers/arepo_catalog.py
+-rwxr-xr-x   0 berlok     (501) staff       (20)    40374 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/readers/arepo_snap.py
+-rw-r--r--   0 berlok     (501) staff       (20)     6759 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/readers/generic_snap.py
+-rw-r--r--   0 berlok     (501) staff       (20)    28011 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/readers/paicos_readers.py
+-rw-r--r--   0 berlok     (501) staff       (20)      814 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/settings.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.869526 paicos-0.1.9/paicos/trees/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2024-01-21 15:16:27.000000 paicos-0.1.9/paicos/trees/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)    17935 2024-01-19 15:45:58.000000 paicos-0.1.9/paicos/trees/bvh_cpu.py
+-rw-r--r--   0 berlok     (501) staff       (20)    17194 2024-01-21 15:16:27.000000 paicos-0.1.9/paicos/trees/bvh_gpu.py
+-rw-r--r--   0 berlok     (501) staff       (20)      536 2024-01-19 15:45:58.000000 paicos-0.1.9/paicos/trees/bvh_tree.pyx
+-rw-r--r--   0 berlok     (501) staff       (20)     7597 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/unit_specifications.py
+-rw-r--r--   0 berlok     (501) staff       (20)    27162 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/units.py
+-rw-r--r--   0 berlok     (501) staff       (20)    15151 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/util.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.869976 paicos-0.1.9/paicos/writers/
+-rw-r--r--   0 berlok     (501) staff       (20)        0 2023-02-16 13:21:53.000000 paicos-0.1.9/paicos/writers/__init__.py
+-rw-r--r--   0 berlok     (501) staff       (20)     5123 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/writers/arepo_image.py
+-rw-r--r--   0 berlok     (501) staff       (20)     6039 2024-04-10 08:41:37.000000 paicos-0.1.9/paicos/writers/paicos_writer.py
+drwxr-xr-x   0 berlok     (501) staff       (20)        0 2024-04-10 08:54:52.863057 paicos-0.1.9/paicos.egg-info/
+-rw-r--r--   0 berlok     (501) staff       (20)     2183 2024-04-10 08:54:52.000000 paicos-0.1.9/paicos.egg-info/PKG-INFO
+-rw-r--r--   0 berlok     (501) staff       (20)     1437 2024-04-10 08:54:52.000000 paicos-0.1.9/paicos.egg-info/SOURCES.txt
+-rw-r--r--   0 berlok     (501) staff       (20)        1 2024-04-10 08:54:52.000000 paicos-0.1.9/paicos.egg-info/dependency_links.txt
+-rw-r--r--   0 berlok     (501) staff       (20)       63 2024-04-10 08:54:52.000000 paicos-0.1.9/paicos.egg-info/requires.txt
+-rw-r--r--   0 berlok     (501) staff       (20)        7 2024-04-10 08:54:52.000000 paicos-0.1.9/paicos.egg-info/top_level.txt
+-rw-r--r--   0 berlok     (501) staff       (20)      120 2024-03-08 19:17:54.000000 paicos-0.1.9/pyproject.toml
+-rw-r--r--   0 berlok     (501) staff       (20)       38 2024-04-10 08:54:52.870781 paicos-0.1.9/setup.cfg
+-rw-r--r--   0 berlok     (501) staff       (20)     3534 2024-04-10 08:41:37.000000 paicos-0.1.9/setup.py
```

### Comparing `paicos-0.1.8/PKG-INFO` & `paicos-0.1.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-Metadata-Version: 2.1
-Name: paicos
-Version: 0.1.8
-Summary: An object-oriented Python package for analysis of (cosmological) simulations performed with Arepo.
-Home-page: https://github.com/tberlok/paicos
-Author: Thomas Berlok
-Author-email: tberlok@gmail.com
-License: BSD 3-clause
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: h5py
-Requires-Dist: astropy
-Requires-Dist: numba
-
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/tberlok/paicos/tree/main.svg?style=svg&circle-token=dbdb37aa907d919a167a8ef5ccf197c0d358c300)](https://dl.circleci.com/status-badge/redirect/gh/tberlok/paicos/tree/main)
 [![pylint](https://github.com/tberlok/paicos/actions/workflows/pylint.yml/badge.svg)](
 https://github.com/tberlok/paicos/actions/workflows/pylint.yml)
 [![flake8](https://github.com/tberlok/paicos/actions/workflows/flake8.yml/badge.svg)](
 https://github.com/tberlok/paicos/actions/workflows/flake8.yml)
 [![Documentation Status](https://readthedocs.org/projects/paicos/badge/?version=latest)](https://paicos.readthedocs.io/en/latest/?badge=latest)
 
 
 # Paicos
 
-A somewhat bare-bones Python package for making projections and slices of
-Arepo simulations. Please note that while Paicos has its visibility set to
-public, it is still in beta mode and under active development.
+An object-oriented Python package for analysis of (cosmological) simulations performed
+with Arepo.
 
 <img src="images/Z24_snap130_wide_projection_notnested.jpg" width="auto">
 
 
-# Documentation
+# Documentation and asking for help
 
 Installation instructions and tips on how to get started can be found
 on [readthedocs](https://paicos.readthedocs.io/en/latest/?badge=latest).
 
+If you have questions not answered there or if you simply can't get things working, then please feel free to create an issue or to send an email to tberlok ad nbi.ku.dk.
+
+# Reporting issues and/or requesting features
+
+Paicos uses GitHub Issues to track bugs and feature requests. Please search the existing issues before filing new issues to avoid duplicates.
 
+# Contributing 
+Contributions are very welcome indeed! Please see instructions [here](https://github.com/tberlok/paicos/blob/main/.github/CONTRIBUTING.md).
```

### Comparing `paicos-0.1.8/paicos/__init__.py` & `paicos-0.1.9/paicos/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 handling of units, derived variables, loading of data upon request.
 
 The module includes a way of writing and reading data with units.
 The code is parallel with an OpenMP Cython implementation
 and a CUDA GPU implementation for visualization.
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = 'Thomas Berlok'
 __credits__ = 'Niels Bohr Institute, University of Copenhagen'
 
 # Dependencies
 import os
 import numpy
 import scipy
@@ -26,14 +26,16 @@
 # One folder up from __init__ (i.e. repo directory or installation directory)
 from .util import root_dir
 
 # HDF5 file readers
 from .readers.arepo_snap import Snapshot
 from .readers.arepo_catalog import Catalog
 from .readers.paicos_readers import PaicosReader, ImageReader, Histogram2DReader
+from .readers.generic_snap import GenericSnapshot
+
 
 # HDF5 file writers
 from .writers.paicos_writer import PaicosWriter, PaicosTimeSeriesWriter
 from .writers.arepo_image import ArepoImage
 
 # Image creators
 from .image_creators.image_creator import ImageCreator
@@ -54,41 +56,75 @@
 
 # Cython functions
 from . import cython
 
 # pylint: disable=W0621
 
 # The place where __init__.py (this file) is located
-code_dir = os.path.dirname(os.path.abspath(__file__))
+code_dir = os.path.dirname(os.path.abspath(__file__)) + '/'
 
 
 def use_units(use_units):
     """
-    pa.use_units(True) turns on paicos quantities globally
-    pa.use_units(False) loads in data without applying units.
+    Parameters
+    ----------
+
+    use_units : bool
+        True for enabling units globally and False for disabling
+        them globally.
+        Note that this will not modify snapshots that have
+        already been loaded.
+
+    Examples
+    --------
+
+    An example::
+
+        import paicos as pa
+        print('Using units:', pa.settings.use_units)
+
+        # Turn on paicos quantities globally
+        pa.use_units(True)
+        print('Using units:', pa.settings.use_units)
+
+        # Loads in data without applying units.
+        pa.use_units(False)
+        print('Using units:', pa.settings.use_units)
 
-    The status can be seen in pa.settings.use_units
     """
     settings.use_units = use_units
 
 
 def add_user_function(variable_string, function):
     """
     This functions allows to enable user functions for obtaining
-    deriving variables. An example could be the following:
+    deriving variables. An example could be the following::
 
-    def TemperaturesTimesMassesSquared(snap, get_depencies=False):
-        if get_depencies:
-            return ['0_Temperatures', '0_Masses']
-        return snap['0_Temperatures'] * snap['0_Masses']**2
+        def TemperaturesTimesMassesSquared(snap, get_depencies=False):
+            if get_depencies:
+                return ['0_Temperatures', '0_Masses']
+            return snap['0_Temperatures'] * snap['0_Masses']**2
 
 
-    pa.add_user_function('0_TM2', TemperaturesTimesMassesSquared)
+        pa.add_user_function('0_TM2', TemperaturesTimesMassesSquared)
 
     """
+    from inspect import signature
+    if ' ' in variable_string:
+        raise RuntimeError(f'{variable_string} contains space(s)!')
+
+    sig = signature(function)
+    if len(sig.parameters) == 2:
+        dependencies = function(None, True)
+        assert isinstance(dependencies, list)
+        err_msg = 'Problem with list of dependencies!'
+        for item in dependencies:
+            assert isinstance(item, str), err_msg
+            assert ' ' not in item, err_msg
+
     derived_variables.user_functions.update({variable_string: function})
 
 
 def use_only_user_functions(use_only_user_functions):
     """
     Passing 'True' to this functions disables automatic derivation of
     variables except for the ones you have added via 'add_user_function'.
@@ -96,56 +132,64 @@
     settings.use_only_user_functions = use_only_user_functions
 
 
 def add_user_unit(field, blockname, unit):
     """
     This function adds user units.
 
-    Parameters:
+    Parameters
+    ----------
+
+    field : string
+        possible values are specified in
+        unit_specifications.pos_fields, currently
+
+        pos_fields = ['default', 'voronoi_cells', 'dark_matter',
+        'stars', 'black_holes', 'groups', 'subhalos']
 
-    field (string): possible values are specified in
-                    unit_specifications.pos_fields, currently
+    blockname : string
+        The blockname that you would like to enable units for.
 
-                    pos_fields = ['default', 'voronoi_cells', 'dark_matter',
-                    'stars', 'black_holes', 'groups', 'subhalos']
+    unit : string
+        The unit that the blockname should have.
+        String inputs are preferred, e.g., ``arepo_mass arepo_length small_a^2 small_h^(-3/2)``.
 
-    blockname (string): The blockname that you would like to enable units for.
+        The available arepo units are:
 
-    unit (string): The unit that the blockname should have.
-                                   String inputs are preferred, e.g.,
+        ``arepo_length`` (often 1 kpc)
 
-                         'arepo_mass arepo_length small_a^2 small_h^(-3/2)'
+        ``arepo_mass`` (often 10^10 Msun)
 
-                   The available arepo units are
+        ``arepo_velocity`` (often 1 km/s)
 
-                   arepo_length (often 1 kpc)
-                   arepo_mass (often 10^10 Msun)
-                   arepo_velocity (often 1 km/s)
-                   arepo_time
-                   arepo_energy
-                   arepo_pressure
-                   arepo_density
+        ``arepo_time``
 
-                   Please note that these only become available once you
-                   actually load a hdf5 file. This is the reason that you can
-                   pass the string only.
+        ``arepo_energy``
+
+        ``arepo_pressure``
+
+        ``arepo_density``
+
+        Please note that these only become available once you
+        actually load a hdf5 file. This is the reason that you can
+        pass the string only.
     """
     if field not in util.user_unit_dict:
         raise RuntimeError(f'unknown field: {field}')
 
     util.user_unit_dict[field][blockname] = unit
 
 
 def numthreads(numthreads):
     """
     Pass the number of threads you would like to use for parallel execution.
 
     numthreads (int): e.g. 16
     """
-    util.check_if_omp_has_issues(False)
+    util._check_if_omp_has_issues(False)
 
     if numthreads > settings.max_threads:
         print(f'Your machine only has {settings.max_threads} available threads')
 
     settings.numthreads = min(numthreads, settings.max_threads)
     if settings.openMP_has_issues:
         settings.numthreads_reduction = 1
@@ -158,48 +202,54 @@
     Input: a boolean controlling whether to provide info to terminal.
     """
     settings.print_info_when_deriving_variables = option
 
 
 def give_openMP_warnings(option):
     """
-    Turns of warnings that will otherwise appear on a mac computer.
+    Turns of warnings that might otherwise appear on a mac computer.
     """
     settings.give_openMP_warnings = option
 
 
 def load_cuda_functionality_on_startup(option):
     """
-    Turns on/off whether to import GPU/cuda on startup
+    Turns on/off whether to import GPU/cuda on startup.
     """
     settings.load_cuda_functionality_on_startup = option
 
 
 def set_aliases(aliases):
     """
     Assign a list of aliases for use as keys in snapshot objects.
 
-    input (dictionary): e.g.
-
-    aliases = {'0_Density': 'dens',
-           '0_Temperatures': 'T',
-           '0_MeanMolecularWeight': 'mu'}
+    Parameters
+    ----------
+        aliases : dict
+            A dictionary containing the mapping of variable names
+            that you would like to have enabled, e.g.::
+
+                aliases = {'0_Density': 'dens',
+                       '0_Temperatures': 'T',
+                       '0_MeanMolecularWeight': 'mu'}
     """
     msg = 'Your user-set aliases seem to not be unique'
     assert len(set(aliases.values())) == len(aliases.values()), msg
 
     inverse = {aliases[key]: key for key in aliases.keys()}
     settings.aliases = aliases
     settings.inverse_aliases = inverse
     settings.use_aliases = True
 
 
 def user_settings_exists():
     """
     Checks if user settings exist in the root directory of Paicos.
+
+    :meta private:
     """
     if os.path.exists(code_dir + '/paicos_user_settings.py'):
         return True
     return False
 
 
 if user_settings_exists():
@@ -215,19 +265,36 @@
             data_dir += '/'
     except:  # noqa: E722
         data_dir = None
 
 
 # Import of GPU functionality only if
 # a simple test with cupy and numba works.
-if settings.load_cuda_functionality_on_startup:
+def gpu_init(gpu_num=0):
+    """
+    Calling this function initializes the GPU parts of the code.
+
+    You can set settings.load_cuda_functionality_on_startup = True,
+    to do this automatically on startup, but you should be aware
+    that loading cupy and numba can be a bit time-consuming,
+    so that this significantly affects the import time.
+
+    Parameters:
+    ----------
+
+        gpu_num (int): The GPU that you want to use for computations,
+                       i.e., we call cupy.cuda.Device(gpu_num).use()
+    """
+
     try:
         import cupy as cp
         from numba import cuda
 
+        cp.cuda.Device(gpu_num).use()
+
         @cuda.jit
         def my_kernel(io_array):
             pos = cuda.grid(1)
             if pos < io_array.size:
                 io_array[pos] *= 2
 
         data = cp.ones(10**6)
@@ -236,18 +303,26 @@
         my_kernel[blockspergrid, threadsperblock](data)
 
         del data
 
         # Test above worked, do the imports
         from .image_creators.gpu_sph_projector import GpuSphProjector
         from .image_creators.gpu_ray_projector import GpuRayProjector
+        import paicos
+        paicos.GpuSphProjector = GpuSphProjector
+        paicos.GpuRayProjector = GpuRayProjector
     except Exception as e:
         import warnings
         print(e)
         err_msg = ('\nPaicos: The simple cuda example using cupy and numba failed '
                    'with the error above. Please check the official documentation for '
                    'cupy and numba for installation procedure. Note that you need '
                    'a GPU that supports CUDA.\n')
         warnings.warn(err_msg)
 
+
+if settings.load_cuda_functionality_on_startup:
+    gpu_init()
+
+
 # Do this at start up
-util.check_if_omp_has_issues()
+util._check_if_omp_has_issues()
```

### Comparing `paicos-0.1.8/paicos/cython/get_derived_variables.pyx` & `paicos-0.1.9/paicos/cython/get_derived_variables.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,37 @@
     np.float32_t
     np.float64_t
 
 
 def get_curvature(real_t[:, :] Bvec, real_t[:, :] Bgradient):
 
     """
-    This function returns the curvature, equivalent
-    to code:
+    This function computes the magnetic field line curvature.
 
-    Kvec  = np.dot(Bgrad_mat[i,],Bvec[i,]) / B[i]**2
-    Kvec -= np.dot(np.dot(Bgrad_mat[i,],Bvec[i,]),Bvec[i,]) * Bvec[i,] / B[i]**4
-    K2 = (Kvec**2).sum())
-    K = np.sqrt(K2)
+    Parameters:
+        Bvec (array N, 3): Magnetic field vector
+        Bgradient (array N, 3, 3): Magnetic field gradient tensor
+
+    Returns:
+        array N: The magnetic field line curvature.
     """
     cdef int ip, ii, jj, kk
     cdef int Np = Bvec.shape[0]
     cdef real_t B2, gradB_ij, gradB_kj, term1, term2
 
     cdef real_t[:] K2 = np.zeros(Np, dtype=np.float64)
 
+    """
+    The code is equivalent to
+    Kvec  = np.dot(Bgrad_mat[i,],Bvec[i,]) / B[i]**2
+    Kvec -= np.dot(np.dot(Bgrad_mat[i,],Bvec[i,]),Bvec[i,]) * Bvec[i,] / B[i]**4
+    K2 = (Kvec**2).sum())
+    K = np.sqrt(K2)
+    """
+
     # Bgradient has not been reshaped, \nabla B_ij
     for ip in prange(Np, nogil=True, schedule='static'): #, num_threads=32):
         B2 = 0.0
         for ii in range(3):
             B2 = B2 + Bvec[ip, ii]**2
         for kk in range(3):
             term1 = 0.0
@@ -49,15 +58,15 @@
     tmp[:] = np.sqrt(K2[:])
     return tmp
 
 
 def get_magnitude_of_vector(real_t[:, :] Bvec):
 
     """
-    Compute the magnitude of a vector, e.g., magnetic field strength
+    Computes the magnitude of a vector, e.g., magnetic field strength.
     """
     cdef int ip, ii
     cdef int Np = Bvec.shape[0]
     cdef real_t B2
 
     cdef real_t[:] B = np.zeros(Np, dtype=np.float64)
 
@@ -72,30 +81,30 @@
     tmp = np.zeros(Np, dtype=np.float64)
     tmp[:] = B[:]
     return tmp
 
 def sum_1d_array_omp(real_t[:] arr, int num_threads):
 
     """
-    Compute sum of an array along the first index.
-    Equivalent to np.sum(arr, axis=0)
+    Computes the sum of a 1D array using openmp.
+    Equivalent to np.sum(arr)
     """
     cdef int ip
     cdef int Np = arr.shape[0]
     cdef real_t the_sum = 0.0
 
     for ip in prange(Np, nogil=True, schedule='static', num_threads=num_threads):
         the_sum += arr[ip]
 
     return the_sum
 
 def sum_2d_array_omp(real_t[:, :] arr, int num_threads):
 
     """
-    Compute sum of an array along the first index.
+    Computes the sum of an array along the first index using openmp.
     Equivalent to np.sum(arr, axis=0)
     """
     cdef int ip
     cdef int Np = arr.shape[0]
     cdef real_t jj_sum = 0.0
 
     the_sum = np.zeros(arr.shape[1])
@@ -107,16 +116,16 @@
         the_sum[jj] = jj_sum
 
     return the_sum
 
 def sum_arr_times_vector_omp(real_t[:] arr, real_t[:, :] vector, int num_threads):
 
     """
-    Compute the sum of an array times a vector.
-    e.g. sum_i M_i \vec{v}_i for calculating the center of mass.
+    Computes the sum of an array times a vector.
+    e.g. sum_i M_i vec{v}_i for calculating the center of mass.
 
     Equivalent to np.sum(arr[:, None] * vector, axis=0)
     """
     cdef int ip
     cdef int Np = arr.shape[0]
     cdef real_t the_sum_x = 0.0
     cdef real_t the_sum_y = 0.0
```

### Comparing `paicos-0.1.8/paicos/cython/histogram.pyx` & `paicos-0.1.9/paicos/cython/histogram.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     double
     np.float32_t
     np.float64_t
 
 
 def get_hist_from_weights_and_idigit(int num_bins, real_t[:] weights,
                                      long[:] i_digit):
+    """
+    This is a cython helper function for calculating 1D histograms.
+    """
 
     cdef int Np = weights.shape[0]
 
     cdef real_t[:] hist = np.zeros(num_bins+1, dtype=np.float64)
 
     cdef int ip, ib
     for ip in range(Np):
@@ -33,16 +36,19 @@
 
 def get_hist2d_from_weights(real_t [:] xvec, real_t [:] yvec,
                             real_t [:] weights,
                             real_t lower_x, real_t upper_x, int nbins_x,
                             real_t lower_y, real_t upper_y, int nbins_y,
                             bint logspace,
                             int numthreads=1):
+    """
+    This is a cython helper function for calculating 2D histograms.
+    """
 
-    assert numthreads == 1, 'use project_image_omp for more than one thread'
+    assert numthreads == 1, 'use get_hist2d_from_weights_omp for more than one thread'
 
     # Number of particles
     cdef int Np = xvec.shape[0]
 
     # Create hist2d array
     cdef real_t[:, :] hist2d = np.zeros((nbins_x, nbins_y),
                                         dtype=np.float64)
@@ -83,14 +89,17 @@
 
 def get_hist2d_from_weights_omp(real_t [:] xvec, real_t [:] yvec,
                                 real_t [:] weights,
                                 real_t lower_x, real_t upper_x, int nbins_x,
                                 real_t lower_y, real_t upper_y, int nbins_y,
                                 bint logspace,
                                 int numthreads=1):
+    """
+    This is a cython helper function for calculating 2D histograms using openmp.
+    """
 
     # Number of particles
     cdef int Np = xvec.shape[0]
 
     cdef int threadnum
 
     cdef int nx = nbins_x
@@ -143,14 +152,18 @@
     tmp[:, :] = hist2d[:, :]
 
     return tmp
 
 
 def find_normalizing_norm_of_2d_hist(real_t [:, :] hist2d, real_t[:] edges_x,
                                      real_t[:] edges_y):
+    """
+    This is a cython helper function for calculating the normalization of
+    a 2D histogram.
+    """
 
     cdef int ix, iy
     cdef real_t dx, dy, cell_area
     cdef real_t norm = 0
 
     cdef int nx = hist2d.shape[0]
     cdef int ny = hist2d.shape[1]
```

### Comparing `paicos-0.1.8/paicos/cython/sph_projectors.pyx` & `paicos-0.1.9/paicos/cython/sph_projectors.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -15,24 +15,38 @@
 def project_image(real_t[:] xvec, real_t[:] yvec, real_t[:] variable,
                   real_t[:] hvec, int nx, real_t xc, real_t yc,
                   real_t sidelength_x, real_t sidelength_y,
                   real_t boxsize, int numthreads=1):
 
     """
 
-    xc, yc are the coordinates at the center of a square image
-    with sidelength=sidelength.
+    Projects particles using an SPH-like kernel.
+
     This function assumes that only particles with coordinates
 
     x0 < x < x0 + sidelength_x
     y0 < y < y0 + sidelength_y
 
     are passed to it. For speed, this is not checked!
 
     Here x0, y0 are the coordinates at the lower, left corner.
+
+    Parameters:
+        xvec (array, N): positions along x (horizontal)
+        yvec (array, N): positions along y (vertical)
+        variable (array, N): variable to be projected (e.g. mass)
+        hsml (array, N): size of particles
+        sidelength_x (double): size of image along x
+        sidelength_y (double): size of image along y
+        boxsize (double): size of simulation domain,
+                           which for now is assumed to be cubic!
+
+    Returns:
+        2d array: A 2D array with the projected variable.
+
     """
 
     assert numthreads == 1, 'use project_image_omp for more than one thread'
 
     # Number of particles
     cdef int Np = xvec.shape[0]
 
@@ -52,16 +66,16 @@
     cdef real_t dx, dy, r2, h, h2, weight
     cdef real_t x, y, norm
     cdef real_t x0, y0
 
     assert sidelength_x/nx == sidelength_y/ny
 
     # Lower left corner of image in Arepo coordinates
-    x0 = xc - sidelength_x/2.0
-    y0 = yc - sidelength_y/2.0
+    x0 = xc - sidelength_x / 2.0
+    y0 = yc - sidelength_y / 2.0
 
     for ip in range(Np):
         # Center coordinate system at x0, y0
         x = xvec[ip] - x0
         y = yvec[ip] - y0
 
         # Apply periodic boundary condition
@@ -133,14 +147,18 @@
 
 
 def project_image_omp(real_t[:] xvec, real_t[:] yvec, real_t[:] variable,
                       real_t[:] hvec, int nx, real_t xc, real_t yc,
                       real_t sidelength_x, real_t sidelength_y,
                       real_t boxsize, int numthreads):
 
+    """
+    Same as project_image but here with an openmp parallel implementation.
+    """
+
     # Number of particles
     cdef int Np = xvec.shape[0]
 
     # Shape of projection array
     cdef int ny = <int> (sidelength_y/sidelength_x * nx)
     msg = '(sidelength_y/sidelength_x * nx) needs to be an integer'
     assert (sidelength_y/sidelength_x * nx) == <float> ny, msg
@@ -251,14 +269,15 @@
                            real_t boxsize,
                            real_t[:] unit_vector_x,
                            real_t[:] unit_vector_y,
                            real_t[:] unit_vector_z,
                            int numthreads=1):
 
     """
+    Same as project_image but here for an arbitrarily oriented image.
     """
 
     assert numthreads == 1, 'use project_image_omp for more than one thread'
 
     # Number of particles
     cdef int Np = xvec.shape[0]
 
@@ -366,15 +385,15 @@
                                real_t boxsize,
                                real_t[:] unit_vector_x,
                                real_t[:] unit_vector_y,
                                real_t[:] unit_vector_z,
                                int numthreads=1):
 
     """
-
+    Same as project_oriented_image but here with an openmp implementation.
     """
 
     # Number of particles
     cdef int Np = xvec.shape[0]
 
     # Shape of projection array
     cdef int ny = <int> (sidelength_y/sidelength_x * nx)
```

### Comparing `paicos-0.1.8/paicos/derived_variables/derived_variables_gas.py` & `paicos-0.1.9/paicos/derived_variables/derived_variables_gas.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,79 +3,79 @@
 """
 import numpy as np
 
 # pylint: disable=import-outside-toplevel
 
 
 def GFM_MetallicityTimesMasses(snap, get_dependencies=False):
-    """Returns the metallicity times the mass"""
+    """Returns the metallicity times the mass."""
     if get_dependencies:
         return ['0_Masses', '0_GFM_Metallicity']
     return snap['0_Masses'] * snap['0_GFM_Metallicity']
 
 
 def Volume(snap, get_dependencies=False):
     """Returns the volume of the Voronoi cells"""
     if get_dependencies:
         return ['0_Masses', '0_Density']
     return snap["0_Masses"] / snap["0_Density"]
 
 
 def MachnumberTimesEnergyDissipation(snap, get_dependencies=False):
-    """Returns the Mach number times the energy dissipation"""
+    """Returns the Mach number times the energy dissipation."""
     if get_dependencies:
         return ['0_Machnumber', '0_EnergyDissipation']
     variable = snap['0_Machnumber'] * snap['0_EnergyDissipation']
     return variable
 
 
 def MagneticFieldSquared(snap, get_dependencies=False):
-    """Returns the magnetic field strength squared"""
+    """Returns the magnetic field strength squared."""
     if get_dependencies:
         return ['0_MagneticField']
     return np.sum(snap['0_MagneticField']**2, axis=1)
 
 
 def MagneticFieldStrength(snap, get_dependencies=False):
-    """Returns the magnetic field strength"""
+    """Returns the magnetic field strength."""
     if get_dependencies:
         return ['0_MagneticField']
     return np.sqrt(np.sum(snap['0_MagneticField']**2, axis=1))
 
 
 def VelocityMagnitude(snap, get_dependencies=False):
-    """Returns the magnitude of the gas velocity"""
+    """Returns the magnitude of the gas velocity."""
     if get_dependencies:
         return ['0_Velocities']
     return np.sqrt(np.sum(snap['0_Velocities']**2, axis=1))
 
 
 def MagneticFieldSquaredTimesVolume(snap, get_dependencies=False):
     """Returns B² × V """
     if get_dependencies:
         return ['0_Volume', '0_MagneticField']
     variable = snap["0_Volume"] * np.sum(snap['0_MagneticField']**2, axis=1)
     return variable
 
 
 def Pressure(snap, get_dependencies=False):
-    """Returns the gas pressure"""
+    """Returns the gas pressures"""
     if get_dependencies:
         return ['0_InternalEnergy', '0_Density']
 
     if snap.gamma == 1:
         msg = 'Temperature field not supported for isothermal EOS!'
         raise RuntimeError(msg)
     gm1 = snap.gamma - 1
     variable = snap["0_InternalEnergy"] * snap["0_Density"] * gm1
-    return variable
+    return variable.to('arepo_pressure')
 
 
 def PressureTimesVolume(snap, get_dependencies=False):
-    """Returns the gas pressure times the volume"""
+    """Returns the gas pressure times the volume."""
     if get_dependencies:
         return ['0_Pressure', '0_Volume']
 
     if '0_Pressure' in snap:
         return snap['0_Pressure'] * snap['0_Volume']
 
     if snap.gamma != 1:
@@ -84,15 +84,15 @@
     else:
         variable = snap['0_Volume'] * snap['0_Pressure']
 
     return variable
 
 
 def Temperatures(snap, get_dependencies=False):
-    """Returns the temperature in Kelvin"""
+    """Returns the temperature in Kelvin."""
 
     if get_dependencies:
         return ['0_InternalEnergy', '0_MeanMolecularWeight']
 
     from astropy import constants as c
     mhydrogen = c.m_e + c.m_p
 
@@ -114,23 +114,23 @@
         variable = (gm1 * snap["0_InternalEnergy"]
                     * u_v**2 * mmean * mhydrogen
                     ).to('K').value
     return variable
 
 
 def TemperaturesTimesMasses(snap, get_dependencies=False):
-    """Returns the temperature times masses"""
+    """Returns the temperature times masses."""
     if get_dependencies:
         return ['0_Temperatures', '0_Masses']
 
     return snap["0_Temperatures"] * snap['0_Masses']
 
 
 def Current(snap, get_dependencies=False):
-    """Returns the magnitude of the current, i.e., |∇×B|"""
+    """Returns the magnitude of the current, i.e., |∇×B|."""
 
     if get_dependencies:
         return ['0_BfieldGradient']
 
     def get_index(ii, jj):
         return ii * 3 + jj
     gradB = snap['0_BfieldGradient']
@@ -139,15 +139,15 @@
     J_z = gradB[:, get_index(1, 0)] - gradB[:, get_index(0, 1)]
 
     J = np.sqrt(J_x**2 + J_y**2 + J_z**2)
     return J
 
 
 def Enstrophy(snap, get_dependencies=False):
-    """Returns the enstrophy, i.e., 1/2|∇×v|²"""
+    """Returns the enstrophy, i.e., 1/2|∇×v|²."""
 
     if get_dependencies:
         return ['0_VelocityGradient']
 
     def get_index(ii, jj):
         return ii * 3 + jj
     gradV = snap['0_VelocityGradient'][()]
@@ -156,15 +156,15 @@
     vor_z = gradV[:, get_index(1, 0)] - gradV[:, get_index(0, 1)]
 
     enstrophy = 0.5 * (vor_x**2 + vor_y**2 + vor_z**2)
     return enstrophy
 
 
 def EnstrophyTimesMasses(snap, get_dependencies=False):
-    """ Returns the enstrophy times masses"""
+    """ Returns the enstrophy times masses."""
 
     if get_dependencies:
         return ['0_VelocityGradient']
 
     # Reshaping is slow
     if False:
         n_cells = snap['0_VelocityGradient'].shape[0]
@@ -188,15 +188,15 @@
     enstrophy = 0.5 * (vor_x**2 + vor_y**2 + vor_z**2)
     variable = enstrophy * snap['0_Masses']
 
     return variable
 
 
 def MeanMolecularWeight(snap, get_dependencies=False):
-    """Returns the mean molecular weight, μ"""
+    """Returns the mean molecular weight, μ."""
 
     if get_dependencies:
         return ['0_Density']
 
     if '0_GFM_Metals' in snap.info(0, False):
         hydrogen_abundance = snap['0_GFM_Metals'][:, 0]
     else:
@@ -226,15 +226,15 @@
     mean_molecular_weight = snap['0_MeanMolecularWeight']
     proton_mass = c.m_p.to('g')
     number_density_gas = density / (mean_molecular_weight * proton_mass)
     return number_density_gas
 
 
 def MagneticCurvature(snap, get_dependencies=False):
-    """Returns the length of the magnetic curvature vector"""
+    """Returns the length of the magnetic curvature vector."""
 
     if get_dependencies:
         return ['0_MagneticField', '0_BfieldGradient']
 
     from .. import util
 
     @util.remove_astro_units
@@ -245,15 +245,15 @@
     curva = get_func(snap['0_MagneticField'], snap['0_BfieldGradient'])
     unit_quantity = snap['0_BfieldGradient'].uq / snap['0_MagneticField'].uq
     curva = curva * unit_quantity
     return curva
 
 
 def VelocityCurvature(snap, get_dependencies=False):
-    """Returns the length of the velocity curvature vector"""
+    """Returns the length of the velocity curvature vector."""
     if get_dependencies:
         return ['0_Velocities', '0_VelocityGradient']
 
     from .. import util
 
     @util.remove_astro_units
     def get_func(V, gradV):
@@ -263,15 +263,15 @@
     curva = get_func(snap['0_Velocities'], snap['0_VelocityGradient'])
     unit_quantity = snap['0_VelocityGradient'].uq / snap['0_Velocities'].uq
     curva = curva * unit_quantity
     return curva
 
 
 def Diameters(snap, get_dependencies=False):
-    """Returns the cell diameter"""
+    """Returns the cell diameters."""
     if get_dependencies:
         return ['0_Volume']
 
     return 2 * np.cbrt((snap['0_Volume']) / (4.0 * np.pi / 3.0))
 
 
 functions = {
```

### Comparing `paicos-0.1.8/paicos/histograms/histogram.py` & `paicos-0.1.9/paicos/histograms/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 import time
 import numpy as np
 from .. import util
 from .. import settings
 from ..cython.histogram import get_hist_from_weights_and_idigit as func
 
 
-def make_bins(bins, logscale):
+def _make_bins(bins, logscale):
     """
     Private method to calculate the edges and centers of the bins
     given lower, upper and number of bins.
 
     Parameters:
         bins (tuple): Tuple of lower edge, upper edge and number of
                       bins for the axis
     Returns:
         edges (array): Edges of the bins
         centers (array): Centers of the bins
     """
 
     lower, upper, nbins = bins
-    edges, centers = make_bins_helper(lower, upper, nbins, logscale)
+    edges, centers = _make_bins_helper(lower, upper, nbins, logscale)
     if settings.use_units:
         assert lower.unit == upper.unit
         edges = np.array(edges) * lower.unit_quantity
         centers = np.array(centers) * lower.unit_quantity
     return edges, centers
 
 
 @util.remove_astro_units
-def make_bins_helper(lower, upper, nbins, logscale):
+def _make_bins_helper(lower, upper, nbins, logscale):
     """
     Private method to calculate the edges and centers of the bins
     in logscale or linear scale based on the class variable logscale
     Parameters:
         lower (float): Lower edge of the bin
         upper (float): Upper edge of the bin
         nbins (int): Number of bins for the axis
@@ -84,15 +84,15 @@
 
         if isinstance(bins, int):
             bins = [x.min(), x.max(), bins]
 
         self.logscale = logscale
         self.verbose = verbose
 
-        self.edges, self.centers = make_bins(bins, self.logscale)
+        self.edges, self.centers = _make_bins(bins, self.logscale)
         self.bin_centers = self.centers
         self.bin_edges = self.edges
 
         if self.verbose:
             t = time.time()
             print('Digitize for histogram begun')
```

### Comparing `paicos-0.1.8/paicos/histograms/histogram2D.py` & `paicos-0.1.9/paicos/histograms/histogram2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import numpy as np
 import h5py
 from astropy import units as u
 from .. import units as pu
 from .. import util
 from .. import settings
-from .histogram import make_bins
+from .histogram import _make_bins
 from ..cython.histogram import find_normalizing_norm_of_2d_hist
 
 
 class Histogram2D:
     """
     This code defines a Histogram2D class which can be used to create 2D
     histograms. The class takes in the bin edges for the x and y axes, and an
@@ -75,29 +75,33 @@
         self.normalize = normalize
 
         if isinstance(bins_x, int):
             bins_x = [self.x.min(), self.x.max(), bins_x]
 
             if logscale:
                 bins_x[0] = self.x[self.x > 0].min()
+        else:
+            assert bins_x[0] < bins_x[1], 'min and max values swapped!'
 
         if isinstance(bins_y, int):
             bins_y = [self.y.min(), self.y.max(), bins_y]
 
             if logscale:
                 bins_y[0] = self.y[self.y > 0].min()
+        else:
+            assert bins_y[0] < bins_y[1], 'min and max values swapped!'
 
         self.logscale = logscale
 
         if logscale:
             assert bins_x[0] > 0
             assert bins_y[0] > 0
 
-        self.edges_x, self.centers_x = make_bins(bins_x, self.logscale)
-        self.edges_y, self.centers_y = make_bins(bins_y, self.logscale)
+        self.edges_x, self.centers_x = _make_bins(bins_x, self.logscale)
+        self.edges_y, self.centers_y = _make_bins(bins_y, self.logscale)
         self.lower_x = self.edges_x[0]
         self.lower_y = self.edges_y[0]
         self.upper_x = self.edges_x[-1]
         self.upper_y = self.edges_y[-1]
 
         self.extent = [self.lower_x, self.upper_x, self.lower_y, self.upper_y]
 
@@ -134,22 +138,23 @@
             self.area_per_bin *= u.Unit('dex')**(2) / self.area_per_bin.unit
         self.centers_x_mat = centers_x_mat
         self.centers_y_mat = centers_y_mat
 
     def get_colorlabel(self, x_symbol, y_symbol, weight_symbol=None):
         """
         Method to generate a color label for the histogram with units
+
         Parameters:
             x_symbol (string): Symbol for x axis
             y_symbol (string): Symbol for y axis
             weight_symbol (string): Symbol for weight of the histogram,
                                     default is None
+
         Returns:
-            colorlabel (string): The color label for the histogram with
-                                 units
+            string: The color label for the histogram with units
         """
 
         assert settings.use_units
 
         unit_label = self.hist2d.label()[1:-1]
 
         if self.logscale:
@@ -241,16 +246,16 @@
 
         hist2d = self._cython_make_histogram(x, y, self.edges_x,
                                              self.edges_y, weights)
 
         hist2d = hist2d.T
 
         if settings.use_units:
-            hist2d = pu.PaicosQuantity(hist2d, self.hist_units, a=self.x.a,
-                                       h=self.x.h,
+            hist2d = pu.PaicosQuantity(hist2d, self.hist_units, a=self.x._a,
+                                       h=self.x._h,
                                        comoving_sim=self.x.comoving_sim)
         if normalize:
             norm = np.sum(self.area_per_bin * hist2d)
             hist2d /= norm
 
             sanity = np.sum(self.area_per_bin * hist2d)
             if settings.use_units:
@@ -260,14 +265,21 @@
                 np.testing.assert_allclose(sanity, 1.0)
 
         return hist2d
 
     def save(self, basedir, basename="2d_histogram"):
         """
         Saves the 2D histogram in the basedir directory.
+
+        Parameters:
+            basedir (path): The directory where the histogram should be saved.
+            basename (string): The basename for the filename, which will take
+                               the form::
+
+                                   filename =  basename + f'_{snapnum:03d}.hdf5'
         """
 
         if basedir[-1] != '/':
             basedir += '/'
 
         snapnum = self.snap.snapnum
         filename = basedir + basename + f'_{snapnum:03d}.hdf5'
@@ -292,8 +304,8 @@
             else:
                 print(("Unable to save colorlabel, please call "
                       + "the 'get_colorlabel' method before saving."))
             # Add attributes
             for key, attr in attrs.items():
                 hdf5file[name].attrs[key] = attr
 
-        util.copy_over_snapshot_information(self.snap.filename, filename)
+        util._copy_over_snapshot_information(self.snap, filename)
```

### Comparing `paicos-0.1.8/paicos/image_creators/gpu_ray_projector.py` & `paicos-0.1.9/paicos/image_creators/gpu_ray_projector.py`

 * *Files identical despite different names*

### Comparing `paicos-0.1.8/paicos/image_creators/gpu_sph_projector.py` & `paicos-0.1.9/paicos/image_creators/gpu_sph_projector.py`

 * *Files identical despite different names*

### Comparing `paicos-0.1.8/paicos/image_creators/image_creator.py` & `paicos-0.1.9/paicos/image_creators/image_creator.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,30 +17,32 @@
 
     def __init__(self, snap, center, widths, direction, npix=512, parttype=0):
         """
         Initialize the ImageCreator class. This method will be called
         by subclasses such as Projector or Slicer.
 
         Parameters:
-            snap (object): Snapshot object from which the image is created
+            snap (object): Snapshot object from which the image is created.
 
-            center: Center of the image (3D coordinates)
+            center: Center of the image (3D coordinates).
 
             widths: Width of the image in each direction (3D coordinates)
 
-            direction (str): Direction of the image ('x', 'y', 'z')
+            direction (str, Orientation): Direction of the image ('x', 'y', 'z')
+                or an Orientation instance.
 
-            npix (int): Number of pixels in the image (default is 512)
+            npix (int): Number of pixels in the image (default is 512).
         """
 
         self._obervers = []
 
         self.snap = snap
 
-        code_length = self.snap.length
+        if settings.use_units:
+            code_length = self.snap.length
 
         if hasattr(center, 'unit'):
             self._center = center.copy
             assert center.unit == code_length.unit, 'this restriction applies'
         elif settings.use_units:
             self._center = np.array(center) * code_length
         else:
@@ -136,30 +138,36 @@
         err_msg = ("_do_region_selection was called from ImageCreator. "
                    + "This should never happen as the Subclasses of "
                    + "ImageCreator should implement this method")
         raise RuntimeError(err_msg)
 
     def info(self):
         """
-        Prints some information about the image creator instance
+        Prints some information about the image creator instance.
         TODO: Add things like the number of cells/particles
         in the current instance.
         """
         s = f'Paicos ImageCreator instance of type: {str(self)}\n'
         s += f'widths: {self.widths}\n'
         s += f'center:  {self.center}\n'
         s += f'orientation:  {self.orientation}'
         print(s)
 
     @property
     def center(self):
+        """
+        Center of the image (3D coordinates).
+        """
         return self._center
 
     @property
     def widths(self):
+        """
+        Width of the image in each direction (3D coordinates).
+        """
         return self._widths
 
     @widths.setter
     def widths(self, value):
         """
         TODO: ensure that nx, ny
         remain consistent with widths
@@ -180,64 +188,97 @@
             self._center = value.copy
         else:
             self._center = np.array(value)
         self._properties_changed = True
 
     @property
     def npix(self):
+        """
+        The number of pixels along the horizontal
+        direction of the image.
+        """
         return self._npix
 
     @npix.setter
     def npix(self, value):
         self._npix = value
         # TODO: Not always needed to do this...
         self._properties_changed = True
 
     @property
     def npix_width(self):
+        """
+        The number of pixels along the horizontal
+        direction of the image.
+        """
         return self._npix
 
     @npix_width.setter
     def npix_width(self, value):
         self.npix = value
 
     @property
     def parttype(self):
+        """
+        The parttype being imaged, e.g. parttype=0
+        are the Voronoi gas cells.
+        """
         return self._parttype
 
     @property
-    def foo(self):
-        return self._foo
-
-    @property
     def x_c(self):
+        """
+        The x-component of .center
+        """
         return self.center[0]
 
     @property
     def y_c(self):
+        """
+        The y-component of .center
+        """
         return self.center[1]
 
     @property
     def z_c(self):
+        """
+        The z-component of .center
+        """
         return self.center[2]
 
     @property
     def width_x(self):
+        """
+        The x-component of .widths
+        """
         return self.widths[0]
 
     @property
     def width_y(self):
+        """
+        The y-component of .widths
+        """
         return self.widths[1]
 
     @property
     def width_z(self):
+        """
+        The z-component of .widths
+        """
         return self.widths[2]
 
     @property
     def extent(self):
+        """
+        The extent of the image in the horizontal-vertical plane.
+        The idea with this property is that it corresponds to the
+        matplotlib imshow keyword argument 'extent'. When using units,
+        one has to remember to pass image_creator.extent.value rather
+        than image_creator.extent.
+        """
         if self.direction == 'orientation':
 
             # This is the extent of the image-plane pre-rotation
             # into the orientation of the image...
             # Use centered_extent for showing rotated images.
             center_width = self.x_c
             center_height = self.y_c
@@ -261,47 +302,59 @@
             extent = units.paicos_quantity_list_to_array(extent)
         else:
             extent = np.array(extent)
         return extent
 
     @property
     def centered_extent(self):
+        """
+        Same as 'extent' but centered on the center of the image.
+        """
         centered_extent = [- self.width / 2, self.width / 2,
                            - self.height / 2, self.height / 2]
 
         if settings.use_units:
             centered_extent = units.paicos_quantity_list_to_array(centered_extent)
         else:
             centered_extent = np.array(centered_extent)
         return centered_extent
 
     @property
     def width(self):
+        """
+        The horizontal width of the image.
+        """
         if self.direction == 'x':
             return self.width_y
 
         elif self.direction == 'y':
             return self.width_z
 
         elif self.direction == 'z' or self.direction == 'orientation':
             return self.width_x
 
     @property
     def height(self):
+        """
+        The vertical height of the image.
+        """
         if self.direction == 'x':
             return self.width_z
 
         elif self.direction == 'y':
             return self.width_x
 
         elif self.direction == 'z' or self.direction == 'orientation':
             return self.width_y
 
     @property
     def depth(self):
+        """
+        The depth of the image.
+        """
         if self.direction == 'x':
             return self.width_x
 
         elif self.direction == 'y':
             return self.width_y
 
         elif self.direction == 'z' or self.direction == 'orientation':
@@ -346,20 +399,39 @@
             self._widths[1] = value.copy
 
         elif self.direction == 'z' or self.direction == 'orientation':
             self._widths[2] = value.copy
         self._properties_changed = True
 
     def double_resolution(self):
+        """
+        Calling this method doubles the pixel resolution of the image
+        creator.
+        """
         self.npix = self.npix * 2
 
     def half_resolution(self):
+        """
+        Calling this method halves the pixel resolution of the image
+        creator.
+        """
         self.npix = self.npix // 2
 
     def zoom(self, factor):
+        """
+        Calling this method zooms the view by the input factor,
+        that is, the horizontal width and vertical height of the
+        image creator is changed like this:
+
+        width = width / factor
+
+        height = height / factor
+
+        A factor less than one zooms out the view.
+        """
         self.width = self.width / factor
         self.height = self.height / factor
 
         self._properties_changed = True
 
     def _move_center_along_unit_vector(self, shift, unit_vector):
         """
@@ -377,49 +449,70 @@
         self._center = new_center
         self._properties_changed = True
 
     def move_center_along_normal_vector(self, shift):
         """
         Moves the center of the image along its depth direction.
         Value can be positive or negative and must have same units
-        as the center (TODO: In principle we would just convert the distance).
+        as the center.
+
+        (TODO: In principle we could just convert the distance to same units).
         """
         self._move_center_along_unit_vector(shift, self.orientation.normal_vector)
 
     def move_center_along_perp_vector1(self, shift):
         """
         Moves the center of the image along its horizontal direction.
         Value can be positive or negative and must have same units
-        as the center (TODO: In principle we would just convert the distance).
+        as the center.
+
+        (TODO: In principle we could just convert the distance to same units).
         """
         self._move_center_along_unit_vector(shift, self.orientation.perp_vector1)
 
     def move_center_along_perp_vector2(self, shift):
         """
         Moves the center of the image along its vertical direction.
         Value can be positive or negative and must have same units
-        as the center (TODO: In principle we would just convert the distance).
+        as the center.
+
+        (TODO: In principle we could just convert the distance to same units).
         """
         self._move_center_along_unit_vector(shift, self.orientation.perp_vector2)
 
     @property
     def npix_height(self):
+        """
+        The number of pixels of an image in the vertical direction.
+        """
         if settings.use_units:
             return int((self.height / self.width).value * self.npix_width)
         else:
             return int((self.height / self.width) * self.npix_width)
 
     @property
     def area(self):
+        """
+        The area of the image plane.
+        """
         return (self.extent[1] - self.extent[0]) * (self.extent[3] - self.extent[2])
 
     @property
     def area_per_pixel(self):
+        """
+        The area per pixel of the image plane.
+        """
         return self.area / (self.npix_width * self.npix_height)
 
     @property
     def volume(self):
+        """
+        The volume of the projection region (0 for slices).
+        """
         return self.width * self.height * self.depth
 
     @property
     def volume_per_pixel(self):
+        """
+        The volume per pixel in the image.
+        """
         return self.volume / (self.npix_width * self.npix_height)
```

### Comparing `paicos-0.1.8/paicos/image_creators/nested_projector.py` & `paicos-0.1.9/paicos/image_creators/nested_projector.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,60 +12,57 @@
     """
     This class implements an SPH-like projection of gas variables using nested
     grids. It is a subclass of the Projector class, and inherits its
     properties. It has additional attributes for handling the nested grid
     projections, and additional methods for dealing with resolution,
     digitizing particles, and summing up the different resolutions of the
     images.
+
+    Please see also the Projector class.
     """
 
     def __init__(self, snap, center, widths, direction,
                  npix=512, nvol=8, factor=3, npix_min=128,
                  verbose=False, make_snap_with_selection=True,
                  store_subimages=False):
         """
         This is the constructor for the NestedProjector class. It initializes
         the properties inherited from the Projector class, as well as the
         properties specific to nested projections.
 
-        Parameters
-        ----------
-        snap : Snapshot
-            A snapshot object of Snapshot class from paicos package.
+        Parameters:
+            snap (Snapshot): A snapshot object of Snapshot class from paicos package.
+
+            center (array): Center of the region on which projection is to be done, e.g.
+                            center = [x_c, y_c, z_c].
 
-        center : numpy array
-            Center of the region on which projection is to be done, e.g.
-            center = [x_c, y_c, z_c].
+            widths (array): Widths of the region on which projection is to be done,
+                            e.g.m widths=[width_x, width_y, width_z].
 
-        widths : numpy array
-            Widths of the region on which projection is to be done,
-            e.g.m widths=[width_x, width_y, width_z].
+            direction (str or Orientation): Direction of the projection, e.g. 'x', 'y' or 'z',
+                                            or its orientation (see Orientation class).
 
-        direction : str
-            Direction of the projection, e.g. 'x', 'y' or 'z'.
 
-        npix : int, optional
-            Number of pixels in the horizontal direction of the image,
-            by default 512.
+            npix (int, optional): Number of pixels in the horizontal direction of the image,
+                                  by default 512.
 
-        nvol : int, optional
-            Integer used to determine the smoothing length, by default 8
+            nvol (int, optional): Integer used to determine the smoothing length, by default 8
 
-        factor (int, optional): Multiplicative factor in digitizing, defaults to 3.
+            factor (int, optional): Multiplicative factor in digitizing, defaults to 3.
 
-        npix_min (int, optional): Minimum number of pixels, defaults to 128.
+            npix_min (int, optional): Minimum number of pixels, defaults to 128.
 
-        verbose (bool, optional): Flag for verbosity, defaults to False.
+            verbose (bool, optional): Flag for verbosity, defaults to False.
 
-        make_snap_with_selection (bool, optional):
-            a boolean indicating if a new snapshot object should be made with
-            the selected region, defaults to False
+            make_snap_with_selection (bool, optional):
+                a boolean indicating if a new snapshot object should be made with
+                the selected region, defaults to False.
 
-        store_subimages (bool, optional): Flag for storing sub-images, which
-        is useful mainly for testing purposes. Defaults to False.
+            store_subimages (bool, optional): Flag for storing sub-images, which
+                is useful mainly for testing purposes. Defaults to False.
 
         """
 
         super().__init__(snap, center, widths, direction,
                          npix=npix, nvol=nvol,
                          make_snap_with_selection=make_snap_with_selection)
 
@@ -150,25 +147,29 @@
 
         return bins, n_grids
 
     def increase_image_resolution(self, image, factor):
         """
         Increase the number of pixes without changing the total 'mass'
         of the image
+
+        :meta private:
         """
         if factor == 1:
             return image
         repeats = factor
         new_image = np.repeat(np.repeat(image, repeats, axis=0),
                               repeats, axis=1)
         return new_image / factor**2
 
     def sum_contributions(self, images):
         """
         Given the list of images at various resolutions, sum them up.
+
+        :meta private:
         """
         full_image = np.zeros(images[-1].shape)
         n = images[-1].shape[0]
         for image in images:
             full_image += self.increase_image_resolution(image,
                                                          n // image.shape[0])
```

### Comparing `paicos-0.1.8/paicos/image_creators/projector.py` & `paicos-0.1.9/paicos/image_creators/projector.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,17 @@
             Center of the region on which projection is to be done, e.g.
             center = [x_c, y_c, z_c].
 
         widths : numpy array
             Widths of the region on which projection is to be done,
             e.g.m widths=[width_x, width_y, width_z].
 
-        direction : str
-            Direction of the projection, e.g. 'x', 'y' or 'z'.
+        direction : str, Orientation
+            Direction of the projection, e.g. 'x', 'y' or 'z'
+            or an Orientation instance.
 
         npix : int, optional
             Number of pixels in the horizontal direction of the image,
             by default 512.
 
         parttype : int, optional
             Number of the particle type to project, by default gas (PartType 0).
@@ -108,20 +109,20 @@
 
         # Calculate the smoothing length
         avail_list = (list(snap.keys()) + snap._auto_list)
         if f'{parttype}_Volume' in avail_list:
             self.hsml = np.cbrt(self.nvol * (self.snap[f"{parttype}_Volume"])
                                 / (4.0 * np.pi / 3.0))
         elif f'{parttype}_SubfindHsml' in avail_list:
-            self.hsml = self.snap[f'{parttype}_SubfindHsml']
+            self.hsml = np.copy(self.snap[f'{parttype}_SubfindHsml'])
         else:
             raise RuntimeError(
                 'There is no smoothing length or volume for the projector')
 
-        self.pos = self.snap[f'{self.parttype}_Coordinates']
+        self.pos = np.copy(self.snap[f'{self.parttype}_Coordinates'])
 
         if settings.use_units:
             self.hsml = self.hsml.to(self.pos.unit)
 
         if not self.make_snap_with_selection:
             self.hsml = self.hsml[self.index]
             self.pos = self.pos[self.index]
@@ -187,21 +188,22 @@
 
     def project_variable(self, variable):
         """
         projects a given variable onto a 2D plane.
 
         Parameters
         ----------
-        variable : str, function, numpy array
-            variable, it can be passed as string or an array
+        variable : str, array
+            The variable to be projected, it can be passed as string
+            or a 1d array.
 
         Returns
         -------
         numpy array
-            The image of the projected variable
+            The image (2d array) of the projected variable.
         """
         self.do_unit_consistency_check()
         # This calls _do_region_selection if resolution, Orientation,
         # widths or center changed
         self._check_if_properties_changed()
 
         if isinstance(variable, str):
```

### Comparing `paicos-0.1.8/paicos/image_creators/slicer.py` & `paicos-0.1.9/paicos/image_creators/slicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,20 @@
             center = [x_c, y_c, z_c].
 
         widths :
             Widths of the region on which slicing is to be done,
             e.g. widths=[width_x, width_y, width_z] where one of the widths
             is zero (e.g. width_x=0 if direction='x').
 
-        direction : str
+        direction : str, Orientation
             Direction of the slicing, e.g. 'x', 'y' or 'z'. For instance,
             setting direction to 'x' gives a slice in the yz plane with the
             constant x-value set to be x_c.
+            For a more general orientation, one can pass an Orientation
+            instance.
 
         npix : int, optional
             Number of pixels in the horizontal direction of the image,
             by default 512.
 
         parttype : int, optional
             The particle type to project, by default gas (PartType 0).
@@ -76,15 +78,15 @@
 
         # Pre-select a narrow region around the region-of-interest
         avail_list = (list(snap.keys()) + snap._auto_list)
         if f'{parttype}_Volume' in avail_list:
             thickness = 4.0 * np.cbrt((snap[f"{parttype}_Volume"])
                                       / (4.0 * np.pi / 3.0))
         elif f'{parttype}_SubfindHsml' in avail_list:
-            thickness = snap[f'{parttype}_SubfindHsml']
+            thickness = np.copy(snap[f'{parttype}_SubfindHsml'])
         else:
             raise RuntimeError(
                 'There is no smoothing length or volume for the thickness of the slice')
 
         if hasattr(thickness, 'unit'):
             thickness = thickness.to(center.unit)
 
@@ -172,19 +174,21 @@
     def slice_variable(self, variable):
         """
         Slice a gas variable based on the Voronoi cells closest to the image
         plane.
 
         Parameters
         ----------
-        variable: a string or an array of shape (N, )
-                  representing the gas variable to slice
+            variable: str, arr
+                The variable to slice. For instance '0_Density' or snap['0_Density'].
 
-        Returns:
-        An array of shape (npix, npix) representing the sliced gas variable
+        Returns
+        -------
+            slice : 2d arr
+                A 2d array of the sliced variable.
         """
 
         # This calls _do_region_selection if resolution, Orientation,
         # widths or center changed
         self._check_if_properties_changed()
 
         if isinstance(variable, str):
@@ -195,14 +199,17 @@
             if not isinstance(variable, np.ndarray):
                 raise RuntimeError('Unexpected type for variable')
 
         return variable[self.index]
 
     @property
     def depth(self):
+        """
+        Depth of the slice, which is zero by definition.
+        """
         if self.direction == 'x':
             return self.width_x
 
         elif self.direction == 'y':
             return self.width_y
 
         elif self.direction == 'z' or self.direction == 'orientation':
```

### Comparing `paicos-0.1.8/paicos/image_creators/tree_projector.py` & `paicos-0.1.9/paicos/image_creators/tree_projector.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,17 @@
             Center of the region on which projection is to be done, e.g.
             center = [x_c, y_c, z_c].
 
         widths :
             Widths of the region on which projection is to be done,
             e.g. widths=[width_x, width_y, width_z].
 
-        direction : str
-            Direction of the projection, e.g. 'x', 'y' or 'z'.
+        direction : str, Orientation
+            Direction of the projection, e.g. 'x', 'y' or 'z',
+            or an Orientation instance.
 
         npix : int, optional
             Number of pixels in the horizontal direction of the image,
             by default 512.
 
         parttype : int, optional
             The particle type to project, by default gas (PartType 0).
@@ -52,15 +53,15 @@
         tol: float, optional
             Smaller values of tol adds more slices to the integration.
             Convergence is expected for tol ≤ 1 but you can experiment with
             higher values.
 
         make_snap_with_selection : bool
             a boolean indicating if a new snapshot object should be made with
-            the selected region, defaults to False
+            the selected region, defaults to False.
 
         """
 
         if make_snap_with_selection:
             raise RuntimeError('make_snap_with_selection not yet implemented!')
 
         super().__init__(snap, center, widths, direction, npix=npix, parttype=parttype)
@@ -82,15 +83,15 @@
         widths = self.widths
 
         # Pre-select a narrow region around the region-of-interest
         avail_list = (list(snap.keys()) + snap._auto_list)
         if f'{parttype}_Volume' in avail_list:
             thickness = 4.0 * np.cbrt((snap[f"{parttype}_Volume"]) / (4.0 * np.pi / 3.0))
         elif f'{parttype}_SubfindHsml' in avail_list:
-            thickness = snap[f'{parttype}_SubfindHsml']
+            thickness = np.copy(snap[f'{parttype}_SubfindHsml'])
         else:
             err_msg = ("There is no smoothing length or volume for calculating"
                        + "the thickness of the slice")
             raise RuntimeError(err_msg)
 
         if hasattr(thickness, 'unit'):
             thickness = thickness.to(center.unit)
@@ -233,46 +234,52 @@
 
         P = 1 / dA ∫ dM
 
         where dA is the area per pixel and dM is the mass inside a voxel.
 
         Parameters
         ----------
-        variable: a string or an array of shape (N, )
-                  representing the gas variable to project
-
-        additive (bool): A boolean indicating whether the variable to be
-                    projected is additive (e.g. Masses, Volumes)
-                    or not (e.g. Temperature, density, achieved by
-                    setting additive=False). This parameter was previously
-                    named 'extrinsic'.
+        variable : str, array
+            The variable to be projected, it can be passed as string
+            or a 1d array.
+
+        additive : bool
+            A boolean indicating whether the variable to be
+            projected is additive (e.g. Masses, Volumes)
+            or not (e.g. Temperature, density).
+            This parameter was previously named 'extrinsic'.
 
         Returns:
-            An array of shape (npix, npix) representing the projected gas variable
 
-            For non-additive (intrinsic) variables, the unit of the projection is
-            identical to the unit of the input variable. For additive (extrinsic)
-            variables, the projection unit is the input variable unit divided by area.
+            projection : 2d arr
+                A 2d array representing the projected gas variable.
+
+                For non-additive (intrinsic) variables, the unit of the projection is
+                identical to the unit of the input variable. For additive (extrinsic)
+                variables, the projection unit is the input variable unit divided by area.
 
         Examples
         ----------
 
-        We can compute the projected density in two ways.
+        We can compute the projected density in two ways, using either
+        additive or non-additive projetions. In both case,
+        we first need to create a TreeProjector object::
 
-        tree_projector = pa.TreeProjector(snap, center, widths, 'z')
+            tree_projector = pa.TreeProjector(snap, center, widths, 'z')
 
-        Method I (divide projected mass by projected volume):
-            tree_M = tree_projector.project_variable('0_Masses')
-            tree_V = tree_projector.project_variable('0_Volume')
+        Method I (divide projected mass by projected volume)::
+
+            tree_M = tree_projector.project_variable('0_Masses', additive=True)
+            tree_V = tree_projector.project_variable('0_Volume', additive=True)
 
             tree_rho = tree_M / tree_V
 
-        Method II (directly project the density):
+        Method II (directly project the density)::
 
-            rho = tree_projector.project_variable('0_Density', extrinsic=False)
+            rho = tree_projector.project_variable('0_Density', additive=False)
 
         """
         # This calls _do_region_selection if resolution, Orientation,
         # widths or center changed
         self._check_if_properties_changed()
 
         if extrinsic is not None:
@@ -292,17 +299,29 @@
 
         assert len(variable.shape) == 1, 'only scalars can be projected'
 
         if additive:
             avail_list = (list(self.snap.keys()) + self.snap._auto_list)
             if f'{parttype}_Volume' in avail_list:
                 variable_density = variable[self.index] / self.snap[f'{parttype}_Volume'][self.index]
-                projection = np.sum(variable_density * self.delta_depth, axis=2) / self.depth
+
+                projection = np.sum(variable_density * self.delta_depth, axis=2)
+                """
+                # Note that the above is equivalent to:
+                volume_per_voxel = area_per_pixel * self.delta_depth
+                projection = np.sum(variable_density * volume_per_voxel, axis=2) \
+                             / area_per_pixel
+                """
             else:
                 err_msg = (f"The volume field for parttype {parttype} is required when"
                            + "using additive=True")
                 raise RuntimeError(err_msg)
         else:
             variable = variable[self.index]
             projection = np.sum(variable * self.delta_depth, axis=2) / self.depth
+            """
+            # Note that the above is equivalent to:
+            projection = np.mean(variable, axis=2)
+            since self.delta_depth is a constant.
+            """
 
         return projection
```

### Comparing `paicos-0.1.8/paicos/orientation.py` & `paicos-0.1.9/paicos/orientation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import numpy as np
 from . import util
 
 """
-Files to modify to implement these changes:
-arepo_image
-image_creators
-all projectors
-the slicer
-arepo snapshot
-
-TODO: Make it possible to pass angles, so that one may easily
-change the viewing inclination in small steps in angle.
+The orientation clas and its helper functions.
 """
 
 
 @util.remove_astro_units
 def normalize_vector(vector):
     """
     Normalize a vector and return it as a numpy array
+
+    :meta private:
     """
     return vector / np.linalg.norm(vector)
 
 
 @util.remove_astro_units
 def find_a_perpendicular_vector(vector):
     """
     Given an input vector, find a vector which is perpendicular.
     Assumes 3D vectors.
+
+    :meta private:
     """
     assert np.linalg.norm(vector) > 0.
     if vector[1] == 0 and vector[2] == 0:
         return np.cross(vector, [0, 1, 0])
     return np.cross(vector, [1, 0, 0])
 
 
@@ -40,14 +36,16 @@
 
 @util.remove_astro_units
 def get_basis_from_2vecs(vector1, vector2):
     """
     Returns a right-hand orthogonal basis, e1, e2, e3,
     where e1 is in the direction of vector1.
     Adapted from code by Ewald Puchwein.
+
+    :meta private:
     """
 
     # unit vector in vector1 direction
     e1 = vector1 / np.linalg.norm(vector1)
 
     e2 = vector2 - np.dot(e1, vector2) * e1
     # unit vector along direction of vector2-component perpendicular to vector1
@@ -63,27 +61,34 @@
     _assert_perpendicular(e2, e3)
     _assert_perpendicular(e3, e1)
 
     return e1, e2, e3
 
 
 class Orientation:
+    """
+    The Orientation class is used to define an orientation of e.g.
+    an image. An instance of this class can be passed to an ImageCreator.
+    """
     def __init__(self, normal_vector=None, perp_vector1=None):
         """
-        Inputs:
-
-        normal_vector: a vector which will be normal to the face
-                       of the image, e.g. pass the angular momentum vector
-                       of a galaxy here for a face on projection.
 
-        perp_vector1: Perpendicular vector to the image plane, e.g.,
-                         pass the angular momentum vector here for an edge-on
-                         projection.
+        Parameters:
 
-        It's possible to supply both inputs.
+            normal_vector: a vector which will be normal to the face of the image,
+                           i.e. the depth direction. You can e.g. pass the angular momentum
+                           vector of a galaxy for a face on projection.
+
+            perp_vector1: a vector which will be parallel to the image plane. This
+                          will become the horizontal direction of your image. You can e.g. pass
+                          the angular momentum vector here for an edge-on projection.
+
+        It's possible to supply both inputs, which then fully determines the
+        orientation (the vertical direction of the image, perp_vector2, is
+        automatically calculated).
         """
 
         # Construct unit vectors for the chosen coordinate system
         self._construct_unit_vectors(normal_vector, perp_vector1)
 
     def _construct_unit_vectors(self, normal_vector, perp_vector1):
         """
@@ -109,14 +114,17 @@
 
         # Set unitless unit-vectors
         self.normal_vector = e1
         self.perp_vector1 = e2
         self.perp_vector2 = e3
 
     def _get_radians(self, degrees=None, radians=None):
+        """
+        Converts from degrees to radians.
+        """
         if radians is not None:
             return radians
         return 2.0 * np.pi * degrees / 360.
 
     def _get_rotation_matrix(self, axis, degrees=None, radians=None):
         """
         Standard implementation of rotation matrices around the
@@ -124,16 +132,17 @@
         around the coordinate axes in the right-handed
         coordinate system (perp_vector1, perp_vector2, normal_vector)
         is done by transforming this system to a coordinate
         system where these three axes are aligned along x, y and z,
         respectively, applying the either Rx, Ry or Rz and
         then transforming back.
         """
-
-        radians = self._get_radians(degrees)
+        if radians is None:
+            assert degrees is not None
+            radians = self._get_radians(degrees)
 
         if axis == 'x':
             R = np.array([[1, 0, 0],
                          [0, np.cos(radians), -np.sin(radians)],
                          [0, np.sin(radians), np.cos(radians)]])
             return R
         elif axis == 'y':
@@ -148,27 +157,14 @@
             return R
         elif axis == 'perp_vector1':
             u = self.perp_vector1
         elif axis == 'perp_vector2':
             u = self.perp_vector2
         elif axis == 'normal_vector':
             u = self.normal_vector
-        #     Rx = self._get_rotation_matrix('x', degrees, radians)
-        #     Rtmp = np.matmul(Rx, self.inverse_rotation_matrix)
-        #     R = np.matmul(self.rotation_matrix, Rtmp)
-
-        # elif axis == 'perp_vector2':
-        #     Ry = self._get_rotation_matrix('y', degrees, radians)
-        #     Rtmp = np.matmul(Ry, self.inverse_rotation_matrix)
-        #     R = np.matmul(self.rotation_matrix, Rtmp)
-
-        # elif axis == 'normal_vector':
-        #     Rz = self._get_rotation_matrix('z', degrees, radians)
-        #     Rtmp = np.matmul(Rz, self.inverse_rotation_matrix)
-        #     R = np.matmul(self.rotation_matrix, Rtmp)
 
         else:
             raise RuntimeError("invalid input")
 
         # Construct rotation matrix that rotates radians around
         # unit vector 'u'
         # see e.g. https://en.wikipedia.org/w/index.php?title=Rotation_matrix
@@ -183,44 +179,56 @@
     def _apply_rotation_matrix(self, R):
         self.normal_vector = np.matmul(R, self.normal_vector)
         self.perp_vector1 = np.matmul(R, self.perp_vector1)
         self.perp_vector2 = np.matmul(R, self.perp_vector2)
 
     def rotate_around_x(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around the 'x'-coordinate axis
         """
         R = self._get_rotation_matrix('x', degrees, radians)
         self._apply_rotation_matrix(R)
 
     def rotate_around_y(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around the 'y'-coordinate axis
         """
         R = self._get_rotation_matrix('y', degrees, radians)
         self._apply_rotation_matrix(R)
 
     def rotate_around_z(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around the 'z'-coordinate axis
         """
         R = self._get_rotation_matrix('z', degrees, radians)
         self._apply_rotation_matrix(R)
 
     def rotate_around_normal_vector(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around its normal_vector.
+
+        For a projection image, this is the depth direction.
         """
         R = self._get_rotation_matrix('normal_vector', degrees, radians)
         self._apply_rotation_matrix(R)
 
     def rotate_around_perp_vector1(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around its perp_vector1.
+
+        For an image, this is the horizontal axis.
         """
         R = self._get_rotation_matrix('perp_vector1', degrees, radians)
         self._apply_rotation_matrix(R)
 
     def rotate_around_perp_vector2(self, degrees=None, radians=None):
         """
+        Rotates the orientation instance around its perp_vector2.
+
+        For an image, this is the vertical axis.
         """
         R = self._get_rotation_matrix('perp_vector2', degrees, radians)
         self._apply_rotation_matrix(R)
 
     @property
     def inverse_rotation_matrix(self):
         """
@@ -241,33 +249,33 @@
         ey = self.cartesian_unit_vectors['y']
         ez = self.cartesian_unit_vectors['z']
         return np.array([ex, ey, ez])
 
     @property
     def rotation_matrix(self):
         """
-        This rotation matrix rotates the standard cartesian unit vectors
+        This rotation matrix rotates the standard cartesian unit vectors::
 
-        ex = [1, 0, 0]
-        ey = [0, 1, 0]
-        ez = [0, 0, 1]
+            ex = [1, 0, 0]
+            ey = [0, 1, 0]
+            ez = [0, 0, 1]
 
-        into the cartesian coordinate system defined by the three unit vectors
+        into the cartesian coordinate system defined by the three unit vectors::
 
-        perp_vector1
-        perp_vector2
-        normal_vector
+            perp_vector1
+            perp_vector2
+            normal_vector
 
         which can also be accessed through the cartesian_unit_vectors method.
 
-        That is, the following equality holds:
+        That is, the following equality holds::
 
-        perp_vector1 = np.matmul(rotation_matrix, [1, 0, 0])
-        perp_vector2 = np.matmul(rotation_matrix, [0, 1, 0])
-        normal_vector = np.matmul(rotation_matrix, [0, 0, 1])
+            perp_vector1 = np.matmul(rotation_matrix, [1, 0, 0])
+            perp_vector2 = np.matmul(rotation_matrix, [0, 1, 0])
+            normal_vector = np.matmul(rotation_matrix, [0, 0, 1])
         """
         return self.inverse_rotation_matrix.T
 
     @property
     def cartesian_unit_vectors(self):
         """
         The x, y, and z unit vectors in the Orientation
@@ -278,29 +286,43 @@
         unit_vectors['x'] = self.perp_vector1
         unit_vectors['y'] = self.perp_vector2
         unit_vectors['z'] = self.normal_vector
         return unit_vectors
 
     @property
     def spherical_unit_vectors(self):
+        """
+        To be implemented.
+
+        :meta private:
+        """
         raise RuntimeError('not implemented')
 
     @property
     def cylindrical_unit_vectors(self):
+        """
+        To be implemented.
+
+        :meta private:
+        """
         raise RuntimeError('not implemented')
 
     @property
     def euler_angles(self):
-        # TODO: intrinsic and extrinsic version?
+        """
+        To be implemented.
+
+        :meta private:
+        """
         raise RuntimeError('not implemented')
 
     @property
     def copy(self):
         """
-        Return a copy of the current Orientation instance.
+        Returns a copy of the current Orientation instance.
         """
         return Orientation(normal_vector=self.normal_vector,
                            perp_vector1=self.perp_vector1)
 
     def _are_equal(self, orientation2):
         """
         Compare the current orientation instance with a
@@ -311,17 +333,27 @@
         u2 = orientation2.cartesian_unit_vectors
         identical = True
         for key in u1:
             identical = np.allclose(u1[key], u2[key], atol=1e-15) and identical
         return identical
 
     def __print__(self):
+        """
+        Useful for displaying an Orientation instance.
+
+        :meta private:
+        """
         print('normal_vector:', self.normal_vector)
         print('perp_vector1: ', self.perp_vector1)
         print('perp_vector2: ', self.perp_vector2)
 
     def __repr__(self):
+        """
+        Useful for displaying an Orientation instance.
+
+        :meta private:
+        """
         s = 'Paicos Orientation instance\n'
         s += f'normal_vector: {self.normal_vector}\n'
         s += f'perp_vector1:  {self.perp_vector1}\n'
         s += f'perp_vector2:  {self.perp_vector2}'
         return s
```

### Comparing `paicos-0.1.8/paicos/paicos_user_settings_template.py` & `paicos-0.1.9/paicos/paicos_user_settings_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import paicos as pa
 
 """
-Set up your own default settings by renaming this file as user_settings.py.
+Set up your own default settings by renaming this file as paicos_user_settings.py
+and saving it at the directory found at: pa.code_dir
 
 Here we are overriding the defaults set in settings.py, so you only need
 to add things you want to change.
 """
 
 # Boolean determining whether we use Paicos quantities as a default
 pa.use_units(True)
```

### Comparing `paicos-0.1.8/paicos/readers/arepo_catalog.py` & `paicos-0.1.9/paicos/readers/arepo_catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This defines a reader for Arepo Friends-of-Friends (FoF) and subhalo catalog files"""
 import numpy as np
 import h5py
 from .paicos_readers import PaicosReader
+from ..writers.paicos_writer import PaicosWriter
 from .. import settings
 import numbers
 import warnings
 
 
 class Catalog(PaicosReader):
     """
@@ -16,37 +17,77 @@
     The class takes in the path of the directory containing the catalog, the
     catalog number, and an optional basename parameter, and uses this
     information to locate and open the catalog files. The class also loads
     the catalog's header, parameters, and configuration.
     The class also includes methods to extract the redshift, scale
     factor, and other properties of the catalog.
 
-    Important methods and attributes.
+    Important methods and attributes:
+    ---------------------------------
 
-    cat = Catalog()
+        cat = Catalog()
 
-    cat.Parameters (dict): Contains information from the parameter
-                            file used in the simulation (e.g. param.txt).
+        cat.Group : dict
+            Contains a dictionary of the FoF-catalog.
 
-    cat.Config (dict): Contains information from the Config
-                        file used in the simulation (e.g. Config.txt).
+        cat.Sub : dict
+            Contains a dictionary of the Subfind-catalog.
 
-    cat.Header (dict): Contains information about this particular catalog
-                        such as its time (e.g scale factor).
+        cat.Parameters : dict
+            Contains information from the parameter file used in the simulation (e.g. param.txt).
 
-    cat.z (float): redshift
+        cat.Config : dict
+            Contains information from the Config file used in the simulation (e.g. Config.txt).
 
-    cat.h (float): reduced Hubble param (e.g. 0.67)
+        cat.Header : dict
+            Contains information about this particular catalog such as its time (e.g scale factor).
 
-    cat.age: the age of the Universe (only for cosmological runs)
-    cat.lookback_time: the age of the Universe (only for cosmological runs)
+        cat.z : float
+            The redshift.
+
+        cat.h : float
+            Reduced Hubble param (e.g. 0.67).
+
+        cat.age : float
+            The age of the Universe (only for cosmological runs).
+
+        cat.lookback_time : float
+            The age of the Universe (only for cosmological runs).
 
     """
-    def __init__(self, basedir='.', snapnum=None,
+    def __init__(self, basedir='.', snapnum=None, load_all=True,
                  to_physical=False, subfind_catalog=True, verbose=False):
+        """
+        Initializes the Catalog class.
+
+        Parameters
+        ----------
+
+            basedir : str
+                The path of the directory containing the catalogs
+                (e.g. the 'output' folder).
+
+            snapnum : int
+                The snapshot number.
+
+            load_all : bool
+                Whether to immediately load all fields or not.
+
+            to_physical : bool
+                whether to convert to physical unit upon loading the data.
+                Default is False.
+
+            subfind_catalog : bool
+                whether the simulation has subfind catalogs,
+                when False the code will look for FoF-catalogs only.
+
+            verbose : bool
+                whether to print information, default is False.
+
+        """
 
         if subfind_catalog:
             basename = 'fof_subhalo_tab'
         else:
             basename = 'fof_tab'
 
         super().__init__(basedir=basedir, snapnum=snapnum, basename=basename,
@@ -58,28 +99,35 @@
         self.ngroups = self.Header["Ngroups_Total"]
 
         if "Nsubgroups_Total" in self.Header.keys():
             self.nsubs = self.Header["Nsubgroups_Total"]
         else:
             self.nsubs = self.Header["Nsubhalos_Total"]
 
+        # Initialize dictionaries
+        self.Group = {}
+        self.Sub = {}
+
         # Load all data
-        self.load_all_data()
+        if load_all:
+            self.load_all_data()
 
     def load_data(self):
         """
-        Overwrite the base class method
+        Overwrite of the base class method.
+
+        :meta private:
         """
         pass
 
     def load_all_data(self):
         """
-        Calling method simply loads all the data in the catalog.
+        Calling this method simply loads all the data in the catalog.
 
-        For large catalogs it might be useful to implement on-demand
+        TODO: For large catalogs it might be useful to implement on-demand
         access in a similar way to what we have for snapshots.
         """
 
         skip_gr = 0
         skip_sub = 0
         for ifile in range(self.nfiles):
             if self.multi_file is False:
@@ -98,47 +146,48 @@
             ng = int(file["Header"].attrs["Ngroups_ThisFile"])
 
             if "Nsubgroups_ThisFile" in file["Header"].attrs.keys():
                 ns = int(file["Header"].attrs["Nsubgroups_ThisFile"])
             else:
                 ns = int(file["Header"].attrs["Nsubhalos_ThisFile"])
 
-            # initialze arrays
+            # initialize arrays
             if ifile == 0:
-                self.Group = {}
-                self.Sub = {}
-                for ikey in file["Group"].keys():
-                    if len(file["Group/" + ikey].shape) == 1:
-                        self.Group[ikey] = np.empty(
-                            self.ngroups, dtype=file["Group/" + ikey].dtype)
-                    elif len(file["Group/" + ikey].shape) == 2:
-                        self.Group[ikey] = np.empty(
-                            (self.ngroups, file["Group/" + ikey].shape[1]),
-                            dtype=file["Group/" + ikey].dtype)
-                    else:
-                        assert False
-
-                for ikey in file["Subhalo"].keys():
-                    if len(file["Subhalo/" + ikey].shape) == 1:
-                        self.Sub[ikey] = np.empty(
-                            self.nsubs, dtype=file["Subhalo/" + ikey].dtype)
-                    elif len(file["Subhalo/" + ikey].shape) == 2:
-                        self.Sub[ikey] = np.empty(
-                            (self.nsubs, file["Subhalo/" + ikey].shape[1]),
-                            dtype=file["Subhalo/" + ikey].dtype)
-                    else:
-                        assert False
+                if "Group" in file:
+                    for ikey in file["Group"].keys():
+                        if len(file["Group/" + ikey].shape) == 1:
+                            self.Group[ikey] = np.empty(
+                                self.ngroups, dtype=file["Group/" + ikey].dtype)
+                        elif len(file["Group/" + ikey].shape) == 2:
+                            self.Group[ikey] = np.empty(
+                                (self.ngroups, file["Group/" + ikey].shape[1]),
+                                dtype=file["Group/" + ikey].dtype)
+                        else:
+                            assert False
+                if "Subhalo" in file:
+                    for ikey in file["Subhalo"].keys():
+                        if len(file["Subhalo/" + ikey].shape) == 1:
+                            self.Sub[ikey] = np.empty(
+                                self.nsubs, dtype=file["Subhalo/" + ikey].dtype)
+                        elif len(file["Subhalo/" + ikey].shape) == 2:
+                            self.Sub[ikey] = np.empty(
+                                (self.nsubs, file["Subhalo/" + ikey].shape[1]),
+                                dtype=file["Subhalo/" + ikey].dtype)
+                        else:
+                            assert False
 
             # read group data
-            for ikey in file["Group"].keys():
-                self.Group[ikey][skip_gr:skip_gr + ng] = file["Group/" + ikey]
+            if ng > 0:
+                for ikey in file["Group"].keys():
+                    self.Group[ikey][skip_gr:skip_gr + ng] = file["Group/" + ikey]
 
             # read subhalo data
-            for ikey in file["Subhalo"].keys():
-                self.Sub[ikey][skip_sub:skip_sub + ns] = file["Subhalo/" + ikey]
+            if ns > 0:
+                for ikey in file["Subhalo"].keys():
+                    self.Sub[ikey][skip_sub:skip_sub + ns] = file["Subhalo/" + ikey]
 
             skip_gr += ng
             skip_sub += ns
 
             file.close()
 
         # Load all variables with double precision
@@ -166,7 +215,43 @@
 
             for key in list(self.Sub.keys()):
                 self.Sub[key] = self.get_paicos_quantity(
                     self.Sub[key], key,
                     field='subhalos')
                 if not hasattr(self.Sub[key], 'unit'):
                     del self.Sub[key]
+
+    def save_new_catalog(self, basename, single_precision=False):
+        """
+        Save a new catalog containing only the currently loaded
+        variables. Useful for reducing datasets to smaller sizes.
+        """
+        writer = PaicosWriter(self, self.basedir, basename, 'w')
+
+        for key in self.Group:
+            Ngroups_Total = self.Group[key].shape[0]
+
+            if single_precision:
+                data = self.Group[key].astype(np.float32)
+            else:
+                data = self.Group[key]
+            writer.write_data(key, data, group='Group')
+
+        for key in self.Sub:
+            Nsubgroups_Total = self.Sub[key].shape[0]
+
+            if single_precision:
+                data = self.Sub[key].astype(np.float32)
+            else:
+                data = self.Sub[key]
+            writer.write_data(key, data, group='Subhalo')
+
+        with h5py.File(writer.tmp_filename, 'r+') as f:
+            f['Header'].attrs["Ngroups_ThisFile"] = Ngroups_Total
+            f['Header'].attrs["Ngroups_Total"] = Ngroups_Total
+            f['Header'].attrs["Nsubgroups_ThisFile"] = Nsubgroups_Total
+            f['Header'].attrs["Nsubgroups_Total"] = Nsubgroups_Total
+            f['Header'].attrs["NumFiles"] = 1
+
+        writer.finalize()
+
+        return writer
```

### Comparing `paicos-0.1.8/paicos/readers/arepo_snap.py` & `paicos-0.1.9/paicos/readers/arepo_snap.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,67 +24,81 @@
     information to locate and open the snapshot files. The class also loads
     the snapshot's header, parameters, and configuration, and uses them to
     create a converter object that can be used to convert units in the
     snapshot. The class also includes methods to extract the redshift, scale
     factor, and other properties of the snapshot, as well as the subfind
     catalog if present.
 
-    Important methods and attributes.
+    Important methods and attributes:
+    ---------------------------------
 
-    snap = Snapshot()
+        snap = Snapshot()
 
-    snap.Parameters (dict): Contains information from the parameter
-                            file used in the simulation (e.g. param.txt).
+        snap.Group : dict
+            Contains a dictionary of the FoF-catalog.
 
-    snap.Config (dict): Contains information from the Config
-                        file used in the simulation (e.g. Config.txt).
+        snap.Sub : dict
+            Contains a dictionary of the Subfind-catalog.
 
-    snap.Header (dict): Contains information about this particular snapshot
-                        such as its time (e.g scale factor).
+        snap.Parameters : dict
+            Contains information from the parameter file used in the simulation (e.g. param.txt).
 
-    snap.z (float): redshift
+        snap.Config : dict
+            Contains information from the Config file used in the simulation (e.g. Config.txt).
 
-    snap.h (float): reduced Hubble param (e.g. 0.67)
+        snap.Header : dict
+            Contains information about this particular catalog such as its time (e.g scale factor).
 
-    snap.age: the age of the Universe (only for cosmological runs)
-    snap.lookback_time: the age of the Universe (only for cosmological runs)
+        snap.z : float
+            The redshift.
 
-    snap.time: the time stamp of the snapshot (only for non-cosmological runs)
+        snap.h : float
+            Reduced Hubble param (e.g. 0.67).
 
-    snap.box_size: the dimensions of the simulation domain
+        snap.age : float
+            The age of the Universe (only for cosmological runs).
+
+        snap.lookback_time : float
+            The age of the Universe (only for cosmological runs).
+
+        snap.time : float
+            The time stamp of the snapshot (only for non-cosmological runs).
+
+        snap.box_size : array with length 3
+            The dimensions of the simulation domain.
 
     """
 
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self, basedir, snapnum=None, basename="snap", load_all=False,
                  to_physical=False, load_catalog=None, verbose=False):
         """
         Initialize the Snapshot class.
 
         Parameters:
 
-        basedir (str): path of the directory containing the snapshot
-                       (e.g. the 'output' folder)
+            basedir (str): path of the directory containing the snapshot
+                           (e.g. the 'output' folder).
 
-        snapnum (int): snapshot number
+            snapnum (int): snapshot number.
 
-        basename (str): name of the snapshot file, default is "snap"
+            basename (str): name of the snapshot file, default is "snap".
 
-        verbose (bool): whether to print information about the snapshot,
-        default is False
+            verbose (bool): whether to print information about the snapshot,
+                            default is False.
 
-        no_snapdir (bool): whether there is no snap directory, i.e.,
-                           default is False
+            no_snapdir (bool): whether there is no snap directory, i.e.,
+                               default is False.
 
-        load_catalog (bool): whether to load the subfind catalog.
-                             The default None is internally changed to
-                             True for comoving simulations and to
-                             False for non-comoving simulations.
-    """
+            load_catalog (bool): whether to load the subfind catalog.
+                                 The default None is internally changed to
+                                 True for comoving simulations and to
+                                 False for non-comoving simulations.
+        """
 
         super().__init__(basedir=basedir, snapnum=snapnum, basename=basename,
                          load_all=load_all, to_physical=to_physical,
                          basesubdir='snapdir', verbose=verbose)
 
         assert self.snapnum is not None
 
@@ -248,15 +262,15 @@
                 self._type_info[p] = 'stars'
 
     def _find_available_functions(self):
         """
         This function goes through all the implemented functions
         for getting derived variables. Checking their dependencies,
         it then figures out which derived variables are actually possible
-        for this particular snapshot. For instance, you can calculate the
+        for this particular snapshot. For instance, you cannot calculate the
         magnetic field strength if the magnetic field is not stored in
         the hdf5 file.
         """
 
         user_functs = derived_variables.user_functions
 
         for func_name, func in user_functs.items():
@@ -283,15 +297,15 @@
                 self._dependency_dic[func_name] = []
 
         dependency_dic = dict(self._dependency_dic)
 
         # We then trim the dependency dictionary
 
         # This will fail for very nested dependencies.
-        for _ in range(3):
+        for _ in range(4):
             # First substitute all dependencies that are
             # at the top level of the dictionary
             for func_name, deps in dependency_dic.items():
                 for dep in list(deps):
                     if dep in dependency_dic:
                         deps.remove(dep)
                         for subdep in dependency_dic[dep]:
@@ -314,14 +328,16 @@
                 del self._this_snap_funcs[func_name]
 
     def get_variable_function(self, p_key, info=False):
         """
         This is a helper function for 'get_derived_data'. It returns a
         function if info is False, and a list of all available
         functions for parttype = p_key[0] if info is True.
+
+        :meta private:
         """
 
         assert isinstance(p_key, str)
 
         if not p_key[0].isnumeric() or p_key[1] != '_':
             msg = (f"The key '{p_key}' is not valid."
                    + "\n\nKeys are expected to consist of an integer "
@@ -348,20 +364,32 @@
         raise RuntimeError(msg)
 
     def info(self, parttype, verbose=True):
         """
         This function provides information about the keys of a certain
         particle type in a snapshot.
 
-        Args: PartType (int): An integer representing the particle type of
-        interest. verbose (bool, optional): A flag indicating whether or not
-        to print the keys to the console. Defaults to True.
+        Parameters
+        -----------
 
-        Returns: list or None : If the PartType exists in the file, a list of
-        keys for that PartType is returned, otherwise None.
+            partType (int):
+                           An integer representing the particle type of
+                           interest, e.g. 0 for gas, 1 for DM etc.
+
+            verbose (bool):
+                           A flag indicating whether or not
+                           to print the keys to the console.
+                           Defaults to True.
+
+        Returns
+        -------
+
+            list or None :
+                          If the requested PartType exists in the file, a list of
+                          keys for that PartType is returned, otherwise None.
         """
         parttype_str = f'PartType{parttype}'
         if parttype >= self.nspecies:
             err_msg = (f"Parttype {self.nspecies-1} is the largest contained"
                        + f" in the snapshot which has nspecies={self.nspecies}.")
             raise RuntimeError(err_msg)
 
@@ -389,27 +417,26 @@
                         msg = alias + '\t' * 5 + '(an alias of {})'
                         print_key = msg.format(key)
 
                 print(print_key)
         else:
             return load_keys
 
-    def load_data_experimental(self, parttype, blockname):
+    def _load_data_experimental(self, parttype, blockname):
         """
-        Load data from hdf5 file(s). Example usage:
-
-        snap = Snapshot(...)
+        Load data from hdf5 file(s). Example usage::
 
-        snap.load_data(0, 'Density')
+            snap = Snapshot(...)
+            snap.load_data(0, 'Density')
 
         Note that subsequent calls does not reload the data. Reloading
-        the data can be done explicitly:
+        the data can be done explicitly::
 
-        snap.remove_data(0, 'Density')
-        snap.load_data(0, 'Density')
+            snap.remove_data(0, 'Density')
+            snap.load_data(0, 'Density')
 
         """
 
         assert parttype < self.nspecies
 
         p_key = f'{parttype}_{blockname}'
         alias_key = p_key
@@ -432,15 +459,17 @@
         if self.verbose:
             print("loading block", blockname,
                   "for species", parttype, "...")
             start_time = time.time()
 
         def read_hdf5_file(filename, parttype, blockname):
             """
-            This helper function does the actual data loading
+            This helper function does the actual data loading.
+
+            :meta private:
             """
             parttype_str = f'PartType{parttype}'
             with h5py.File(filename, 'r') as f:
                 # Load a dataset
                 dataset = f[parttype_str][blockname][()]
 
             if settings.double_precision:
@@ -489,26 +518,24 @@
                 raise RuntimeError('Data has unexpected shape!')
 
         if self.verbose:
             print("... done! (took", time.time() - start_time, "s)")
 
     def load_data(self, parttype, blockname):
         """
-        Load data from hdf5 file(s). Example usage:
+        Load data from hdf5 file(s). Example usage::
 
-        snap = Snapshot(...)
-
-        snap.load_data(0, 'Density')
+            snap = Snapshot(...)
+            snap.load_data(0, 'Density')
 
         Note that subsequent calls does not reload the data. Reloading
-        the data can be done explicitly:
-
-        snap.remove_data(0, 'Density')
-        snap.load_data(0, 'Density')
+        the data can be done explicitly::
 
+            snap.remove_data(0, 'Density')
+            snap.load_data(0, 'Density')
         """
 
         assert parttype < self.nspecies
 
         p_key = f'{parttype}_{blockname}'
         alias_key = p_key
 
@@ -542,15 +569,15 @@
                 if self.no_subdir:
                     cur_filename = self.multi_wo_dir.format(ifile)
                 else:
                     cur_filename = self.multi_filename.format(ifile)
 
             f = h5py.File(cur_filename, "r")
 
-            np_file = f["Header"].attrs["NumPart_ThisFile"][parttype]
+            np_file = int(f["Header"].attrs["NumPart_ThisFile"][parttype])
 
             if ifile == 0:   # initialize array
                 shape = self._part_specs[parttype][blockname]['shape']
                 dtype = self._part_specs[parttype][blockname]['dtype']
                 if len(shape) == 1:
                     self[alias_key] = np.empty(self.npart[parttype], dtype=dtype)
                 else:
@@ -602,14 +629,15 @@
         """
         Get derived quantities. Example usage:
 
         snap = Snapshot(...)
 
         snap.get_derived_data(0, 'Temperatures')
 
+        :meta private:
         """
         # from .derived_variables import get_variable_function
 
         p_key = str(parttype) + "_" + blockname
 
         msg = (f'\n\n{blockname} is in the hdf5 file(s), please use load_data '
                + 'instead of get_derived_data')
@@ -729,17 +757,18 @@
             del self.P_attrs[p_key]
 
     def select(self, selection_index, parttype=None):
         """
         Create a new snapshot object which will only contain
         cells with a selection_index.
 
-        Example use:
-        index = snap['0_Density'] > snap['0_Density'].unit_quantity*1e-6
-        selected_snap = snap.select(index, parttype=0)
+        Example use::
+
+            index = snap['0_Density'] > snap['0_Density'].unit_quantity*1e-6
+            selected_snap = snap.select(index, parttype=0)
 
         """
         if parttype is None:
             parttype = 0
             msg = ("You have not specified the parttype that the selection index"
                    + " corresponds to. The code will assume parttype=0. Future versions"
                    + " of this method will likely have parttype as a required input")
@@ -786,17 +815,19 @@
             else:
                 select_snap[key] = self[key]
 
         return select_snap
 
     def radial_select(self, center, r_max, r_min=0.0, parttype=None):
         """
-        A convenient function for selecting in radius
+        A convenience function for selecting in radius.
 
-        Returns a new snapshot with the radial selection
+        Returns a new snapshot with the radial selection.
+
+        :meta private:
         """
         from .. import util
         if parttype is None:
 
             index = util.get_index_of_radial_range(self['0_Coordinates'],
                                                    center, r_min, r_max)
 
@@ -833,24 +864,27 @@
                     else:
                         data = self[key]
                     writer.write_data(key[2:], data, group=parttype_str)
 
         with h5py.File(writer.tmp_filename, 'r+') as f:
             f['Header'].attrs["NumFilesPerSnapshot"] = 1
             f['Header'].attrs["NumPart_Total"] = np.array(new_npart)
+            f['Header'].attrs["NumPart_ThisFile"] = np.array(new_npart)
 
         writer.finalize()
 
         return writer
 
     def get_sum_of_array(self, variable):
         """
         Find the sum of a 1D array.
 
         Equivalent to np.sum(arr, axis=0) but with open_mp
+
+        :meta private:
         """
         from .. import util
 
         if isinstance(variable, str):
             variable = self[variable]
         else:
             if not isinstance(variable, np.ndarray):
@@ -871,14 +905,16 @@
         return sum_omp(variable, settings.numthreads_reduction)
 
     def get_sum_of_array_times_vector(self, arr, vector):
         """
         Find the sum of a 1D array times a 2D array
 
         Equivalent to np.sum(arr[:, None] * vector, axis=0) but with open_mp
+
+        :meta private:
         """
         from .. import util
         from ..cython.get_derived_variables import sum_arr_times_vector_omp
         numthreads = settings.numthreads_reduction
 
         if isinstance(arr, str):
             arr = self[arr]
@@ -902,14 +938,16 @@
         return sum_arr_times_vector_omp(arr, vector, numthreads)
 
     def get_sum_of_arr_times_vector_cross_product(self, mass, coord, velocity, center):
         """
         This code calculates sum_i (mass_i (coord_ij - center) x velocity_ij).
 
         That is, it returns the total angular momentum vector.
+
+        :meta private:
         """
         from .. import util
         from ..cython.get_derived_variables import sum_arr_times_vector_cross_product
         numthreads = settings.numthreads_reduction
 
         if isinstance(mass, str):
             mass = self[mass]
@@ -936,21 +974,22 @@
             return sum_func(mass, coord, velocity, center, numthreads) * uq
         return sum_func(mass, coord, velocity, center, numthreads)
 
     def center_of_mass(self, parttype=None):
         """
         Finds the center of mass for the entire snapshot.
 
-        parttype (default None): if None, then all parttypes are included in the
+        parttype (default None):
+                                 If None, then all parttypes are included in the
                                  center-of-mass calculation. If e.g. parttype=0,
                                  then the center of mass of the gas is returned.
                                  if parttype=None, then the total center and
                                  a list of of the parttype centers are returned
 
-        Can be used in combination with self.select to find the
+        This method can be used in combination with the select method to find the
         center of mass of a selection.
         """
         if parttype is None:
             mass = [self.get_sum_of_array(f'{p}_Masses') for p in range(self.nspecies)]
             mcord = [self.get_sum_of_array_times_vector(f'{p}_Masses', f'{p}_Coordinates')
                      for p in range(self.nspecies)]
             centers = [mcord[p] / mass[p] for p in range(self.nspecies)]
@@ -966,19 +1005,20 @@
 
     def total_angular_momentum(self, center, parttype=None):
         """
         Finds the total angular momentum for the entire snapshot.
 
         center: the center around which to calculate the angular momentum
 
-        parttype (default None): if None, then all parttypes are included in the
+        parttype (default None):
+                                 If None, then all parttypes are included in the
                                  calculation. If e.g. parttype=0,
                                  then total angular momentum of the gas is returned.
 
-        Can be used in combination with self.select to find the
+        This method can be used in combination with the select method to find the
         total angular momentum of a selection.
         """
         func = self.get_sum_of_arr_times_vector_cross_product
         if parttype is None:
             if settings.use_units:
                 for p in range(self.nspecies):
                     assert self[f'{p}_Coordinates'].unit == center.unit
```

### Comparing `paicos-0.1.8/paicos/readers/paicos_readers.py` & `paicos-0.1.9/paicos/readers/paicos_readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Defines the PaicosReader, Histogram2DReader and ImageReader which
 can be used to load derived variables.
 """
 import os
 import h5py
 import numpy as np
+import traceback
 from astropy import units as u
 from astropy.cosmology import LambdaCDM
 from .. import util
 from .. import units as pu
 from .. import settings
 from ..orientation import Orientation
 from ..image_creators.image_creator import ImageCreator
@@ -28,32 +29,40 @@
     def __init__(self, basedir='.', snapnum=None, basename="snap",
                  basesubdir='snapdir', load_all=True, to_physical=False,
                  verbose=False):
 
         """
         Initialize the PaicosReader class.
 
-        Parameters:
+        Parameters
+        ----------
 
-        basedir (str): path of the directory containing the hdf5 files
-                       (e.g. the 'output' folder)
+            basedir : str
+                The path of the directory containing the hdf5 files
+                (e.g. the 'output' folder).
 
-        snapnum (int): e.g. snapshot number
+            snapnum : int
+                e.g. the snapshot number
 
-        basename (str): name of the file takes the form 'basename_{:03d}.hdf5'
-                        or 'basename_{:03d}.{}.hdf5'. Default is 'snap'.
+            basename : str
+                name of the file takes the form ``basename_{:03d}.hdf5``
+                or ``basename_{:03d}.{}.hdf5``. Default is ``snap``.
 
-        basesubdir (str): name of the subfolder. Default is "snapdir".
+            basesubdir : str
+                The name of the subfolder. Default is ``snapdir``.
 
-        load_all (bool): whether to simply load all data, default is True
+            load_all : bool
+                Whether to simply load all data, default is True.
 
-        to_physical (bool): whether to convert from comoving to physical
-                            variables upon load, not yet implemented!
+            to_physical : bool
+                Whether to convert from comoving to physical
+                variables upon load.
 
-        verbose (bool): whether to print information, default is False
+            verbose : bool
+                Whether to print information, default is False.
         """
 
         self.to_physical = to_physical
         self.verbose = verbose
 
         if '.hdf5' in basedir:
             # User is trying to load a single hdf5 file directly, let's see if
@@ -114,176 +123,214 @@
         with h5py.File(self.filename, 'r') as f:
             self.Header = dict(f['Header'].attrs)
             self.Config = dict(f['Config'].attrs)
             self.Parameters = dict(f['Parameters'].attrs)
             keys = list(f.keys())
 
         # Enable units
-        self.get_units_and_other_parameters()
-        self.enable_units()
-        self.add_user_units()
+            self.get_units_and_other_parameters()
+        if settings.use_units:
+            self.enable_units()
+            self.add_user_units()
 
         # Find the adiabatic index
         self.gamma = self.get_adiabiatic_index()
 
         # Load all data sets
         if load_all:
             for key in keys:
                 self.load_data(key)
 
         self.load_org_info()
 
     def load_org_info(self):
         """
-        Load some extra info about original data
+        Load some extra info about original data.
+
+        :meta private:
         """
         with h5py.File(self.filename, 'r') as f:
             if 'org_info' in f:
                 self['org_info'] = {}
                 for key in f['org_info'].attrs.keys():
                     self['org_info'][key] = f['org_info'].attrs[key]
 
     def get_units_and_other_parameters(self):
         """
         Define arepo units, scale factor (a) and h (HubbleParam).
 
         The input required is a hdf5 file with the Parameters and Header
         groups found in arepo snapshots.
-        """
 
+        :meta private:
+        """
         self._Time = self.Header['Time']
-        self._Redshift = self.Header['Redshift']
         self._HubbleParam = self.Parameters['HubbleParam']
 
-        unit_length = self.Parameters['UnitLength_in_cm'] * u.cm
-        unit_mass = self.Parameters['UnitMass_in_g'] * u.g
-        unit_velocity = self.Parameters['UnitVelocity_in_cm_per_s'] * u.cm / u.s
-        unit_time = unit_length / unit_velocity
-        unit_energy = unit_mass * unit_velocity**2
-        unit_pressure = (unit_mass / unit_length) / unit_time**2
-        unit_density = unit_mass / unit_length**3
-        Omega0 = self.Parameters['Omega0']
-        OmegaBaryon = self.Parameters['OmegaBaryon']
-        OmegaLambda = self.Parameters['OmegaLambda']
-
         ComovingIntegrationOn = self.Parameters['ComovingIntegrationOn']
 
         self.ComovingIntegrationOn = bool(ComovingIntegrationOn)
         self.comoving_sim = self.ComovingIntegrationOn
 
         if self.ComovingIntegrationOn:
+            self._Redshift = self.Header['Redshift']
+
+            Omega0 = self.Parameters['Omega0']
+            OmegaBaryon = self.Parameters['OmegaBaryon']
+            OmegaLambda = self.Parameters['OmegaLambda']
+
             # Set up LambdaCDM cosmology to calculate times, etc
             self.cosmo = LambdaCDM(H0=100 * self.h, Om0=Omega0,
                                    Ob0=OmegaBaryon, Ode0=OmegaLambda)
             # Current age of the universe and look back time
             self._age = self.get_age(self.z)
             self._lookback_time = self.get_lookback_time(self.z)
 
-        _ns = globals()
-        arepo_mass = u.def_unit(
-            ["arepo_mass"],
-            unit_mass,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo mass unit",
-            format={"latex": r"arepo\_mass"},
-        )
-        arepo_time = u.def_unit(
-            ["arepo_time"],
-            unit_time,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo time unit",
-            format={"latex": r"arepo\_time"},
-        )
-        arepo_length = u.def_unit(
-            ["arepo_length"],
-            unit_length,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo length unit",
-            format={"latex": r"arepo\_length"},
-        )
-        arepo_velocity = u.def_unit(
-            ["arepo_velocity"],
-            unit_velocity,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo velocity unit",
-            format={"latex": r"arepo\_velocity"},
-        )
-        arepo_pressure = u.def_unit(
-            ["arepo_pressure"],
-            unit_pressure,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo pressure unit",
-            format={"latex": r"arepo\_pressure"},
-        )
-        arepo_energy = u.def_unit(
-            ["arepo_energy"],
-            unit_energy,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo energy unit",
-            format={"latex": r"arepo\_energy"},
-        )
-        arepo_density = u.def_unit(
-            ["arepo_density"],
-            unit_density,
-            prefixes=False,
-            namespace=_ns,
-            doc="Arepo density unit",
-            format={"latex": r"arepo\_density"},
-        )
-
-        self.arepo_units_in_cgs = {'unit_length': unit_length,
-                                   'unit_mass': unit_mass,
-                                   'unit_velocity': unit_velocity,
-                                   'unit_time': unit_time,
-                                   'unit_energy': unit_energy,
-                                   'unit_pressure': unit_pressure,
-                                   'unit_density': unit_density}
-
-        self.arepo_units = {'unit_length': arepo_length,
-                            'unit_mass': arepo_mass,
-                            'unit_velocity': arepo_velocity,
-                            'unit_time': arepo_time,
-                            'unit_energy': arepo_energy,
-                            'unit_pressure': arepo_pressure,
-                            'unit_density': arepo_density}
+        missing_unitinfo = True
+        if 'UnitLength_in_cm' in self.Parameters:
+            if 'UnitMass_in_g' in self.Parameters:
+                if 'UnitVelocity_in_cm_per_s' in self.Parameters:
+                    missing_unitinfo = False
+
+        if settings.use_units and missing_unitinfo:
+            raise RuntimeError("Units mssing in self.Parameters!")
+
+        if not missing_unitinfo:
+            unit_length = self.Parameters['UnitLength_in_cm'] * u.cm
+            unit_mass = self.Parameters['UnitMass_in_g'] * u.g
+            unit_velocity = self.Parameters['UnitVelocity_in_cm_per_s'] * u.cm / u.s
+            unit_time = unit_length / unit_velocity
+            unit_energy = unit_mass * unit_velocity**2
+            unit_pressure = (unit_mass / unit_length) / unit_time**2
+            unit_density = unit_mass / unit_length**3
+
+            self.arepo_units_in_cgs = {'unit_length': unit_length,
+                                       'unit_mass': unit_mass,
+                                       'unit_velocity': unit_velocity,
+                                       'unit_time': unit_time,
+                                       'unit_energy': unit_energy,
+                                       'unit_pressure': unit_pressure,
+                                       'unit_density': unit_density}
+
+        if settings.use_units:
+
+            _ns = globals()
+
+            try:
+                arepo_mass = u.def_unit(
+                    ["arepo_mass"],
+                    unit_mass,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo mass unit",
+                    format={"latex": r"arepo\_mass"},
+                )
+                arepo_time = u.def_unit(
+                    ["arepo_time"],
+                    unit_time,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo time unit",
+                    format={"latex": r"arepo\_time"},
+                )
+                arepo_length = u.def_unit(
+                    ["arepo_length"],
+                    unit_length,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo length unit",
+                    format={"latex": r"arepo\_length"},
+                )
+                arepo_velocity = u.def_unit(
+                    ["arepo_velocity"],
+                    unit_velocity,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo velocity unit",
+                    format={"latex": r"arepo\_velocity"},
+                )
+                arepo_pressure = u.def_unit(
+                    ["arepo_pressure"],
+                    unit_pressure,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo pressure unit",
+                    format={"latex": r"arepo\_pressure"},
+                )
+                arepo_energy = u.def_unit(
+                    ["arepo_energy"],
+                    unit_energy,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo energy unit",
+                    format={"latex": r"arepo\_energy"},
+                )
+                arepo_density = u.def_unit(
+                    ["arepo_density"],
+                    unit_density,
+                    prefixes=False,
+                    namespace=_ns,
+                    doc="Arepo density unit",
+                    format={"latex": r"arepo\_density"},
+                )
+            except ValueError:
+                traceback.print_exc()
+                err_msg = ("Re-declaration of arepo code units attempted "
+                           + "within same Python session. "
+                           + "See https://github.com/tberlok/paicos/issues/59")
+                raise RuntimeError(err_msg)
+
+            self.arepo_units = {'unit_length': arepo_length,
+                                'unit_mass': arepo_mass,
+                                'unit_velocity': arepo_velocity,
+                                'unit_time': arepo_time,
+                                'unit_energy': arepo_energy,
+                                'unit_pressure': arepo_pressure,
+                                'unit_density': arepo_density}
 
     def enable_units(self):
         """
-        Enables arepo units globally
+        Enables arepo units globally.
+
+        :meta private:
         """
         for unit_name, unit in self.arepo_units.items():
             u.add_enabled_units(unit)
             phys_type = unit_name.split('_')[1]
             u.def_physical_type(unit, phys_type)
 
         self._length = self.get_paicos_quantity(1, 'Coordinates')
         self._mass = self.get_paicos_quantity(1, 'Masses')
         self._velocity = self.get_paicos_quantity(1, 'Velocities')
 
     @property
     def length(self):
+        """The unit of length used in the simulation."""
         return self._length
 
     @property
     def mass(self):
+        """The unit of mass used in the simulation."""
         return self._mass
 
     @property
     def velocity(self):
+        """
+        One of the units used for velocities in the simulation.
+
+        Note: The a and h-scalings are not the same for velocities
+        in the halo catalogs and in the snapshots.
+        """
         return self._velocity
 
     def add_user_units(self):
         """
         Add all user supplied units
+
+        :meta private:
         """
         # pylint: disable=import-outside-toplevel, consider-using-dict-items
         from .. import unit_specifications
 
         unit_dict = unit_specifications.unit_dict
         user_unit_dict = util.user_unit_dict
 
@@ -494,15 +541,15 @@
                 raise RuntimeError(msg.format(field, name))
             return False
 
         return self._sanitize_unit(unit)
 
     def unit_quantity(self, astropy_unit_str):
         """
-        Return a Paicos quantity with value 1 and any
+        Returns a Paicos quantity with value 1 and any
         astropy unit.
         """
         unit = u.Unit(astropy_unit_str)
         return pu.PaicosQuantity(1.0, unit, a=self._Time, h=self.h,
                                  comoving_sim=self.comoving_sim,
                                  dtype=float)
 
@@ -529,16 +576,16 @@
 
     def load_data(self, name, group=None):
         """
         Load data from a generic Paicos hdf5 file (written by a PaicosWriter
         instance).
 
         The method requires that the data sets have a 'unit' attribute
-        and hence does work for Arepo hdf5 files.
-        For this reason, the method is overloaded in the Snapshot and Catalog
+        and hence does not work for Arepo hdf5 files.
+        For this reason, this method is overloaded in the Snapshot and Catalog
         classes.
         """
 
         with h5py.File(self.filename, 'r') as f:
             if isinstance(f[name], h5py.Dataset):
                 self[name] = util.load_dataset(f, name, group=group)
                 if isinstance(self[name], pu.PaicosQuantity) and self.to_physical:
@@ -626,14 +673,25 @@
 
         self.area_per_pixel = self.area / (self.npix_width * self.npix_height)
         self.volume_per_pixel = self.volume / (self.npix_width * self.npix_height)
 
         self.dw = self.width / self.npix_width
         self.dh = self.height / self.npix_height
 
+        # Get derived images
+        self.get_derived_images()
+
+    @np.errstate(divide='ignore', invalid='ignore')
+    def get_derived_images(self):
+        """
+        Calculate images automatically for convenience,
+        e.g., 0_MagneticFieldSquaredTimesVolume and 0_Volume
+        are divided to obtain a 2D-array with 0_MagneticFieldSquared
+        """
+
         # Get derived images from projection-files
         keys = list(self.keys())
         for key in keys:
             if 'Times' in key:
                 # Keys of the form 'MagneticFieldSquaredTimesVolume'
                 # are split up
                 start, end = key.split('Times')
```

### Comparing `paicos-0.1.8/paicos/settings.py` & `paicos-0.1.9/paicos/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # Enable spherical coordinates
 spherical_coords = False
 
 # Enable cylindrical coordinates
 cyl_coords = False
 
 # Whether to load GPU/cuda functionality on startup
-load_cuda_functionality_on_startup = True
+load_cuda_functionality_on_startup = False
```

### Comparing `paicos-0.1.8/paicos/trees/bvh_cpu.py` & `paicos-0.1.9/paicos/trees/bvh_cpu.py`

 * *Files identical despite different names*

### Comparing `paicos-0.1.8/paicos/trees/bvh_gpu.py` & `paicos-0.1.9/paicos/trees/bvh_gpu.py`

 * *Files identical despite different names*

### Comparing `paicos-0.1.8/paicos/trees/bvh_tree.pyx` & `paicos-0.1.9/paicos/trees/bvh_tree.pyx`

 * *Files identical despite different names*

### Comparing `paicos-0.1.8/paicos/unit_specifications.py` & `paicos-0.1.9/paicos/unit_specifications.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,37 @@
 https://www.tng-project.org/data/docs/specifications/
 """
 
 unit_less = u.Unit('')
 
 Coordinates = u.Unit('arepo_length small_a / small_h')
 Masses = u.Unit('arepo_mass / small_h')
+
+# The velocity output has this scaling for historical reasons
 Velocities = u.Unit('arepo_velocity  small_a^(1/2)')
 
+# Gas velocities have a different scaling internally in Arepo,
+# i.e., they are given in terms of w = u a,
+# where u is the peculiar velocity
+InternalVelocities = u.Unit('arepo_velocity  small_a^(-1)')
+
 Potential = u.Unit('arepo_velocity^2 / small_a')
 
 MagneticField = u.Unit('arepo_pressure^(1/2) small_a^-2 small_h')
 
 Volume = Coordinates**3
 Density = Masses / Volume
 Density = u.Unit('arepo_density small_h2 / small_a3')
 
+# NOTE: Velocity gradients are written out in unit of
+# internal velocity, w, divided by internal coordinates
+VelocityGradient = InternalVelocities / Coordinates
+
+Pressure = u.Unit('arepo_pressure  small_h^2 small_a^-3')
+
 default = {
     'Coordinates': Coordinates,
     'Masses': Masses,
     'Velocities': Velocities
 }
 
 
@@ -54,22 +67,24 @@
     'MagneticField': MagneticField,
     'MagneticFieldDivergence': MagneticField / Coordinates,
     'MagneticFieldDivergenceAlternative': MagneticField / Coordinates,
     'Masses': Masses,
     'NeutralHydrogenAbundance': unit_less,
     'ParticleIDs': unit_less,
     'Potential': Potential,
-    'Pressure': 'arepo_pressure  small_h^2 small_a^-3',
+    'Pressure': Pressure,
     'StarFormationRate': StarFormationRate,
     'SubfindDMDensity': Density,
     'SubfindDensity': Density,
     'SubfindHsml': Coordinates,
     'SubfindVelDisp': 'arepo_velocity',
     'Velocities': Velocities,
-    'VelocityGradient': Velocities / Coordinates
+    'VelocityGradient': VelocityGradient,
+    'DensityGradient': Density / Coordinates,
+    'PressureGradient': Pressure / Coordinates
 }
 
 dark_matter = {
     'Coordinates': Coordinates,
     'Masses': Masses,
     'ParticleIDs': unit_less,
     'Potential': Potential,
```

### Comparing `paicos-0.1.8/paicos/units.py` & `paicos-0.1.9/paicos/units.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 u.add_enabled_equivalencies(equiv_B_no_small_h)
 
 
 def get_unit_dictionaries(unit):
     """
     Returns dictionaries with information about the units of the
     quantity.
+
+    :meta private:
     """
     codic = {}
     dic = {}
     for base, power in zip(unit.bases, unit.powers):
         if base in (small_a, small_h):
             codic[base] = power
         else:
@@ -67,38 +69,44 @@
 
     return codic, dic
 
 
 def construct_unit_from_dic(dic):
     """
     Construct unit from a dictionary with the format returned
-    from __get_unit_dictionaries
+    from get_unit_dictionaries
+
+    :meta private:
     """
     return np.prod([unit**dic[unit] for unit in dic])
 
 
 def separate_units(unit):
     """
-    Separate the standard physical units (u_unit) from the units involving
-    a and h (pu_unit). That is,
+    Separates the standard physical units (u_unit) from the units involving
+    a and h (pu_unit). That is::
 
-    u_unit, pu_unit = separate_units(unit)
+        u_unit, pu_unit = separate_units(unit)
 
     where pu_unit contains small_a and small_h and u_unit contains
-    everything else such that unit = u_unit * pu_unit
+    everything else such that::
+
+        unit = u_unit * pu_unit
     """
     codic, dic = get_unit_dictionaries(unit)
     u_unit = construct_unit_from_dic(dic)
     pu_unit = construct_unit_from_dic(codic)
     return u_unit, pu_unit
 
 
 def get_new_unit(unit, remove_list=[]):
     """
     Return new unit where base units in the remove list have been removed.
+
+    :meta private:
     """
     unit_list = []
     for base, power in zip(unit.bases, unit.powers):
         if base not in remove_list:
             unit_list.append(base**power)
 
     return np.prod(unit_list)
@@ -118,66 +126,72 @@
 
     value: the numeric values of your data (similar to astropy Quantity)
 
     a: the cosmological scale factor of your data
 
     h: the reduced Hubble parameter, e.g. h = 0.7
 
-    unit: a string, e.g. 'g/cm^3 small_a^-3 small_h^2' or astropy Unit
-    The latter can be defined like this:
+    unit: a string, e.g. ``g/cm^3 small_a^-3 small_h^2`` or an astropy Unit
+          The latter can be defined like this::
 
-    from paicos import units as pu
-    from astropy import units as u
-    unit = u.g*u.cm**(-3)*small_a**(-3)*small_h**(2)
+            from paicos import units as pu
+            from astropy import units as u
+            unit = u.g*u.cm**(-3)*small_a**(-3)*small_h**(2)
 
-    The naming of small_a and small_h is to avoid conflict with the already
-    existing 'annum' (i.e. a year) and 'h' (hour) units.
+          The naming of small_a and small_h is to avoid conflict with the already
+          existing 'annum' (i.e. a year) and 'h' (hour) units.
 
-    Returns
-    ----------
 
-    Methods/properties
-    ----------
+    Methods/key properties
+    ----------------------
 
-    no_small_h: returns a new comoving quantity where the h-factors have
-               been removed and the numeric value adjusted accordingly.
+        no_small_h
+                    Returns a new comoving quantity where the h-factors
+                    have been removed and the numeric value adjusted
+                    accordingly.
 
-    to_physical: returns a new  object where both a and h factors have been
-                 removed, i.e. we have switched from comoving values to
-                 the physical value.
+        to_physical
+                      Returns a new  object where both a and h factors have been
+                      removed, i.e. we have switched from comoving values to
+                      the physical value.
 
-    label: Return a Latex label for use in plots.
+        label
+                Returns a Latex label for use in plots.
 
     Examples
-    ----------
+    --------
+
+    Here is an example::
 
-    units = 'g cm^-3 small_a^-3 small_h^2'
-    A = PaicosQuantity(2, units, h=0.7, a=1/128)
+        units = 'g cm^-3 small_a^-3 small_h^2'
+        A = PaicosQuantity(2, units, h=0.7, a=1/128)
 
-    # Create a new comoving quantity where the h-factors have been removed
-    B = A.no_small_h
+        # Create a new comoving quantity where the h-factors have been removed
+        B = A.no_small_h
 
-    # Create a new quantity where both a and h factor have been removed,
-    # i.e. we have switched from a comoving quantity to the physical value
+        # Create a new quantity where both a and h factor have been removed,
+        # i.e. we have switched from a comoving quantity to the physical value
 
-    C = A.to_physical
+        C = A.to_physical
 
     """
 
     # pylint: disable=too-many-arguments
 
     def __new__(cls, value, unit=None, dtype=None, copy=False, order=None,
                 subok=False, ndmin=0, h=None, a=None, comoving_sim=None):
         """
         Here we initialize the Paicos Quantity. The three additional
         input arguments (compared to a standard astropy quantity) are
 
         h
         a
         comoving_sim
+
+        :meta private:
         """
 
         assert h is not None, 'Paicos quantity is missing a value for h'
         assert a is not None, 'Paicos quantity is missing a value for a'
         assert comoving_sim is not None, 'is this from a comoving_sim?'
 
         if hasattr(value, 'unit'):
@@ -191,15 +205,17 @@
         obj._a = a
         obj._comoving_sim = comoving_sim
 
         return obj
 
     def __array_finalize__(self, obj):
         """
-        Heavily inspired by the astropy Quantity version
+        Heavily inspired by the astropy Quantity version.
+
+        :meta private:
         """
         super_array_finalize = super().__array_finalize__
         if super_array_finalize is not None:
             super_array_finalize(obj)
 
         # If we're a new object or viewing an ndarray, nothing has to be done.
         if obj is None or obj.__class__ is np.ndarray:
@@ -290,15 +306,15 @@
         """
         return PaicosQuantity(1., self.unit, a=self._a, h=self.h,
                               comoving_sim=self.comoving_sim)
 
     @property
     def copy(self):
         """
-        Returns a copy of the PaicosQuantity
+        Returns a copy of the PaicosQuantity.
         """
         return PaicosQuantity(np.array(self.value), self.unit, a=self._a, h=self.h,
                               comoving_sim=self.comoving_sim, copy=True)
 
     @property
     def uq(self):
         """
@@ -306,14 +322,16 @@
         """
         return self.unit_quantity
 
     @property
     def hdf5_attrs(self):
         """
         Give the units as a dictionary for hdf5 data set attributes
+
+        :meta private:
         """
         return {'unit': self.unit.to_string()}
 
     @property
     def no_small_h(self):
         """
         Remove scaling with h, returning a quantity with adjusted values.
@@ -402,14 +420,16 @@
     def decompose(self, bases=[]):
         """
         Decompose into a different set of units, e.g.
 
         A = B.decompose(bases=[u.kpc, u.Msun, u.s, u.uG, u.keV])
 
         small_a and small_h are automatically included in the bases.
+
+        :meta private:
         """
         _, pu_unit = separate_units(self.unit)
         if len(bases) == 0 or pu_unit == u.Unit(''):
             return super().decompose(bases)
 
         if isinstance(bases, set):
             bases = list(bases)
@@ -418,15 +438,15 @@
         bases = set(bases)
         return super().decompose(bases)
 
     def label(self, variable=''):
         """
         Return a Latex string for use in plots. The optional
         input variable could be the Latex symbol for the physical variable,
-        for instance \rho or \nabla\times\vec{v}.
+        for instance \\rho or \\nabla\\times\\vec{v}.
         """
 
         a_sc, a_sc_str = self.__scaling_and_scaling_str(small_a)
         h_sc, h_sc_str = self.__scaling_and_scaling_str(small_h)
 
         co_label = a_sc_str + h_sc_str
 
@@ -518,22 +538,27 @@
         Convert quantity to any (possible) unit.
 
         The .to method only allows converting standard
         physical units while the .to_comoving only allows
         modifying the a and h factors. This method allows
         changing the units in one go.
         """
+        if isinstance(new_unit, str):
+            new_unit = u.Unit(new_unit)
+
         u_unit, pu_unit = separate_units(new_unit)
         new_quant = self.to(u_unit)
         new_quant = new_quant.to_comoving(pu_unit)
         return new_quant
 
     def __scaling_and_scaling_str(self, unit):
         """
         Helper function to create labels
+
+        :meta private:
         """
         codic, dic = get_unit_dictionaries(self.unit)
         # print(unit, dic, codic)
         if unit in codic:
             scaling = codic[unit]
         elif unit in dic:
             scaling = dic[unit]
@@ -594,39 +619,67 @@
         return super().__mul__(value)
 
     def __truediv__(self, value):
         self._sanity_check(value)
         return super().__truediv__(value)
 
     def dump(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def dumps(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def tobytes(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def tofile(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def tolist(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def tostring(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
     def choose(self):
-        """This astropy Quantity method has not been implemented the Paicos subclasses."""
+        """
+        This astropy Quantity method has not been implemented in the Paicos subclass.
+
+        :meta private:
+        """
         raise RuntimeError("not implemented")
 
 
 class PaicosTimeSeries(PaicosQuantity):
 
     """
     PaicosTimeSeries is a subclass of the PaicosQuantity and and shares many
@@ -748,27 +801,30 @@
 
         return self._new_view(new_value, new_unit)
 
     @property
     def hdf5_attrs(self):
         """
         Give the units as a dictionary for hdf5 data set attributes
+
+        :meta private:
         """
         return {'unit': self.unit.to_string(), 'Paicos': 'PaicosTimeSeries'}
 
     @property
     def copy(self):
         """
-        Returns a copy of the PaicosQuantity
+        Returns a copy of the PaicosTimeSeries.
         """
         return PaicosTimeSeries(self.value, self.unit, a=self._a, h=self.h,
                                 copy=True, comoving_sim=self.comoving_sim)
 
     def make_matrix(self, vec):
         """
+        :meta private:
         """
         assert vec.shape[0] == self.shape[0]
         return np.vstack([vec for _ in range(self.shape[1])]).T
 
     def _sanity_check(self, value):
         """
         Function for sanity-checking addition, subtraction, multiplication
@@ -791,14 +847,16 @@
                 info = f'\nObj1.h={self.h}.\n\nObj2.h={value.h}'
                 raise RuntimeError(err_msg + info)
 
 
 def paicos_quantity_list_to_array(list_to_convert):
     """
     Only works on 1D lists...
+
+    :meta private:
     """
     e0 = list_to_convert[0]
     if hasattr(e0, 'unit'):
         for e in list_to_convert:
             assert e0.unit == e.unit
             assert e0.comoving_sim == e.comoving_sim
             assert e0._a == e._a
```

### Comparing `paicos-0.1.8/paicos/util.py` & `paicos-0.1.9/paicos/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import h5py
 from functools import wraps
 from . import settings
 from . import units as pu
 from .cython.get_index_of_region import get_cube, get_radial_range
 from .cython.get_index_of_region import get_cube_plus_thin_layer
+from .cython.get_index_of_region import get_radial_range_plus_thin_layer
 from .cython.get_index_of_region import get_rotated_cube
 from .cython.get_index_of_region import get_rotated_cube_plus_thin_layer
 from .cython.openmp_info import simple_reduction, get_openmp_settings
 
 # These will be set by the user using the add_user_unit function
 user_unit_dict = {'default': {},
                   'voronoi_cells': {},
@@ -227,61 +228,96 @@
     x_c, y_c, z_c = center[0], center[1], center[2]
     index = get_radial_range(pos, x_c, y_c, z_c, r_min, r_max,
                              settings.numthreads)
     return index
 
 
 @remove_astro_units
+def get_index_of_radial_range_plus_thin_layer(pos, center, r_min, r_max, thickness):
+    """
+    Get a boolean array for the positions, pos, which are inside the spherical
+    shell with inner radius r_min and outer radius r_max, centered at center.
+    The thickness array argument adds a variable thickness, e.g., the cell
+    diameters, so that point close to the selection are also included.
+    """
+    assert center.shape[0] == 3
+    x_c, y_c, z_c = center[0], center[1], center[2]
+    index = get_radial_range_plus_thin_layer(pos, x_c, y_c, z_c, r_min, r_max,
+                                             thickness, settings.numthreads)
+    return index
+
+
+@remove_astro_units
 def get_index_of_cubic_region(pos, center, widths, box):
     """
     Get a boolean array to the position array, pos, which are inside a cubic
     region.
 
-    pos (array): position array with dimensions = (n, 3)
-    center (array with length 3): the center of the box (x, y, z)
-    widths (array with length 3): the widths of the box
-    box: the box size of the simulation (e.g. snap.box)
+    Parameters
+    ----------
+    pos : array
+         position array with dimensions = (n, 3)
+    center : array with length 3
+             The center of the box (x, y, z).
+    widths : array with length 3
+             The widths of the box.
+    box : float
+                 The box size of the simulation (e.g. snap.box).
     """
     x_c, y_c, z_c = center[0], center[1], center[2]
     width_x, width_y, width_z = widths
     index = get_cube(pos, x_c, y_c, z_c, width_x, width_y, width_z, box,
                      settings.numthreads)
     return index
 
 
 @remove_astro_units
 def get_index_of_cubic_region_plus_thin_layer(pos, center, widths, thickness, box):
     """
     Get a boolean array to the position array, pos, which are inside a cubic
     region plus a thin layer with a cell-dependent thickness
 
-    pos (array): position array with dimensions = (n, 3)
-    center (array with length 3): the center of the box (x, y, z)
-    widths (array with length 3): the widths of the box
-    thickness: (array): array with same length as the position array
-    box: the box size of the simulation (e.g. snap.box)
+    Parameters
+    ----------
+    pos : array
+         position array with dimensions = (n, 3)
+    center : array with length 3
+             The center of the box (x, y, z).
+    widths : array with length 3
+             The widths of the box.
+    thickness : array
+                Array with same length as the position array.
+    box : float
+         The box size of the simulation (e.g. snap.box).
     """
     x_c, y_c, z_c = center[0], center[1], center[2]
     width_x, width_y, width_z = widths
     index = get_cube_plus_thin_layer(pos, x_c, y_c, z_c, width_x, width_y,
                                      width_z, thickness, box, settings.numthreads)
     return index
 
 
 @remove_astro_units
 def get_index_of_rotated_cubic_region(pos, center, widths, box, orientation):
     """
     Get a boolean array to the position array, pos, which are inside a cubic
     region
 
-    pos (array): position array with dimensions = (n, 3)
-    center (array with length 3): the center of the box (x, y, z)
-    widths (array with length 3): the widths of the box
-    thickness: (array): array with same length as the position array
-    box: the box size of the simulation (e.g. snap.box)
+    Parameters
+    ----------
+    pos : array
+         position array with dimensions = (n, 3)
+    center : array with length 3
+             The center of the box (x, y, z).
+    widths : array with length 3
+             The widths of the box.
+    thickness : array
+                Array with same length as the position array.
+    box : float
+         The box size of the simulation (e.g. snap.box).
     """
     x_c, y_c, z_c = center[0], center[1], center[2]
     width_x, width_y, width_z = widths
     unit_vectors = orientation.cartesian_unit_vectors
     index = get_rotated_cube(pos, x_c, y_c, z_c, width_x, width_y,
                              width_z, box,
                              unit_vectors['x'],
@@ -294,36 +330,42 @@
 @remove_astro_units
 def get_index_of_rotated_cubic_region_plus_thin_layer(pos, center, widths, thickness,
                                                       box, orientation):
     """
     Get a boolean array to the position array, pos, which are inside a cubic
     region plus a thin layer with a cell-dependent thickness
 
-    pos (array): position array with dimensions = (n, 3)
-    center (array with length 3): the center of the box (x, y, z)
-    widths (array with length 3): the widths of the box
-    thickness: (array): array with same length as the position array
-    box: the box size of the simulation (e.g. snap.box)
+    Parameters
+    ----------
+    pos : array
+         position array with dimensions = (n, 3)
+    center : array with length 3
+             The center of the box (x, y, z).
+    widths : array with length 3
+             The widths of the box.
+    thickness : array
+                Array with same length as the position array.
+    box : float
+         The box size of the simulation (e.g. snap.box).
     """
     x_c, y_c, z_c = center[0], center[1], center[2]
     width_x, width_y, width_z = widths
     unit_vectors = orientation.cartesian_unit_vectors
     index = get_rotated_cube_plus_thin_layer(pos, x_c, y_c, z_c, width_x, width_y,
                                              width_z, thickness, box,
                                              unit_vectors['x'],
                                              unit_vectors['y'],
                                              unit_vectors['z'],
                                              settings.numthreads)
     return index
 
 
-def check_if_omp_has_issues(verbose=True):
+def _check_if_omp_has_issues(verbose=True):
     """
     Check if the parallelization via OpenMP works.
-
     Parameters
     ----------
     numthreads : int
         Number of threads used in parallelization
     """
 
     if settings.give_openMP_warnings is False:
@@ -355,19 +397,21 @@
                + "compiler problem, discussed here:\n"
                + "https://stackoverflow.com/questions/54776301/"
                + "cython-prange-is-repeating-not-parallelizing.\n\n")
         if verbose:
             warnings.warn(msg)
 
 
-def copy_over_snapshot_information(org_filename, new_filename, mode='r+'):
+def _copy_over_snapshot_information(snap, new_filename, mode='r+'):
     """
     Copy over attributes from the original arepo snapshot.
     In this way we will have access to units used, redshift etc
     """
-    g = h5py.File(org_filename, 'r')
+    info_dic = {}
+    info_dic['Header'] = dict(snap.Header)
+    info_dic['Parameters'] = dict(snap.Parameters)
+    info_dic['Config'] = dict(snap.Config)
     with h5py.File(new_filename, mode) as f:
         for group in ['Header', 'Parameters', 'Config']:
             f.create_group(group)
-            for key in g[group].attrs.keys():
-                f[group].attrs[key] = g[group].attrs[key]
-    g.close()
+            for key in info_dic[group]:
+                f[group].attrs[key] = info_dic[group][key]
```

### Comparing `paicos-0.1.8/paicos/writers/arepo_image.py` & `paicos-0.1.9/paicos/writers/arepo_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,24 +37,37 @@
 
         The `mode` argument controls whether the file is opened in write mode
         ('w') or amend mode ('a'). If `mode` is 'w', the file will be created
         at `self.tmp_filename` and the image information will be written to
         the file. Setting the mode to amend mode, 'a', allows to add new images
         to an already existing file.
 
-        Parameters: image_creator (object): A Paicos Projector or Slicer
-        object used to create the image.
+        Parameters
+        ----------
 
-        basedir (file path): The folder where the image file should be saved.
+            image_creator : object
+                A Paicos Projector or Slicer object used to create the image.
 
-        basename (string): The base name for the image file, which will be in
-        the format `basename_{:03d}`. (default: "projection")
+            basedir (file: path
+                The folder where the image file should be saved.
 
-        mode (string): The mode to open the file in, either 'w' for write mode
-        or 'r' for read mode. (default: 'w')
+            basename : string
+                The base name for the image file, which will be in
+                the format ``basename_{:03d}``. (default: "projection").
+
+            mode : string
+                The mode to open the file in, either 'w' for write mode
+                or 'a' for append mode. (default: 'w').
+
+        Methods
+        -------
+
+            finalize :
+                Changes the filename from a temporary one to the final one,
+                e.g., from self.tmp_filename to self.filename.
         """
 
         self.center = image_creator.center
         self.widths = image_creator.widths
         self.extent = image_creator.extent
         self.direction = image_creator.direction
         self.orientation = image_creator.orientation
@@ -74,19 +87,19 @@
 
                 if self.direction == 'orientation':
                     file['image_info'].attrs['normal_vector'] = self.orientation.normal_vector
                     file['image_info'].attrs['perp_vector1'] = self.orientation.perp_vector1
 
     def save_image(self, name, data):
         """
-        This function saves a 2D image to the hdf5 file.
+        This method saves a 2D image to the hdf5 file.
         """
         self.write_data(name, data)
 
-    def perform_extra_consistency_checks(self):
+    def _perform_extra_consistency_checks(self):
         """
         Perform extra consistency checks on the HDF5 file to ensure the
         current values match the values stored in the HDF5 file that we intend
         to amend.
 
         The function opens the HDF5 file, loads the 'center' and 'widths'
         datasets from the 'image_info' group, and compares them to the
```

### Comparing `paicos-0.1.8/paicos/writers/paicos_writer.py` & `paicos-0.1.9/paicos/writers/paicos_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,46 @@
 import os
 import h5py
 from .. import util
 
 
 class PaicosWriter:
     """
-    This class writes data to self-documenting hdf5 files.
+    This class can be used for writing data to self-documenting hdf5 files.
 
     It is the base class for the ArepoImage writer.
     """
 
     def __init__(self, reader_object, basedir,
                  basename="paicos_file", add_snapnum=True, mode='w'):
         """
         The constructor for the `PaicosWriter` class.
 
         Parameters
         ----------
 
-        reader_object (obj): A PaicosReader object (or Snaphot or Catalog object).
+            reader_object :  obj
+                A PaicosReader object (or Snaphot or Catalog object).
 
-        basedir (file path): The folder where the HDF5 file will be saved.
+            basedir : file path
+                 The folder where the HDF5 file will be saved.
 
-        basename (str, optional): Base name of the HDF5 file. Defaults
-                                  to "paicos_file".
+            basename : str, optional
+                 Base name of the HDF5 file. Defaults to "paicos_file".
 
-        add_snapnum (bool): Whether to add the snapnum to the HDF5 filename.
-                            When True, the filename will be "basename_{:03d}.hdf5",
-                            when False it will simply be "basename.hdf5"
-                            Defaults to True.
+            add_snapnum :  bool
+                Whether to add the snapnum to the HDF5 filename.
 
-        mode (string): The mode to open the file in, either 'w' for write mode
-        or 'r' for read mode. (default: 'w')
+                When True, the filename will be "basename_{:03d}.hdf5",
+                when False it will simply be "basename.hdf5"
+                Defaults to True.
+
+            mode :  string
+                The mode to open the file in, either 'w' for write mode
+                or 'a' for append mode. (default: 'w').
 
         """
 
         self.reader_object = reader_object
         self.org_filename = reader_object.filename
 
         self.mode = mode
@@ -60,21 +65,21 @@
             name += f'_{snapnum:03d}.hdf5'
         else:
             name += '.hdf5'
         self.filename = basedir + name
         self.tmp_filename = basedir + 'tmp_' + name
 
         if mode == 'w':
-            util.copy_over_snapshot_information(self.org_filename,
-                                                self.tmp_filename, 'w')
-            self.write_info_about_org_file()
+            util._copy_over_snapshot_information(self.reader_object,
+                                                 self.tmp_filename, 'w')
+            self._write_info_about_org_file()
         else:
-            self.perform_consistency_checks()
+            self._perform_consistency_checks()
 
-    def write_info_about_org_file(self):
+    def _write_info_about_org_file(self):
         """
         This function saves some attributes in org_info.
         """
         with h5py.File(self.tmp_filename, 'r+') as file:
             file.create_group('org_info')
             if hasattr(self.reader_object, 'snapnum'):
                 file['org_info'].attrs['snapnum'] = self.reader_object.snapnum
@@ -84,33 +89,34 @@
             file['org_info'].attrs['basename'] = self.reader_object.basename
             file['org_info'].attrs['filename'] = self.reader_object.filename
 
     def write_data(self, name, data, data_attrs={}, group=None, group_attrs={}):
         """
         Write a data set to the hdf5 file.
 
-        Parameters
-        ----------
+        Parameters:
+
+            name (str): Name of the data to be written.
+
+            data (obj): The data to be written (e.g. PaicosQuantity, PaicosTimeSeries,
+                        Astropy Quantity, numpy array).
+
+            data_attrs (dict):
+                Dictionary of attributes for the data. E.g.::
 
-        name (str): Name of the data to be written.
+                    {'info': 'Here I have written some extra information about the data set'}
 
-        data (obj): The data to be written (e.g. PaicosQuantity, PaicosTimeSeries,
-                    Astropy Quantity, numpy array).
+                Defaults to an empty dictionary.
 
-        data_attrs (dict): Dictionary of attributes for the data. E.g.
-                           {'info': 'Here I have written some extra information
-                                    about the data set'}. Defaults to an empty
-                                    dictionary.
-
-        group (str, optional): Group in the HDF5 file where the data should
-                               be saved. Defaults to None in which case the
-                               data set is saved at the top level of the hdf5 file).
+            group (str, optional): Group in the HDF5 file where the data should
+                                   be saved. Defaults to None in which case the
+                                   data set is saved at the top level of the hdf5 file).
 
-        group_attrs (dict, optional): Dictionary of attributes for the group.
-                                      Defaults to an empty dictionary.
+            group_attrs (dict, optional): Dictionary of attributes for the group.
+                                          Defaults to an empty dictionary.
         """
 
         # pylint: disable= dangerous-default-value
 
         if self.mode == 'w':
             filename = self.tmp_filename
         else:
@@ -131,36 +137,36 @@
                     if name in file[group]:
                         raise RuntimeError(msg)
 
         # Save the data
         util.save_dataset(file, name, data=data, data_attrs=data_attrs,
                           group=group, group_attrs=group_attrs)
 
-    def perform_extra_consistency_checks(self):
+    def _perform_extra_consistency_checks(self):
         """
         Perform extra consistency checks. This can be overloaded by
         subclasses.
         """
         # pylint: disable=unnecessary-pass
         pass
 
-    def perform_consistency_checks(self):
+    def _perform_consistency_checks(self):
         """
         Perform consistency checks when trying to amend a file (to avoid
         saving data at different times, for instance)
         """
         with h5py.File(self.filename, 'r') as f:
             org_time = self.reader_object.Header['Time']
             assert f['Header'].attrs['Time'] == org_time
 
-        self.perform_extra_consistency_checks()
+        self._perform_extra_consistency_checks()
 
     def finalize(self):
         """
-        Move from a temporary to the final filename.
+        Move from a temporary filename to the final filename.
         """
         if self.mode == 'w':
             os.rename(self.tmp_filename, self.filename)
 
 
 class PaicosTimeSeriesWriter(PaicosWriter):
     """
```

### Comparing `paicos-0.1.8/paicos.egg-info/SOURCES.txt` & `paicos-0.1.9/paicos.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 paicos/__init__.py
 paicos/orientation.py
-paicos/paicos_user_settings.py
 paicos/paicos_user_settings_template.py
 paicos/settings.py
 paicos/unit_specifications.py
 paicos/units.py
 paicos/util.py
 paicos.egg-info/PKG-INFO
 paicos.egg-info/SOURCES.txt
@@ -35,14 +34,15 @@
 paicos/image_creators/nested_projector.py
 paicos/image_creators/projector.py
 paicos/image_creators/slicer.py
 paicos/image_creators/tree_projector.py
 paicos/readers/__init__.py
 paicos/readers/arepo_catalog.py
 paicos/readers/arepo_snap.py
+paicos/readers/generic_snap.py
 paicos/readers/paicos_readers.py
 paicos/trees/__init__.py
 paicos/trees/bvh_cpu.py
 paicos/trees/bvh_gpu.py
 paicos/trees/bvh_tree.pyx
 paicos/writers/__init__.py
 paicos/writers/arepo_image.py
```

### Comparing `paicos-0.1.8/setup.py` & `paicos-0.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,32 +71,37 @@
 
 ]
 
 install_requires = ['scipy',
                     'numpy',
                     'h5py',
                     'astropy',
-                    'numba']
+                    'numba',
+                    'matplotlib']
 
 
 cur = os.path.abspath(__file__).replace('setup.py', '')
 with open(cur + 'README.md') as f:
     long_description = f.read()
 
+with open(cur + 'dev_requirements.txt') as f:
+    dev_requirements = f.read().strip().split('\n')
+
 setup(
     name='paicos',
-    version='0.1.8',
+    version='0.1.9',
     description=('An object-oriented Python package for analysis of '
                  + '(cosmological) simulations performed with Arepo.'),
     url='https://github.com/tberlok/paicos',
     author='Thomas Berlok',
     author_email='tberlok@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='BSD 3-clause',
     packages=setuptools.find_packages(),
     install_requires=install_requires,
+    extras_require={'dev': dev_requirements},
     package_data={'paicos/cython': ['*.c', '*.so']},
     classifiers=['Programming Language :: Python :: 3'],
     ext_modules=cythonize(ext_modules,
                           compiler_directives=compiler_directives),
     cmdclass={'build_ext': Cython.Build.build_ext})
```

