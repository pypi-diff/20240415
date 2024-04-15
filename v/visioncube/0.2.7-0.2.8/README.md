# Comparing `tmp/visioncube-0.2.7.tar.gz` & `tmp/visioncube-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visioncube-0.2.7.tar", last modified: Fri Mar 29 06:22:12 2024, max compression
+gzip compressed data, was "visioncube-0.2.8.tar", last modified: Mon Apr 15 03:37:02 2024, max compression
```

## Comparing `visioncube-0.2.7.tar` & `visioncube-0.2.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.992645 visioncube-0.2.7/
--rw-rw-rw-   0        0        0      206 2024-03-29 06:22:11.991320 visioncube-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4857 2024-03-28 06:16:12.000000 visioncube-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-29 06:22:11.993649 visioncube-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      914 2024-03-28 04:03:14.000000 visioncube-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.600468 visioncube-0.2.7/test/
--rw-rw-rw-   0        0        0     2297 2024-02-20 09:55:40.000000 visioncube-0.2.7/test/test_cost_time.py
--rw-rw-rw-   0        0        0      645 2024-02-20 10:32:44.000000 visioncube-0.2.7/test/test_image_transforms.py
--rw-rw-rw-   0        0        0     2295 2024-03-13 03:16:30.000000 visioncube-0.2.7/test/test_multiple_times.py
--rw-rw-rw-   0        0        0     1280 2024-03-28 06:31:38.000000 visioncube-0.2.7/test/test_operator.py
--rw-rw-rw-   0        0        0     1533 2024-03-18 03:08:18.000000 visioncube-0.2.7/test/test_parameter.py
--rw-rw-rw-   0        0        0     2567 2024-03-19 08:44:21.000000 visioncube-0.2.7/test/test_single_time.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.664857 visioncube-0.2.7/visioncube/
--rw-rw-rw-   0        0        0       78 2024-03-13 03:33:01.000000 visioncube-0.2.7/visioncube/__init__.py
--rw-rw-rw-   0        0        0    22931 2024-03-26 07:15:27.000000 visioncube-0.2.7/visioncube/alignment.py
--rw-rw-rw-   0        0        0     3053 2024-02-29 10:31:42.000000 visioncube-0.2.7/visioncube/analysis.py
--rw-rw-rw-   0        0        0     3187 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/camera_calibration.py
--rw-rw-rw-   0        0        0     7559 2024-03-28 03:36:06.000000 visioncube-0.2.7/visioncube/common.py
--rw-rw-rw-   0        0        0     2010 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/docstring.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.764951 visioncube-0.2.7/visioncube/functional/
--rw-rw-rw-   0        0        0      410 2024-03-25 02:29:17.000000 visioncube-0.2.7/visioncube/functional/__init__.py
--rw-rw-rw-   0        0        0     1658 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/arithmetic.py
--rw-rw-rw-   0        0        0     5799 2024-03-11 03:05:00.000000 visioncube-0.2.7/visioncube/functional/basic.py
--rw-rw-rw-   0        0        0     3647 2024-03-22 02:46:33.000000 visioncube-0.2.7/visioncube/functional/code_reader.py
--rw-rw-rw-   0        0        0     1142 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/color.py
--rw-rw-rw-   0        0        0     1722 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/contour.py
--rw-rw-rw-   0        0        0     2739 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/draw.py
--rw-rw-rw-   0        0        0     1846 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/filters.py
--rw-rw-rw-   0        0        0     4308 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/geometric.py
--rw-rw-rw-   0        0        0     4003 2024-02-20 10:40:48.000000 visioncube-0.2.7/visioncube/functional/imageio.py
--rw-rw-rw-   0        0        0      763 2024-03-25 02:28:35.000000 visioncube-0.2.7/visioncube/functional/measure.py
--rw-rw-rw-   0        0        0     2935 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/misc.py
--rw-rw-rw-   0        0        0     2478 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/morphological.py
--rw-rw-rw-   0        0        0     2099 2024-03-13 02:59:34.000000 visioncube-0.2.7/visioncube/functional/ocr.py
--rw-rw-rw-   0        0        0      315 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/plotting.py
--rw-rw-rw-   0        0        0     1389 2024-03-25 08:51:07.000000 visioncube-0.2.7/visioncube/functional/polar_unwrap.py
--rw-rw-rw-   0        0        0     1438 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional/threshold.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.787455 visioncube-0.2.7/visioncube/functional_cuda/
--rw-rw-rw-   0        0        0      138 2024-03-12 10:46:21.000000 visioncube-0.2.7/visioncube/functional_cuda/__init__.py
--rw-rw-rw-   0        0        0     1811 2024-03-11 03:53:29.000000 visioncube-0.2.7/visioncube/functional_cuda/imageio.py
--rw-rw-rw-   0        0        0     2331 2024-03-13 03:00:12.000000 visioncube-0.2.7/visioncube/functional_cuda/ocr.py
--rw-rw-rw-   0        0        0     2999 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/functional_cuda/pcd_proc.py
--rw-rw-rw-   0        0        0     3287 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/hdr.py
--rw-rw-rw-   0        0        0     6165 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/light_segment.py
--rw-rw-rw-   0        0        0     1958 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/match_template.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.802918 visioncube-0.2.7/visioncube/measure/
--rw-rw-rw-   0        0        0      131 2024-03-22 03:31:26.000000 visioncube-0.2.7/visioncube/measure/__init__.py
--rw-rw-rw-   0        0        0     1376 2024-03-28 06:33:09.000000 visioncube-0.2.7/visioncube/measure/color.py
--rw-rw-rw-   0        0        0     8299 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/merge_mertens.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.884039 visioncube-0.2.7/visioncube/operators/
--rw-rw-rw-   0        0        0      377 2024-03-27 08:47:12.000000 visioncube-0.2.7/visioncube/operators/__init__.py
--rw-rw-rw-   0        0        0     4080 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/arithmetic.py
--rw-rw-rw-   0        0        0     9135 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/blur.py
--rw-rw-rw-   0        0        0     4513 2024-03-13 08:19:37.000000 visioncube-0.2.7/visioncube/operators/code_reader.py
--rw-rw-rw-   0        0        0    17763 2024-03-18 03:01:05.000000 visioncube-0.2.7/visioncube/operators/color.py
--rw-rw-rw-   0        0        0     4317 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/edge_detection.py
--rw-rw-rw-   0        0        0     1634 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/flip.py
--rw-rw-rw-   0        0        0     8934 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/geometric.py
--rw-rw-rw-   0        0        0    11281 2024-03-22 02:09:31.000000 visioncube-0.2.7/visioncube/operators/morphological.py
--rw-rw-rw-   0        0        0     2220 2024-03-25 09:00:23.000000 visioncube-0.2.7/visioncube/operators/polar_unwrap.py
--rw-rw-rw-   0        0        0     3625 2024-03-27 09:05:11.000000 visioncube-0.2.7/visioncube/operators/sample.py
--rw-rw-rw-   0        0        0     9128 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators/size.py
--rw-rw-rw-   0        0        0     4454 2024-03-27 08:52:58.000000 visioncube-0.2.7/visioncube/operators/threshold.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.963205 visioncube-0.2.7/visioncube/operators_cuda/
--rw-rw-rw-   0        0        0      321 2024-03-27 08:24:00.000000 visioncube-0.2.7/visioncube/operators_cuda/__init__.py
--rw-rw-rw-   0        0        0     6394 2024-03-14 08:28:38.000000 visioncube-0.2.7/visioncube/operators_cuda/arithmetic.py
--rw-rw-rw-   0        0        0     1449 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators_cuda/bbs.py
--rw-rw-rw-   0        0        0    13187 2024-03-18 07:34:59.000000 visioncube-0.2.7/visioncube/operators_cuda/blur.py
--rw-rw-rw-   0        0        0    19932 2024-03-25 09:08:27.000000 visioncube-0.2.7/visioncube/operators_cuda/color.py
--rw-rw-rw-   0        0        0     4867 2024-03-13 09:19:31.000000 visioncube-0.2.7/visioncube/operators_cuda/edge_detection.py
--rw-rw-rw-   0        0        0     3730 2024-03-13 09:19:37.000000 visioncube-0.2.7/visioncube/operators_cuda/flip.py
--rw-rw-rw-   0        0        0    19599 2024-03-13 09:19:44.000000 visioncube-0.2.7/visioncube/operators_cuda/geometric.py
--rw-rw-rw-   0        0        0     2466 2024-02-20 10:35:30.000000 visioncube-0.2.7/visioncube/operators_cuda/kmeans.py
--rw-rw-rw-   0        0        0     5933 2024-03-22 02:07:58.000000 visioncube-0.2.7/visioncube/operators_cuda/morphological.py
--rw-rw-rw-   0        0        0     1594 2024-03-27 09:27:24.000000 visioncube-0.2.7/visioncube/operators_cuda/sample.py
--rw-rw-rw-   0        0        0    17587 2024-03-13 09:20:53.000000 visioncube-0.2.7/visioncube/operators_cuda/size.py
--rw-rw-rw-   0        0        0     5525 2024-03-28 06:05:03.000000 visioncube-0.2.7/visioncube/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.983323 visioncube-0.2.7/visioncube/recognition/
--rw-rw-rw-   0        0        0      142 2024-03-28 03:30:01.000000 visioncube-0.2.7/visioncube/recognition/__init__.py
--rw-rw-rw-   0        0        0     4538 2024-03-26 03:00:34.000000 visioncube-0.2.7/visioncube/recognition/code_reader.py
--rw-rw-rw-   0        0        0     6829 2024-03-28 05:53:08.000000 visioncube-0.2.7/visioncube/recognition/ocr.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:11.697375 visioncube-0.2.7/visioncube.egg-info/
--rw-rw-rw-   0        0        0      206 2024-03-29 06:22:09.000000 visioncube-0.2.7/visioncube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2408 2024-03-29 06:22:11.000000 visioncube-0.2.7/visioncube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 06:22:09.000000 visioncube-0.2.7/visioncube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-11 03:08:40.000000 visioncube-0.2.7/visioncube.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2024-03-29 06:22:10.000000 visioncube-0.2.7/visioncube.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-29 06:22:10.000000 visioncube-0.2.7/visioncube.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.095902 visioncube-0.2.8/
+-rw-rw-rw-   0        0        0      206 2024-04-15 03:37:02.094906 visioncube-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4857 2024-03-28 06:16:12.000000 visioncube-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:37:02.095902 visioncube-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      914 2024-04-15 03:36:03.000000 visioncube-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:01.935999 visioncube-0.2.8/test/
+-rw-rw-rw-   0        0        0     2297 2024-02-20 09:55:40.000000 visioncube-0.2.8/test/test_cost_time.py
+-rw-rw-rw-   0        0        0      645 2024-02-20 10:32:44.000000 visioncube-0.2.8/test/test_image_transforms.py
+-rw-rw-rw-   0        0        0     2295 2024-03-13 03:16:30.000000 visioncube-0.2.8/test/test_multiple_times.py
+-rw-rw-rw-   0        0        0     1273 2024-04-02 03:45:40.000000 visioncube-0.2.8/test/test_operator.py
+-rw-rw-rw-   0        0        0     1533 2024-03-18 03:08:18.000000 visioncube-0.2.8/test/test_parameter.py
+-rw-rw-rw-   0        0        0     2501 2024-04-02 03:48:28.000000 visioncube-0.2.8/test/test_single_time.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:01.958544 visioncube-0.2.8/visioncube/
+-rw-rw-rw-   0        0        0       78 2024-03-13 03:33:01.000000 visioncube-0.2.8/visioncube/__init__.py
+-rw-rw-rw-   0        0        0    22931 2024-03-26 07:15:27.000000 visioncube-0.2.8/visioncube/alignment.py
+-rw-rw-rw-   0        0        0     3053 2024-02-29 10:31:42.000000 visioncube-0.2.8/visioncube/analysis.py
+-rw-rw-rw-   0        0        0     3187 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/camera_calibration.py
+-rw-rw-rw-   0        0        0     7662 2024-04-15 03:34:53.000000 visioncube-0.2.8/visioncube/common.py
+-rw-rw-rw-   0        0        0     2010 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/docstring.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.011353 visioncube-0.2.8/visioncube/functional/
+-rw-rw-rw-   0        0        0      410 2024-03-25 02:29:17.000000 visioncube-0.2.8/visioncube/functional/__init__.py
+-rw-rw-rw-   0        0        0     1658 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/arithmetic.py
+-rw-rw-rw-   0        0        0     5799 2024-03-11 03:05:00.000000 visioncube-0.2.8/visioncube/functional/basic.py
+-rw-rw-rw-   0        0        0     3647 2024-03-22 02:46:33.000000 visioncube-0.2.8/visioncube/functional/code_reader.py
+-rw-rw-rw-   0        0        0     1142 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/color.py
+-rw-rw-rw-   0        0        0     1722 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/contour.py
+-rw-rw-rw-   0        0        0     2739 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/draw.py
+-rw-rw-rw-   0        0        0     1846 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/filters.py
+-rw-rw-rw-   0        0        0     4308 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/geometric.py
+-rw-rw-rw-   0        0        0     4003 2024-02-20 10:40:48.000000 visioncube-0.2.8/visioncube/functional/imageio.py
+-rw-rw-rw-   0        0        0      763 2024-03-25 02:28:35.000000 visioncube-0.2.8/visioncube/functional/measure.py
+-rw-rw-rw-   0        0        0     2935 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/misc.py
+-rw-rw-rw-   0        0        0     2478 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/morphological.py
+-rw-rw-rw-   0        0        0     2099 2024-03-13 02:59:34.000000 visioncube-0.2.8/visioncube/functional/ocr.py
+-rw-rw-rw-   0        0        0      315 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/plotting.py
+-rw-rw-rw-   0        0        0     1389 2024-03-25 08:51:07.000000 visioncube-0.2.8/visioncube/functional/polar_unwrap.py
+-rw-rw-rw-   0        0        0     1438 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional/threshold.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.022327 visioncube-0.2.8/visioncube/functional_cuda/
+-rw-rw-rw-   0        0        0      138 2024-03-12 10:46:21.000000 visioncube-0.2.8/visioncube/functional_cuda/__init__.py
+-rw-rw-rw-   0        0        0     1811 2024-03-11 03:53:29.000000 visioncube-0.2.8/visioncube/functional_cuda/imageio.py
+-rw-rw-rw-   0        0        0     2331 2024-03-13 03:00:12.000000 visioncube-0.2.8/visioncube/functional_cuda/ocr.py
+-rw-rw-rw-   0        0        0     2999 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/functional_cuda/pcd_proc.py
+-rw-rw-rw-   0        0        0     3287 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/hdr.py
+-rw-rw-rw-   0        0        0     6165 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/light_segment.py
+-rw-rw-rw-   0        0        0     1958 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/match_template.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.027224 visioncube-0.2.8/visioncube/measure/
+-rw-rw-rw-   0        0        0      131 2024-03-22 03:31:26.000000 visioncube-0.2.8/visioncube/measure/__init__.py
+-rw-rw-rw-   0        0        0     1376 2024-03-28 06:33:09.000000 visioncube-0.2.8/visioncube/measure/color.py
+-rw-rw-rw-   0        0        0     8299 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/merge_mertens.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.055501 visioncube-0.2.8/visioncube/operators/
+-rw-rw-rw-   0        0        0      377 2024-03-27 08:47:12.000000 visioncube-0.2.8/visioncube/operators/__init__.py
+-rw-rw-rw-   0        0        0     4080 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/arithmetic.py
+-rw-rw-rw-   0        0        0     9135 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/blur.py
+-rw-rw-rw-   0        0        0     4513 2024-03-13 08:19:37.000000 visioncube-0.2.8/visioncube/operators/code_reader.py
+-rw-rw-rw-   0        0        0    17763 2024-04-02 03:53:08.000000 visioncube-0.2.8/visioncube/operators/color.py
+-rw-rw-rw-   0        0        0     4317 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/edge_detection.py
+-rw-rw-rw-   0        0        0     1634 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/flip.py
+-rw-rw-rw-   0        0        0     8934 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/geometric.py
+-rw-rw-rw-   0        0        0    11281 2024-03-22 02:09:31.000000 visioncube-0.2.8/visioncube/operators/morphological.py
+-rw-rw-rw-   0        0        0     2220 2024-03-25 09:00:23.000000 visioncube-0.2.8/visioncube/operators/polar_unwrap.py
+-rw-rw-rw-   0        0        0     3625 2024-03-27 09:05:11.000000 visioncube-0.2.8/visioncube/operators/sample.py
+-rw-rw-rw-   0        0        0     9128 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators/size.py
+-rw-rw-rw-   0        0        0     4454 2024-03-27 08:52:58.000000 visioncube-0.2.8/visioncube/operators/threshold.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.083396 visioncube-0.2.8/visioncube/operators_cuda/
+-rw-rw-rw-   0        0        0      321 2024-03-27 08:24:00.000000 visioncube-0.2.8/visioncube/operators_cuda/__init__.py
+-rw-rw-rw-   0        0        0     6394 2024-03-14 08:28:38.000000 visioncube-0.2.8/visioncube/operators_cuda/arithmetic.py
+-rw-rw-rw-   0        0        0     1449 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators_cuda/bbs.py
+-rw-rw-rw-   0        0        0    13187 2024-03-18 07:34:59.000000 visioncube-0.2.8/visioncube/operators_cuda/blur.py
+-rw-rw-rw-   0        0        0    19932 2024-03-25 09:08:27.000000 visioncube-0.2.8/visioncube/operators_cuda/color.py
+-rw-rw-rw-   0        0        0     4867 2024-03-13 09:19:31.000000 visioncube-0.2.8/visioncube/operators_cuda/edge_detection.py
+-rw-rw-rw-   0        0        0     3730 2024-03-13 09:19:37.000000 visioncube-0.2.8/visioncube/operators_cuda/flip.py
+-rw-rw-rw-   0        0        0    19599 2024-03-13 09:19:44.000000 visioncube-0.2.8/visioncube/operators_cuda/geometric.py
+-rw-rw-rw-   0        0        0     2466 2024-02-20 10:35:30.000000 visioncube-0.2.8/visioncube/operators_cuda/kmeans.py
+-rw-rw-rw-   0        0        0     5933 2024-03-22 02:07:58.000000 visioncube-0.2.8/visioncube/operators_cuda/morphological.py
+-rw-rw-rw-   0        0        0     1594 2024-03-27 09:27:24.000000 visioncube-0.2.8/visioncube/operators_cuda/sample.py
+-rw-rw-rw-   0        0        0    17587 2024-03-13 09:20:53.000000 visioncube-0.2.8/visioncube/operators_cuda/size.py
+-rw-rw-rw-   0        0        0     5525 2024-03-28 06:05:03.000000 visioncube-0.2.8/visioncube/pipeline.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:02.092906 visioncube-0.2.8/visioncube/recognition/
+-rw-rw-rw-   0        0        0      142 2024-03-28 03:30:01.000000 visioncube-0.2.8/visioncube/recognition/__init__.py
+-rw-rw-rw-   0        0        0     4538 2024-03-26 03:00:34.000000 visioncube-0.2.8/visioncube/recognition/code_reader.py
+-rw-rw-rw-   0        0        0     6829 2024-03-28 05:53:08.000000 visioncube-0.2.8/visioncube/recognition/ocr.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:37:01.971066 visioncube-0.2.8/visioncube.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2408 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 03:37:01.000000 visioncube-0.2.8/visioncube.egg-info/top_level.txt
```

### Comparing `visioncube-0.2.7/README.md` & `visioncube-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/setup.py` & `visioncube-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'visioncube.functional',
         'visioncube.functional_cuda',
         'visioncube.operators',
         'visioncube.operators_cuda',
         'visioncube.recognition',
         'visioncube.measure',
     ],
-    version='0.2.7',
+    version='0.2.8',
     description='Image Processing Tool',
     author='yanaenen, xi',
     install_requires=[
         'numpy',
         'imgaug',
         'opencv-python',
         'opencv-contrib-python',
```

### Comparing `visioncube-0.2.7/test/test_cost_time.py` & `visioncube-0.2.8/test/test_cost_time.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/test/test_image_transforms.py` & `visioncube-0.2.8/test/test_image_transforms.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/test/test_multiple_times.py` & `visioncube-0.2.8/test/test_multiple_times.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/test/test_operator.py` & `visioncube-0.2.8/test/test_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import cv2
 import numpy as np
 from visioncube.measure import ColorMeasurement
 
 from visioncube import TransformPipeline
 from visioncube.recognition import CnOCR
 
-img_path = 'data/识别/ocr_test.jpg'
+img_path = 'data/test-150.jpg'
 img = cv2.imdecode(np.fromfile(img_path, dtype=np.uint8), cv2.IMREAD_COLOR)
 img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
 """算子如何用"""
 # ocr
 # 方式1
 output = CnOCR(use_gpu=False)({"image": img})['ocr']
```

### Comparing `visioncube-0.2.7/test/test_parameter.py` & `visioncube-0.2.8/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/test/test_single_time.py` & `visioncube-0.2.8/test/test_single_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,32 @@
     # image = cv2.imread(img_path)
     image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
     # image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     return image
 
 
 def pipeline_test(img_path=None):
-    device = 'cuda'
+    device = 'cpu'
 
-    img_path = 'D:\\BaiduNetdiskDownload\\数据\\CF中间盘\\区域2_v3\\OK3\\1\\1.bmp'
-    # img_path = 'data/anomaly.jpg'
+    # img_path = 'data'
+    img_path = 'data/anomaly.jpg'
     image = read_image(img_path)
     doc = {'image': image}
 
     pipeline = TransformPipeline('test/config.yml', training=True, device=device)
     # pipeline = TransformPipeline([
     #     {'name': 'Add', 'tag': 'train', 'kwargs': {'value': 100}}
     # ], training=True, device=device)
 
     output = pipeline(doc)
     # print(output['ocr'])
     image1 = output['image']
     # cv2.imwrite('1.jpg', cv2.cvtColor(image1, cv2.COLOR_RGB2BGR))
 
-    plt.imshow(image1, cmap='gray')
+    plt.imshow(image1) #, cmap='gray')
     plt.show()
 
 
 def operator_functional_test():
     """单图单算子随机测试"""
 
     device = 'cpu'
```

### Comparing `visioncube-0.2.7/visioncube/alignment.py` & `visioncube-0.2.8/visioncube/alignment.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/analysis.py` & `visioncube-0.2.8/visioncube/analysis.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/camera_calibration.py` & `visioncube-0.2.8/visioncube/camera_calibration.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/common.py` & `visioncube-0.2.8/visioncube/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,17 @@
 
         if self.label is not None:
             self.doc[DEFAULT_LABEL_FIELD] = self.label
 
         if self.qr_code is not None:
             self.doc[DEFAULT_QR_CODE_FIELD] = self.qr_code
 
+        if self.bar_code is not None:
+            self.doc[DEFAULT_BAR_CODE_FIELD] = self.bar_code
+
         if self.data_matrix_code is not None:
             self.doc[DEFAULT_DATA_MATRIX_CODE_FIELD] = self.data_matrix_code
 
         if self.color_measure is not None:
             self.doc[DEFAULT_COLOR_MEASURE_FIELD] = self.color_measure
 
         return self.doc
```

### Comparing `visioncube-0.2.7/visioncube/docstring.py` & `visioncube-0.2.8/visioncube/docstring.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/arithmetic.py` & `visioncube-0.2.8/visioncube/functional/arithmetic.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/basic.py` & `visioncube-0.2.8/visioncube/functional/basic.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/code_reader.py` & `visioncube-0.2.8/visioncube/functional/code_reader.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/color.py` & `visioncube-0.2.8/visioncube/functional/color.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/contour.py` & `visioncube-0.2.8/visioncube/functional/contour.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/draw.py` & `visioncube-0.2.8/visioncube/functional/draw.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/filters.py` & `visioncube-0.2.8/visioncube/functional/filters.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/geometric.py` & `visioncube-0.2.8/visioncube/functional/geometric.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/imageio.py` & `visioncube-0.2.8/visioncube/functional/imageio.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/measure.py` & `visioncube-0.2.8/visioncube/functional/measure.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/misc.py` & `visioncube-0.2.8/visioncube/functional/misc.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/morphological.py` & `visioncube-0.2.8/visioncube/functional/morphological.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/ocr.py` & `visioncube-0.2.8/visioncube/functional/ocr.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/polar_unwrap.py` & `visioncube-0.2.8/visioncube/functional/polar_unwrap.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional/threshold.py` & `visioncube-0.2.8/visioncube/functional/threshold.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional_cuda/imageio.py` & `visioncube-0.2.8/visioncube/functional_cuda/imageio.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional_cuda/ocr.py` & `visioncube-0.2.8/visioncube/functional_cuda/ocr.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/functional_cuda/pcd_proc.py` & `visioncube-0.2.8/visioncube/functional_cuda/pcd_proc.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/hdr.py` & `visioncube-0.2.8/visioncube/hdr.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/light_segment.py` & `visioncube-0.2.8/visioncube/light_segment.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/match_template.py` & `visioncube-0.2.8/visioncube/match_template.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/measure/color.py` & `visioncube-0.2.8/visioncube/measure/color.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/merge_mertens.py` & `visioncube-0.2.8/visioncube/merge_mertens.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/arithmetic.py` & `visioncube-0.2.8/visioncube/operators/arithmetic.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/blur.py` & `visioncube-0.2.8/visioncube/operators/blur.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/code_reader.py` & `visioncube-0.2.8/visioncube/operators/code_reader.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/color.py` & `visioncube-0.2.8/visioncube/operators/color.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/edge_detection.py` & `visioncube-0.2.8/visioncube/operators/edge_detection.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/flip.py` & `visioncube-0.2.8/visioncube/operators/flip.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/geometric.py` & `visioncube-0.2.8/visioncube/operators/geometric.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/morphological.py` & `visioncube-0.2.8/visioncube/operators/morphological.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/polar_unwrap.py` & `visioncube-0.2.8/visioncube/operators/polar_unwrap.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/sample.py` & `visioncube-0.2.8/visioncube/operators/sample.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/size.py` & `visioncube-0.2.8/visioncube/operators/size.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators/threshold.py` & `visioncube-0.2.8/visioncube/operators/threshold.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/arithmetic.py` & `visioncube-0.2.8/visioncube/operators_cuda/arithmetic.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/bbs.py` & `visioncube-0.2.8/visioncube/operators_cuda/bbs.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/blur.py` & `visioncube-0.2.8/visioncube/operators_cuda/blur.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/color.py` & `visioncube-0.2.8/visioncube/operators_cuda/color.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/edge_detection.py` & `visioncube-0.2.8/visioncube/operators_cuda/edge_detection.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/flip.py` & `visioncube-0.2.8/visioncube/operators_cuda/flip.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/geometric.py` & `visioncube-0.2.8/visioncube/operators_cuda/geometric.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/kmeans.py` & `visioncube-0.2.8/visioncube/operators_cuda/kmeans.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/morphological.py` & `visioncube-0.2.8/visioncube/operators_cuda/morphological.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/sample.py` & `visioncube-0.2.8/visioncube/operators_cuda/sample.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/operators_cuda/size.py` & `visioncube-0.2.8/visioncube/operators_cuda/size.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/pipeline.py` & `visioncube-0.2.8/visioncube/pipeline.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/recognition/code_reader.py` & `visioncube-0.2.8/visioncube/recognition/code_reader.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube/recognition/ocr.py` & `visioncube-0.2.8/visioncube/recognition/ocr.py`

 * *Files identical despite different names*

### Comparing `visioncube-0.2.7/visioncube.egg-info/SOURCES.txt` & `visioncube-0.2.8/visioncube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

