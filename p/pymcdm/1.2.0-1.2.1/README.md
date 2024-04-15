# Comparing `tmp/pymcdm-1.2.0.tar.gz` & `tmp/pymcdm-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcdm-1.2.0.tar", last modified: Fri Aug 11 08:12:40 2023, max compression
+gzip compressed data, was "pymcdm-1.2.1.tar", last modified: Mon Apr 15 06:12:20 2024, max compression
```

## Comparing `pymcdm-1.2.0.tar` & `pymcdm-1.2.1.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.372410 pymcdm-1.2.0/
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1113 2022-11-24 08:21:26.000000 pymcdm-1.2.0/LICENSE
--rw-r--r--   0 sheh      (1000) sheh      (1000)       33 2022-11-24 08:21:26.000000 pymcdm-1.2.0/MANIFEST.in
--rw-r--r--   0 sheh      (1000) sheh      (1000)    24557 2023-08-11 08:12:40.372410 pymcdm-1.2.0/PKG-INFO
--rw-r--r--   0 sheh      (1000) sheh      (1000)    24041 2023-08-11 08:07:39.000000 pymcdm-1.2.0/README.md
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.355743 pymcdm-1.2.0/pymcdm/
--rw-r--r--   0 sheh      (1000) sheh      (1000)      144 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/__init__.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5826 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/correlations.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     8984 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/helpers.py
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.362410 pymcdm-1.2.0/pymcdm/methods/
--rw-r--r--   0 sheh      (1000) sheh      (1000)      558 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/__init__.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3825 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/aras.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4004 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/cocoso.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4119 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/codas.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     9580 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet.py
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.365743 pymcdm-1.2.0/pymcdm/methods/comet_tools/
--rw-r--r--   0 sheh      (1000) sheh      (1000)      620 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/__init__.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2704 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/compromise_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7583 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/esp_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1464 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/function_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7945 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/manual_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1870 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/method_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     6327 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/structural_comet.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4933 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/triad_supported_expert.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2575 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/comet_tools/triads_consistency.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3491 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/copras.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3649 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/edas.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5256 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/ervd.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4140 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/mabac.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3621 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/mairca.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4570 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/marcos.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1370 2023-08-11 08:07:33.000000 pymcdm-1.2.0/pymcdm/methods/mcda_method.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3100 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/moora.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3905 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/ocra.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4954 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/probid.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5306 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/promethee.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5556 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/rim.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5865 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/spotis.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3522 2023-08-11 08:07:33.000000 pymcdm-1.2.0/pymcdm/methods/topsis.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4913 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/methods/vikor.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4033 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/waspas.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3249 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/wpm.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3240 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/methods/wsm.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5153 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/normalizations.py
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.372410 pymcdm-1.2.0/pymcdm/visuals/
--rw-r--r--   0 sheh      (1000) sheh      (1000)      791 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/__init__.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1506 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/boxplot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3650 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/comet_2d_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4284 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/comet_3d_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3563 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/comet_contourf.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     4360 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/comet_esp_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3171 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/comet_tfns.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5210 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/correlation_heatmap.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2806 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/correlation_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2586 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/mej_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3579 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/polar_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2658 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/polar_weights.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3361 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/promethee_I_flows.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3856 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/promethee_I_graph.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3029 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/ranking_bar.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7641 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/ranking_flows.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2016 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/ranking_scatter.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     3870 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/rankings_flow_correlation.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     1502 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/violin.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2448 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pymcdm/visuals/weights_plot.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7603 2022-11-24 08:21:26.000000 pymcdm-1.2.0/pymcdm/weights.py
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.355743 pymcdm-1.2.0/pymcdm.egg-info/
--rw-r--r--   0 sheh      (1000) sheh      (1000)    24557 2023-08-11 08:12:40.000000 pymcdm-1.2.0/pymcdm.egg-info/PKG-INFO
--rw-r--r--   0 sheh      (1000) sheh      (1000)     2029 2023-08-11 08:12:40.000000 pymcdm-1.2.0/pymcdm.egg-info/SOURCES.txt
--rw-r--r--   0 sheh      (1000) sheh      (1000)        1 2023-08-11 08:12:40.000000 pymcdm-1.2.0/pymcdm.egg-info/dependency_links.txt
--rw-r--r--   0 sheh      (1000) sheh      (1000)       32 2023-08-11 08:12:40.000000 pymcdm-1.2.0/pymcdm.egg-info/requires.txt
--rw-r--r--   0 sheh      (1000) sheh      (1000)       12 2023-08-11 08:12:40.000000 pymcdm-1.2.0/pymcdm.egg-info/top_level.txt
--rw-r--r--   0 sheh      (1000) sheh      (1000)       81 2023-08-11 08:07:39.000000 pymcdm-1.2.0/pyproject.toml
--rw-r--r--   0 sheh      (1000) sheh      (1000)       38 2023-08-11 08:12:40.372410 pymcdm-1.2.0/setup.cfg
--rw-r--r--   0 sheh      (1000) sheh      (1000)      855 2023-08-11 08:08:23.000000 pymcdm-1.2.0/setup.py
-drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:12:40.372410 pymcdm-1.2.0/test/
--rw-r--r--   0 sheh      (1000) sheh      (1000)        0 2023-08-11 08:07:39.000000 pymcdm-1.2.0/test/__init__.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     5739 2023-08-11 08:07:39.000000 pymcdm-1.2.0/test/test_comet_tools.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)    25494 2023-08-11 08:07:39.000000 pymcdm-1.2.0/test/test_mcdm.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7982 2022-11-24 08:21:26.000000 pymcdm-1.2.0/test/test_normalizations.py
--rw-r--r--   0 sheh      (1000) sheh      (1000)     7173 2022-11-24 08:21:26.000000 pymcdm-1.2.0/test/test_weights.py
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.333982 pymcdm-1.2.1/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1113 2024-03-24 11:55:20.000000 pymcdm-1.2.1/LICENSE
+-rw-r--r--   0 sheh      (1000) sheh      (1000)       33 2024-03-24 11:55:20.000000 pymcdm-1.2.1/MANIFEST.in
+-rw-r--r--   0 sheh      (1000) sheh      (1000)    25953 2024-04-15 06:12:20.333982 pymcdm-1.2.1/PKG-INFO
+-rw-r--r--   0 sheh      (1000) sheh      (1000)    24948 2024-04-15 05:49:28.000000 pymcdm-1.2.1/README.md
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.330649 pymcdm-1.2.1/pymcdm/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      144 2024-04-15 05:53:52.000000 pymcdm-1.2.1/pymcdm/__init__.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5829 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/correlations.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     9731 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/helpers.py
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.330649 pymcdm-1.2.1/pymcdm/methods/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      579 2024-04-15 05:56:12.000000 pymcdm-1.2.1/pymcdm/methods/__init__.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3822 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/aras.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4004 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/cocoso.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4109 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/codas.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     9627 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/comet.py
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.330649 pymcdm-1.2.1/pymcdm/methods/comet_tools/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      694 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/__init__.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2704 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/compromise_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     8304 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/esp_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1464 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/function_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1387 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/local_weights.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     8178 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/manual_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1870 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/method_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     6426 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/structural_comet.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5136 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/triad_supported_expert.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2594 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/comet_tools/triads_consistency.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3758 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/copras.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3646 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/edas.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5271 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/ervd.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4157 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/mabac.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3623 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/mairca.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4585 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/marcos.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1370 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/methods/mcda_method.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3118 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/moora.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3916 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/ocra.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4973 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/probid.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5317 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/promethee.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3446 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/ram.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5570 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/rim.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5864 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/spotis.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3537 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/topsis.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4925 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/vikor.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4048 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/waspas.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3258 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/wpm.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3249 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pymcdm/methods/wsm.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5153 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/normalizations.py
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.333982 pymcdm-1.2.1/pymcdm/visuals/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      846 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/__init__.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1506 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/boxplot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4366 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_2d_esp_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3650 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_2d_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4129 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_3d_esp_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     4278 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_3d_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3563 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_contourf.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3171 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/comet_tfns.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5210 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/correlation_heatmap.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2806 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/correlation_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2601 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/mej_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3579 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/polar_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2658 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/polar_weights.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3361 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/promethee_I_flows.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3856 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/promethee_I_graph.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3029 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/ranking_bar.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     7641 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/ranking_flows.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2016 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/ranking_scatter.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3870 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/rankings_flow_correlation.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     1502 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/violin.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     3489 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/visuals/weights_plot.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     7603 2024-03-24 11:55:20.000000 pymcdm-1.2.1/pymcdm/weights.py
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.333982 pymcdm-1.2.1/pymcdm.egg-info/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)    25953 2024-04-15 06:12:20.000000 pymcdm-1.2.1/pymcdm.egg-info/PKG-INFO
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     2108 2024-04-15 06:12:20.000000 pymcdm-1.2.1/pymcdm.egg-info/SOURCES.txt
+-rw-r--r--   0 sheh      (1000) sheh      (1000)        1 2024-04-15 06:12:20.000000 pymcdm-1.2.1/pymcdm.egg-info/dependency_links.txt
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      121 2024-04-15 06:12:20.000000 pymcdm-1.2.1/pymcdm.egg-info/requires.txt
+-rw-r--r--   0 sheh      (1000) sheh      (1000)        7 2024-04-15 06:12:20.000000 pymcdm-1.2.1/pymcdm.egg-info/top_level.txt
+-rw-r--r--   0 sheh      (1000) sheh      (1000)      938 2024-04-15 05:49:28.000000 pymcdm-1.2.1/pyproject.toml
+-rw-r--r--   0 sheh      (1000) sheh      (1000)       38 2024-04-15 06:12:20.333982 pymcdm-1.2.1/setup.cfg
+drwxr-xr-x   0 sheh      (1000) sheh      (1000)        0 2024-04-15 06:12:20.333982 pymcdm-1.2.1/test/
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     5719 2024-04-15 05:49:28.000000 pymcdm-1.2.1/test/test_comet_tools.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)    28128 2024-03-24 11:55:20.000000 pymcdm-1.2.1/test/test_mcdm.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)    10687 2024-03-24 11:55:20.000000 pymcdm-1.2.1/test/test_normalizations.py
+-rw-r--r--   0 sheh      (1000) sheh      (1000)     7173 2024-03-24 11:55:20.000000 pymcdm-1.2.1/test/test_weights.py
```

### Comparing `pymcdm-1.2.0/LICENSE` & `pymcdm-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/PKG-INFO` & `pymcdm-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pymcdm
-Version: 1.2.0
-Summary: Python library for Multi-Criteria Decision-Making
-Home-page: https://gitlab.com/shekhand/mcda
-Author: Andrii Shekhovtsov, Bartłomiej Kizielewicz
-Author-email: andrii-shekhovtsov@zut.edu.pl, bartlomiej-kizielewicz@zut.edu.pl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyMCDM
 
 Python 3 library for solving multi-criteria decision-making (MCDM) problems.
 
 Documentation is avaliable on [readthedocs](https://pymcdm.readthedocs.io/en/master/).
 
 ___
@@ -62,37 +48,38 @@
 
 # Available methods
 
 The library contains:
 
 * MCDA methods:
 
-|  Acronym            	|  Method Name                                                                   	|                Reference               	|
-| :-------------------- | -------------------------------------------------------------------------------   | :--------------------------------------:	|
-|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution     	|               [[1]](#c1)               	|
-|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                          	|               [[2]](#c2)               	|
-|  COPRAS             	|  COmplex PRoportional ASsessment                                               	|               [[3]](#c3)               	|
-|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II   	|               [[4]](#c4)               	|
-|  COMET              	|  Characteristic Objects Method                                                 	|               [[5]](#c5)               	|
-|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                             	|               [[6]](#c6)               	|
-|  ARAS               	|  Additive Ratio ASsessment                                                     	|          [[7]](#c7),[[8]](#c8)         	|
-|  COCOSO             	|  COmbined COmpromise SOlution                                                  	|               [[9]](#c9)               	|
-|  CODAS              	|  COmbinative Distance-based ASsessment                                         	|              [[10]](#c10)              	|
-|  EDAS               	|  Evaluation based on Distance from Average Solution                            	|        [[11]](#c11),[[12]](#c12)       	|
-|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                        	|              [[13]](#c13)              	|
-|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                              	| [[14]](#c14),[[15]](#c15),[[16]](#c16) 	|
-|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution         	|        [[17]](#c17),[[18]](#c18)       	|
-|  OCRA               	|  Operational Competitiveness Ratings                                           	|        [[19]](#c19),[[20]](#c20)       	|
-|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                         	|        [[21]](#c21),[[22]](#c22)       	|
-|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               	|
-|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               	|
-|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               	|
-|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               	|
-|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               	|
-|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               	|
+|  Acronym            	|  Method Name                                                                      |                Reference                 |
+| :-------------------- | --------------------------------------------------------------------------------- | :--------------------------------------: |
+|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution        |               [[1]](#c1)                 |
+|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                             |               [[2]](#c2)                 |
+|  COPRAS             	|  COmplex PRoportional ASsessment                                                  |               [[3]](#c3)                 |
+|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II      |               [[4]](#c4)                 |
+|  COMET              	|  Characteristic Objects Method                                                    |               [[5]](#c5)                 |
+|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                                |               [[6]](#c6)                 |
+|  ARAS               	|  Additive Ratio ASsessment                                                        |          [[7]](#c7),[[8]](#c8)           |
+|  COCOSO             	|  COmbined COmpromise SOlution                                                     |               [[9]](#c9)                 |
+|  CODAS              	|  COmbinative Distance-based ASsessment                                            |              [[10]](#c10)                |
+|  EDAS               	|  Evaluation based on Distance from Average Solution                               |        [[11]](#c11),[[12]](#c12)         |
+|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                           |              [[13]](#c13)                |
+|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                                 | [[14]](#c14),[[15]](#c15),[[16]](#c16)   |
+|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution            |        [[17]](#c17),[[18]](#c18)         |
+|  OCRA               	|  Operational Competitiveness Ratings                                              |        [[19]](#c19),[[20]](#c20)         |
+|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                            |        [[21]](#c21),[[22]](#c22)         |
+|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               |
+|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               |
+|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               |
+|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               |
+|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               |
+|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               |
+|  RAM                	|  Root Assesment Method                                                            |               [[62]](#c62)               |
 
 * Weighting methods:
 
 | Acronym   	| Method Name                                             	|                 Reference                	|
 |-----------	|---------------------------------------------------------	|:----------------------------------------:	|
 | -         	| Equal/Mean weights                                      	|               [[23]](#c23)               	|
 | -         	| Entropy weights                                         	| [[23]](#c23),[[24]](#c24),[[25]](#c25) 	|
@@ -126,17 +113,17 @@
 |----------------------------------------------------	|:-------------------------:	|
 | Spearman's rank correlation coefficient            	| [[41]](#c41),[[42]](#c42) 	|
 | Pearson correlation coefficient                    	|        [[43]](#c43)       	|
 | Weighted Spearman’s rank correlation coefficient   	|        [[44]](#c44)       	|
 | Rank Similarity Coefficient                        	|        [[45]](#c45)       	|
 | Kendall rank correlation coefficient               	|        [[46]](#c46)       	|
 | Goodman and Kruskal's gamma                        	|        [[47]](#c47)       	|
-| Drastic Weighted Similarity (draWS)                   |        In Press           	|
-| Weights Similarity Coefficient (WSC)                  |        In Press           	|
-| Weights Similarity Coefficient 2 (WSC2)               |        In Press           	|
+| Drastic Weighted Similarity (draWS)                   |        [[59]](#c59)       	|
+| Weights Similarity Coefficient (WSC)                  |        [[60]](#c60)       	|
+| Weights Similarity Coefficient 2 (WSC2)               |        [[60]](#c60)       	|
 
 * Helpers
 
 | Helpers submodule     | Description                                                                                                      |
 |---------------------  |------------                                                                                                      |
 | `rankdata`            | Create ranking vector from the preference vector. Smaller preference values has higher positions in the ranking. |
 | `rrankdata`           | Alias to the `rankdata` which reverse the sorting order.                                                         |
@@ -148,15 +135,15 @@
 | Class/Function       | Description                                                                                        | Reference     |
 |----------------------|----------------------------------------------------------------------------------------------------|:-------------:|
 | `MethodExpert`       | Class which allows to evaluate CO in COMET using any MCDA method.                                  | [[56]](#c56)  |
 | `ManualExpert`       | Class which allows to evaluate CO in COMET manually by pairwise comparisons.                       | [[57]](#c57)  |
 | `FunctionExpert`     | Class which allows to evaluate CO in COMET using any expert function.                              | [[58]](#c58)  |
 | `CompromiseExpert`   | Class which allows to evaluate CO in COMET using compromise between several different methods.     | -             |
 | `TriadSupportExpert` | Class which allows to evaluate CO in COMET manually but with triads support.                       | In Press      |
-| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | In Press      |
+| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | [[61]](#c61)  |
 | `triads_consistency` | Function to which evaluates consistency of the MEJ matrix.                                         | [[55]](#c55)  |
 | `Submodel`           | Class mostly for internal use in StructuralCOMET class.                                            | [[54]](#c54)  |
 | `StructuralCOMET`    | Class which allows to split a decision problem into submodels to be evaluated by the COMET method. | [[54]](#c54)  |
 
 
 ___
 # Usage example
@@ -199,122 +186,130 @@
 4 0.0
 2 0.7829
 1 1.0
 ```
 ---
 # References
 
-<a name="c1">**[1]**</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
+<a name="c1">[1]</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
+
+<a name="c2">[2]</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
+
+<a name="c3">[3]</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
+
+<a name="c4">[4]</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
+
+<a name="c5">[5]</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
 
-<a name="c2">**[2]**</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
+<a name="c6">[6]</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
 
-<a name="c3">**[3]**</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
+<a name="c7">[7]</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
 
-<a name="c4">**[4]**</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
+<a name="c8">[8]</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
 
-<a name="c5">**[5]**</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
+<a name="c9">[9]</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
 
-<a name="c6">**[6]**</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
+<a name="c10">[10]</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
 
-<a name="c7">**[7]**</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
+<a name="c11">[11]</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
 
-<a name="c8">**[8]**</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
+<a name="c12">[12]</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
 
-<a name="c9">**[9]**</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
+<a name="c13">[13]</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
 
-<a name="c10">**[10]**</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
+<a name="c14">[14]</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
 
-<a name="c11">**[11]**</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
+<a name="c15">[15]</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
 
-<a name="c12">**[12]**</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
+<a name="c16">[16]</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
 
-<a name="c13">**[13]**</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
+<a name="c17">[17]</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
 
-<a name="c14">**[14]**</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
+<a name="c18">[18]</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
 
-<a name="c15">**[15]**</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
+<a name="c19">[19]</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
 
-<a name="c16">**[16]**</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
+<a name="c20">[20]</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
 
-<a name="c17">**[17]**</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
+<a name="c21">[21]</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
 
-<a name="c18">**[18]**</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
+<a name="c22">[22]</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
 
-<a name="c19">**[19]**</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
+<a name="c23">[23]</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
 
-<a name="c20">**[20]**</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
+<a name="c24">[24]</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
 
-<a name="c21">**[21]**</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
+<a name="c25">[25]</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
 
-<a name="c22">**[22]**</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
+<a name="c26">[26]</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
 
-<a name="c23">**[23]**</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
+<a name="c27">[27]</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
 
-<a name="c24">**[24]**</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
+<a name="c28">[28]</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
 
-<a name="c25">**[25]**</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
+<a name="c29">[29]</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
 
-<a name="c26">**[26]**</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
+<a name="c30">[30]</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
 
-<a name="c27">**[27]**</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
+<a name="c31">[31]</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
 
-<a name="c28">**[28]**</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
+<a name="c32">[32]</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
 
-<a name="c29">**[29]**</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
+<a name="c33">[33]</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
 
-<a name="c30">**[30]**</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
+<a name="c34">[34]</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
 
-<a name="c31">**[31]**</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
+<a name="c35">[35]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c32">**[32]**</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
+<a name="c36">[36]</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
 
-<a name="c33">**[33]**</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
+<a name="c37">[37]</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
 
-<a name="c34">**[34]**</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
+<a name="c38">[38]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c35">**[35]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c39">[39]</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
 
-<a name="c36">**[36]**</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
+<a name="c40">[40]</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
 
-<a name="c37">**[37]**</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
+<a name="c41">[41]</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
 
-<a name="c38">**[38]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c42">[42]</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
 
-<a name="c39">**[39]**</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
+<a name="c43">[43]</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
 
-<a name="c40">**[40]**</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
+<a name="c44">[44]</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
 
-<a name="c41">**[41]**</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
+<a name="c45">[45]</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
 
-<a name="c42">**[42]**</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
+<a name="c46">[46]</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
 
-<a name="c43">**[43]**</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
+<a name="c47">[47]</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
 
-<a name="c44">**[44]**</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
+<a name="c48">[48]</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
 
-<a name="c45">**[45]**</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
+<a name="c49">[49]</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
 
-<a name="c46">**[46]**</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
+<a name="c50">[50]</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
 
-<a name="c47">**[47]**</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
+<a name="c51">[51]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c48">**[48]**</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
+<a name="c52">[52]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c49">**[49]**</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
+<a name="c53">[53]</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
 
-<a name="c50">**[50]**</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
+<a name="c54">[54]</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
 
-<a name="c51">**[51]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c55">[55]</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
 
-<a name="c52">**[52]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c56">[56]</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
 
-<a name="c53">**[53]**</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
+<a name="c57">[57]</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
 
-<a name="c54">**[54]**</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
+<a name="c58">[58]</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
 
-<a name="c55">**[55]**</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
+<a name="c59">[59]</a> Sałabun, W., & Shekhovtsov, A. (2023, September). An Innovative Drastic Metric for Ranking Similarity in Decision-Making Problems. In 2023 18th Conference on Computer Science and Intelligence Systems (FedCSIS) (pp. 731-738). IEEE.
 
-<a name="c56">**[56]**</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
+<a name="c60">[60]</a> Shekhovtsov, A. (2023). Evaluating the Performance of Subjective Weighting Methods for Multi-Criteria Decision-Making using a novel Weights Similarity Coefficient. Procedia Computer Science, 225, 4785-4794.
 
-<a name="c57">**[57]**</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
+<a name="c61">[61]</a> Shekhovtsov, A., Kizielewicz, B., & Sałabun, W. (2023). Advancing individual decision-making: An extension of the characteristic objects method using expected solution point. Information Sciences, 647, 119456.
 
-<a name="c58">**[58]**</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
+<a name="c62">[62]</a> Sotoudeh-Anvari, A. (2023). Root Assessment Method (RAM): a novel multi-criteria decision making method and its applications in sustainability challenges. Journal of Cleaner Production, 423, 138695.
```

### Comparing `pymcdm-1.2.0/README.md` & `pymcdm-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: pymcdm
+Version: 1.2.1
+Summary: Python library for Multi-Criteria Decision-Making
+Author-email: Andrii Shekhovtsov <andrii-shekhovtsov@zut.edu.pl>, Bartłomiej Kizielewicz <bartlomiej-kizielewicz@zut.edu.pl>
+Project-URL: Homepage, https://gitlab.com/shekhand/mcda
+Project-URL: Issues, https://gitlab.com/shekhand/mcda/-/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: tabulate
+Provides-Extra: docs
+Requires-Dist: sphinx-autoapi; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: IPython; extra == "docs"
+Requires-Dist: myst_parser; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: recommonmark; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+
 # PyMCDM
 
 Python 3 library for solving multi-criteria decision-making (MCDM) problems.
 
 Documentation is avaliable on [readthedocs](https://pymcdm.readthedocs.io/en/master/).
 
 ___
@@ -48,37 +74,38 @@
 
 # Available methods
 
 The library contains:
 
 * MCDA methods:
 
-|  Acronym            	|  Method Name                                                                   	|                Reference               	|
-| :-------------------- | -------------------------------------------------------------------------------   | :--------------------------------------:	|
-|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution     	|               [[1]](#c1)               	|
-|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                          	|               [[2]](#c2)               	|
-|  COPRAS             	|  COmplex PRoportional ASsessment                                               	|               [[3]](#c3)               	|
-|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II   	|               [[4]](#c4)               	|
-|  COMET              	|  Characteristic Objects Method                                                 	|               [[5]](#c5)               	|
-|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                             	|               [[6]](#c6)               	|
-|  ARAS               	|  Additive Ratio ASsessment                                                     	|          [[7]](#c7),[[8]](#c8)         	|
-|  COCOSO             	|  COmbined COmpromise SOlution                                                  	|               [[9]](#c9)               	|
-|  CODAS              	|  COmbinative Distance-based ASsessment                                         	|              [[10]](#c10)              	|
-|  EDAS               	|  Evaluation based on Distance from Average Solution                            	|        [[11]](#c11),[[12]](#c12)       	|
-|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                        	|              [[13]](#c13)              	|
-|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                              	| [[14]](#c14),[[15]](#c15),[[16]](#c16) 	|
-|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution         	|        [[17]](#c17),[[18]](#c18)       	|
-|  OCRA               	|  Operational Competitiveness Ratings                                           	|        [[19]](#c19),[[20]](#c20)       	|
-|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                         	|        [[21]](#c21),[[22]](#c22)       	|
-|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               	|
-|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               	|
-|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               	|
-|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               	|
-|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               	|
-|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               	|
+|  Acronym            	|  Method Name                                                                      |                Reference                 |
+| :-------------------- | --------------------------------------------------------------------------------- | :--------------------------------------: |
+|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution        |               [[1]](#c1)                 |
+|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                             |               [[2]](#c2)                 |
+|  COPRAS             	|  COmplex PRoportional ASsessment                                                  |               [[3]](#c3)                 |
+|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II      |               [[4]](#c4)                 |
+|  COMET              	|  Characteristic Objects Method                                                    |               [[5]](#c5)                 |
+|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                                |               [[6]](#c6)                 |
+|  ARAS               	|  Additive Ratio ASsessment                                                        |          [[7]](#c7),[[8]](#c8)           |
+|  COCOSO             	|  COmbined COmpromise SOlution                                                     |               [[9]](#c9)                 |
+|  CODAS              	|  COmbinative Distance-based ASsessment                                            |              [[10]](#c10)                |
+|  EDAS               	|  Evaluation based on Distance from Average Solution                               |        [[11]](#c11),[[12]](#c12)         |
+|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                           |              [[13]](#c13)                |
+|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                                 | [[14]](#c14),[[15]](#c15),[[16]](#c16)   |
+|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution            |        [[17]](#c17),[[18]](#c18)         |
+|  OCRA               	|  Operational Competitiveness Ratings                                              |        [[19]](#c19),[[20]](#c20)         |
+|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                            |        [[21]](#c21),[[22]](#c22)         |
+|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               |
+|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               |
+|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               |
+|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               |
+|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               |
+|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               |
+|  RAM                	|  Root Assesment Method                                                            |               [[62]](#c62)               |
 
 * Weighting methods:
 
 | Acronym   	| Method Name                                             	|                 Reference                	|
 |-----------	|---------------------------------------------------------	|:----------------------------------------:	|
 | -         	| Equal/Mean weights                                      	|               [[23]](#c23)               	|
 | -         	| Entropy weights                                         	| [[23]](#c23),[[24]](#c24),[[25]](#c25) 	|
@@ -112,17 +139,17 @@
 |----------------------------------------------------	|:-------------------------:	|
 | Spearman's rank correlation coefficient            	| [[41]](#c41),[[42]](#c42) 	|
 | Pearson correlation coefficient                    	|        [[43]](#c43)       	|
 | Weighted Spearman’s rank correlation coefficient   	|        [[44]](#c44)       	|
 | Rank Similarity Coefficient                        	|        [[45]](#c45)       	|
 | Kendall rank correlation coefficient               	|        [[46]](#c46)       	|
 | Goodman and Kruskal's gamma                        	|        [[47]](#c47)       	|
-| Drastic Weighted Similarity (draWS)                   |        In Press           	|
-| Weights Similarity Coefficient (WSC)                  |        In Press           	|
-| Weights Similarity Coefficient 2 (WSC2)               |        In Press           	|
+| Drastic Weighted Similarity (draWS)                   |        [[59]](#c59)       	|
+| Weights Similarity Coefficient (WSC)                  |        [[60]](#c60)       	|
+| Weights Similarity Coefficient 2 (WSC2)               |        [[60]](#c60)       	|
 
 * Helpers
 
 | Helpers submodule     | Description                                                                                                      |
 |---------------------  |------------                                                                                                      |
 | `rankdata`            | Create ranking vector from the preference vector. Smaller preference values has higher positions in the ranking. |
 | `rrankdata`           | Alias to the `rankdata` which reverse the sorting order.                                                         |
@@ -134,15 +161,15 @@
 | Class/Function       | Description                                                                                        | Reference     |
 |----------------------|----------------------------------------------------------------------------------------------------|:-------------:|
 | `MethodExpert`       | Class which allows to evaluate CO in COMET using any MCDA method.                                  | [[56]](#c56)  |
 | `ManualExpert`       | Class which allows to evaluate CO in COMET manually by pairwise comparisons.                       | [[57]](#c57)  |
 | `FunctionExpert`     | Class which allows to evaluate CO in COMET using any expert function.                              | [[58]](#c58)  |
 | `CompromiseExpert`   | Class which allows to evaluate CO in COMET using compromise between several different methods.     | -             |
 | `TriadSupportExpert` | Class which allows to evaluate CO in COMET manually but with triads support.                       | In Press      |
-| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | In Press      |
+| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | [[61]](#c61)  |
 | `triads_consistency` | Function to which evaluates consistency of the MEJ matrix.                                         | [[55]](#c55)  |
 | `Submodel`           | Class mostly for internal use in StructuralCOMET class.                                            | [[54]](#c54)  |
 | `StructuralCOMET`    | Class which allows to split a decision problem into submodels to be evaluated by the COMET method. | [[54]](#c54)  |
 
 
 ___
 # Usage example
@@ -185,122 +212,130 @@
 4 0.0
 2 0.7829
 1 1.0
 ```
 ---
 # References
 
-<a name="c1">**[1]**</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
+<a name="c1">[1]</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
+
+<a name="c2">[2]</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
+
+<a name="c3">[3]</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
+
+<a name="c4">[4]</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
+
+<a name="c5">[5]</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
 
-<a name="c2">**[2]**</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
+<a name="c6">[6]</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
 
-<a name="c3">**[3]**</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
+<a name="c7">[7]</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
 
-<a name="c4">**[4]**</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
+<a name="c8">[8]</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
 
-<a name="c5">**[5]**</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
+<a name="c9">[9]</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
 
-<a name="c6">**[6]**</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
+<a name="c10">[10]</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
 
-<a name="c7">**[7]**</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
+<a name="c11">[11]</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
 
-<a name="c8">**[8]**</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
+<a name="c12">[12]</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
 
-<a name="c9">**[9]**</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
+<a name="c13">[13]</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
 
-<a name="c10">**[10]**</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
+<a name="c14">[14]</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
 
-<a name="c11">**[11]**</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
+<a name="c15">[15]</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
 
-<a name="c12">**[12]**</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
+<a name="c16">[16]</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
 
-<a name="c13">**[13]**</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
+<a name="c17">[17]</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
 
-<a name="c14">**[14]**</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
+<a name="c18">[18]</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
 
-<a name="c15">**[15]**</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
+<a name="c19">[19]</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
 
-<a name="c16">**[16]**</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
+<a name="c20">[20]</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
 
-<a name="c17">**[17]**</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
+<a name="c21">[21]</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
 
-<a name="c18">**[18]**</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
+<a name="c22">[22]</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
 
-<a name="c19">**[19]**</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
+<a name="c23">[23]</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
 
-<a name="c20">**[20]**</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
+<a name="c24">[24]</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
 
-<a name="c21">**[21]**</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
+<a name="c25">[25]</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
 
-<a name="c22">**[22]**</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
+<a name="c26">[26]</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
 
-<a name="c23">**[23]**</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
+<a name="c27">[27]</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
 
-<a name="c24">**[24]**</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
+<a name="c28">[28]</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
 
-<a name="c25">**[25]**</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
+<a name="c29">[29]</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
 
-<a name="c26">**[26]**</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
+<a name="c30">[30]</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
 
-<a name="c27">**[27]**</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
+<a name="c31">[31]</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
 
-<a name="c28">**[28]**</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
+<a name="c32">[32]</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
 
-<a name="c29">**[29]**</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
+<a name="c33">[33]</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
 
-<a name="c30">**[30]**</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
+<a name="c34">[34]</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
 
-<a name="c31">**[31]**</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
+<a name="c35">[35]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c32">**[32]**</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
+<a name="c36">[36]</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
 
-<a name="c33">**[33]**</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
+<a name="c37">[37]</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
 
-<a name="c34">**[34]**</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
+<a name="c38">[38]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c35">**[35]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c39">[39]</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
 
-<a name="c36">**[36]**</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
+<a name="c40">[40]</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
 
-<a name="c37">**[37]**</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
+<a name="c41">[41]</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
 
-<a name="c38">**[38]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c42">[42]</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
 
-<a name="c39">**[39]**</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
+<a name="c43">[43]</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
 
-<a name="c40">**[40]**</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
+<a name="c44">[44]</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
 
-<a name="c41">**[41]**</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
+<a name="c45">[45]</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
 
-<a name="c42">**[42]**</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
+<a name="c46">[46]</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
 
-<a name="c43">**[43]**</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
+<a name="c47">[47]</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
 
-<a name="c44">**[44]**</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
+<a name="c48">[48]</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
 
-<a name="c45">**[45]**</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
+<a name="c49">[49]</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
 
-<a name="c46">**[46]**</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
+<a name="c50">[50]</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
 
-<a name="c47">**[47]**</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
+<a name="c51">[51]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c48">**[48]**</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
+<a name="c52">[52]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c49">**[49]**</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
+<a name="c53">[53]</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
 
-<a name="c50">**[50]**</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
+<a name="c54">[54]</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
 
-<a name="c51">**[51]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c55">[55]</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
 
-<a name="c52">**[52]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c56">[56]</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
 
-<a name="c53">**[53]**</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
+<a name="c57">[57]</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
 
-<a name="c54">**[54]**</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
+<a name="c58">[58]</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
 
-<a name="c55">**[55]**</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
+<a name="c59">[59]</a> Sałabun, W., & Shekhovtsov, A. (2023, September). An Innovative Drastic Metric for Ranking Similarity in Decision-Making Problems. In 2023 18th Conference on Computer Science and Intelligence Systems (FedCSIS) (pp. 731-738). IEEE.
 
-<a name="c56">**[56]**</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
+<a name="c60">[60]</a> Shekhovtsov, A. (2023). Evaluating the Performance of Subjective Weighting Methods for Multi-Criteria Decision-Making using a novel Weights Similarity Coefficient. Procedia Computer Science, 225, 4785-4794.
 
-<a name="c57">**[57]**</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
+<a name="c61">[61]</a> Shekhovtsov, A., Kizielewicz, B., & Sałabun, W. (2023). Advancing individual decision-making: An extension of the characteristic objects method using expected solution point. Information Sciences, 647, 119456.
 
-<a name="c58">**[58]**</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
+<a name="c62">[62]</a> Sotoudeh-Anvari, A. (2023). Root Assessment Method (RAM): a novel multi-criteria decision making method and its applications in sustainability challenges. Journal of Cleaner Production, 423, 138695.
```

### Comparing `pymcdm-1.2.0/pymcdm/correlations.py` & `pymcdm-1.2.1/pymcdm/correlations.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from itertools import permutations
 import numpy as np
 
 __all__ = [
     'spearman',
     'rs',
     'pearson',
-    'r'
+    'r',
     'weighted_spearman',
-    'rw'
+    'rw',
     'rank_similarity_coef',
-    'ws'
+    'ws',
     'kendall_tau',
     'goodman_kruskal_gamma',
     'draws',
     'wsc',
     'wsc2'
 ]
```

### Comparing `pymcdm-1.2.0/pymcdm/helpers.py` & `pymcdm-1.2.1/pymcdm/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2021 Andrii Shekhovtsov
 # Copyright (c) 2022 Bartłomiej Kizielewicz
 
 import numpy as np
 from collections import Counter
+from collections.abc import Iterable
 
 __all__ = [
     'rankdata',
     'rrankdata',
     'correlation_matrix',
     'normalize_matrix',
     'leave_one_out_rr'
@@ -84,39 +85,45 @@
                 Otherwise the matrix will be calculated for the rows.
 
         Returns
         -------
             ndarray
                 Correlation between two rankings vectors.
     """
+    rankings = np.array(rankings)
     if columns:
         rankings = rankings.T
     n = rankings.shape[0]
     corr = np.zeros((n, n))
     for i in range(n):
         for j in range(n):
             corr[i, j] = method(rankings[i], rankings[j])
     return corr
 
 
 def normalize_matrix(matrix, method, criteria_types):
-    """ Normalize each column in `matrix`, using `normalization` function according `criteria_types`.
+    """ Normalize each column in `matrix`, using `method`normalization
+        function according to `criteria_types`.
 
         Parameters
         ----------
             matrix : ndarray
                 Decision matrix representation.
                 The rows are considered as alternatives and the columns are considered as criteria.
 
-            normalization : callable
-                Function which should be used for normalize `matrix` columns.
-                It should match signature `foo(x, cost)`, where `x` is a vector which would be normalized and `cost` is
-                a bool variable which says if `x` is a cost or profit criteria.
+            method : Callable or Iterable[Callable]
+                Function or Functions which should be used to normalize `matrix` columns.
+                Functions should match signature `foo(x, cost)`, where `x` is
+                a vector which would be normalized and `cost` is a bool variable
+                which says if `x` is a cost or profit criteria. In case of providing
+                list or tuple of the functions, number of functions should be
+                the same as number of criteria in `matrix` (columns) and same as
+                the lenght of the `criteria_types`.
 
-            criteria_types : None or ndarray
+            criteria_types : None or Iterable
                 Describes criteria types.
                 1 if criteria is profit and -1 if criteria is cost for each criteria in `matrix`.
                 If None all criteria are considered as profit
 
         Returns
         -------
             ndarray
@@ -124,29 +131,34 @@
 
         Raises
         ------
             ValueError
                 If `criteria_types` and `matrix` has different number of criteria.
     """
     if criteria_types is None:
-        nmatrix = matrix.astype('float')
-        for i in range(matrix.shape[1]):
-            nmatrix[:, i] = method(matrix[:, i], cost=False)
-        return nmatrix
-
-    if matrix.shape[1] != len(criteria_types):
-        raise ValueError(f'Matrix has {matrix.shape[1]} criteria and criteria_types has {len(criteria_types)}. This '
-                         f'values must be equal.')
+        criteria_types = np.ones(matrix.shape[1])
+    else:
+        criteria_types = np.array(criteria_types, dtype='int')
+        if np.any(np.logical_and(criteria_types != 1, criteria_types != -1)):
+            raise ValueError('Types should include only values 1 or -1.')
+
+    if (matrix.shape[1] != len(criteria_types)):
+        raise ValueError(f'Matrix has {matrix.shape[1]} criteria, criteria_types has {len(criteria_types)}. However, those values should be equal.')
+    if isinstance(method, Iterable) and matrix.shape[1] != len(method):
+        raise ValueError(f'Matrix has {matrix.shape[1]} criteria, but method has {len(method)}. Those values should be equal.')
+
+    if callable(method):
+        method = (method,) * matrix.shape[1]
 
     nmatrix = matrix.astype('float')
-    for i, type in enumerate(criteria_types):
+    for i, (type, met) in enumerate(zip(criteria_types, method)):
         if type == 1:  # If profit
-            nmatrix[:, i] = method(matrix[:, i], cost=False)
+            nmatrix[:, i] = met(matrix[:, i], cost=False)
         else:
-            nmatrix[:, i] = method(matrix[:, i], cost=True)
+            nmatrix[:, i] = met(matrix[:, i], cost=True)
     return nmatrix
 
 
 def leave_one_out_rr(method, matrix, weights, types,
                      corr_function,
                      ideal_corr_value=1,
                      only_rr=True):
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/aras.py` & `pymcdm-1.2.1/pymcdm/methods/aras.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from .mcda_method import MCDA_method
 
 
 class ARAS(MCDA_method):
     """ Additive Ratio ASsessment (ARAS) method.
 
         The ARAS method is based on a utility function value that determines the complex relative efficiency of a feasible
-        alternative [1]. This relationship is directly proportional to the relative effect of the values and weights of the
+        alternative [#aras1]_. This relationship is directly proportional to the relative effect of the values and weights of the
         main criteria.
 
-        Read more in the :ref:`User Guide <ARAS>`.
+        Read more in the User Guide.
 
 
         Parameters
         ----------
             normalization_function : callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                 cost or profit criterion.
 
         References
         ----------
-        .. [1] Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria
+        .. [#aras1] Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria
                decision‐making. Technological and economic development of economy, 16(2), 159-172.
 
         Examples
         --------
         >>> from pymcdm.methods import ARAS
         >>> import numpy as np
         >>> body = ARAS()
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/cocoso.py` & `pymcdm-1.2.1/pymcdm/methods/cocoso.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from .mcda_method import MCDA_method
 
 
 class COCOSO(MCDA_method):
     """ COmbined COmpromise SOlution (COCOSO) method.
 
         The COCOSO method is based on an integrated model of simple additive weighting and exponentially weighted
-        product [1].
+        product [#cocoso1]_.
 
-        Read more in the :ref:`User Guide <COCOSO>`.
+        Read more in the User Guide.
 
         Parameters
         ----------
             normalization_function : callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is
                 a cost or profit criterion.
 
         References
         ----------
-        .. [1] Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo)
+        .. [#cocoso1] Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo)
                method for multi-criteria decision-making problems. Management Decision.
 
         Examples
         --------
         >>> from pymcdm.methods import COCOSO
         >>> import numpy as np
         >>> body = COCOSO()
@@ -92,8 +92,8 @@
         ksi_a = (P + S) / np.sum(P + S, axis=0)
         ksi_b = S / np.min(S) + P / np.min(P)
         ksi_c = (l * S + (1 - l) * P) / (l * np.max(S) + (1 - l) * np.max(P))
 
         # Compute the prefomance score
         ksi = np.power(ksi_a * ksi_b * ksi_c, 1/3) + 1/3 * (ksi_a + ksi_b + ksi_c)
 
-        return ksi
+        return ksi
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/codas.py` & `pymcdm-1.2.1/pymcdm/methods/codas.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,28 @@
         return 1
     return 0
 
 
 class CODAS(MCDA_method):
     """ COmbinative Distance-based ASsessment (CODAS) method.
 
-        The CODAS method is based on an approach based on Euclidean distance and Taxicab from the negative ideal solution
-        [1].
+        The CODAS method is based on an approach based on Euclidean distance and Taxicab from the negative ideal solution [#codas1]_.
 
-        Read more in the :ref:`User Guide <CODAS>`.
+        Read more in the User Guide.
 
         Parameters
         ----------
             normalization_function : callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                 cost or profit criterion.
 
         References
         ----------
-        .. [1] Keshavarz Ghorabaee, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2016). A new combinative
+        .. [#codas1] Keshavarz Ghorabaee, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2016). A new combinative
                distance-based assessment (CODAS) method for multi-criteria decision-making. Economic Computation &
                Economic Cybernetics Studies & Research, 50(3).
 
         Examples
         --------
         >>> from pymcdm.methods import CODAS
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet.py` & `pymcdm-1.2.1/pymcdm/methods/comet.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     return tfn
 
 
 class COMET(MCDA_method):
     """ Characteristic Objects METhod (COMET).
 
         COMET is a method based on characteristic objects on the basis of which preference of the deicision variants is
-        calculated [1]. Due to this dependence the method is resistant to the phenomenon of ranking reversal paradox.
+        calculated [#comet1]_. Due to this dependence the method is resistant to the phenomenon of ranking reversal paradox.
 
-        Read more in the :ref:`User Guide <COMET>`.
+        Read more in the User Guide.
 
         Parameters
         ----------
            cvalues : ndarray or list of lists
                Each row represent characteristic values for each criteria.
 
            expert_function : callable
@@ -48,15 +48,15 @@
 
                Please, see the implementation of ManualExpert and MethodExpert
                in the pymcdm.comet_tools submodule if you want to create your
                own custom expert_function.
 
         References
         ----------
-        .. [1] Sałabun, W. (2015). The Characteristic Objects Method: A New Distance‐based Approach to Multicriteria
+        .. [#comet1] Sałabun, W. (2015). The Characteristic Objects Method: A New Distance‐based Approach to Multicriteria
                Decision‐making Problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
 
         Examples
         --------
         >>> from pymcdm.methods import COMET, TOPSIS
         >>> from pymcdm.comet_tools import MethodExpert
         >>> import numpy as np
@@ -144,16 +144,16 @@
             raise ValueError(
                 'Number of criteria in decision matrix must be equal to number of criteria in characteristic '
                 'values. '
             )
 
         tfns = self.tfns
 
-        pref_level_vectors = [[tfn(values) for tfn in tfns_icrit]
-                              for values, tfns_icrit in zip(alts.T, tfns)]
+        pref_level_vectors = ((lambda tfns_icrit=tfns_icrit, values=values: (tfn(values) for tfn in tfns_icrit))()
+                              for values, tfns_icrit in zip(alts.T, tfns))
 
         tfns_values_product = product(*pref_level_vectors)
         multiplayed_co = (reduce(lambda a, b: a * b, co_values) * p
                           for p, co_values in zip(self.p, tfns_values_product))
         return sum(multiplayed_co)
 
     def get_MEJ(self):
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/__init__.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from .manual_expert import ManualExpert
 from .compromise_expert import CompromiseExpert
 from .function_expert import FunctionExpert
 from .triad_supported_expert import TriadSupportExpert
 from .triads_consistency import triads_consistency
 from .structural_comet import Submodel, StructuralCOMET
 from .esp_expert import ESPExpert
+from .local_weights import get_local_weights
 
 __all__ = [
         'MethodExpert',
         'ManualExpert',
         'CompromiseExpert',
         'FunctionExpert',
         'TriadSupportExpert',
         'triads_consistency',
+        'get_local_weights',
         'Submodel',
         'StructuralCOMET',
         'ESPExpert'
         ]
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/compromise_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/compromise_expert.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/esp_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/esp_expert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) 2023 Andrii Shekhovtsov
 
+import warnings
 import numpy as np
 
 class ESPExpert:
     """ Create an object which will rate characteristic objects using Expected
         Solution Points (ESPs) provided by an expert to rate the characteristic
         objects.
 
@@ -61,15 +62,15 @@
             >>> # Generate ESP-guided cvalues based on provided ESP and psi
             >>> cvalues = expert.make_cvalues()
             >>> # Create and identify COMET model
             >>> comet = pm.methods.COMET(cvalues, expert)
             >>> # Create a visualization of the characteriscic values,
             >>> # ESP and preference function
             >>> fig, ax = plt.subplots(figsize=(4, 3.5), dpi=200)
-            >>> ax, cax = pm.visuals.comet_esp_plot(comet, esps, bounds)
+            >>> ax, cax = pm.visuals.comet_2d_esp_plot(comet, esps, bounds)
             >>> plt.tight_layout()
             >>> plt.show()
     """
 
     def __init__(self,
                  esps,
                  bounds,
@@ -134,22 +135,43 @@
         nesps = self._normalize(self.esps)
 
         distances = []
         for nesp in nesps:
             distances.append(self.distance_function(co, nesp))
         distances = self.distance_aggregation(distances, axis=0)
 
-        mej = np.zeros((co.shape[0], co.shape[0]), dtype=np.float32)
+        try:
+            result = self._call_mej(distances)
+        except MemoryError:
+            warnings.warn('Optimized version is used,'
+                          ' MEJ will be not created.')
+            result = self._call_optimized(distances)
+
+        return result
+
+    def _call_mej(self, distances):
+        mej = np.zeros((distances.shape[0], distances.shape[0]),
+                       dtype=np.float16)
         mask_better = distances[:, None] < distances
         mask_ties = distances[:, None] == distances
         mej[mask_better] = 1
         mej[~mask_better] = 0
         mej[mask_ties] = 0.5
 
-        return mej.sum(axis=1), mej
+        return mej.sum(axis=1).astype(np.float32), mej
+
+    def _call_optimized(self, distances):
+        sj = np.zeros(distances.shape[0], dtype=np.float16)
+        for dist_i in distances:
+            mask_better = distances < dist_i
+            mask_ties = distances == dist_i
+            sj[mask_better] += 1
+            sj[mask_ties] += 0.5
+
+        return sj.astype(np.float32), None
 
     def make_cvalues(self):
         """ Generate the characteristic values array based on provided
             ESPs and psi values. Usually using COMET with such cvalues will
             provide better results, however it is not mandatory.
 
             Returns
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/function_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/function_expert.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/manual_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/manual_expert.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,22 @@
         ...     show_MEJ=True
         ...     )
         >>> # You will prompted to evaluate all CO
         >>> comet = COMET(cvalues, expert_function)
     """
 
     def __init__(self, criteria_names, show_MEJ=False,
-                 tablefmt='simple_grid', filename='mej.csv'):
+                 tablefmt='simple_grid', filename='mej.csv',
+                 force_file_use=False):
         self.criteria_names = criteria_names
         self.show_MEJ = show_MEJ
         self.tablefmt = tablefmt
         self.filename = filename
         self.co_names = None
+        self.force_file_use = force_file_use
 
         self.q = None
         self.max_q = None
         self.characteristic_objects = None
 
     def __call__(self, characteristic_objects):
         """ Evaluate characteristic objects by asking pairwise comparison
@@ -144,19 +146,23 @@
                              'arguments.')
 
         print(f'\nMEJ from the file ({self.filename}):')
         self.co_names = [self._co_name(i) for i in range(1, n + 1)]
         self._show_mej(mej)
         print('\n')
 
-        print('Do you want to use this MEJ? [Y/n]')
-        ans = input('>>> ').strip().lower()
-        while ans not in ('', 'n', 'y'):
+        if not self.force_file_use:
+            print('Do you want to use this MEJ? [Y/n]')
             ans = input('>>> ').strip().lower()
-        print('\n')
+            while ans not in ('', 'n', 'y'):
+                ans = input('>>> ').strip().lower()
+            print('\n')
+        else:
+            print('This MEJ will be used in the model.')
+            ans = 'y'
 
         if ans == '' or ans == 'y':
             return mej.sum(axis=1), mej
         else:
             return None # Explicitely return None, matrix will be re-identified
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/method_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/method_expert.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/structural_comet.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/structural_comet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2023 Andrii Shekhovtsov
 
 import numpy as np
 
 from ..comet import COMET
+from ..mcda_method import MCDA_method
 
 class Submodel:
     """ Create object of the COMET submodel. This class is mostly for internal
         use in the StructuralCOMET class or for creating StructuralCOMET
         object.
 
         Parameters
@@ -77,16 +78,16 @@
         if self.model:
             return self.model(np.array([results[struct]
                                         for struct in self.structure]).T)
 
         raise ValueError('Model is not build!')
 
 
-class StructuralCOMET:
-    """ Create Structural COMET model with defined structure.
+class StructuralCOMET(MCDA_method):
+    """ Create Structural COMET model with defined structure [#struct1]_.
 
         Parameters
         ----------
             submodels : list of Submodel objects
                 List of the submodels which defines structure of the model.
                 See example for more details.
 
@@ -94,27 +95,28 @@
                 Characteristic values for criteria.
 
             criteria_names : list or None
                 Names of the criteria
 
         References
         ----------
-        .. [1] Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
+        .. [#struct1] Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
 
         Examples
         --------
-        See examples/structural_comet_example.py for example with explanation.
+        See examples/comet_tool_examples.ipynb for example with explanation.
     """
     def __init__(self,
                  submodels,
                  cvalues,
                  criteria_names=None):
         if criteria_names is not None and len(cvalues) != len(criteria_names):
             raise ValueError('Length of cvalues and cvalues_names should be equal')
 
+        self.cvalues = cvalues
         # This dict will be used to map name
         # to structure and other way around
         self._name_struct_mapper = {}
         # Build every submodel, even for each criterion alone
         self._submodels = {}
         for struct, (n, c) in enumerate(zip(criteria_names, cvalues)):
             self._name_struct_mapper[n] = struct
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/triad_supported_expert.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/triad_supported_expert.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,19 @@
         print('\nResulted MEJ:')
         self._show_mej(mej)
         print('\n')
 
         print(f'Answered by the expert: {user_q}')
         print(f'Completed by the triads: {triads_q}')
 
+        if self.filename is not None:
+            np.savetxt(self.filename, mej,
+                       fmt='%.1f', delimiter=',')
+            print(f'Identified MEJ was written to "{self.filename}".')
+
         return mej.sum(axis=1), mej
 
     def _triad_support_message(self, mej, i, j, k):
         sign = {0.0: '<', 1.0: '>', 0.5: '='}
         print('\nTriad support:')
         print(f'{self.co_names[i]} {sign[mej[i, j]]} {self.co_names[j]} and ',
               f'{self.co_names[j]} {sign[mej[j, k]]} {self.co_names[k]}')
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/comet_tools/triads_consistency.py` & `pymcdm-1.2.1/pymcdm/methods/comet_tools/triads_consistency.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,28 +43,28 @@
     (0.5, 1.0, 0.0),
     (0.5, 0.0, 1.0),
     (0.0, 0.5, 1.0),
     (0.0, 0.0, 1.0),
     )
 
 def triads_consistency(comet_or_mej):
-    """ MEJ consistency coefficient based on inconsistence triads.
+    """ MEJ consistency coefficient based on inconsistence triads [#triads1]_.
 
         Parameters
         ----------
             comet_or_mej : COMET or np.array
                 Either identified COMET method object or MEJ matrix from it.
 
         Returns
         -------
             Consistency coefficient value. See reference for details.
 
         References
         ----------
-        .. [1] Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
+        .. [#triads1] Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
 
         Examples
         --------
         >>> import numpy as np
         >>> from pymcdm.methods.comet_tools import triads_consistency
         >>> mej = np.array([
         ...     [0.5, 0.0, 0.0, 1.0, 0.0, 1.0],
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/copras.py` & `pymcdm-1.2.1/pymcdm/methods/copras.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from .mcda_method import MCDA_method
 
 
 class COPRAS(MCDA_method):
     """ COmplex PRoportional ASsessment (COPRAS) method.
 
         COPRAS is used to assess the maximizing and minimizing index values, and the effect of maximizing and minimizing
-        indexes of attributes on the results assessment is considered separately [1].
+        indexes of attributes on the results assessment is considered separately. See [#copras1]_ [#copras2]_.
 
-        Read more in the :ref:`User Guide <COPRAS>`.
+        Read more in the User Guide.
 
         References
         ----------
-        .. [1] Zavadskas, E. K., Kaklauskas, A., & Sarka, V. (1994). The new method of multicriteria complex
+        .. [#copras1] Zavadskas, E. K., Kaklauskas, A., & Sarka, V. (1994). The new method of multicriteria complex
                proportional assessment of projects. Technological and economic development of economy, 1(3), 131-139.
+        .. [#copras2] Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis,
+        Z. (2007). Multi-attribute assessment of road design solutions by
+        using the COPRAS method. The Baltic journal of Road and Bridge
+        engineering, 2(4), 195-203.
 
         Examples
         --------
         >>> from pymcdm.methods import COPRAS
         >>> import numpy as np
         >>> body = COPRAS()
         >>> matrix = np.array([[1543, 2000, 39000, 15, 13.76, 3.86, 5, 3, 5000],
@@ -27,15 +31,15 @@
         ...                    [1584, 3100, 24500, 10, 13.1, 3.7, 2, 2, 3500],
         ...                    [1560, 2700, 36000, 12, 13.2, 3.2, 3, 3, 3500],
         ...                    [1572, 2500, 31500, 13, 13.3, 3.4, 3, 2, 3500],
         ...                    [1580, 2400, 20000, 12, 12.8, 3.9, 2, 2, 3000]])
         >>> weights = np.array([0.2027, 0.1757, 0.1622, 0.1351, 0.1081, 0.0946, 0.0676, 0.0405, 0.0135])
         >>> types = np.array([-1, -1, -1, 1, 1, -1, 1, 1, 1])
         >>> [round(preference, 4) for preference in body(matrix, weights, types)]
-        [1, 0.9167, 0.8675, 0.9084, 0.9315, 0.9486]
+        [0.9459, 1.0, 0.8192, 0.8839, 0.8556, 0.7789]
     """
 
     def __init__(self):
         pass
 
     def __call__(self, matrix, weights, types, *args, **kwargs):
         """Rank alternatives from decision matrix `matrix`, with criteria weights `weights` and criteria types `types`.
@@ -74,10 +78,10 @@
 
         # Difficult normalized decision making matrix
         wmatrix = nmatrix * weights
 
         Sp = np.sum(wmatrix[:, criteria_types == 1], axis=1)
         Sm = np.sum(wmatrix[:, criteria_types == -1], axis=1)
 
-        Q = Sp + ((np.min(Sm) * np.sum(Sm)) / (Sm * np.sum(np.min(Sm) / Sm)))
+        Q = Sp + ((np.min(Sm) * Sm) / (Sm * (np.min(Sm) / Sm)))
 
         return Q / np.max(Q)
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/edas.py` & `pymcdm-1.2.1/pymcdm/methods/edas.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from .mcda_method import MCDA_method
 
 
 class EDAS(MCDA_method):
     """ Evaluation based on Distance from Average Solution (EDAS) method.
 
         The EDAS method is based on an approach in which the decision alternatives are evaluated with respect to their
-        distance from the mean solutions i.e. negative mean solution and positive mean solution [1].
+        distance from the mean solutions i.e. negative mean solution and positive mean solution [#edas1]_.
 
-        Read more in the :ref:`User Guide <EDAS>`.
+        Read more in the User Guide.
 
         References
         ----------
-        .. [1] Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory
+        .. [#edas1] Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory
                classification using a new method of evaluation based on distance from average solution (EDAS).
                Informatica, 26(3), 435-451.
 
         Examples
         --------
         >>> from pymcdm.methods import EDAS
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/ervd.py` & `pymcdm-1.2.1/pymcdm/methods/ervd.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from pymcdm import helpers
 from pymcdm import normalizations
 
 from pymcdm.methods.mcda_method import MCDA_method
 
 class ERVD(MCDA_method):
-    """ Election based on Relative Value Distances method.
+    """ Election based on Relative Value Distances method [#ervd1]_.
 
     References
     ----------
-    .. [1] Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
+    .. [#ervd1] Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
 
     Examples
     --------
     >>> matrix = np.array([
     ...     [80, 70, 87, 77, 76, 80, 75],
     ...     [85, 65, 76, 80, 75, 65, 75],
     ...     [78, 90, 72, 80, 85, 90, 85],
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/mabac.py` & `pymcdm-1.2.1/pymcdm/methods/mabac.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from .mcda_method import MCDA_method
 
 
 class MABAC(MCDA_method):
     """ Multi-Attributive Border Approximation Area Comparison (MABAC) method.
 
         The MABAC method is based on determining the distance measure between each possible alternative and the Boundary
-        Approximation Area (BAA).
+        Approximation Area (BAA) [#mabac1]_.
 
         Parameters
         ----------
            normalization_function : callable
                Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                cost or profit criterion.
 
         References
         ----------
-        .. [1] Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics
+        .. [#mabac1] Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics
                centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with
                applications, 42(6), 3016-3028.
 
         Examples
         --------
         >>> from pymcdm.methods import MABAC
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/mairca.py` & `pymcdm-1.2.1/pymcdm/methods/mairca.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from .. import helpers
 from .mcda_method import MCDA_method
 
 
 class MAIRCA(MCDA_method):
     """ Multi-Attributive RealIdeal Comparative Analysis (MARICA) method.
 
-        The MAIRCA method is based on an assumption in which it determines the gap between ideal and empirical rates.\
+        The MAIRCA method is based on an assumption in which it determines the gap between ideal and empirical rates [#mairca1]_.
 
-        Read more in the :ref:`User Guide <MAIRCA>`.
+        Read more in the User Guide.
 
         Parameters
         ----------
             normalization_function : callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                 cost or profit criterion.
 
         References
         ----------
-        .. [1] Pamučar, D., Vasin, L., & Lukovac, L. (2014, October). Selection of railway level crossings for investing
+        .. [#mairca1] Pamučar, D., Vasin, L., & Lukovac, L. (2014, October). Selection of railway level crossings for investing
                in security equipment using hybrid DEMATEL-MARICA model. In XVI international scientific-expert
                conference on railway, railcon (pp. 89-92).
 
         Examples
         --------
         >>> from pymcdm.methods import MAIRCA
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/marcos.py` & `pymcdm-1.2.1/pymcdm/methods/marcos.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     return x / x[-2]
 
 
 class MARCOS(MCDA_method):
     """ Measurement of Alternatives and Ranking according to COmpromise Solution (MARCOS) method.
 
         The MARCOS method is based on the approach of evaluating alternatives according to reference values (ideal and
-        anti-ideal) using a utility function [1].
+        anti-ideal) using a utility function [#marcos1]_.
 
         Parameters
         ----------
             normalization_function : callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                 cost or profit criterion.
 
         References
         ----------
-        .. [1] Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in
+        .. [#marcos1] Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in
                healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to
                COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
 
 
         Examples
         --------
         >>> from pymcdm.methods import MARCOS
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/mcda_method.py` & `pymcdm-1.2.1/pymcdm/methods/mcda_method.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/methods/moora.py` & `pymcdm-1.2.1/pymcdm/methods/moora.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import numpy as np
 from .mcda_method import MCDA_method
 
 
 class MOORA(MCDA_method):
     """ Multi-Objective Optimization on the basis of Ratio Analysis (MOORA) method.
 
-        The MOORA method is based on an approach using multi-objective optimization to evaluate alternatives.
+        The MOORA method is based on an approach using multi-objective optimization to evaluate alternatives [#moora1]_.
 
         References
         ----------
-        .. [1] Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a
+        .. [#moora1] Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a
              transition economy. Control and cybernetics, 35(2), 445-469.
 
 
         Examples
         --------
         >>> from pymcdm.methods import MOORA
         >>> import numpy as np
@@ -71,8 +71,8 @@
     def _moora(matrix, weights, cryteria_types):
         nmatrix = matrix / np.sqrt(np.sum(matrix ** 2, axis=0))
 
         # Difficult normalized decision making matrix
         wmatrix = nmatrix * weights
         # Calculate the composite score
         cscore = np.sum(wmatrix[:, cryteria_types == 1], axis=1) - np.sum(wmatrix[:, cryteria_types == -1], axis=1)
-        return cscore
+        return cscore
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/ocra.py` & `pymcdm-1.2.1/pymcdm/methods/ocra.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 
 class OCRA(MCDA_method):
     """ Operational Competitiveness Rating (OCRA) method.
 
         The main idea of the OCRA method is toperform   independent evaluation ofalternatives  with  respect  to
         beneficial  andnon beneficial  criteria,  and  finally  tocombine these two sets of ratings to obtainthe
-        operational competitiveness ratings [1].
+        operational competitiveness ratings [#ocra1]_.
 
         Parameters
         ----------
           normalization_function : callable
               Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
               where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
               cost or profit criterion.
 
         References
         ----------
-        .. [1] Madić, M., Petković, D., & Radovanović, M. (2015). Selection of non-conventional machining processes using
+        .. [#ocra1] Madić, M., Petković, D., & Radovanović, M. (2015). Selection of non-conventional machining processes using
              the OCRA method. Serbian Journal of Management, 10(1), 61-73.
 
 
         Examples
         --------
         >>> from pymcdm.methods import OCRA
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/probid.py` & `pymcdm-1.2.1/pymcdm/methods/probid.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from pymcdm import helpers
 from pymcdm import normalizations
 
 from pymcdm.methods.mcda_method import MCDA_method
 
 class PROBID(MCDA_method):
-    """ Preference Ranking on the Basis of Ideal-Average Distance Method.
+    """ Preference Ranking on the Basis of Ideal-Average Distance Method [#probid1]_.
 
     References
     ----------
-    .. [1] Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
+    .. [#probid1] Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
 
     Examples
     --------
     >>> matrix = np.array([
     ...     [1.679 * 10**6, 1.525 * 10**(-7), 3.747 * 10**(-5), 0.251, 2.917],
     ...     [2.213 * 10**6, 1.304 * 10**(-7), 3.250 * 10**(-5), 0.218, 6.633],
     ...     [2.461 * 10**6, 1.445 * 10**(-7), 3.854 * 10**(-5), 0.259, 0.553],
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/promethee.py` & `pymcdm-1.2.1/pymcdm/methods/promethee.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from .. import normalizations
 from .mcda_method import MCDA_method
 
 
 class PROMETHEE_II(MCDA_method):
     """ Preference Ranking Organization Method for Enrichment of Evaluations II (PROMETHEE II) method.
 
-        The PROMETHEE II method is based on a pairwise comparison of alternatives given a preference function [1].
+        The PROMETHEE II method is based on a pairwise comparison of alternatives given a preference function [#prom1]_.
 
         Parameters
         ----------
             preference_function: str
                 Name of the preference function ('usual', 'ushape', 'vshape', 'level', 'vshape_2')
 
         References
         ----------
-            .. [1] Mareschal, B., De Smet, Y., & Nemery, P. (2008, December). Rank reversal in the PROMETHEE II method:
+            .. [#prom1] Mareschal, B., De Smet, Y., & Nemery, P. (2008, December). Rank reversal in the PROMETHEE II method:
                    some new results. In 2008 IEEE International Conference on Industrial Engineering and Engineering
                    Management (pp. 959-963). IEEE.
 
         Examples
         --------
         >>> from pymcdm.methods import PROMETHEE_II
         >>> import numpy as np
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/rim.py` & `pymcdm-1.2.1/pymcdm/methods/rim.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,21 @@
     elif (a <= x < c) and (a != c):
         return 1 - (_dmin(x, c, d) / abs(a - c))
     elif (d < x <= b) and (d != b):
         return 1 - (_dmin(x, c, d) / abs(d - b))
 
 
 class RIM(MCDA_method):
-    """ Reference Ideal Method
+    """ Reference Ideal Method [#rim1]_.
 
     RIM is an MCDA method which uses criteria bounds and reference ideal to evaluate alternatives.
 
     References
     ----------
-    .. [1] Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
+    .. [#rim1] Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
 
     Examples
     --------
     >>> import numpy as np
     >>> from pymcdm.methods import RIM
     >>> matrix = np.array([
     ...     [30,  0, 2, 3, 3, 2],
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/spotis.py` & `pymcdm-1.2.1/pymcdm/methods/spotis.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 
 class SPOTIS(MCDA_method):
     """ Stable Preference Ordering Towards Ideal Solution (SPOTIS) method.
 
         The SPOTIS method is based on an approach in which it evaluates
         given decision alternatives using the distance from the best
-        ideal solution. [1].
+        ideal solution. [#spotis1]_.
 
-        Read more in the :ref:`User Guide <SPOTIS>`.
+        Read more in the User Guide.
 
         References
         ----------
-        .. [1] Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The SPOTIS rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
+        .. [#spotis1] Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The SPOTIS rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
 
         Examples
         --------
         >>> from pymcdm.methods import SPOTIS
         >>> import numpy as np
         >>> matrix = np.array([[10.5, -3.1, 1.7],
         ...                    [-4.7, 0, 3.4],
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/topsis.py` & `pymcdm-1.2.1/pymcdm/methods/topsis.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from .mcda_method import MCDA_method
 
 
 class TOPSIS(MCDA_method):
     """ Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS).
 
         The TOPSIS method is based on an approach in which it evaluates alternatives to a positive ideal solution and a
-        negative ideal solution [1].
+        negative ideal solution [#topsis1]_.
 
         Parameters
         ----------
            normalization_function : callable
                Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                cost or profit criterion.
 
         References
         ----------
-        .. [1] Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute
+        .. [#topsis1] Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute
                decision making (pp. 58-191). Springer, Berlin, Heidelberg.
 
         Examples
         --------
         >>> from pymcdm.methods import TOPSIS
         >>> import numpy as np
         >>> body = TOPSIS()
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/vikor.py` & `pymcdm-1.2.1/pymcdm/methods/vikor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
         return x
 
 
 class VIKOR(MCDA_method):
     """ VIšekriterijumsko KOmpromisno Rangiranje (VIKOR) method.
 
         The VIKOR method is based on an approach that uses a compromise mechanism to evaluate alternatives using
-        distance from the ideal [1].
+        distance from the ideal [#vikor1]_.
 
         Parameters
         ----------
             normalization_function : None or callable
                 Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                 where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                 cost or profit criterion.
 
-         References
+        References
         ----------
-        .. [1] Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water
+        .. [#vikor1] Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water
                resources research, 16(1), 14-20.
 
         Examples
         --------
         >>> from pymcdm.methods import VIKOR
         >>> import numpy as np
         >>> body = VIKOR()
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/waspas.py` & `pymcdm-1.2.1/pymcdm/methods/waspas.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import numpy as np
 from .. import normalizations
 from .. import helpers
 from .mcda_method import MCDA_method
 
 
 class WASPAS(MCDA_method):
-    """ Weighted Aggregated Sum Product ASSessment (WASPAS) [1].
+    """ Weighted Aggregated Sum Product ASSessment (WASPAS) [#waspas1]_.
 
         The WASPAS method is a unique combination of two well-known MCDM approaches, i.e. Weighted Sum Model (WSM) and
         Weighted Product Model (WPM).
 
         Parameters
         ----------
            normalization_function : callable
                Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                cost or profit criterion.
 
         References
         ----------
-        .. [1] Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted
+        .. [#waspas1] Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted
         aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
 
         Examples
         --------
         >>> from pymcdm.methods import WASPAS
         >>> import numpy as np
         >>> body = WASPAS()
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/wpm.py` & `pymcdm-1.2.1/pymcdm/methods/wpm.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import numpy as np
 from .. import normalizations
 from .. import helpers
 from .mcda_method import MCDA_method
 
 
 class WPM(MCDA_method):
-    """ Weighted Product Model (WPM) [1].
+    """ Weighted Product Model (WPM) [#wpm1]_.
 
         WPM is based on an approach that evaluates alternatives by weighted product.
 
         Parameters
         ----------
            normalization_function : callable
                Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                cost or profit criterion.
 
         References
         ----------
-        .. [1] Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability
+        .. [#wpm1] Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability
         estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
         Examples
         --------
         >>> from pymcdm.methods import WPM
         >>> import numpy as np
         >>> body = WPM()
```

### Comparing `pymcdm-1.2.0/pymcdm/methods/wsm.py` & `pymcdm-1.2.1/pymcdm/methods/wsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import numpy as np
 from .. import normalizations
 from .. import helpers
 from .mcda_method import MCDA_method
 
 
 class WSM(MCDA_method):
-    """ Weighted Sum Model (WSM) [1].
+    """ Weighted Sum Model (WSM) [#wsm1]_.
 
         WSM is based on an approach that evaluates alternatives by weighted sum.
 
         Parameters
         ----------
            normalization_function : callable
                Function which should be used to normalize `matrix` columns. It should match signature `foo(x, cost)`,
                where `x` is a vector which should be normalized and `cost` is a bool variable which says if `x` is a
                cost or profit criterion.
 
         References
         ----------
-        .. [1] Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability
+        .. [#wsm1] Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability
         estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
         Examples
         --------
         >>> from pymcdm.methods import WSM
         >>> import numpy as np
         >>> body = WSM()
```

### Comparing `pymcdm-1.2.0/pymcdm/normalizations.py` & `pymcdm-1.2.1/pymcdm/normalizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,9 +201,9 @@
 
     Returns
     -------
         ndarray
             One-dimensional numpy array of normalized values.
     """
     if cost:
-        return 1 - np.abs((np.max(x) - x) / np.max(x))
-    return 1 - np.abs((np.min(x) - x) / np.min(x))
+        return 1 - np.abs((np.min(x) - x) / np.min(x))
+    return 1 - np.abs((np.max(x) - x) / np.max(x))
```

### Comparing `pymcdm-1.2.0/pymcdm/visuals/__init__.py` & `pymcdm-1.2.1/pymcdm/visuals/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 from .violin import violin
 from .polar_plot import polar_plot
 from .polar_weights import polar_weights
 from .weights_plot import weights_plot
 from .comet_2d_plot import comet_2d_plot
 from .comet_3d_plot import comet_3d_plot
 from .comet_contourf import comet_contourf
-from .comet_esp_plot import comet_esp_plot
+from .comet_2d_esp_plot import comet_2d_esp_plot
+from .comet_3d_esp_plot import comet_3d_esp_plot
 from .comet_tfns import comet_tfns
```

### Comparing `pymcdm-1.2.0/pymcdm/visuals/boxplot.py` & `pymcdm-1.2.1/pymcdm/visuals/boxplot.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/comet_2d_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/comet_2d_plot.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/comet_3d_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/comet_3d_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,14 @@
                 f'Characteristic values must be sorted in ascending order and does not contain repeated elements. '
                 f'Check criterion with index {i}.'
             )
 
     if ax is None:
         ax = plt.axes(projection='3d')
 
-    alternatives = np.array(alternatives)
-
     plot_kwargs = dict(
         marker='x',
         linestyle='-',
         color='k',
         linewidth=0.5,
         markersize=3,
         zorder=1
@@ -102,15 +100,16 @@
     scatter_kwargs = dict(
         marker='*',
         color='green',
         s=40,
         zorder=2
     ) | scatter_kwargs
 
-    ax.scatter3D(alternatives[:, 0], alternatives[:, 1], alternatives[:, 2], **scatter_kwargs)
+    if alternatives is not None:
+        ax.scatter3D(alternatives[:, 0], alternatives[:, 1], alternatives[:, 2], **scatter_kwargs)
 
     if alternatives_labels:
         labels = ['$A_{' + str(i) + '}$' for i in range(1, alternatives.shape[0] + 1)]
 
         text_kwargs = dict(
             color='green',
             zorder=2
```

### Comparing `pymcdm-1.2.0/pymcdm/visuals/comet_contourf.py` & `pymcdm-1.2.1/pymcdm/visuals/comet_contourf.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/comet_esp_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/comet_2d_esp_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 from .comet_contourf import comet_contourf
 
-def comet_esp_plot(comet,
+def comet_2d_esp_plot(comet,
                    esps,
                    bounds,
                    alternatives=None,
                    comet_contourf_kwargs=dict(),
                    contourf_kwargs=dict(),
                    scatter_kwargs=dict(),
                    text_kwargs=dict(),
@@ -73,15 +73,15 @@
             >>> # Generate ESP-guided cvalues based on provided ESP and psi
             >>> cvalues = expert.make_cvalues()
             >>> # Create and identify COMET model
             >>> comet = pm.methods.COMET(cvalues, expert)
             >>> # Create a visualization of the characteriscic values,
             >>> # ESP and preference function
             >>> fig, ax = plt.subplots(figsize=(4, 3.5), dpi=200)
-            >>> ax, cax = pm.visuals.comet_esp_plot(comet, esps, bounds)
+            >>> ax, cax = pm.visuals.comet_2d_esp_plot(comet, esps, bounds)
             >>> plt.tight_layout()
             >>> plt.show()
     """
     if alternatives is None:
         alternatives = np.array([[], []]).T
 
     if ax is None:
```

### Comparing `pymcdm-1.2.0/pymcdm/visuals/comet_tfns.py` & `pymcdm-1.2.1/pymcdm/visuals/comet_tfns.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/correlation_heatmap.py` & `pymcdm-1.2.1/pymcdm/visuals/correlation_heatmap.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/correlation_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/mej_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/mej_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         >>> plt.show()
     """
     if ax is None:
         ax = plt.gca()
 
     if cmap is None:
         cmap = ListedColormap(['tab:red', 'tab:blue', 'tab:green'])
-    im = ax.imshow(mej, cmap=cmap)
+    im = ax.imshow(mej, cmap=cmap, aspect='auto')
 
     for edge, spine in ax.spines.items():
         spine.set_visible(False)
 
     ax.set_xticks(np.arange(mej.shape[1]+1)-0.51, minor=True)
     ax.set_yticks(np.arange(mej.shape[0]+1)-0.51, minor=True)
```

### Comparing `pymcdm-1.2.0/pymcdm/visuals/polar_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/polar_plot.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/polar_weights.py` & `pymcdm-1.2.1/pymcdm/visuals/polar_weights.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/promethee_I_flows.py` & `pymcdm-1.2.1/pymcdm/visuals/promethee_I_flows.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/promethee_I_graph.py` & `pymcdm-1.2.1/pymcdm/visuals/promethee_I_graph.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/ranking_bar.py` & `pymcdm-1.2.1/pymcdm/visuals/ranking_bar.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/ranking_flows.py` & `pymcdm-1.2.1/pymcdm/visuals/ranking_flows.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/ranking_scatter.py` & `pymcdm-1.2.1/pymcdm/visuals/ranking_scatter.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/rankings_flow_correlation.py` & `pymcdm-1.2.1/pymcdm/visuals/rankings_flow_correlation.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/violin.py` & `pymcdm-1.2.1/pymcdm/visuals/violin.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm/visuals/weights_plot.py` & `pymcdm-1.2.1/pymcdm/visuals/weights_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import matplotlib.pyplot as plt
 
 def weights_plot(weights,
                  xticklabels=None,
                  bar_kwargs=dict(),
                  legend_ncol=5,
                  colors=None,
+                 show_text=False,
+                 show_text_threshold=0.0,
+                 text_kwargs=dict(),
                  ax=None):
     """ Function for criteria weights visualisation.
 
         Parameters
         ----------
             weights : ndarray
                 Matrix of weights. Each row is a vector of weights.
@@ -24,14 +27,25 @@
                 Keywors arguments to pass into bar function.
 
             legend_ncol : int
                 Number of columns in legend.
 
             colors : Iterable or None
                 Colors for bars. If there are less colors then criteria, then colors will be cycled.
+
+            show_text : bool
+                Show the weights values as text on bars.
+
+            show_text_threshold : float
+                The smallest value of the weights to be show.
+                The values below this threshold wont be shown.
+
+            text_kwargs : dict
+                Keyword arguments for weights text.
+
             ax : Axes or None
                 Axes object to dwaw on.
 
         Returns
         -------
             ax : Axes
                 Axes object on which plot were drawn.
@@ -56,22 +70,44 @@
         xticklabels = [f'$M_{{{i + 1}}}$' for i in range(weights.shape[1])]
 
     bar_kwargs = dict(
         linewidth=1,
         edgecolor='black'
     ) | bar_kwargs
 
+    text_kwargs = dict(
+        ha='center',
+        va='center',
+        color='w',
+        fontweight='bold',
+        fontsize=8
+    ) | text_kwargs
+
     bottom = np.zeros(weights.shape[1], dtype=float)
     for i, alt in enumerate(weights):
         if colors is not None:
             bar_kwargs['color'] = colors[i % len(colors)]
 
         ax.bar(xticklabels, alt, label=f'$C_{i + 1}$', bottom=bottom, **bar_kwargs)
         bottom += alt
 
+    if show_text:
+        bottom = np.zeros(weights.shape[1])
+        for j, w in enumerate(weights):
+            means = (w / 2) + bottom
+            for i in range(len(w)):
+                if w[i] >= show_text_threshold:
+                    ax.text(
+                        i,
+                        means[i],
+                        f'{w[i]:0.3f}',
+                        **text_kwargs
+                    )
+            bottom += w
+
     ax.grid(alpha=0.5, linestyle='--')
     ax.set_axisbelow(True)
 
     ax.set_xticks(range(len(xticklabels)), labels=xticklabels)
     ax.set_xticklabels(xticklabels)
     ax.set_xlabel('Method')
```

### Comparing `pymcdm-1.2.0/pymcdm/weights.py` & `pymcdm-1.2.1/pymcdm/weights.py`

 * *Files identical despite different names*

### Comparing `pymcdm-1.2.0/pymcdm.egg-info/PKG-INFO` & `pymcdm-1.2.1/pymcdm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: pymcdm
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python library for Multi-Criteria Decision-Making
-Home-page: https://gitlab.com/shekhand/mcda
-Author: Andrii Shekhovtsov, Bartłomiej Kizielewicz
-Author-email: andrii-shekhovtsov@zut.edu.pl, bartlomiej-kizielewicz@zut.edu.pl
+Author-email: Andrii Shekhovtsov <andrii-shekhovtsov@zut.edu.pl>, Bartłomiej Kizielewicz <bartlomiej-kizielewicz@zut.edu.pl>
+Project-URL: Homepage, https://gitlab.com/shekhand/mcda
+Project-URL: Issues, https://gitlab.com/shekhand/mcda/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: tabulate
+Provides-Extra: docs
+Requires-Dist: sphinx-autoapi; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: IPython; extra == "docs"
+Requires-Dist: myst_parser; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: recommonmark; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
 
 # PyMCDM
 
 Python 3 library for solving multi-criteria decision-making (MCDM) problems.
 
 Documentation is avaliable on [readthedocs](https://pymcdm.readthedocs.io/en/master/).
 
@@ -62,37 +74,38 @@
 
 # Available methods
 
 The library contains:
 
 * MCDA methods:
 
-|  Acronym            	|  Method Name                                                                   	|                Reference               	|
-| :-------------------- | -------------------------------------------------------------------------------   | :--------------------------------------:	|
-|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution     	|               [[1]](#c1)               	|
-|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                          	|               [[2]](#c2)               	|
-|  COPRAS             	|  COmplex PRoportional ASsessment                                               	|               [[3]](#c3)               	|
-|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II   	|               [[4]](#c4)               	|
-|  COMET              	|  Characteristic Objects Method                                                 	|               [[5]](#c5)               	|
-|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                             	|               [[6]](#c6)               	|
-|  ARAS               	|  Additive Ratio ASsessment                                                     	|          [[7]](#c7),[[8]](#c8)         	|
-|  COCOSO             	|  COmbined COmpromise SOlution                                                  	|               [[9]](#c9)               	|
-|  CODAS              	|  COmbinative Distance-based ASsessment                                         	|              [[10]](#c10)              	|
-|  EDAS               	|  Evaluation based on Distance from Average Solution                            	|        [[11]](#c11),[[12]](#c12)       	|
-|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                        	|              [[13]](#c13)              	|
-|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                              	| [[14]](#c14),[[15]](#c15),[[16]](#c16) 	|
-|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution         	|        [[17]](#c17),[[18]](#c18)       	|
-|  OCRA               	|  Operational Competitiveness Ratings                                           	|        [[19]](#c19),[[20]](#c20)       	|
-|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                         	|        [[21]](#c21),[[22]](#c22)       	|
-|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               	|
-|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               	|
-|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               	|
-|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               	|
-|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               	|
-|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               	|
+|  Acronym            	|  Method Name                                                                      |                Reference                 |
+| :-------------------- | --------------------------------------------------------------------------------- | :--------------------------------------: |
+|  TOPSIS             	|  Technique for the Order of Prioritisation by Similarity to Ideal Solution        |               [[1]](#c1)                 |
+|  VIKOR              	|  VIseKriterijumska Optimizacija I Kompromisno Resenje                             |               [[2]](#c2)                 |
+|  COPRAS             	|  COmplex PRoportional ASsessment                                                  |               [[3]](#c3)                 |
+|  PROMETHEE I & II   	|  Preference Ranking Organization METHod for Enrichment of Evaluations I & II      |               [[4]](#c4)                 |
+|  COMET              	|  Characteristic Objects Method                                                    |               [[5]](#c5)                 |
+|  SPOTIS             	|  Stable Preference Ordering Towards Ideal Solution                                |               [[6]](#c6)                 |
+|  ARAS               	|  Additive Ratio ASsessment                                                        |          [[7]](#c7),[[8]](#c8)           |
+|  COCOSO             	|  COmbined COmpromise SOlution                                                     |               [[9]](#c9)                 |
+|  CODAS              	|  COmbinative Distance-based ASsessment                                            |              [[10]](#c10)                |
+|  EDAS               	|  Evaluation based on Distance from Average Solution                               |        [[11]](#c11),[[12]](#c12)         |
+|  MABAC              	|  Multi-Attributive Border Approximation area Comparison                           |              [[13]](#c13)                |
+|  MAIRCA             	|  MultiAttributive Ideal-Real Comparative Analysis                                 | [[14]](#c14),[[15]](#c15),[[16]](#c16)   |
+|  MARCOS             	|  Measurement Alternatives and Ranking according to COmpromise Solution            |        [[17]](#c17),[[18]](#c18)         |
+|  OCRA               	|  Operational Competitiveness Ratings                                              |        [[19]](#c19),[[20]](#c20)         |
+|  MOORA              	|  Multi-Objective Optimization Method by Ratio Analysis                            |        [[21]](#c21),[[22]](#c22)         |
+|  RIM                	|  Reference Ideal Method                                                           |               [[48]](#c48)               |
+|  ERVD               	|  Election Based on relative Value Distances                                       |               [[49]](#c49)               |
+|  PROBID               |  Preference Ranking On the Basis of Ideal-average Distance                        |               [[50]](#c50)               |
+|  WSM                  |  Weighted Sum Model                                                               |               [[51]](#c51)               |
+|  WPM                  |  Weighted Product Model                                                           |               [[52]](#c52)               |
+|  WASPAS               |  Weighted Aggregated Sum Product ASSessment                                       |               [[53]](#c53)               |
+|  RAM                	|  Root Assesment Method                                                            |               [[62]](#c62)               |
 
 * Weighting methods:
 
 | Acronym   	| Method Name                                             	|                 Reference                	|
 |-----------	|---------------------------------------------------------	|:----------------------------------------:	|
 | -         	| Equal/Mean weights                                      	|               [[23]](#c23)               	|
 | -         	| Entropy weights                                         	| [[23]](#c23),[[24]](#c24),[[25]](#c25) 	|
@@ -126,17 +139,17 @@
 |----------------------------------------------------	|:-------------------------:	|
 | Spearman's rank correlation coefficient            	| [[41]](#c41),[[42]](#c42) 	|
 | Pearson correlation coefficient                    	|        [[43]](#c43)       	|
 | Weighted Spearman’s rank correlation coefficient   	|        [[44]](#c44)       	|
 | Rank Similarity Coefficient                        	|        [[45]](#c45)       	|
 | Kendall rank correlation coefficient               	|        [[46]](#c46)       	|
 | Goodman and Kruskal's gamma                        	|        [[47]](#c47)       	|
-| Drastic Weighted Similarity (draWS)                   |        In Press           	|
-| Weights Similarity Coefficient (WSC)                  |        In Press           	|
-| Weights Similarity Coefficient 2 (WSC2)               |        In Press           	|
+| Drastic Weighted Similarity (draWS)                   |        [[59]](#c59)       	|
+| Weights Similarity Coefficient (WSC)                  |        [[60]](#c60)       	|
+| Weights Similarity Coefficient 2 (WSC2)               |        [[60]](#c60)       	|
 
 * Helpers
 
 | Helpers submodule     | Description                                                                                                      |
 |---------------------  |------------                                                                                                      |
 | `rankdata`            | Create ranking vector from the preference vector. Smaller preference values has higher positions in the ranking. |
 | `rrankdata`           | Alias to the `rankdata` which reverse the sorting order.                                                         |
@@ -148,15 +161,15 @@
 | Class/Function       | Description                                                                                        | Reference     |
 |----------------------|----------------------------------------------------------------------------------------------------|:-------------:|
 | `MethodExpert`       | Class which allows to evaluate CO in COMET using any MCDA method.                                  | [[56]](#c56)  |
 | `ManualExpert`       | Class which allows to evaluate CO in COMET manually by pairwise comparisons.                       | [[57]](#c57)  |
 | `FunctionExpert`     | Class which allows to evaluate CO in COMET using any expert function.                              | [[58]](#c58)  |
 | `CompromiseExpert`   | Class which allows to evaluate CO in COMET using compromise between several different methods.     | -             |
 | `TriadSupportExpert` | Class which allows to evaluate CO in COMET manually but with triads support.                       | In Press      |
-| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | In Press      |
+| `ESPExpert`          | Class which allows to identify MEJ using expert-defined Expected Solution Points.                  | [[61]](#c61)  |
 | `triads_consistency` | Function to which evaluates consistency of the MEJ matrix.                                         | [[55]](#c55)  |
 | `Submodel`           | Class mostly for internal use in StructuralCOMET class.                                            | [[54]](#c54)  |
 | `StructuralCOMET`    | Class which allows to split a decision problem into submodels to be evaluated by the COMET method. | [[54]](#c54)  |
 
 
 ___
 # Usage example
@@ -199,122 +212,130 @@
 4 0.0
 2 0.7829
 1 1.0
 ```
 ---
 # References
 
-<a name="c1">**[1]**</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
+<a name="c1">[1]</a> Hwang, C. L., & Yoon, K. (1981). Methods for multiple attribute decision making. In Multiple attribute decision making (pp. 58-191). Springer, Berlin, Heidelberg.
 
-<a name="c2">**[2]**</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
+<a name="c2">[2]</a> Duckstein, L., & Opricovic, S. (1980). Multiobjective optimization in river basin development. Water resources research, 16(1), 14-20.
 
-<a name="c3">**[3]**</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
+<a name="c3">[3]</a> Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007). Multi-attribute assessment of road design solutions by using the COPRAS method. The Baltic Journal of Road and Bridge Engineering, 2(4), 195-203.
 
-<a name="c4">**[4]**</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
+<a name="c4">[4]</a> Brans, J. P., Vincke, P., & Mareschal, B. (1986). How to select and how to rank projects: The PROMETHEE method. European journal of operational research, 24(2), 228-238.
 
-<a name="c5">**[5]**</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
+<a name="c5">[5]</a> Sałabun, W., Karczmarczyk, A., Wątróbski, J., & Jankowski, J. (2018, November). Handling data uncertainty in decision making with COMET. In 2018 IEEE Symposium Series on Computational Intelligence (SSCI) (pp. 1478-1484). IEEE.
 
-<a name="c6">**[6]**</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
+<a name="c6">[6]</a> Dezert, J., Tchamova, A., Han, D., & Tacnet, J. M. (2020, July). The spotis rank reversal free method for multi-criteria decision-making support. In 2020 IEEE 23rd International Conference on Information Fusion (FUSION) (pp. 1-8). IEEE.
 
-<a name="c7">**[7]**</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
+<a name="c7">[7]</a> Zavadskas, E. K., & Turskis, Z. (2010). A new additive ratio assessment (ARAS) method in multicriteria decision‐making. Technological and economic development of economy, 16(2), 159-172.
 
-<a name="c8">**[8]**</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
+<a name="c8">[8]</a> Stanujkic, D., Djordjevic, B., & Karabasevic, D. (2015). Selection of candidates in the process of recruitment and selection of personnel based on the SWARA and ARAS methods. Quaestus, (7), 53.
 
-<a name="c9">**[9]**</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
+<a name="c9">[9]</a> Yazdani, M., Zarate, P., Zavadskas, E. K., & Turskis, Z. (2019). A Combined Compromise Solution (CoCoSo) method for multi-criteria decision-making problems. Management Decision.
 
-<a name="c10">**[10]**</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
+<a name="c10">[10]</a> Badi, I., Shetwan, A. G., & Abdulshahed, A. M. (2017, September). Supplier selection using COmbinative Distance-based ASsessment (CODAS) method for multi-criteria decision-making. In Proceedings of The 1st International Conference on Management, Engineering and Environment (ICMNEE) (pp. 395-407).
 
-<a name="c11">**[11]**</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
+<a name="c11">[11]</a> Keshavarz Ghorabaee, M., Zavadskas, E. K., Olfat, L., & Turskis, Z. (2015). Multi-criteria inventory classification using a new method of evaluation based on distance from average solution (EDAS). Informatica, 26(3), 435-451.
 
-<a name="c12">**[12]**</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
+<a name="c12">[12]</a> Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D., & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model. Sustainable Operations and Computers, 1, 35-42.
 
-<a name="c13">**[13]**</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
+<a name="c13">[13]</a> Pamučar, D., & Ćirović, G. (2015). The selection of transport and handling resources in logistics centers using Multi-Attributive Border Approximation area Comparison (MABAC). Expert systems with applications, 42(6), 3016-3028.
 
-<a name="c14">**[14]**</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
+<a name="c14">[14]</a> Gigović, L., Pamučar, D., Bajić, Z., & Milićević, M. (2016). The combination of expert judgment and GIS-MAIRCA analysis for the selection of sites for ammunition depots. Sustainability, 8(4), 372.
 
-<a name="c15">**[15]**</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
+<a name="c15">[15]</a> Pamucar, D. S., Pejcic Tarle, S., & Parezanovic, T. (2018). New hybrid multi-criteria decision-making DEMATELMAIRCA model: sustainable selection of a location for the development of multimodal logistics centre. Economic research-Ekonomska istraživanja, 31(1), 1641-1665.
 
-<a name="c16">**[16]**</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
+<a name="c16">[16]</a> Aksoy, E. (2021). An Analysis on Turkey's Merger and Acquisition Activities: MAIRCA Method. Gümüşhane Üniversitesi Sosyal Bilimler Enstitüsü Elektronik Dergisi, 12(1), 1-11.
 
-<a name="c17">**[17]**</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
+<a name="c17">[17]</a> Stević, Ž., Pamučar, D., Puška, A., & Chatterjee, P. (2020). Sustainable supplier selection in healthcare industries using a new MCDM method: Measurement of alternatives and ranking according to COmpromise solution (MARCOS). Computers & Industrial Engineering, 140, 106231.
 
-<a name="c18">**[18]**</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
+<a name="c18">[18]</a> Ulutaş, A., Karabasevic, D., Popovic, G., Stanujkic, D., Nguyen, P. T., & Karaköy, Ç. (2020). Development of a novel integrated CCSD-ITARA-MARCOS decision-making approach for stackers selection in a logistics system. Mathematics, 8(10), 1672.
 
-<a name="c19">**[19]**</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
+<a name="c19">[19]</a> Parkan, C. (1994). Operational competitiveness ratings of production units. Managerial and Decision Economics, 15(3), 201-221.
 
-<a name="c20">**[20]**</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
+<a name="c20">[20]</a> Işık, A. T., & Adalı, E. A. (2016). A new integrated decision making approach based on SWARA and OCRA methods for the hotel selection problem. International Journal of Advanced Operations Management, 8(2), 140-151.
 
-<a name="c21">**[21]**</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
+<a name="c21">[21]</a> Brauers, W. K. (2003). Optimization methods for a stakeholder society: a revolution in economic thinking by multi-objective optimization (Vol. 73). Springer Science & Business Media.
 
-<a name="c22">**[22]**</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
+<a name="c22">[22]</a> Hussain, S. A. I., & Mandal, U. K. (2016). Entropy based MCDM approach for Selection of material. In National Level Conference on Engineering Problems and Application of Mathematics (pp. 1-6).
 
-<a name="c23">**[23]**</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
+<a name="c23">[23]</a> Sałabun, W., Wątróbski, J., & Shekhovtsov, A. (2020). Are mcda methods benchmarkable? a comparative study of topsis, vikor, copras, and promethee ii methods. Symmetry, 12(9), 1549.
 
-<a name="c24">**[24]**</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
+<a name="c24">[24]</a> Lotfi, F. H., & Fallahnejad, R. (2010). Imprecise Shannon’s entropy and multi attribute decision making. Entropy, 12(1), 53-62.
 
-<a name="c25">**[25]**</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
+<a name="c25">[25]</a> Li, X., Wang, K., Liu, L., Xin, J., Yang, H., & Gao, C. (2011). Application of the entropy weight and TOPSIS method in safety evaluation of coal mines. Procedia engineering, 26, 2085-2091.
 
-<a name="c26">**[26]**</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
+<a name="c26">[26]</a> Wang, Y. M., & Luo, Y. (2010). Integration of correlations with standard deviations for determining attribute weights in multiple attribute decision making. Mathematical and Computer Modelling, 51(1-2), 1-12.
 
-<a name="c27">**[27]**</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
+<a name="c27">[27]</a> Keshavarz-Ghorabaee, M., Amiri, M., Zavadskas, E. K., Turskis, Z., & Antucheviciene, J. (2021). Determination of Objective Weights Using a New Method Based on the Removal Effects of Criteria (MEREC). Symmetry, 13(4), 525.
 
-<a name="c28">**[28]**</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
+<a name="c28">[28]</a> Diakoulaki, D., Mavrotas, G., & Papayannakis, L. (1995). Determining objective weights in multiple criteria problems: The critic method. Computers & Operations Research, 22(7), 763-770.
 
-<a name="c29">**[29]**</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
+<a name="c29">[29]</a> Tuş, A., & Adalı, E. A. (2019). The new combination with CRITIC and WASPAS methods for the time and attendance software selection problem. Opsearch, 56(2), 528-538.
 
-<a name="c30">**[30]**</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
+<a name="c30">[30]</a> Zavadskas, E. K., & Podvezko, V. (2016). Integrated determination of objective criteria weights in MCDM. International Journal of Information Technology & Decision Making, 15(02), 267-283.
 
-<a name="c31">**[31]**</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
+<a name="c31">[31]</a> Shuai, D., Zongzhun, Z., Yongji, W., & Lei, L. (2012, May). A new angular method to determine the objective weights. In 2012 24th Chinese Control and Decision Conference (CCDC) (pp. 3889-3892). IEEE.
 
-<a name="c32">**[32]**</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
+<a name="c32">[32]</a> Li, G., & Chi, G. (2009, December). A new determining objective weights method-gini coefficient weight. In 2009 First International Conference on Information Science and Engineering (pp. 3726-3729). IEEE.
 
-<a name="c33">**[33]**</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
+<a name="c33">[33]</a> Rao, R. V., & Patel, B. K. (2010). A subjective and objective integrated multiple attribute decision making method for material selection. Materials & Design, 31(10), 4738-4747.
 
-<a name="c34">**[34]**</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
+<a name="c34">[34]</a> Brauers, W. K., & Zavadskas, E. K. (2006). The MOORA method and its application to privatization in a transition economy. Control and cybernetics, 35, 445-469.
 
-<a name="c35">**[35]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c35">[35]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c36">**[36]**</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
+<a name="c36">[36]</a> Gardziejczyk, W., & Zabicki, P. (2017). Normalization and variant assessment methods in selection of road alignment variants–case study. Journal of civil engineering and management, 23(4), 510-523.
 
-<a name="c37">**[37]**</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
+<a name="c37">[37]</a> Zavadskas, E. K., & Turskis, Z. (2008). A new logarithmic normalization method in games theory. Informatica, 19(2), 303-314.
 
-<a name="c38">**[38]**</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
+<a name="c38">[38]</a> Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342.
 
-<a name="c39">**[39]**</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
+<a name="c39">[39]</a> Peldschus, F., Vaigauskas, E., & Zavadskas, E. K. (1983). Technologische entscheidungen bei der berücksichtigung mehrerer Ziehle. Bauplanung Bautechnik, 37(4), 173-175.
 
-<a name="c40">**[40]**</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
+<a name="c40">[40]</a> Zeng, Q. L., Li, D. D., & Yang, Y. B. (2013). VIKOR method with enhanced accuracy for multiple criteria decision making in healthcare management. Journal of medical systems, 37(2), 1-9.
 
-<a name="c41">**[41]**</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
+<a name="c41">[41]</a> Binet, A., & Henri, V. (1898). La fatigue intellectuelle (Vol. 1). Schleicher frères.
 
-<a name="c42">**[42]**</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
+<a name="c42">[42]</a> Spearman, C. (1910). Correlation calculated from faulty data. British Journal of Psychology, 1904‐1920, 3(3), 271-295.
 
-<a name="c43">**[43]**</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
+<a name="c43">[43]</a> Pearson, K. (1895). VII. Note on regression and inheritance in the case of two parents. proceedings of the royal society of London, 58(347-352), 240-242.
 
-<a name="c44">**[44]**</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
+<a name="c44">[44]</a> Dancelli, L., Manisera, M., & Vezzoli, M. (2013). On two classes of Weighted Rank Correlation measures deriving from the Spearman’s ρ. In Statistical Models for Data Analysis (pp. 107-114). Springer, Heidelberg.
 
-<a name="c45">**[45]**</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
+<a name="c45">[45]</a> Sałabun, W., & Urbaniak, K. (2020, June). A new coefficient of rankings similarity in decision-making problems. In International Conference on Computational Science (pp. 632-645). Springer, Cham.
 
-<a name="c46">**[46]**</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
+<a name="c46">[46]</a> Kendall, M. G. (1938). A new measure of rank correlation. Biometrika, 30(1/2), 81-93.
 
-<a name="c47">**[47]**</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
+<a name="c47">[47]</a> Goodman, L. A., & Kruskal, W. H. (1979). Measures of association for cross classifications. Measures of association for cross classifications, 2-34.
 
-<a name="c48">**[48]**</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
+<a name="c48">[48]</a> Cables, E., Lamata, M. T., & Verdegay, J. L. (2016). RIM-reference ideal method in multicriteria decision making. Information Sciences, 337, 1-10.
 
-<a name="c49">**[49]**</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
+<a name="c49">[49]</a> Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
 
-<a name="c50">**[50]**</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
+<a name="c50">[50]</a> Wang, Z., Rangaiah, G. P., & Wang, X. (2021). Preference ranking on the basis of ideal-average distance method for multi-criteria decision-making. Industrial & Engineering Chemistry Research, 60(30), 11216-11230.
 
-<a name="c51">**[51]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c51">[51]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c52">**[52]**</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
+<a name="c52">[52]</a> Fishburn, P. C., Murphy, A. H., & Isaacs, H. H. (1968). Sensitivity of decisions to probability estimation errors: A reexamination. Operations Research, 16(2), 254-267.
 
-<a name="c53">**[53]**</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
+<a name="c53">[53]</a> Zavadskas, E. K., Turskis, Z., Antucheviciene, J., & Zakarevicius, A. (2012). Optimization of weighted aggregated sum product assessment. Elektronika ir elektrotechnika, 122(6), 3-6.
 
-<a name="c54">**[54]**</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
+<a name="c54">[54]</a> Shekhovtsov, A., Kołodziejczyk, J., & Sałabun, W. (2020). Fuzzy model identification using monolithic and structured approaches in decision problems with partially incomplete data. Symmetry, 12(9), 1541.
 
-<a name="c55">**[55]**</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
+<a name="c55">[55]</a> Sałabun, W., Shekhovtsov, A., & Kizielewicz, B. (2021, June). A new consistency coefficient in the multi-criteria decision analysis domain. In Computational Science–ICCS 2021: 21st International Conference, Krakow, Poland, June 16–18, 2021, Proceedings, Part I (pp. 715-727). Cham: Springer International Publishing.
 
-<a name="c56">**[56]**</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
+<a name="c56">[56]</a> Paradowski, B., Bączkiewicz, A., & Watrąbski, J. (2021). Towards proper consumer choices-MCDM based product selection. Procedia Computer Science, 192, 1347-1358.
 
-<a name="c57">**[57]**</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
+<a name="c57">[57]</a> Sałabun, W. (2015). The characteristic objects method: A new distance‐based approach to multicriteria decision‐making problems. Journal of Multi‐Criteria Decision Analysis, 22(1-2), 37-50.
 
-<a name="c58">**[58]**</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
+<a name="c58">[58]</a> Sałabun, W., & Piegat, A. (2017). Comparative analysis of MCDM methods for the assessment of mortality in patients with acute coronary syndrome. Artificial Intelligence Review, 48, 557-571.
+
+<a name="c59">[59]</a> Sałabun, W., & Shekhovtsov, A. (2023, September). An Innovative Drastic Metric for Ranking Similarity in Decision-Making Problems. In 2023 18th Conference on Computer Science and Intelligence Systems (FedCSIS) (pp. 731-738). IEEE.
+
+<a name="c60">[60]</a> Shekhovtsov, A. (2023). Evaluating the Performance of Subjective Weighting Methods for Multi-Criteria Decision-Making using a novel Weights Similarity Coefficient. Procedia Computer Science, 225, 4785-4794.
+
+<a name="c61">[61]</a> Shekhovtsov, A., Kizielewicz, B., & Sałabun, W. (2023). Advancing individual decision-making: An extension of the characteristic objects method using expected solution point. Information Sciences, 647, 119456.
+
+<a name="c62">[62]</a> Sotoudeh-Anvari, A. (2023). Root Assessment Method (RAM): a novel multi-criteria decision making method and its applications in sustainability challenges. Journal of Cleaner Production, 423, 138695.
```

### Comparing `pymcdm-1.2.0/pymcdm.egg-info/SOURCES.txt` & `pymcdm-1.2.1/pymcdm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 pymcdm/__init__.py
 pymcdm/correlations.py
 pymcdm/helpers.py
 pymcdm/normalizations.py
 pymcdm/weights.py
 pymcdm.egg-info/PKG-INFO
 pymcdm.egg-info/SOURCES.txt
@@ -25,48 +24,50 @@
 pymcdm/methods/mairca.py
 pymcdm/methods/marcos.py
 pymcdm/methods/mcda_method.py
 pymcdm/methods/moora.py
 pymcdm/methods/ocra.py
 pymcdm/methods/probid.py
 pymcdm/methods/promethee.py
+pymcdm/methods/ram.py
 pymcdm/methods/rim.py
 pymcdm/methods/spotis.py
 pymcdm/methods/topsis.py
 pymcdm/methods/vikor.py
 pymcdm/methods/waspas.py
 pymcdm/methods/wpm.py
 pymcdm/methods/wsm.py
 pymcdm/methods/comet_tools/__init__.py
 pymcdm/methods/comet_tools/compromise_expert.py
 pymcdm/methods/comet_tools/esp_expert.py
 pymcdm/methods/comet_tools/function_expert.py
+pymcdm/methods/comet_tools/local_weights.py
 pymcdm/methods/comet_tools/manual_expert.py
 pymcdm/methods/comet_tools/method_expert.py
 pymcdm/methods/comet_tools/structural_comet.py
 pymcdm/methods/comet_tools/triad_supported_expert.py
 pymcdm/methods/comet_tools/triads_consistency.py
 pymcdm/visuals/__init__.py
 pymcdm/visuals/boxplot.py
+pymcdm/visuals/comet_2d_esp_plot.py
 pymcdm/visuals/comet_2d_plot.py
+pymcdm/visuals/comet_3d_esp_plot.py
 pymcdm/visuals/comet_3d_plot.py
 pymcdm/visuals/comet_contourf.py
-pymcdm/visuals/comet_esp_plot.py
 pymcdm/visuals/comet_tfns.py
 pymcdm/visuals/correlation_heatmap.py
 pymcdm/visuals/correlation_plot.py
 pymcdm/visuals/mej_plot.py
 pymcdm/visuals/polar_plot.py
 pymcdm/visuals/polar_weights.py
 pymcdm/visuals/promethee_I_flows.py
 pymcdm/visuals/promethee_I_graph.py
 pymcdm/visuals/ranking_bar.py
 pymcdm/visuals/ranking_flows.py
 pymcdm/visuals/ranking_scatter.py
 pymcdm/visuals/rankings_flow_correlation.py
 pymcdm/visuals/violin.py
 pymcdm/visuals/weights_plot.py
-test/__init__.py
 test/test_comet_tools.py
 test/test_mcdm.py
 test/test_normalizations.py
 test/test_weights.py
```

### Comparing `pymcdm-1.2.0/test/test_comet_tools.py` & `pymcdm-1.2.1/test/test_comet_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) 2023 Andrii Shekhovtsov
 # Copyright (c) 2023 Bartłomiej Kizielewicz
 
 import unittest
 
 import numpy as np
-import pandas as pd
 
 from pymcdm.methods import TOPSIS, COMET
 from pymcdm.methods.comet_tools import (MethodExpert, Submodel,
                                         StructuralCOMET, triads_consistency)
 
 
 class TestStructuralCOMET(unittest.TestCase):
```

### Comparing `pymcdm-1.2.0/test/test_mcdm.py` & `pymcdm-1.2.1/test/test_mcdm.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,36 +128,69 @@
         output_method = [round(preference, 4) for preference in body(matrix)]
 
         self.assertListEqual(output, output_method)
 
 
 class TestCOPRAS(unittest.TestCase):
     """ Test output method with reference:
-    [1] Kundakcı, N., & Işık, A. (2016). Integration of MACBETH and COPRAS
-    methods to select air compressor for a textile company. Decision Science Letters, 5(3), 381-394.
+    [1] Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007).
+    Multi-attribute assessment of road design solutions by using the COPRAS
+    method. The Baltic journal of Road and Bridge engineering, 2(4), 195-203.
     """
 
     def test_output(self):
         body = methods.COPRAS()
-        matrix = np.array([[1543, 2000, 39000, 15, 13.76, 3.86, 5, 3, 5000],
-                           [1496, 3600, 43000, 14, 14, 2.5, 4, 4, 4000],
-                           [1584, 3100, 24500, 10, 13.1, 3.7, 2, 2, 3500],
-                           [1560, 2700, 36000, 12, 13.2, 3.2, 3, 3, 3500],
-                           [1572, 2500, 31500, 13, 13.3, 3.4, 3, 2, 3500],
-                           [1580, 2400, 20000, 12, 12.8, 3.9, 2, 2, 3000]])
 
-        types = np.array([-1, -1, -1, 1, 1, -1, 1, 1, 1])
-        weights = np.array([0.2027, 0.1757, 0.1622, 0.1351, 0.1081, 0.0946, 0.0676, 0.0405, 0.0135])
+        # The alternatives are in columns in the referenced paper,
+        # so we transpose the matrix to fit the pymcdm input format.
+        matrix = np.array([
+                [30, 20, 27, 18, 24, 16],
+                [12.487, 12.372, 11.096, 10.982, 11.017, 10.903],
+                [6.261, 5.961, 6.262, 5.962, 6.283, 5.983],
+                [10.880, 10.880, 9.920, 9.920, 9.980, 9.980],
+                [7.610, 7.460, 6.690, 6.540, 7.000, 6.850]
+            ]).T
+
+        types = np.array([1, -1, -1, -1, -1])
+        weights = np.array([0.5300, 0.1175, 0.1175, 0.1175, 0.1175])
 
-        output = [1, 0.9167, 0.8675, 0.9084, 0.9315, 0.9486]
+        output = [1.0, 0.797, 0.9078, 0.7243, 0.8537, 0.6898]
         output_method = [round(preference, 4) for preference in body(matrix, weights, types)]
 
         self.assertListEqual(output, output_method)
 
 
+class TestCOPRAS2(unittest.TestCase):
+    """ Test output method with reference:
+    [1] Zavadskas, E. K., Kaklauskas, A., Peldschus, F., & Turskis, Z. (2007).
+    Multi-attribute assessment of road design solutions by using the COPRAS
+    method. The Baltic journal of Road and Bridge engineering, 2(4), 195-203.
+    """
+
+    def test_output(self):
+        body = methods.COPRAS()
+
+        # The alternatives are in columns in the referenced paper,
+        # so we transpose the matrix to fit the pymcdm input format.
+        matrix = np.array([
+                [30, 20, 27, 18, 24, 16],
+                [12.487, 12.372, 11.096, 10.982, 11.017, 10.903],
+                [6.261, 5.961, 6.262, 5.962, 6.283, 5.983],
+                [10.880, 10.880, 9.920, 9.920, 9.980, 9.980],
+                [7.610, 7.460, 6.690, 6.540, 7.000, 6.850]
+            ]).T
+
+        types = np.array([1, -1, -1, -1, -1])
+        weights = np.array([0.075, 0.700, 0.075, 0.075, 0.075])
+
+        output = [1.0, 0.9585, 0.8984, 0.86, 0.8886, 0.8532]
+        output_method = [round(preference, 4) for preference in body(matrix, weights, types)]
+
+        self.assertListEqual(output, output_method)
+
 class TestEDAS(unittest.TestCase):
     """ Test output method with reference:
     [1] Yazdani, M., Torkayesh, A. E., Santibanez-Gonzalez, E. D.,
     & Otaghsara, S. K. (2020). Evaluation of renewable energy resources using integrated Shannon Entropy—EDAS model.
     Sustainable Operations and Computers, 1, 35-42.
     """
 
@@ -491,14 +524,49 @@
 
         output_method = list(np.round(output_method, 5))
         output = [0.58663, 0.75584, 0.37163, 0.46658, 0.74015]
 
         self.assertListEqual(output, output_method)
 
 
+class TestRAM(unittest.TestCase):
+    """ Test output method with reference:
+    [1] Sotoudeh-Anvari, A. (2023). Root Assessment Method (RAM): A novel
+    multi-criteria decision making method and its applications in
+    sustainability challenges. Journal of Cleaner Production, 138695.
+    """
+    def test_output(self):
+        matrix = np.array([
+            [0.068, 0.066, 0.150, 0.098, 0.156, 0.114, 0.098],
+            [0.078, 0.076, 0.108, 0.136, 0.082, 0.171, 0.105],
+            [0.157, 0.114, 0.128, 0.083, 0.108, 0.113, 0.131],
+            [0.106, 0.139, 0.058, 0.074, 0.132, 0.084, 0.120],
+            [0.103, 0.187, 0.125, 0.176, 0.074, 0.064, 0.057],
+            [0.105, 0.083, 0.150, 0.051, 0.134, 0.094, 0.113],
+            [0.137, 0.127, 0.056, 0.133, 0.122, 0.119, 0.114],
+            [0.100, 0.082, 0.086, 0.060, 0.062, 0.109, 0.093],
+            [0.053, 0.052, 0.043, 0.100, 0.050, 0.078, 0.063],
+            [0.094, 0.074, 0.097, 0.087, 0.080, 0.054, 0.106]
+        ])
+
+        weights = np.array([0.132, 0.135, 0.138, 0.162, 0.09, 0.223, 0.12])
+
+        types = np.array([1, -1, -1, 1, 1, 1, 1])
+
+        ram = methods.RAM()
+        output_method = ram(matrix, weights, types)
+
+        output_method = list(np.round(output_method, 4))
+
+        output = [1.4332, 1.4392, 1.4353, 1.4322, 1.4279,
+                  1.4301, 1.4394, 1.4308, 1.4294, 1.4288]
+        self.assertListEqual(output, output_method)
+
+
+
 class TestERVD(unittest.TestCase):
     """ Test output method with reference:
     [1] Shyur, H. J., Yin, L., Shih, H. S., & Cheng, C. B. (2015). A multiple criteria decision making method based on
     relative value distances. Foundations of Computing and Decision Sciences, 40(4), 299-315.
     """
     def test_output(self):
         matrix = np.array([
```

### Comparing `pymcdm-1.2.0/test/test_normalizations.py` & `pymcdm-1.2.1/test/test_normalizations.py`

 * *Files 25% similar despite different names*

```diff
@@ -176,13 +176,86 @@
                            [61, 55, 166],
                            [65, 49, 113],
                            [95, 56, 99],
                            [63, 43, 178],
                            [74, 59, 140]])
 
         types = np.array([-1, -1, 1])
-        output = [0.69473684, 0.94915254, 1.0, 0.64210526, 0.93220339, 0.25263158, 0.68421053, 0.83050847, 0.81052632,
-                  1.0, 0.94915254, 0.95789474, 0.66315789, 0.72881356, 0.12631579, 0.77894737, 1.0, 0.52631579]
+        output = [0.91803279, 0.69767442, 0.53370787,
+                  1.0, 0.72093023, 0.93258427,
+                  0.93442623, 0.86046512, 0.63483146,
+                  0.44262295, 0.69767442, 0.55617978,
+                  0.96721311, 1.0, 1.0,
+                  0.78688525, 0.62790698, 0.78651685]
 
         output_method = helpers.normalize_matrix(matrix, norm.zavadskas_turskis_normalization, types).reshape(-1)
         output_method = [round(val, 8) for val in output_method]
         self.assertListEqual(output, output_method)
+
+class TestZTNormalization2(unittest.TestCase):
+    """ [1] Jahan, A., & Edwards, K. L. (2015). A state-of-the-art survey on the influence of normalization techniques in ranking: Improving the materials selection process in engineering design. Materials & Design (1980-2015), 65, 335-342. """
+
+    def test_output(self):
+        matrix = np.array([[1, 6],
+                           [2, 7],
+                           [5, 10]])
+
+        types = np.array([1, 1])
+
+        output = [0.2, 0.6, 0.4, 0.7, 1.0, 1.0]
+
+        output_method = helpers.normalize_matrix(matrix, norm.zavadskas_turskis_normalization, types).reshape(-1)
+        output_method = [round(val, 1) for val in output_method]
+        self.assertListEqual(output, output_method)
+
+
+class TestNormalizeMatrix(unittest.TestCase):
+    """ Test output method without reference """
+    def setUp(self):
+        self.matrix = np.array([[10, 3],
+                                [4, 2],
+                                [6, 5]])
+        self.good_types = np.array([1, 1])
+        self.bad_types = np.array([1, 1, -1])
+        self.bad_types1 = np.array([0, 1])
+        self.one_method = norm.max_normalization
+        self.two_methods = [norm.max_normalization, norm.sum_normalization]
+        self.wrong_methods = [norm.max_normalization]
+
+    def test_correct_data1(self):
+        output = list(helpers.normalize_matrix(self.matrix,
+                                               self.one_method,
+                                               self.good_types).T.reshape(-1))
+        self.assertListEqual(output, [1, 0.4, 0.6, 0.6, 0.4, 1.0])
+
+    def test_correct_data2(self):
+        output = list(helpers.normalize_matrix(self.matrix,
+                                               self.two_methods,
+                                               self.good_types).T.reshape(-1))
+        self.assertListEqual(output, [1, 0.4, 0.6, 0.3, 0.2, 0.5])
+
+    def test_wrong_data1(self):
+        self.assertRaises(
+                ValueError,
+                helpers.normalize_matrix,
+                self.matrix,
+                self.wrong_methods,
+                self.good_types
+                )
+
+    def test_wrong_data2(self):
+        self.assertRaises(
+                ValueError,
+                helpers.normalize_matrix,
+                self.matrix,
+                self.one_method,
+                self.bad_types
+                )
+
+    def test_wrong_data3(self):
+        self.assertRaises(
+                ValueError,
+                helpers.normalize_matrix,
+                self.matrix,
+                self.one_method,
+                self.bad_types1
+                )
```

### Comparing `pymcdm-1.2.0/test/test_weights.py` & `pymcdm-1.2.1/test/test_weights.py`

 * *Files identical despite different names*

