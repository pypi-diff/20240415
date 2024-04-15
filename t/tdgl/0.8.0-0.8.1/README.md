# Comparing `tmp/tdgl-0.8.0.tar.gz` & `tmp/tdgl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdgl-0.8.0.tar", last modified: Mon Oct 30 16:36:14 2023, max compression
+gzip compressed data, was "tdgl-0.8.1.tar", last modified: Mon Apr 15 17:44:03 2024, max compression
```

## Comparing `tdgl-0.8.0.tar` & `tdgl-0.8.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.316691 tdgl-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-30 16:35:55.000000 tdgl-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2023-10-30 16:36:14.316691 tdgl-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-30 16:35:55.000000 tdgl-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 16:36:14.316691 tdgl-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2023-10-30 16:35:55.000000 tdgl-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.304691 tdgl-0.8.0/tdgl/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.304691 tdgl-0.8.0/tdgl/device/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34273 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/device/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/device/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/device/meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21261 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/device/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18393 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/em.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.308691 tdgl-0.8.0/tdgl/finite_volume/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/finite_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/finite_volume/edge_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    16538 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/finite_volume/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/finite_volume/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13398 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/finite_volume/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.308691 tdgl-0.8.0/tdgl/solution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solution/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    26901 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solution/plot_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)    43506 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solution/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.308691 tdgl-0.8.0/tdgl/solver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16689 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/screening.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/solver/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.308691 tdgl-0.8.0/tdgl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/sources/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/sources/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.312691 tdgl-0.8.0/tdgl/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (127)    12581 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_em.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/test/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.312691 tdgl-0.8.0/tdgl/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualization/snapshot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2023-10-30 16:35:55.000000 tdgl-0.8.0/tdgl/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:36:14.304691 tdgl-0.8.0/tdgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2023-10-30 16:36:14.000000 tdgl-0.8.0/tdgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-10-30 16:36:14.000000 tdgl-0.8.0/tdgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 16:36:14.000000 tdgl-0.8.0/tdgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-30 16:36:14.000000 tdgl-0.8.0/tdgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-30 16:36:14.000000 tdgl-0.8.0/tdgl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.034427 tdgl-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 17:43:53.000000 tdgl-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-15 17:44:03.034427 tdgl-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-15 17:43:53.000000 tdgl-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:44:03.034427 tdgl-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 17:43:53.000000 tdgl-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.022427 tdgl-0.8.1/tdgl/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.026427 tdgl-0.8.1/tdgl/device/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34269 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/device/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18393 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/em.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.026427 tdgl-0.8.1/tdgl/finite_volume/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/finite_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/finite_volume/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/finite_volume/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/finite_volume/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/finite_volume/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.026427 tdgl-0.8.1/tdgl/solution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solution/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26901 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solution/plot_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43492 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solution/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.026427 tdgl-0.8.1/tdgl/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16699 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/screening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34239 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/solver/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.030427 tdgl-0.8.1/tdgl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/sources/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/sources/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.030427 tdgl-0.8.1/tdgl/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/test/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.030427 tdgl-0.8.1/tdgl/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualization/snapshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2024-04-15 17:43:53.000000 tdgl-0.8.1/tdgl/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:44:03.030427 tdgl-0.8.1/tdgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-15 17:44:03.000000 tdgl-0.8.1/tdgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-15 17:44:03.000000 tdgl-0.8.1/tdgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:44:03.000000 tdgl-0.8.1/tdgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-15 17:44:03.000000 tdgl-0.8.1/tdgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 17:44:03.000000 tdgl-0.8.1/tdgl.egg-info/top_level.txt
```

### Comparing `tdgl-0.8.0/LICENSE` & `tdgl-0.8.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2023 Logan Bishop-Van Horn
+Copyright (c) 2022-2024 Logan Bishop-Van Horn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tdgl-0.8.0/PKG-INFO` & `tdgl-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.8.0
+Version: 0.8.1
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
```

### Comparing `tdgl-0.8.0/README.md` & `tdgl-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/setup.py` & `tdgl-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/__init__.py` & `tdgl-0.8.1/tdgl/__init__.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/about.py` & `tdgl-0.8.1/tdgl/about.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/device/device.py` & `tdgl-0.8.1/tdgl/device/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import numbers
 import os
 import time
 from contextlib import contextmanager, nullcontext
 from operator import attrgetter, itemgetter
 from typing import Any, Dict, List, NamedTuple, Optional, Sequence, Tuple, Union
 
 import h5py
@@ -84,15 +85,15 @@
             terminal.mesh = False
             if terminal.name is None or terminal.name in terminal_names:
                 raise ValueError("All terminals must have a unique name")
             terminal_names.add(terminal.name)
 
         for polygon in [self.film] + self.holes:
             if not polygon.is_valid:
-                raise ValueError("Invalid Polygon: {polygon!r}.")
+                raise ValueError(f"Invalid Polygon: {polygon!r}.")
 
         if len(self.holes) != len(set(hole.name for hole in self.holes)):
             raise ValueError("All holes must have a unique name.")
 
         if probe_points is not None:
             probe_points = np.asarray(probe_points).squeeze()
             if probe_points.ndim != 2 or probe_points.shape[1] != 2:
@@ -147,17 +148,15 @@
     def kappa(self) -> float:
         """The Ginzburg-Landau parameter, :math:`\\kappa=\\lambda/\\xi`."""
         return (self.london_lambda / self.coherence_length).to_base_units().magnitude
 
     @property
     def Bc2(self) -> pint.Quantity:
         """Upper critical field, :math:`B_{c2}=\\Phi_0/(2\\pi\\xi^2)`."""
-        return (
-            ureg("Phi_0") / (2 * np.pi * self.coherence_length**2)
-        ).to_base_units()
+        return (ureg("Phi_0") / (2 * np.pi * self.coherence_length**2)).to_base_units()
 
     @property
     def A0(self) -> pint.Quantity:
         """Scale for the magnetic vector potential, :math:`A_0=\\xi B_{c2}`."""
         return (self.Bc2 * self.coherence_length).to_base_units()
 
     @property
@@ -414,15 +413,15 @@
 
         Returns:
             The scaled ``Device``.
         """
         if not (
             isinstance(origin, tuple)
             and len(origin) == 2
-            and all(isinstance(val, (int, float)) for val in origin)
+            and all(isinstance(val, numbers.Real) for val in origin)
         ):
             raise TypeError("Origin must be a tuple of floats (x, y).")
         self._warn_if_mesh_exist("scale()")
         device = self.copy(with_mesh=False)
         for polygon in device.polygons:
             polygon.scale(xfact=xfact, yfact=yfact, origin=origin, inplace=True)
         if device.probe_points is not None:
@@ -445,15 +444,15 @@
 
         Returns:
             The rotated ``Device``.
         """
         if not (
             isinstance(origin, tuple)
             and len(origin) == 2
-            and all(isinstance(val, (int, float)) for val in origin)
+            and all(isinstance(val, numbers.Real) for val in origin)
         ):
             raise TypeError("Origin must be a tuple of floats (x, y).")
         self._warn_if_mesh_exist("rotate()")
         device = self.copy(with_mesh=False)
         for polygon in device.polygons:
             polygon.rotate(degrees, origin=origin, inplace=True)
         if self.probe_points is not None:
@@ -580,15 +579,15 @@
         """
         self.mesh = Mesh.from_triangulation(
             points / self.coherence_length.magnitude,
             triangles,
             create_submesh=True,
         )
 
-    def mesh_stats_dict(self) -> Dict[str, Union[int, float, str]]:
+    def mesh_stats_dict(self) -> Dict[str, Union[numbers.Real, str]]:
         """Returns a dictionary of information about the mesh."""
         edge_lengths = self.edge_lengths
         areas = self.areas
 
         def _min(arr):
             if arr is not None:
                 return arr.min()
```

### Comparing `tdgl-0.8.0/tdgl/device/layer.py` & `tdgl-0.8.1/tdgl/device/layer.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/device/meshing.py` & `tdgl-0.8.1/tdgl/device/meshing.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/device/polygon.py` & `tdgl-0.8.1/tdgl/device/polygon.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/distance.py` & `tdgl-0.8.1/tdgl/distance.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/em.py` & `tdgl-0.8.1/tdgl/em.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/finite_volume/edge_mesh.py` & `tdgl-0.8.1/tdgl/finite_volume/edge_mesh.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/finite_volume/mesh.py` & `tdgl-0.8.1/tdgl/finite_volume/mesh.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/finite_volume/operators.py` & `tdgl-0.8.1/tdgl/finite_volume/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from typing import Callable, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
 
 try:
     import cupy  # type: ignore
-    from cupyx.scipy.sparse import csc_matrix, csr_matrix  # type: ignore
-    from cupyx.scipy.sparse.linalg import factorized  # type: ignore
 except ImportError:
     cupy = None
+else:
+    from cupyx.scipy.sparse import csc_matrix, csr_matrix  # type: ignore
+    from cupyx.scipy.sparse.linalg import factorized  # type: ignore
 
 from ..solver.options import SparseSolver
 from .mesh import Mesh
 
 
 def _get_spmatrix_offsets_cupy(spmatrix, i, j):
     """Calculates the sparse matrix offsets for a set of rows ``i`` and columns ``j``."""
@@ -293,14 +294,17 @@
             self.areas = cupy.array(self.areas)
             self.edge_directions = cupy.array(self.edge_directions)
         if self.sparse_solver is SparseSolver.CUPY:
             assert cupy is not None
             self.mu_laplacian = csc_matrix(self.mu_laplacian)
             self.mu_laplacian_lu = factorized(self.mu_laplacian)
         elif self.sparse_solver is SparseSolver.PARDISO:
+            # https://github.com/loganbvh/py-tdgl/issues/74
+            # https://github.com/haasad/PyPardiso/issues/68
+            self.mu_laplacian = sp.csc_matrix(self.mu_laplacian)
             self.mu_laplacian_lu = None
         else:
             use_umfpack = self.sparse_solver is SparseSolver.UMFPACK
             sp.linalg.use_solver(useUmfpack=use_umfpack)
             self.mu_laplacian_lu = sp.linalg.factorized(self.mu_laplacian)
 
     def set_link_exponents(self, link_exponents: np.ndarray) -> None:
```

### Comparing `tdgl-0.8.0/tdgl/finite_volume/util.py` & `tdgl-0.8.1/tdgl/finite_volume/util.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/fluxoid.py` & `tdgl-0.8.1/tdgl/fluxoid.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/geometry.py` & `tdgl-0.8.1/tdgl/geometry.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/parameter.py` & `tdgl-0.8.1/tdgl/parameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import inspect
 import operator
+from numbers import Number
 from typing import Callable, Optional, Union
 
 import cloudpickle
 import numpy as np
 
 
 class _FakeArgSpec:
@@ -63,34 +64,34 @@
 
 
 class Parameter:
     """A callable object that computes a scalar or vector quantity
     as a function of position coordinates x, y (and optionally z and time t).
 
     Addition, subtraction, multiplication, and division
-    between multiple Parameters and/or real numbers (ints and floats)
-    is supported. The result of any of these operations is a
-    ``CompositeParameter`` object.
+    between multiple Parameters and/or numbers is supported.
+    The result of any of these operations is a ``CompositeParameter`` object.
 
     Args:
         func: A callable/function that actually calculates the parameter's value.
             The function must take x, y (and optionally z) as the first and only
             positional arguments, and all other arguments must be keyword arguments.
             Therefore func should have a signature like
             ``func(x, y, z, a=1, b=2, c=True)``, ``func(x, y, *, a, b, c)``,
             ``func(x, y, z, *, a, b, c)``, or ``func(x, y, z, *, a, b=None, c=3)``.
             For time-dependent Parameters, ``func`` must also take time ``t`` as a
             keyword-only argument.
         time_dependent: Specifies that ``func`` is a function of time ``t``.
         kwargs: Keyword arguments for func.
     """
 
-    __slots__ = ("func", "kwargs", "time_dependent", "_cache")
+    __slots__ = ("func", "kwargs", "time_dependent", "_cache", "_use_cache")
 
     def __init__(self, func: Callable, time_dependent: bool = False, **kwargs):
+        self._use_cache = kwargs.pop("use_cache", None)
         argspec = inspect.getfullargspec(func)
         args = argspec.args
         num_args = 2
         if args[:num_args] != ["x", "y"]:
             raise ValueError(
                 "The first function arguments must be x and y, "
                 f"not {', '.join(args[:num_args])!r}."
@@ -148,34 +149,48 @@
             hex(hash(_to_tuple(self.kwargs.items())))
             + hashlib.sha1(np.ascontiguousarray(x)).hexdigest()
             + hashlib.sha1(np.ascontiguousarray(y)).hexdigest()
             + hashlib.sha1(np.ascontiguousarray(z)).hexdigest()
             + hex(hash(t))
         )
 
+    def _evaluate(
+        self,
+        x: Union[Number, np.ndarray],
+        y: Union[Number, np.ndarray],
+        z: Optional[Union[Number, np.ndarray]] = None,
+        t: Optional[float] = None,
+    ) -> Union[Number, np.ndarray]:
+        kwargs = self.kwargs.copy()
+        if t is not None:
+            kwargs["t"] = t
+        x, y = np.atleast_1d(x, y)
+        if z is not None:
+            kwargs["z"] = np.atleast_1d(z)
+        result = np.asarray(self.func(x, y, **kwargs)).squeeze()
+        if result.ndim == 0:
+            result = result.item()
+        return result
+
     def __call__(
         self,
-        x: Union[int, float, np.ndarray],
-        y: Union[int, float, np.ndarray],
-        z: Optional[Union[int, float, np.ndarray]] = None,
+        x: Union[Number, np.ndarray],
+        y: Union[Number, np.ndarray],
+        z: Optional[Union[Number, np.ndarray]] = None,
         t: Optional[float] = None,
-    ) -> Union[int, float, np.ndarray]:
-        cache_key = self._hash_args(x, y, z, t)
-        if cache_key not in self._cache:
-            kwargs = self.kwargs.copy()
-            if t is not None:
-                kwargs["t"] = t
-            x, y = np.atleast_1d(x, y)
-            if z is not None:
-                kwargs["z"] = np.atleast_1d(z)
-            result = np.asarray(self.func(x, y, **kwargs)).squeeze()
-            if result.ndim == 0:
-                result = result.item()
-            self._cache[cache_key] = result
-        return self._cache[cache_key]
+    ) -> Union[Number, np.ndarray]:
+        if self._use_cache:
+            cache_key = self._hash_args(x, y, z, t)
+            if cache_key not in self._cache:
+                self._cache[cache_key] = self._evaluate(x, y, z, t)
+            return self._cache[cache_key]
+        return self._evaluate(x, y, z, t)
+
+    def _clear_cache(self) -> None:
+        self._cache.clear()
 
     def _get_argspec(self) -> _FakeArgSpec:
         if self.kwargs:
             kwargs, kwarg_values = list(zip(*self.kwargs.items()))
         else:
             kwargs = []
             kwarg_values = []
@@ -263,20 +278,19 @@
 
 
 class CompositeParameter(Parameter):
     """A callable object that behaves like a Parameter
     (i.e. it computes a scalar or vector quantity as a function of
     position coordinates x, y, z). A CompositeParameter object is created as
     a result of mathematical operations between Parameters, CompositeParameters,
-    and/or real numbers.
+    and/or numbers.
 
     Addition, subtraction, multiplication, division, and exponentiation
-    between Parameters, CompositeParameters and real numbers (ints and floats)
-    are supported. The result of any of these operations is a new
-    CompositeParameter object.
+    between ``Parameters``, ``CompositeParameters`` and numbers are supported.
+    The result of any of these operations is a new ``CompositeParameter`` object.
 
     Args:
         left: The object on the left-hand side of the operator.
         right: The object on the right-hand side of the operator.
         operator_: The operator acting on left and right (or its string representation).
     """
 
@@ -286,57 +300,69 @@
         operator.mul: "*",
         operator.truediv: "/",
         operator.pow: "**",
     }
 
     def __init__(
         self,
-        left: Union[int, float, Parameter, "CompositeParameter"],
-        right: Union[int, float, Parameter, "CompositeParameter"],
+        left: Union[Number, Parameter, "CompositeParameter"],
+        right: Union[Number, Parameter, "CompositeParameter"],
         operator_: Union[Callable, str],
     ):
-        valid_types = (int, float, complex, Parameter, CompositeParameter)
+        valid_types = (Number, Parameter, CompositeParameter)
         if not isinstance(left, valid_types):
             raise TypeError(
                 f"Left must be a number, Parameter, or CompositeParameter, "
                 f"not {type(left)!r}."
             )
         if not isinstance(right, valid_types):
             raise TypeError(
                 f"Right must be a number, Parameter, or CompositeParameter, "
                 f"not {type(right)!r}."
             )
-        if isinstance(left, (int, float)) and isinstance(right, (int, float)):
+        if isinstance(left, Number) and isinstance(right, Number):
             raise TypeError(
                 "Either left or right must be a Parameter or CompositeParameter."
             )
         if isinstance(operator_, str):
             operators = {v: k for k, v in self.VALID_OPERATORS.items()}
             operator_ = operators.get(operator_.strip(), None)
         if operator_ not in self.VALID_OPERATORS:
             raise ValueError(
                 f"Unknown operator, {operator_!r}. "
                 f"Valid operators are {list(self.VALID_OPERATORS)!r}."
             )
+        self._cache = {}
         self.left = left
         self.right = right
         self.operator = operator_
         self.time_dependent = False
         if isinstance(self.left, Parameter) and self.left.time_dependent:
             self.time_dependent = True
+            if self.left._use_cache is None:
+                self.left._use_cache = True
         if isinstance(self.right, Parameter) and self.right.time_dependent:
             self.time_dependent = True
+            if self.right._use_cache is None:
+                self.right._use_cache = True
+
+    def _clear_cache(self) -> None:
+        self._cache.clear()
+        if isinstance(self.right._cache, Parameter):
+            self.right._clear_cache()
+        if isinstance(self.left, Parameter):
+            self.left._clear_cache()
 
     def __call__(
         self,
-        x: Union[int, float, np.ndarray],
-        y: Union[int, float, np.ndarray],
-        z: Optional[Union[int, float, np.ndarray]] = None,
+        x: Union[Number, np.ndarray],
+        y: Union[Number, np.ndarray],
+        z: Union[Number, np.ndarray, None] = None,
         t: Optional[float] = None,
-    ) -> Union[int, float, np.ndarray]:
+    ) -> Union[Number, np.ndarray]:
         kwargs = dict() if t is None else dict(t=t)
         values = []
         for operand in (self.left, self.right):
             if isinstance(operand, Parameter):
                 if operand.time_dependent:
                     value = operand(x, y, z, **kwargs)
                 else:
@@ -393,15 +419,15 @@
         state["right"] = cloudpickle.loads(state["right"])
         self.__dict__.update(state)
 
 
 class Constant(Parameter):
     """A Parameter whose value doesn't depend on position or time."""
 
-    def __init__(self, value: Union[int, float, complex], dimensions: int = 2):
+    def __init__(self, value: Number, dimensions: int = 2):
         if dimensions not in (2, 3):
             raise ValueError(f"Dimensions must be 2 or 3, got {dimensions}.")
         if dimensions == 2:
 
             def constant(x, y, value=0):
                 return value * np.ones_like(x)
```

### Comparing `tdgl-0.8.0/tdgl/solution/data.py` & `tdgl-0.8.1/tdgl/solution/data.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/solution/plot_solution.py` & `tdgl-0.8.1/tdgl/solution/plot_solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             method="cubic",
             units=str(units),
             with_units=False,
         )
         Jx, Jy = Jgrid
         J = np.sqrt(Jx**2 + Jy**2)
         xy = np.array([xgrid.ravel(), ygrid.ravel()]).T
-        ix = np.where(~solution.device.contains_points(xy)[0])
+        ix = np.where(~solution.device.contains_points(xy))[0]
         ix = np.unravel_index(ix, J.shape)
         Jx[ix] = np.nan
         Jy[ix] = np.nan
         if min_stream_amp is not None:
             cutoff = np.nanmax(J) * min_stream_amp
             Jx[J < cutoff] = np.nan
             Jy[J < cutoff] = np.nan
```

### Comparing `tdgl-0.8.0/tdgl/solution/solution.py` & `tdgl-0.8.1/tdgl/solution/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import logging
+import numbers
 import operator
 import os
-import pickle
 import shutil
 from contextlib import nullcontext
 from datetime import datetime
 from typing import Any, Callable, Dict, Literal, NamedTuple, Optional, Tuple, Union
 
 import cloudpickle
 import h5py
@@ -717,15 +717,15 @@
         if positions.shape[1] == 3:
             if zs is not None:
                 raise ValueError(
                     "If positions has shape (m, 3) then zs cannot be specified."
                 )
             zs = positions[:, 2]
             positions = positions[:, :2]
-        elif isinstance(zs, (int, float, np.generic)):
+        elif isinstance(zs, numbers.Real):
             # constant zs
             zs = zs * np.ones(len(positions))
         zs = zs.squeeze()
         if not isinstance(zs, np.ndarray):
             raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
         weights = device.mesh.areas * device.coherence_length.magnitude**2
         # Compute the fields at the specified positions from the currents in each layer
@@ -817,15 +817,15 @@
         if positions.shape[1] == 3:
             if zs is not None:
                 raise ValueError(
                     "If positions has shape (m, 3) then zs cannot be specified."
                 )
             zs = positions[:, 2]
             positions = positions[:, :2]
-        elif isinstance(zs, (int, float, np.generic)):
+        elif isinstance(zs, numbers.Real):
             # constant zs
             zs = zs * np.ones(len(positions))
         if not isinstance(zs, np.ndarray):
             raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
         if zs.ndim == 1:
             # We need zs to be shape (m, 1)
             zs = zs[:, np.newaxis]
@@ -887,14 +887,15 @@
         if isinstance(h5file, str):
             mode = "x" if save_tdgl_data else "r+"
             save_context = h5py.File(h5file, mode)
         else:
             save_context = nullcontext(h5file)
 
         with save_context as f:
+            f.require_group("version_info").attrs.update(self.version_info)
             if "mesh" in f:
                 del f["mesh"]
             data_grp = f.require_group("data")
             if save_tdgl_data:
                 self.tdgl_data.to_hdf5(data_grp)
                 self.dynamics.to_hdf5(
                     data_grp.require_group(f"{self.tdgl_data.step}/running_state")
@@ -965,22 +966,20 @@
             The loaded Solution instance.
         """
 
         def deserialize_func(name, h5group):
             if name in h5group.attrs:
                 return h5group.attrs[name]
             if f"{name}.pickle" in h5group:
-                return pickle.loads(np.void(grp[f"{name}.pickle"]).tobytes())
+                return cloudpickle.loads(np.void(grp[f"{name}.pickle"]).tobytes())
             raise IOError(f"Unable to load {name}.")
 
         with h5py.File(path, "r") as f:
             grp = f["solution"]
-            options_kwargs = dict()
-            for k, v in grp["options"].attrs.items():
-                options_kwargs[k] = v
+            options_kwargs = dict(grp["options"].attrs)
             options = SolverOptions(**options_kwargs)
             options.validate()
             time_created = datetime.fromisoformat(grp.attrs["time_created"])
             vector_potential = deserialize_func("applied_vector_potential", grp)
             terminal_currents = deserialize_func("terminal_currents", grp)
             disorder_epsilon = deserialize_func("disorder_epsilon", grp)
             total_seconds = grp.attrs["total_seconds"]
```

### Comparing `tdgl-0.8.0/tdgl/solver/options.py` & `tdgl-0.8.1/tdgl/solver/options.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/solver/runner.py` & `tdgl-0.8.1/tdgl/solver/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import logging
+import numbers
 import os
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
 import warnings
@@ -149,15 +150,15 @@
         for key, value in fixed_data.items():
             value = _get(value)
             self.output_file[key] = value
             self.tmp_file[key] = value
 
     def save_time_step(
         self,
-        state: Dict[str, Union[int, float]],
+        state: Dict[str, numbers.Real],
         data: Dict[str, np.ndarray],
         running_state: Union[Dict[str, np.ndarray], None],
     ) -> None:
         """Save the state and data that are updated at each solve step."""
         group = self.time_step_group.create_group(f"{self.save_number}")
         group.attrs["timestamp"] = datetime.now().isoformat()
         self.save_number += 1
```

### Comparing `tdgl-0.8.0/tdgl/solver/screening.py` & `tdgl-0.8.1/tdgl/solver/screening.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/solver/solve.py` & `tdgl-0.8.1/tdgl/solver/solve.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/solver/solver.py` & `tdgl-0.8.1/tdgl/solver/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import itertools
 import logging
 import math
+import numbers
 import os
 from datetime import datetime
 from typing import Callable, Dict, List, NamedTuple, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
 
@@ -99,16 +100,16 @@
             or of position and time ``(x, y, z, *, t)``. If a float ``B`` is given,
             the applied vector potential will be that of a uniform magnetic field with
             strength ``B`` ``field_units``. If the applied vector potential is time-dependent,
             this argument must be a :class:`tdgl.Parameter`.
         terminal_currents: A dict of ``{terminal_name: current}`` or a callable with signature
             ``func(time: float) -> {terminal_name: current}``, where ``current`` is a float
             in units of ``current_units`` and ``time`` is the dimensionless time.
-        disorder_epsilon: A float in range [-1, 1], or a function that returns
-            :math:`\\epsilon\\in[-1, 1]` as a function of position ``r=(x, y)`` or
+        disorder_epsilon: A float <= 1, or a function that returns
+            :math:`\\epsilon\\leq 1` as a function of position ``r=(x, y)`` or
             position and time ``(x, y, *, t)``.
             Setting :math:`\\epsilon(\\mathbf{r}, t)=T_c/T - 1 < 1` suppresses the
             order parameter at position :math:`\\mathbf{r}=(x, y)`, which can be used
             to model inhomogeneity.
         seed_solution: A :class:`tdgl.Solution` instance to use as the initial state
             for the simulation.
     """
@@ -207,16 +208,22 @@
 
         self.disorder_epsilon = disorder_epsilon
         kw = dict(t=0) if self.dynamic_epsilon else dict()
         if self.vectorized_epsilon:
             epsilon = disorder_epsilon(self.sites, **kw)
         else:
             epsilon = np.array([float(disorder_epsilon(r, **kw)) for r in self.sites])
-        if np.any(epsilon < -1) or np.any(epsilon > 1):
-            raise ValueError("The disorder parameter epsilon must be in range [-1, 1].")
+        if np.any(epsilon > 1):
+            raise ValueError("The disorder parameter epsilon must be <= 1")
+
+        # Clear the Parameter caches
+        if isinstance(self.applied_vector_potential, Parameter):
+            self.applied_vector_potential._clear_cache()
+        if isinstance(self.disorder_epsilon, Parameter):
+            self.disorder_epsilon._clear_cache()
 
         # Find the current terminal sites.
         self.terminal_info = device.terminal_info()
         self.terminal_names = [term.name for term in self.terminal_info]
         for term_info in self.terminal_info:
             if term_info.length == 0:
                 raise ValueError(
@@ -568,15 +575,15 @@
             screening_error = float(xp.max(numerator / denominator))
             del velocity[:-2]
             del A_induced_vals[:-2]
         return A_induced, screening_error
 
     def update(
         self,
-        state: Dict[str, Union[int, float]],
+        state: Dict[str, numbers.Real],
         running_state: RunningState,
         dt: float,
         *,
         psi: np.ndarray,
         mu: np.ndarray,
         supercurrent: np.ndarray,
         normal_current: np.ndarray,
@@ -795,14 +802,20 @@
                 logger=logger,
             )
             data_was_generated = runner.run()
             end_time = datetime.now()
             logger.info(f"Simulation ended at {end_time}")
             logger.info(f"Simulation took {end_time - start_time}")
 
+            # Clear the Parameter caches
+            if isinstance(self.applied_vector_potential, Parameter):
+                self.applied_vector_potential._clear_cache()
+            if isinstance(self.disorder_epsilon, Parameter):
+                self.disorder_epsilon._clear_cache()
+
             solution = None
             if data_was_generated:
                 solution = Solution(
                     device=self.device,
                     path=data_handler.output_path,
                     options=options,
                     applied_vector_potential=self.applied_vector_potential,
```

### Comparing `tdgl-0.8.0/tdgl/sources/constant.py` & `tdgl-0.8.1/tdgl/sources/constant.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/sources/loop.py` & `tdgl-0.8.1/tdgl/sources/loop.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/sources/scaling.py` & `tdgl-0.8.1/tdgl/sources/scaling.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/conftest.py` & `tdgl-0.8.1/tdgl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_device.py` & `tdgl-0.8.1/tdgl/test/test_device.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_distance.py` & `tdgl-0.8.1/tdgl/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_em.py` & `tdgl-0.8.1/tdgl/test/test_em.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_parameter.py` & `tdgl-0.8.1/tdgl/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_solution.py` & `tdgl-0.8.1/tdgl/test/test_solution.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_solve.py` & `tdgl-0.8.1/tdgl/test/test_solve.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_visualization.py` & `tdgl-0.8.1/tdgl/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/test/test_visualize.py` & `tdgl-0.8.1/tdgl/test/test_visualize.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/version.py` & `tdgl-0.8.1/tdgl/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version_info__ = (0, 8, 0)
+__version_info__ = (0, 8, 1)
 __version__ = ".".join(map(str, __version_info__))
 
 
 def git_version():
     import os.path
     import subprocess
```

### Comparing `tdgl-0.8.0/tdgl/visualization/animate.py` & `tdgl-0.8.1/tdgl/visualization/animate.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/visualization/common.py` & `tdgl-0.8.1/tdgl/visualization/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,20 @@
     return fig, axes
 
 
 @contextmanager
 def non_gui_backend():
     """A contextmanager that temporarily uses a non-GUI backend for matplotlib."""
     with warnings.catch_warnings():
-        warnings.filterwarnings(
-            "ignore", category=UserWarning, message="Matplotlib is currently using agg"
-        )
+        ignore_messages = [
+            "Matplotlib is currently using agg",
+            "FigureCanvasAgg is non-interactive",
+        ]
+        for msg in ignore_messages:
+            warnings.filterwarnings("ignore", category=UserWarning, message=msg)
         try:
             old_backend = mpl.get_backend()
             mpl.use("Agg")
             yield
         finally:
             mpl.use(old_backend)
```

### Comparing `tdgl-0.8.0/tdgl/visualization/convert.py` & `tdgl-0.8.1/tdgl/visualization/convert.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/visualization/interactive.py` & `tdgl-0.8.1/tdgl/visualization/interactive.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/visualization/io.py` & `tdgl-0.8.1/tdgl/visualization/io.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/visualization/monitor.py` & `tdgl-0.8.1/tdgl/visualization/monitor.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl/visualization/snapshot.py` & `tdgl-0.8.1/tdgl/visualization/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numbers
 from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 
 from ..solution.data import get_data_range
@@ -44,15 +45,15 @@
         full_title: Include the full "state" for each frame in the figure suptitle.
         figure_kwargs: Keyword arguments passed to ``plt.subplots()`` when creating
             the figure.
 
     Returns:
         The matplotlib figure and axes for each time in ``times``
     """
-    if isinstance(times, (int, float)):
+    if isinstance(times, numbers.Real):
         times = [times]
     if quantities is None:
         quantities = Quantity.get_keys()
     if isinstance(quantities, str):
         quantities = [quantities]
     quantities = [Quantity.from_key(name.upper()) for name in quantities]
     num_plots = len(quantities)
```

### Comparing `tdgl-0.8.0/tdgl/visualize.py` & `tdgl-0.8.1/tdgl/visualize.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.8.0/tdgl.egg-info/PKG-INFO` & `tdgl-0.8.1/tdgl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.8.0
+Version: 0.8.1
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
```

### Comparing `tdgl-0.8.0/tdgl.egg-info/SOURCES.txt` & `tdgl-0.8.1/tdgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

