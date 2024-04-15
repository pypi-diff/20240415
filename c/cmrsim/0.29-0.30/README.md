# Comparing `tmp/cmrsim-0.29.tar.gz` & `tmp/cmrsim-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrsim-0.29.tar", last modified: Thu Aug 31 15:59:25 2023, max compression
+gzip compressed data, was "cmrsim-0.30.tar", last modified: Mon Apr 15 12:19:29 2024, max compression
```

## Comparing `cmrsim-0.29.tar` & `cmrsim-0.30.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.341876 cmrsim-0.29/
--rw-rw-rw-   0 root         (0) root         (0)    35060 2023-07-31 15:32:09.000000 cmrsim-0.29/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3261 2023-08-31 15:59:25.341876 cmrsim-0.29/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2852 2023-07-31 15:32:09.000000 cmrsim-0.29/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.329876 cmrsim-0.29/cmrsim/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.333876 cmrsim-0.29/cmrsim/analytic/
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5193 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/_composite_signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.333876 cmrsim-0.29/cmrsim/analytic/contrast/
--rw-r--r--   0 root         (0) root         (0)      850 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18558 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/_spatial.py
--rw-rw-rw-   0 root         (0) root         (0)    15609 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/contrast/base.py
--rw-r--r--   0 root         (0) root         (0)    12862 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/coil_sensitivities.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/diffusion_weighting.py
--rw-r--r--   0 root         (0) root         (0)     4871 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/offresonance.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/phase_tracking.py
--rw-r--r--   0 root         (0) root         (0)    13231 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/sequences.py
--rw-r--r--   0 root         (0) root         (0)     4847 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/contrast/t2_star.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.333876 cmrsim-0.29/cmrsim/analytic/encoding/
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/encoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/encoding/_from_sequence.py
--rw-r--r--   0 root         (0) root         (0)    14772 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/encoding/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9396 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/analytic/encoding/cartesian.py
--rw-r--r--   0 root         (0) root         (0)    13333 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/analytic/simulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.337876 cmrsim-0.29/cmrsim/bloch/
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/bloch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/bloch/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    27331 2023-08-31 15:55:02.000000 cmrsim-0.29/cmrsim/bloch/_generic.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/bloch/_ideal.py
--rw-rw-rw-   0 root         (0) root         (0)     6674 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/bloch/_multi_coil.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/bloch/submodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.337876 cmrsim-0.29/cmrsim/datasets/
--rw-rw-rw-   0 root         (0) root         (0)      702 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/datasets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/datasets/_analytic.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/datasets/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/datasets/_bloch.py
--rw-rw-rw-   0 root         (0) root         (0)    41560 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/datasets/_cardiac_mesh.py
--rw-r--r--   0 root         (0) root         (0)    23210 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/datasets/_flow.py
--rw-r--r--   0 root         (0) root         (0)    14039 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/datasets/_regular_grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.337876 cmrsim-0.29/cmrsim/reconstruction/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/reconstruction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/reconstruction/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6823 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/reconstruction/cartesian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.337876 cmrsim-0.29/cmrsim/simulation_templates/
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/simulation_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9173 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/simulation_templates/experimental_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    20333 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/simulation_templates/flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.341876 cmrsim-0.29/cmrsim/trajectory/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/trajectory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3299 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/trajectory/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5577 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/trajectory/_breathing.py
--rw-rw-rw-   0 root         (0) root         (0)     8492 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/trajectory/_diffusion.py
--rw-r--r--   0 root         (0) root         (0)    26069 2023-08-31 12:05:06.000000 cmrsim-0.29/cmrsim/trajectory/_flow.py
--rw-rw-rw-   0 root         (0) root         (0)    10486 2023-08-31 15:55:02.000000 cmrsim-0.29/cmrsim/trajectory/_proper_ortho_decomp.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/trajectory/_taylor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.341876 cmrsim-0.29/cmrsim/utils/
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/utils/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     6671 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/utils/display.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/utils/particle_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     7023 2023-07-31 15:32:09.000000 cmrsim-0.29/cmrsim/utils/snr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-31 15:59:25.329876 cmrsim-0.29/cmrsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3261 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1734 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-31 15:59:25.000000 cmrsim-0.29/cmrsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-31 15:59:25.341876 cmrsim-0.29/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1683 2023-08-31 12:05:06.000000 cmrsim-0.29/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/
+-rw-rw-rw-   0 root         (0) root         (0)    35060 2024-04-15 12:17:37.000000 cmrsim-0.30/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-04-15 12:19:29.836124 cmrsim-0.30/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2852 2024-04-15 12:17:37.000000 cmrsim-0.30/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim/analytic/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/_composite_signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/analytic/contrast/
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18570 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/_spatial.py
+-rw-rw-rw-   0 root         (0) root         (0)    15609 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12862 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/coil_sensitivities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4116 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/diffusion_weighting.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/offresonance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4644 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/phase_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)    13231 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/sequences.py
+-rw-rw-rw-   0 root         (0) root         (0)     4847 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/t2_star.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/analytic/encoding/
+-rw-rw-rw-   0 root         (0) root         (0)      707 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/_from_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14772 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9396 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/cartesian.py
+-rw-rw-rw-   0 root         (0) root         (0)    13333 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/bloch/
+-rw-rw-rw-   0 root         (0) root         (0)      493 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    27331 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_generic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3456 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_ideal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6674 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_multi_coil.py
+-rw-rw-rw-   0 root         (0) root         (0)     7960 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/submodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/datasets/
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_bloch.py
+-rw-rw-rw-   0 root         (0) root         (0)    41550 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_cardiac_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)    23193 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    14195 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_regular_grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/reconstruction/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6823 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/cartesian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/simulation_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9173 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/experimental_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    20333 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/trajectory/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5577 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_breathing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8492 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_diffusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    26069 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    10625 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_proper_ortho_decomp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_taylor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     6671 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/display.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/particle_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     7023 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/snr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1734 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 12:19:29.836124 cmrsim-0.30/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2024-04-15 12:17:37.000000 cmrsim-0.30/setup.py
```

### Comparing `cmrsim-0.29/LICENSE` & `cmrsim-0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/PKG-INFO` & `cmrsim-0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrsim
-Version: 0.29
+Version: 0.30
 Home-page: https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Author: Jonathan Weine, Charles McGrath
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrsim/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Project-URL: Institute, https://cmr.ethz.ch/
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `cmrsim-0.29/README.rst` & `cmrsim-0.30/README.rst`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/_composite_signal.py` & `cmrsim-0.30/cmrsim/analytic/_composite_signal.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/__init__.py` & `cmrsim-0.30/cmrsim/analytic/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/_spatial.py` & `cmrsim-0.30/cmrsim/analytic/contrast/_spatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,17 +246,17 @@
         orthonormality_bool = [np.allclose(mat, np.eye(3, 3), atol=1e-3) for mat in orthonormality]
 
         if not all(orthonormality_bool):
             raise ValueError("All encoding directions per repetitions must form an orthonormal basis: "
                              f"{orthonormality_bool} \n {orthonormality}")
 
     def update(self):
-        self._validate_shapes(self.orientation_matrix.read_value()[:, 0],
-                              self.orientation_matrix.read_value()[:, 1],
-                              self.orientation_matrix.read_value()[:, 2],
+        self._validate_shapes(self.orientation_matrix.read_value()[:, 0, :3],
+                              self.orientation_matrix.read_value()[:, 1, :3],
+                              self.orientation_matrix.read_value()[:, 2, :3],
                               self.slice_position.read_value(),
                               self.spatial_extend.read_value())
         self.expansion_factor.assign(tf.shape(self.orientation_matrix.read_value())[0])
 
 
     def __call__(self, signal_tensor: tf.Tensor, r_vectors_excitation: tf.Tensor, **kwargs):  # noqa
         """ Call function for analytice local look with REST slabs weighting
```

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/base.py` & `cmrsim-0.30/cmrsim/analytic/contrast/base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/coil_sensitivities.py` & `cmrsim-0.30/cmrsim/analytic/contrast/coil_sensitivities.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/diffusion_weighting.py` & `cmrsim-0.30/cmrsim/analytic/contrast/diffusion_weighting.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/offresonance.py` & `cmrsim-0.30/cmrsim/analytic/contrast/offresonance.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/phase_tracking.py` & `cmrsim-0.30/cmrsim/analytic/contrast/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/sequences.py` & `cmrsim-0.30/cmrsim/analytic/contrast/sequences.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/contrast/t2_star.py` & `cmrsim-0.30/cmrsim/analytic/contrast/t2_star.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/encoding/__init__.py` & `cmrsim-0.30/cmrsim/analytic/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/encoding/base.py` & `cmrsim-0.30/cmrsim/analytic/encoding/base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/encoding/cartesian.py` & `cmrsim-0.30/cmrsim/analytic/encoding/cartesian.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/analytic/simulation.py` & `cmrsim-0.30/cmrsim/analytic/simulation.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/bloch/_base.py` & `cmrsim-0.30/cmrsim/bloch/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/bloch/_generic.py` & `cmrsim-0.30/cmrsim/bloch/_generic.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/bloch/_ideal.py` & `cmrsim-0.30/cmrsim/bloch/_ideal.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/bloch/_multi_coil.py` & `cmrsim-0.30/cmrsim/bloch/_multi_coil.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/bloch/submodules.py` & `cmrsim-0.30/cmrsim/bloch/submodules.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/datasets/__init__.py` & `cmrsim-0.30/cmrsim/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/datasets/_analytic.py` & `cmrsim-0.30/cmrsim/datasets/_analytic.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/datasets/_base.py` & `cmrsim-0.30/cmrsim/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/datasets/_bloch.py` & `cmrsim-0.30/cmrsim/datasets/_bloch.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/datasets/_cardiac_mesh.py` & `cmrsim-0.30/cmrsim/datasets/_cardiac_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :param rotation_only: If true the transformation includes a normalization, thus results in a
                 rotation only.
         """
         reference_positions = self.get_positions_at_time(reference_time)
 
         # pylint: disable=E1101
         deformation_mesh = pyvista.UnstructuredGrid(
-            {vtk.VTK_TETRA: self.mesh.cell_connectivity.reshape(-1, 4)},
+            {vtk.VTK_TETRA: self.mesh.cells.reshape(-1, 5)[:, 1:]},
             reference_positions)
 
         # Apply transformation for all time steps
         for tstamp in tqdm(time_stamps, desc="Computing deformation matrices", leave=False):
 
             # Compute the deformation matrix on the mesh serving as transformation
             disps_at_timestamp = self.mesh[f"displacements_{tstamp}ms"]
@@ -196,15 +196,15 @@
         :param reference_time:
         :return:
         """
         reference_positions = self.get_positions_at_time(reference_time)
 
         # pylint: disable=E1101
         probing_mesh = pyvista.UnstructuredGrid(
-            {vtk.VTK_TETRA: self.mesh.cell_connectivity.reshape(-1, 4)},
+            {vtk.VTK_TETRA: self.mesh.cells.reshape(-1, 5)[:, 1:]},
             reference_positions)
         probing_mesh = reference_mesh.probe(probing_mesh)
         for name in field_names:
             self.mesh[name] = probing_mesh[name]
 
     def get_field(self, field_name: str, timing_indices: Iterable[int] = None) \
             -> (Quantity, np.ndarray):
```

### Comparing `cmrsim-0.29/cmrsim/datasets/_flow.py` & `cmrsim-0.30/cmrsim/datasets/_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,28 +105,26 @@
             - self.gridded_mesh
 
         :param mesh: 'pyvista.UnstructuredGrid' 3D mesh of flow-field
         :param lookup_map_spacing: (3, ) in meter - determines the pixel size of the
                              uniformly gridded mesh
         :return: None
         """
+        self.original_mesh = mesh.copy()
         image_box = np.max(mesh.points, axis=0) - np.min(mesh.points, axis=0)
         dims = (image_box / lookup_map_spacing).astype(int)
         resolution = image_box / dims
         origin = np.min(mesh.points, axis=0)
 
-        uniform_grid = pyvista.ImageData(dimensions=dims,
-                                           spacing=resolution,
-                                           origin=origin)
+        uniform_grid = pyvista.ImageData(dimensions=dims, spacing=resolution, origin=origin)
         self.lookup_map_spacing = lookup_map_spacing
-
-        uniform_grid = uniform_grid.sample(mesh)
+        uniform_grid = uniform_grid.sample(mesh, mark_blank=False)
         uniform_grid["in_mesh"] = np.array(uniform_grid["vtkValidPointMask"], dtype=np.float64)
         self.gridded_mesh = uniform_grid
-        self.original_mesh = mesh
+        
         print("Updated Mesh")
 
     # pylint: disable=multiple-statements
     # pylint: disable=too-many-arguments
     def update_seeding_volume(self,
                               seeding_vol_spacing: np.ndarray = None,
                               slice_position: np.ndarray = None,
@@ -168,17 +166,17 @@
 
         # Create uniform grid with specified seeding slice boundaries
         image_box = np.max(r_slice, axis=0) - np.min(r_slice, axis=0)
         dims = (image_box / self.seeding_vol_spacing).astype(int)
         resolution = image_box / dims
         origin = np.min(r_slice, axis=0)
         gridded_seeding_volume = pyvista.ImageData(dimensions=dims + 1,
-                                                     spacing=resolution,
-                                                     origin=origin)
-        self.gridded_seeding_volume = self.gridded_mesh.probe(gridded_seeding_volume)
+                                                   spacing=resolution,
+                                                   origin=origin)
+        self.gridded_seeding_volume = gridded_seeding_volume.sample(self.gridded_mesh, mark_blank=False)
 
         active_indx = np.where(self.gridded_seeding_volume.ptc().cell_data["in_mesh"] > 0.7)
         active_cell_centers = self.gridded_seeding_volume.cell_centers().ptc().points[active_indx]
 
         self._active_cell_centers, in_slice = self._select_slice(active_cell_centers,
                                                                  self.seeding_slice_normal,
                                                                  self.seeding_slice_position,
@@ -247,15 +245,15 @@
             in_tolerance = self._filter_positions_by_distance_to_slice(residual_particle_pos,
                                                                        distance_tolerance)
             self.n_drop = residual_particle_pos.shape[0] - in_tolerance[0].shape[0]
 
             # Re-seed particles in un-populated areas with Monte-Carlo rejection:
             # 1. Estimate current particle density within slice
             self._estimate_particle_density(residual_particle_pos[in_tolerance])
-            sampled_particle_pos = self.gridded_seeding_volume.probe(sampled_particle_pos)
+            sampled_particle_pos = pyvista.PointSet(sampled_particle_pos).sample(self.gridded_seeding_volume)
             density = np.array(sampled_particle_pos["density"])
             decision_boundaries = density / particle_density
             # 2. To prevent unintentionally increasing particle density, set the decision boundary
             # to 1 where it is larger than the defined threshold
             decision_boundaries[decision_boundaries > reseed_threshold] = 1
             # 3. MC-rejection step based on density
             mc_samples = np.random.uniform(0., 1., size=len(sampled_particle_pos.points))
@@ -409,8 +407,8 @@
                      * self.gridded_mesh.spacing[i] + self.gridded_mesh.origin[i]
                      for i in range(3)]
         residual_histogram, _ = np.histogramdd(particles, bins=bin_edges)
         sigma = self.lookup_map_spacing / self.seeding_vol_spacing * 0.75
         smoothed_histogram = gaussian_filter(residual_histogram / sampling_volume,
                                              sigma=sigma, truncate=2.5)
         self.gridded_mesh.cell_data["density"] = smoothed_histogram.reshape(-1, order="F")
-        return self.gridded_mesh.probe(self.original_mesh)
+        return self.original_mesh.sample(self.gridded_mesh)
```

### Comparing `cmrsim-0.29/cmrsim/datasets/_regular_grid.py` & `cmrsim-0.30/cmrsim/datasets/_regular_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,18 @@
         :return:
         """
         from cmrsim.utils.coordinates import compute_orientation_matrix
         total_transform = compute_orientation_matrix(slice_normal, slice_position,
                                                      readout_direction)
         nbins = (field_of_view / spacing).m_as("dimensionless").astype(int)
         new_slice = pyvista.ImageData(dimensions=nbins, spacing=spacing.m_as("m"),
-                                        origin=-field_of_view.m_as("m") / 2)
+                                      origin=-field_of_view.m_as("m") / 2)
         new_slice = new_slice.transform(total_transform, inplace=False)
-        new_slice = self.mesh.probe(new_slice)
+        new_slice = new_slice.sample(self.mesh)
+        # new_slice = self.mesh.probe(new_slice)
 
         if in_mps:
             inv_transform = np.eye(4, 4)
             inv_transform[:3, :3] = total_transform[:3, :3].T
             inv_transform[:3, 3] = -np.einsum('ij, j', inv_transform[:3, :3], slice_position.m_as("m"))
             new_slice = new_slice.transform(inv_transform, inplace=False,
                                             transform_all_input_vectors=True)
@@ -119,15 +120,15 @@
         """Approximates the magnetic field variations in z-direction due to interfaces with varying
         susceptibilities by applying a convolution (Fourier Product) with a dipole kernel to the
         susceptibility field contained in self.mesh. The name of the mesh array is specified by
         argument.
 
         Assumes that the main magnetic field is pointing in z-direction of the contained mesh.
         The susceptibility os assumed to be specified as parts per million
-        (e.g. :math:`\chi_{air} = 0.36ppm`).
+        (e.g. :math:`\\chi_{air} = 0.36ppm`).
 
         The result is store in self.mesh["offres"] and is also returned as Quantity.
 
         .. Dropdown:: Literature Reference
 
             This function is based on the work of Frank-Zijlstra, published on Mathworks:
 
@@ -159,16 +160,18 @@
         # Together this is referred to as the "DUAL" distribution:
         # down_sampled_chi = tf.nn.avg_pool3d(chi_3d[np.newaxis, ..., np.newaxis], ksize=(2, 2, 2),
         #                                     strides=(2, 2, 2), padding="VALID")
         # imaginary_channel = self._zc(down_sampled_chi[0, ..., 0])
         # ft_chi_3d_dual = tf.signal.fft3d(chi_3d + 1j * imaginary_channel)
         ft_chi_3d_dual = tf.signal.fft3d(chi_3d)
         # 2) multiplication with the dipole function
-        dipole_kernel = self._compute_fourier_dipole_kernel(field_of_view,
-                                                       np.array(ft_chi_3d_dual.shape))
+        dipole_kernel = self._compute_fourier_dipole_kernel(
+                                        field_of_view,
+                                        np.array(ft_chi_3d_dual.shape))
+        
         ft_field_3d = ft_chi_3d_dual * dipole_kernel
         # 3) inverse FT to spatial domain
         field_3d_dual = tf.signal.ifft3d(ft_field_3d)
         # 4) Subtract the up-scaled cropped center of the aliasing
         # field_3d = tf.math.real(field_3d_dual) - UC(tf.math.imag(field_3d_dual))
         field_3d = tf.math.real(field_3d_dual)
         i, j, k = [_ if _ != 0 else None for _ in -residual_per_dim]
@@ -203,15 +206,16 @@
         """
         if padding is None:
             padding = Quantity([0., 0., 0.], "m")
         r_max = np.max(input_mesh.points, axis=0) + padding.m_as("m") / 2
         r_min = np.min(input_mesh.points, axis=0) - padding.m_as("m") / 2
         nbins = (Quantity(r_max - r_min, "m") / pixel_spacing.to("m")).m.astype(int)
         mesh = pyvista.ImageData(dimensions=nbins, spacing=pixel_spacing.m_as("m"), origin=r_min)
-        mesh = input_mesh.probe(mesh)
+        mesh = mesh.sample(input_mesh)
+        # mesh = input_mesh.probe(mesh)
         return cls(mesh)
 
     @classmethod
     def from_numpy(cls, data: Union[np.ndarray, Dict[str, np.ndarray]],
                    origin_offset: Quantity = Quantity([0, 0, 0], "m"), extent: Quantity = None,
                    pixel_spacing: Quantity = None) -> 'RegularGridDataset':
         """Constructs a uniform regular 3D grid of the same shape as the data provided as argument.
@@ -244,16 +248,17 @@
 
         if extent is not None:
             pixel_spacing = extent.to("m") / np.array(shapes[0])
 
         shape = np.array(shapes[0][0:3])
         origin = - pixel_spacing * shape / 2 + origin_offset
 
-        mesh = pyvista.ImageData(dimensions=shape, spacing=pixel_spacing.m_as("m"),
-                                   origin=origin.m_as("m"))
+        mesh = pyvista.ImageData(dimensions=shape,
+                                 spacing=pixel_spacing.m_as("m"),
+                                 origin=origin.m_as("m"))
 
         for name, arr in data.items():
             mesh[name] = arr.reshape([shape.prod(), *arr.shape[3:]], order="F")
 
         return cls(mesh)
 
     @classmethod
```

### Comparing `cmrsim-0.29/cmrsim/reconstruction/base.py` & `cmrsim-0.30/cmrsim/reconstruction/base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/reconstruction/cartesian.py` & `cmrsim-0.30/cmrsim/reconstruction/cartesian.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/simulation_templates/experimental_optimization.py` & `cmrsim-0.30/cmrsim/simulation_templates/experimental_optimization.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/simulation_templates/flow.py` & `cmrsim-0.30/cmrsim/simulation_templates/flow.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/__init__.py` & `cmrsim-0.30/cmrsim/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/_base.py` & `cmrsim-0.30/cmrsim/trajectory/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/_breathing.py` & `cmrsim-0.30/cmrsim/trajectory/_breathing.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/_diffusion.py` & `cmrsim-0.30/cmrsim/trajectory/_diffusion.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/_flow.py` & `cmrsim-0.30/cmrsim/trajectory/_flow.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/trajectory/_proper_ortho_decomp.py` & `cmrsim-0.30/cmrsim/trajectory/_proper_ortho_decomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                                     dtype=tf.float32, shape=(), trainable=False)
         self.n_modes = tf.Variable(n_modes, shape=(), dtype=tf.int32)
 
         if additional_data is None: additional_data = {}
         self._additional_keys = tuple(additional_data.keys())
         self._additional_channels = tuple([additional_data[k].shape[-1] for k in self._additional_keys])
         self._additional_channel_idx = tuple([3, ] + np.cumsum(np.array(self._additional_channels)+3).tolist())
-
+        print(self._additional_channel_idx)
         data = np.concatenate([trajectories, ] + [additional_data[k] for k in self._additional_keys], axis=-1)
 
         self._nchannels = tf.Variable(data.shape[2], shape=(), dtype=tf.int32)
         phi, mode_weights = self.calculate_pod(time_grid, data, n_modes, remove_mean=False)
         self.basis_function = tf.Variable(phi, shape=(None, n_modes), dtype=tf.float32)
 
         if batch_size is not None:
@@ -160,15 +160,15 @@
         :param timing: (#timesteps) in milliseconds
         :return: (#particles, #timesteps, self._channels), {k: v} - additional data
         """
         idx_before = self.current_batch_idx.read_value()
         self.current_batch_idx.assign(batch_index)
         data = self._evaluate_trajectory(timing)
         if len(self._additional_keys) > 0:
-            additional_data = {k: data[self._additional_channel_idx[i:i+1]]
+            additional_data = {k: data[..., self._additional_channel_idx[i]:self._additional_channel_idx[i+1]]
                                for i, k in enumerate(self._additional_keys)}
         else:
             additional_data = {}
 
         self.current_batch_idx.assign(idx_before)
         return data[:, :, :3], additional_data
 
@@ -183,22 +183,22 @@
         :param kwargs: unused parameter (to adhere to calling signature of trajectory modules)
         :return: (#batch, self._channels),  {k: v} - additional data
         """
         self._taylor_module.current_time_ms.assign_add(dt)
         _t = tf.reshape(self._taylor_module.current_time_ms, [1, ])
         data = self._evaluate_trajectory(_t)
         if len(self._additional_keys) > 0:
-            additional_data = {k: data[self._additional_channel_idx[i:i+1]]
+            additional_data = {k: data[..., self._additional_channel_idx[i]:self._additional_channel_idx[i + 1]]
                                for i, k in enumerate(self._additional_keys)}
         else:
             additional_data = {}
 
         return tf.ensure_shape(data[:, 0, :3], (None, 3)), additional_data
 
-    @tf.function(jit_compile=True)
+    @tf.function(jit_compile=False, reduce_retracing=True)
     def _evaluate_trajectory(self, t: tf.Tensor) -> tf.Tensor:
         """Reconstructs the data state at given times t, by evaluating the taylor series
         of mode-weights and computing the weighted sum.
 
         :param t: (#steps) time-points to reconstruct at
         :return: data-states (#particles, #steps, #channels)
         """
```

### Comparing `cmrsim-0.29/cmrsim/trajectory/_taylor.py` & `cmrsim-0.30/cmrsim/trajectory/_taylor.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/utils/coordinates.py` & `cmrsim-0.30/cmrsim/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/utils/display.py` & `cmrsim-0.30/cmrsim/utils/display.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/utils/particle_properties.py` & `cmrsim-0.30/cmrsim/utils/particle_properties.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim/utils/snr.py` & `cmrsim-0.30/cmrsim/utils/snr.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/cmrsim.egg-info/PKG-INFO` & `cmrsim-0.30/cmrsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrsim
-Version: 0.29
+Version: 0.30
 Home-page: https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Author: Jonathan Weine, Charles McGrath
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrsim/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Project-URL: Institute, https://cmr.ethz.ch/
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `cmrsim-0.29/cmrsim.egg-info/SOURCES.txt` & `cmrsim-0.30/cmrsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmrsim-0.29/setup.py` & `cmrsim-0.30/setup.py`

 * *Files identical despite different names*

