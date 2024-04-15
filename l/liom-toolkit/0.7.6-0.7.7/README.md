# Comparing `tmp/liom_toolkit-0.7.6.tar.gz` & `tmp/liom_toolkit-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liom_toolkit-0.7.6.tar", last modified: Mon Apr 15 19:07:23 2024, max compression
+gzip compressed data, was "liom_toolkit-0.7.7.tar", last modified: Mon Apr 15 19:14:47 2024, max compression
```

## Comparing `liom_toolkit-0.7.6.tar` & `liom_toolkit-0.7.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.139719 liom_toolkit-0.7.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.143719 liom_toolkit-0.7.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.143719 liom_toolkit-0.7.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.143719 liom_toolkit-0.7.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.147719 liom_toolkit-0.7.6/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.registration.register.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.registration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.registration.templating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.registration.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.cldice.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.loss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.make_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.predict_one.rst
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.training.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.utils.conversion.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.utils.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.utils.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.visualization.slice_extraction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.visualization.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/docs/source/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.147719 liom_toolkit-0.7.6/liom_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.151719 liom_toolkit-0.7.6/liom_toolkit/registration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/registration/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/registration/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/registration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.151719 liom_toolkit-0.7.6/liom_toolkit/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/plane_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/volume_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.151719 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/cldice.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/make_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4105 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4210 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/predict_one.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/training.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12942 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/liom_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/liom_toolkit/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/liom_toolkit/visualization/slice_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/liom_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-15 19:07:23.000000 liom_toolkit-0.7.6/liom_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-15 19:07:23.000000 liom_toolkit-0.7.6/liom_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:07:23.000000 liom_toolkit-0.7.6/liom_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:07:23.000000 liom_toolkit-0.7.6/liom_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:07:23.000000 liom_toolkit-0.7.6/liom_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:07:23.155719 liom_toolkit-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-15 19:07:19.000000 liom_toolkit-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.463130 liom_toolkit-0.7.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.463130 liom_toolkit-0.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.463130 liom_toolkit-0.7.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.467130 liom_toolkit-0.7.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.471130 liom_toolkit-0.7.7/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.registration.register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.registration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.registration.templating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.registration.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.cldice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.make_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.predict_one.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.training.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.utils.conversion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.utils.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.utils.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.visualization.slice_extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.visualization.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/docs/source/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.471130 liom_toolkit-0.7.7/liom_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.471130 liom_toolkit-0.7.7/liom_toolkit/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/registration/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/registration/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/registration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/liom_toolkit/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/plane_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/volume_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/cldice.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/make_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4105 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4210 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/predict_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12942 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/liom_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/liom_toolkit/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/liom_toolkit/visualization/slice_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/liom_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-15 19:14:47.000000 liom_toolkit-0.7.7/liom_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-15 19:14:47.000000 liom_toolkit-0.7.7/liom_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:14:47.000000 liom_toolkit-0.7.7/liom_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:14:47.000000 liom_toolkit-0.7.7/liom_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:14:47.000000 liom_toolkit-0.7.7/liom_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:14:47.475130 liom_toolkit-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-15 19:14:43.000000 liom_toolkit-0.7.7/setup.py
```

### Comparing `liom_toolkit-0.7.6/.github/workflows/main.yml` & `liom_toolkit-0.7.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/.gitignore` & `liom_toolkit-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/LICENSE` & `liom_toolkit-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/PKG-INFO` & `liom_toolkit-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.6
+Version: 0.7.7
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom_toolkit-0.7.6/README.md` & `liom_toolkit-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/docs/Makefile` & `liom_toolkit-0.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/docs/make.bat` & `liom_toolkit-0.7.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/docs/source/conf.py` & `liom_toolkit-0.7.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/docs/source/index.rst` & `liom_toolkit-0.7.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/docs/source/reference/liom_toolkit.segmentation.vseg.rst` & `liom_toolkit-0.7.7/docs/source/reference/liom_toolkit.segmentation.vseg.rst`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/registration/register.py` & `liom_toolkit-0.7.7/liom_toolkit/registration/register.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/registration/templating.py` & `liom_toolkit-0.7.7/liom_toolkit/registration/templating.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/registration/utils.py` & `liom_toolkit-0.7.7/liom_toolkit/registration/utils.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/plane_segmentation.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/plane_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/stats.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/stats.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/volume_segmentation.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/volume_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/cldice.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/cldice.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/data.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/data.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/loss.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/loss.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/make_dataset.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/make_dataset.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/model.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/model.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/predict_one.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/predict_one.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/training.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/training.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/utils.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/utils.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/segmentation/vseg/validation.py` & `liom_toolkit-0.7.7/liom_toolkit/segmentation/vseg/validation.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/utils/conversion.py` & `liom_toolkit-0.7.7/liom_toolkit/utils/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pywt
 import zarr
 from ome_zarr.io import parse_url
 from ome_zarr.writer import write_image
 from tqdm.auto import tqdm
 
 from liom_toolkit.registration import align_annotations_to_volume
-from liom_toolkit.utils import load_zarr, load_zarr_image_from_node, save_atlas_to_zarr, \
+from .io import load_zarr, load_zarr_image_from_node, save_atlas_to_zarr, \
     CustomScaler, create_transformation_dict, generate_axes_dict, create_mask_from_zarr, save_label_to_zarr, \
     generate_label_color_dict_mask, load_node_by_name
 
 
 def remove_stripe_based_wavelet_fft(image: np.ndarray, level: int = 5, sigma: int = 1, order: int = 8,
                                     pad: int = 150) -> np.ndarray:
     """
```

### Comparing `liom_toolkit-0.7.6/liom_toolkit/utils/io.py` & `liom_toolkit-0.7.7/liom_toolkit/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ome_zarr.writer import write_labels
 from skimage.io import imsave
 from skimage.transform import resize
 from tqdm import tqdm
 
 from liom_toolkit.registration import download_allen_atlas
 from liom_toolkit.segmentation import segment_3d_brain
-from utils import convert_to_png_for_saving
+from .utils import convert_to_png_for_saving
 
 
 def load_zarr(zarr_file: str) -> list[Node]:
     """
     Load a zarr file to an ANTs image.
 
     :param zarr_file: The zarr file to load.
```

### Comparing `liom_toolkit-0.7.6/liom_toolkit/utils/utils.py` & `liom_toolkit-0.7.7/liom_toolkit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit/visualization/slice_extraction.py` & `liom_toolkit-0.7.7/liom_toolkit/visualization/slice_extraction.py`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/liom_toolkit.egg-info/PKG-INFO` & `liom_toolkit-0.7.7/liom_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.6
+Version: 0.7.7
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom_toolkit-0.7.6/liom_toolkit.egg-info/SOURCES.txt` & `liom_toolkit-0.7.7/liom_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liom_toolkit-0.7.6/setup.py` & `liom_toolkit-0.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="liom-toolkit",
-    version="0.7.6",
+    version="0.7.7",
     author="Laboratoire d’Imagerie Optique et Moléculaire",
     author_email="frederic.lesage@polymtl.ca",
     packages=find_packages(),
     description="Package to support the research of LIOM.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/LIOMLab/liom-toolkit",
```

