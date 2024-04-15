# Comparing `tmp/figaro-1.6.0.tar.gz` & `tmp/figaro-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.0.tar", last modified: Sun Apr 14 08:24:11 2024, max compression
+gzip compressed data, was "figaro-1.6.1.tar", last modified: Mon Apr 15 09:15:34 2024, max compression
```

## Comparing `figaro-1.6.0.tar` & `figaro-1.6.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.959134 figaro-1.6.0/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.0/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.0/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-14 08:24:11.958908 figaro-1.6.0/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.0/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.944293 figaro-1.6.0/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.949364 figaro-1.6.0/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.951787 figaro-1.6.0/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.956945 figaro-1.6.0/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.0/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-09 08:31:38.000000 figaro-1.6.0/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.0/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.958449 figaro-1.6.0/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    13557 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    18761 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10486 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9321 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2341 2024-04-10 10:07:12.000000 figaro-1.6.0/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.0/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    33823 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6282 2024-02-24 19:48:07.000000 figaro-1.6.0/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    54015 2024-04-12 07:55:46.000000 figaro-1.6.0/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40056 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.0/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.0/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16060 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.958648 figaro-1.6.0/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1746 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-14 08:23:36.000000 figaro-1.6.0/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-14 08:24:11.959184 figaro-1.6.0/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464909 figaro-1.6.1/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.1/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.1/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-15 09:15:34.464695 figaro-1.6.1/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.1/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.451147 figaro-1.6.1/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.456055 figaro-1.6.1/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.458485 figaro-1.6.1/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.462635 figaro-1.6.1/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.1/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-09 08:31:38.000000 figaro-1.6.1/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.1/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464209 figaro-1.6.1/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    13588 2024-04-15 07:19:49.000000 figaro-1.6.1/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    18793 2024-04-15 07:19:52.000000 figaro-1.6.1/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10486 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9321 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2341 2024-04-10 10:07:12.000000 figaro-1.6.1/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.1/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    33823 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6282 2024-02-24 19:48:07.000000 figaro-1.6.1/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    54015 2024-04-15 09:14:03.000000 figaro-1.6.1/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40056 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.1/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.1/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16147 2024-04-14 14:47:57.000000 figaro-1.6.1/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464424 figaro-1.6.1/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1746 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-15 09:15:16.000000 figaro-1.6.1/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-15 09:15:34.464954 figaro-1.6.1/setup.cfg
```

### Comparing `figaro-1.6.0/LICENSE` & `figaro-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/PKG-INFO` & `figaro-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.0
+Version: 1.6.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.0/README.md` & `figaro-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/docs/source/index.rst` & `figaro-1.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/_likelihood.py` & `figaro-1.6.1/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/_numba_functions.py` & `figaro-1.6.1/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.1/figaro/_pipelines/hierarchical_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,17 @@
     if options.inj_density_file is not None:
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
     # If provided, load selecton function
-    selfunc = None
-    inj_pdf = None
+    selfunc     = None
+    inj_pdf     = None
+    n_total_inj = None
     if options.selfunc_file is not None:
         selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
         if not callable(selfunc) and not options.probit:
             # Keeping only the samples within bounds
             selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
             inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
     # If provided, load true values
```

### Comparing `figaro-1.6.0/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.1/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,17 +204,18 @@
     inj_density = None
     if options.inj_density_file is not None:
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
-    #If provided, load selecton function
-    selfunc = None
-    inj_pdf = None
+    # If provided, load selecton function
+    selfunc     = None
+    inj_pdf     = None
+    n_total_inj = None
     if options.selfunc_file is not None:
         selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
         if not callable(selfunc):
             # Keeping only the samples within bounds
             selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
             inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
     # If provided, load true values
```

### Comparing `figaro-1.6.0/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.1/figaro/_pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/_pipelines/probability_density.py` & `figaro-1.6.1/figaro/_pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/cosmology.py` & `figaro-1.6.1/figaro/cosmology.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/credible_regions.py` & `figaro-1.6.1/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/cumulative.py` & `figaro-1.6.1/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/decorators.py` & `figaro-1.6.1/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/diagnostic.py` & `figaro-1.6.1/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/exceptions.py` & `figaro-1.6.1/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/load.py` & `figaro-1.6.1/figaro/load.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/marginal.py` & `figaro-1.6.1/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/mixture.py` & `figaro-1.6.1/figaro/mixture.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/montecarlo.py` & `figaro-1.6.1/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/plot.py` & `figaro-1.6.1/figaro/plot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/plot_settings.py` & `figaro-1.6.1/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/transform.py` & `figaro-1.6.1/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/figaro/utils.py` & `figaro-1.6.1/figaro/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,36 +237,38 @@
     idx = np.random.choice(np.arange(len(draws)), size = int(size))
     ctr = Counter(idx)
     samples = np.empty(shape = (1, draws[0].dim))
     for i, n in zip(ctr.keys(), ctr.values()):
         samples = np.concatenate((samples, draws[i].rvs(n)))
     return samples[1:]
     
-def make_gaussian_mixture(mu, cov, bounds, out_folder = '.', names = None, save = False, save_samples = False, n_samps = 3000, probit = True):
+def make_gaussian_mixture(mu, cov, bounds, out_folder = '.', names = None, save = False, save_samples = False, n_samps = 3000, probit = True, ext = 'json'):
     """
     Builds mixtures composed of equally-weighted Gaussian distribution.
     WARNING: due to the probit coordinate change, a Gaussian distribution in the natural space does not correspond to a Gaussian distribution in the probit space.
     The resulting distributions in probit space, therefore, are just an approximation. This approximation holds for distributions which are far from boundaries.
     In general, a more robust (but slower) approach would be to draw samples from each original Gaussian distribution and to use them to make a hierarchical inference.
     
     Arguments:
         np.ndarray mu:     mean for each Gaussian distribution
         np.ndarray cov:    covariance matrix for each Gaussian distribution
         np.ndarray bounds: boundaries for probit transformation
         str out_folder:    output folder
         bool save:         whether to save the draws or not
         bool save_samples: whether to save the samples or not
         int n_samps:       number of samples to estimate mean and covariance in probit space
-        bool probit        whether to use the probit transformation or not
+        bool probit:       whether to use the probit transformation or not
+        str ext:           file extension (pkl or json)
     
     Returns:
         np.ndarray: mixtures
     """
     # Here to avoid circular import
     from figaro.mixture import mixture
+    from figaro.load import save_density
     bounds = np.atleast_2d(bounds)
     dim    = len(bounds)
     
     out_folder = Path(out_folder)
     if not out_folder.exists():
         out_folder.mkdir()
     
@@ -314,22 +316,22 @@
             if names is not None:
                 name = names[i]
             else:
                 name = 'event_{0}'.format(i+1)
             np.savetxt(Path(events_folder, name+'.txt'), samples[1:])
         mix = mixture(np.atleast_2d(mm), np.atleast_3d(cc), np.ones(len(means))/len(means), bounds, len(bounds), len(means), 0, probit = probit, alpha = 1.)
         if save:
-            with open(Path(draws_folder, name+'.pkl'), 'wb') as f:
-                dill.dump(np.array([mix]), f)
+            save_density([mix], draws_folder, name, ext)
         mixtures.append([mix])
     mixtures = np.array(mixtures)
     
     if save:
-        with open(Path(draws_folder, 'posteriors_single_event.pkl'), 'wb') as f:
-            dill.dump(mixtures, f)
+        # Circular import
+        from figaro.load import save_density
+        save_density(mixtures, draws_folder, 'posteriors_single_event', ext)
     
     return mixtures
 
 #-------------#
 #   Options   #
 #-------------#
```

### Comparing `figaro-1.6.0/figaro.egg-info/PKG-INFO` & `figaro-1.6.1/figaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.0
+Version: 1.6.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.0/figaro.egg-info/SOURCES.txt` & `figaro-1.6.1/figaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figaro-1.6.0/pyproject.toml` & `figaro-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.0'
+version = '1.6.1'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

