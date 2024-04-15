# Comparing `tmp/damo-2.2.9.tar.gz` & `tmp/damo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.2.9.tar", last modified: Mon Apr  8 22:34:51 2024, max compression
+gzip compressed data, was "damo-2.3.0.tar", last modified: Mon Apr 15 16:42:20 2024, max compression
```

## Comparing `damo-2.2.9.tar` & `damo-2.3.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.056609 damo-2.2.9/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-08 22:34:51.052609 damo-2.2.9/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-08 22:34:47.000000 damo-2.2.9/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.2.9/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-08 22:34:51.056609 damo-2.2.9/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.2.9/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.040609 damo-2.2.9/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.052609 damo-2.2.9/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:47.000000 damo-2.2.9/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.2.9/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.2.9/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.2.9/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    42317 2024-04-06 17:58:11.000000 damo-2.2.9/src/damo/_damo_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.2.9/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    21260 2024-03-09 20:09:49.000000 damo-2.2.9/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.2.9/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.2.9/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.2.9/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.2.9/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.2.9/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.2.9/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.2.9/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.2.9/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.2.9/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.2.9/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.2.9/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.2.9/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5020 2024-04-06 19:34:24.000000 damo-2.2.9/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.2.9/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.2.9/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1425 2024-03-02 20:08:09.000000 damo-2.2.9/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.2.9/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.2.9/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.2.9/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.2.9/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.2.9/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.2.9/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.2.9/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.2.9/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-02-17 20:35:23.000000 damo-2.2.9/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.2.9/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-08 22:33:49.000000 damo-2.2.9/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5437 2024-04-06 16:22:15.000000 damo-2.2.9/src/damo/damo_wss.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.2.9/src/damo/python_access_perf.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.052609 damo-2.2.9/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1274 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-15 16:42:20.516967 damo-2.3.0/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-15 16:42:20.516967 damo-2.3.0/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-15 16:42:16.000000 damo-2.3.0/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.0/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-15 16:42:20.516967 damo-2.3.0/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.3.0/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-15 16:42:20.500967 damo-2.3.0/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-15 16:42:20.512966 damo-2.3.0/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-15 16:42:16.000000 damo-2.3.0/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.3.0/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.3.0/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.3.0/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.3.0/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.3.0/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.3.0/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.3.0/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.3.0/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    43070 2024-04-14 16:50:45.000000 damo-2.3.0/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.3.0/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.3.0/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22289 2024-04-14 15:18:46.000000 damo-2.3.0/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.3.0/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.3.0/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.3.0/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.3.0/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.3.0/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.3.0/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.3.0/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.3.0/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.3.0/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.3.0/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.3.0/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.3.0/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5116 2024-04-14 16:27:26.000000 damo-2.3.0/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.3.0/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.3.0/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-04-14 17:07:12.000000 damo-2.3.0/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4284 2024-04-14 17:19:16.000000 damo-2.3.0/src/damo/damo_report_footprint.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.3.0/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.3.0/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.3.0/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.3.0/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.3.0/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.3.0/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.3.0/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.3.0/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-04-14 15:16:45.000000 damo-2.3.0/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.3.0/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-15 16:32:33.000000 damo-2.3.0/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5437 2024-04-14 16:31:45.000000 damo-2.3.0/src/damo/damo_wss.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.3.0/src/damo/python_access_perf.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-15 16:42:20.516967 damo-2.3.0/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-15 16:42:20.000000 damo-2.3.0/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1308 2024-04-15 16:42:20.000000 damo-2.3.0/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-15 16:42:20.000000 damo-2.3.0/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-15 16:42:20.000000 damo-2.3.0/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-15 16:42:20.000000 damo-2.3.0/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.2.9/PKG-INFO` & `damo-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.9
+Version: 2.3.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.9/README.md` & `damo-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,29 +75,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.9/setup.py` & `damo-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_ascii_color.py` & `damo-2.3.0/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_deprecated.py` & `damo-2.3.0/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_deprecation_notice.py` & `damo-2.3.0/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_dist.py` & `damo-2.3.0/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_fmt_str.py` & `damo-2.3.0/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_fs.py` & `damo-2.3.0/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_paddr_layout.py` & `damo-2.3.0/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_print.py` & `damo-2.3.0/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damo_records.py` & `damo-2.3.0/src/damo/_damo_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,44 +524,72 @@
     resident = None
     shared = None
     trs = None
     lrs = None
     drs = None
     dt = None
 
-    def __init__(self, pid):
+    def __init__(self, pid=None):
+        if pid is None:
+            return
+
         with open('/proc/%s/statm' % pid, 'r') as f:
             fields = [int(x) for x in f.read().split()]
         self.size = fields[0]
         self.resident = fields[1]
         self.shared = fields[2]
         self.trs = fields[3]
         self.lrs = fields[4]
         self.drs = fields[5]
         self.dt = fields[6]
 
     def to_kvpairs(self):
         return self.__dict__
 
+    @classmethod
+    def from_kvpairs(cls, kvpairs):
+        self = cls()
+        self.size = kvpairs['size']
+        self.resident = kvpairs['resident']
+        self.shared = kvpairs['shared']
+        self.trs = kvpairs['trs']
+        self.lrs = kvpairs['lrs']
+        self.drs = kvpairs['drs']
+        self.dt = kvpairs['dt']
+        return self
+
 class MemFootprintsSnapshot:
     time = None
     footprints = None
 
-    def __init__(self, pids):
+    def __init__(self, pids=None):
+        if pids is None:
+            return
+
         self.time = time.time()
         self.footprints = {}
         for pid in pids:
             self.footprints[pid] = MemFootprint(pid)
 
     def to_kvpairs(self):
         footprints = []
         for pid, fp in self.footprints.items():
             footprints.append({'pid': pid, 'footprint': fp.to_kvpairs()})
         return {'time': self.time, 'footprints': footprints}
 
+    @classmethod
+    def from_kvpairs(cls, kvpairs):
+        self = cls()
+        self.time = kvpairs['time']
+        self.footprints = {}
+        for fp in kvpairs['footprints']:
+            pid, footprint = fp['pid'], fp['footprint']
+            self.footprints[pid] = MemFootprint.from_kvpairs(footprint)
+        return self
+
 def record_mem_footprint(kdamonds, snapshots):
     pids = []
     for kdamond in kdamonds:
         for ctx in kdamond.contexts:
             for target in ctx.targets:
                 if target.pid is None:
                     continue
@@ -569,14 +597,19 @@
     snapshots.append(MemFootprintsSnapshot(pids))
 
 def save_mem_footprint(snapshots, filepath, file_permission):
     with open(filepath, 'w') as f:
         json.dump([s.to_kvpairs() for s in snapshots], f, indent=4)
     os.chmod(filepath, file_permission)
 
+def load_mem_footprint(filepath):
+    with open(filepath, 'r') as f:
+        kvpairs = json.load(f)
+    return [MemFootprintsSnapshot.from_kvpairs(x) for x in kvpairs]
+
 # record-polling
 
 def pid_running(pid):
     '''pid should be string'''
     try:
         subprocess.check_output(['ps', '--pid', pid])
         return True
@@ -632,68 +665,70 @@
         if err != None:
             # this might be not a problem; some of processes might
             # finished meanwhile
             return False
     return True
 
 def poll_target_pids(handle):
+    if (not handle.poll_add_child_tasks and
+        handle.mem_footprint_snapshots is None):
+        return False
     rc = __poll_target_pids(handle)
     if rc is True and handle.mem_footprint_snapshots is not None:
         record_mem_footprint(handle.kdamonds, handle.mem_footprint_snapshots)
     return rc
 
 # for recording
 
 class RecordingHandle:
+    # for tracepoint recording
+    tracepoint = None
     file_path = None
     file_format = None
     file_permission = None
     monitoring_intervals = None
     perf_pipe = None
+
+    # for CPU clock event recording
+    do_profile = None
     perf_profile_pipe = None
-    # for polling
+
+    # for adding child tasks and memory footprint recording
     kdamonds = None
     poll_add_child_tasks = None
     mem_footprint_snapshots = None
 
-    def __init__(self, file_path, file_format, file_permission,
-                 monitoring_intervals, perf_pipe, perf_profile_pipe,
+    def __init__(self, tracepoint, file_path, file_format, file_permission,
+                 monitoring_intervals,
+                 do_profile,
                  kdamonds, poll_add_child_tasks, poll_add_mem_footprint):
+        self.tracepoint = tracepoint
         self.file_path = file_path
         self.file_format = file_format
         self.file_permission = file_permission
         self.monitoring_intervals = monitoring_intervals
-        self.perf_pipe = perf_pipe
-        self.perf_profile_pipe = perf_profile_pipe
+
+        self.do_profile = do_profile
+
         self.kdamonds = kdamonds
         self.poll_add_child_tasks = poll_add_child_tasks
         if poll_add_mem_footprint is True:
             self.mem_footprint_snapshots = []
 
-'''
-Start recording DAMON's monitoring results and/or profile.
-
-Returns a handle object.  The handle should be passed to finish_recording()
-later.
-'''
-def start_recording(tracepoint, file_path, file_format, file_permission,
-                    monitoring_intervals, profile, profile_target_pid,
-                    kdamonds, poll_add_child_tasks, poll_add_mem_footprint):
-    pipe = subprocess.Popen(
-            [PERF, 'record', '-a', '-e', tracepoint, '-o', file_path])
-    profile_pipe = None
-    if profile is True:
+def start_recording(handle):
+    if handle.tracepoint is not None:
+        handle.perf_pipe = subprocess.Popen(
+                [PERF, 'record', '-a', '-e', handle.tracepoint,
+                 '-o', handle.file_path])
+    if handle.do_profile:
         cmd = [PERF, 'record', '-o', '%s.profile' % file_path]
-        if profile_target_pid is not None:
-            cmd += ['--pid', profile_target_pid]
-        profile_pipe = subprocess.Popen(cmd)
-    return RecordingHandle(
-            file_path, file_format, file_permission, monitoring_intervals,
-            pipe, profile_pipe, kdamonds, poll_add_child_tasks,
-            poll_add_mem_footprint)
+        handle.perf_profile_pipe = subprocess.Popen(cmd)
+    while poll_target_pids(handle):
+        time.sleep(1)
+    _damon.wait_kdamonds_turned_off()
 
 def finish_recording(handle):
     try:
         handle.perf_pipe.send_signal(signal.SIGINT)
         handle.perf_pipe.wait()
     except:
         # perf might already finished
```

### Comparing `damo-2.2.9/src/damo/_damo_subcmds.py` & `damo-2.3.0/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damon.py` & `damo-2.3.0/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damon_args.py` & `damo-2.3.0/src/damo/_damon_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,45 @@
             warn_option_override('--ops')
         args.ops = 'vaddr'
     if args.regions:
         if not args.ops in ['fvaddr', None]:
             print('warning: override --ops by <deducible target> and --regions')
         args.ops = 'fvaddr'
 
+def evaluate_args(args):
+    '''
+    Verify if 'damons_action' is present when any 'damos_*' is specified
+    '''
+    if not args.damos_action:
+        for key, value in args.__dict__.items():
+            if key.startswith('damos_') and len(value):
+                if key == 'damos_action': continue
+                return False, '\'damos_action\' not specified while using --damos_* option(s)'
+
+    '''
+    Verify if 'reset_interval_ms' is specified in args when setting quota goals
+    '''
+    if args.damos_quota_goal:
+        damos_quotas = args.damos_quotas
+
+        if not len(damos_quotas):
+            return False, '\'reset_interval_ms\' not specified when setting quota goals'
+
+        #reset_interval_ms is specified in --damos_quotas as 3rd arg
+        for quota in damos_quotas:
+            if len(quota) < 3:
+                return False, '\'reset_interval_ms\' not specified when setting quota goals'
+
+    return True, None
+
 def kdamonds_for(args):
+    correct, err = evaluate_args(args)
+    if err is not None:
+        return None, err
+
     if args.kdamonds:
         return kdamonds_from_json_arg(args.kdamonds)
 
     if args.deducible_target:
         kdamonds, e = kdamonds_from_json_arg(args.deducible_target)
         if e == None:
             return kdamonds, e
```

### Comparing `damo-2.2.9/src/damo/_damon_dbgfs.py` & `damo-2.3.0/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/_damon_sysfs.py` & `damo-2.3.0/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo.py` & `damo-2.3.0/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_adjust.py` & `damo-2.3.0/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_convert_record_format.py` & `damo-2.3.0/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_features.py` & `damo-2.3.0/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_fmt_json.py` & `damo-2.3.0/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_heats.py` & `damo-2.3.0/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_lru_sort.py` & `damo-2.3.0/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_monitor.py` & `damo-2.3.0/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_nr_regions.py` & `damo-2.3.0/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_reclaim.py` & `damo-2.3.0/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_record.py` & `damo-2.3.0/src/damo/damo_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,28 +105,29 @@
         kdamonds = None
 
     if args.schemes_target_regions == False:
         tracepoint = _damo_records.perf_event_damon_aggregated
     else:
         tracepoint = _damo_records.perf_event_damos_before_apply
 
-    data_for_cleanup.record_handle = _damo_records.start_recording(
-            tracepoint, args.out, args.output_type, args.output_permission,
-            monitoring_intervals,
-            profile=args.profile is True, profile_target_pid=None,
+    record_handle = _damo_records.RecordingHandle(
+            # for access pattern monitoring
+            tracepoint=tracepoint, file_path=args.out,
+            file_format=args.output_type,
+            file_permission=args.output_permission,
+            monitoring_intervals=monitoring_intervals,
+            # for perf profile
+            do_profile=args.profile is True,
+            # for childs recording and memory footprint
             kdamonds=kdamonds, poll_add_child_tasks=args.include_child_tasks,
             poll_add_mem_footprint=args.footprint)
-    print('Press Ctrl+C to stop')
-
-    if _damon_args.self_started_target(args):
-        while _damo_records.poll_target_pids(data_for_cleanup.record_handle):
-            time.sleep(1)
-
-    _damon.wait_kdamonds_turned_off()
+    data_for_cleanup.record_handle = record_handle
 
+    print('Press Ctrl+C to stop')
+    _damo_records.start_recording(record_handle)
     cleanup_exit(0)
 
 def set_argparser(parser):
     parser = _damon_args.set_argparser(parser, add_record_options=True)
     parser.add_argument('--output_type',
                         choices=_damo_records.file_types,
                         default=_damo_records.file_type_json_compressed,
```

### Comparing `damo-2.2.9/src/damo/damo_record_info.py` & `damo-2.3.0/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_replay.py` & `damo-2.3.0/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_report.py` & `damo-2.3.0/src/damo/damo_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import _damo_subcmds
 import damo_heats
 import damo_nr_regions
+import damo_report_footprint
 import damo_report_profile
 import damo_report_raw
 import damo_report_times
 import damo_wss
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='raw', module=damo_report_raw,
@@ -19,14 +20,17 @@
             msg='working set size'),
         _damo_subcmds.DamoSubCmd(name='nr_regions', module=damo_nr_regions,
             msg='number of regions'),
         _damo_subcmds.DamoSubCmd(name='profile', module=damo_report_profile,
             msg='profile report for specific access pattern'),
         _damo_subcmds.DamoSubCmd(name='times', module=damo_report_times,
             msg='times of record having specific access pattern'),
+        _damo_subcmds.DamoSubCmd(
+            name='footprints', module=damo_report_footprint,
+            msg='memory footprints'),
         ]
 
 def main(args):
     for subcmd in subcmds:
         if subcmd.name == args.report_type:
             subcmd.execute(args)
```

### Comparing `damo-2.2.9/src/damo/damo_report_profile.py` & `damo-2.3.0/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_report_raw.py` & `damo-2.3.0/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_report_times.py` & `damo-2.3.0/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_schemes.py` & `damo-2.3.0/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_show.py` & `damo-2.3.0/src/damo/damo_show.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_start.py` & `damo-2.3.0/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_status.py` & `damo-2.3.0/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_stop.py` & `damo-2.3.0/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_tune.py` & `damo-2.3.0/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_validate.py` & `damo-2.3.0/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo/damo_wss.py` & `damo-2.3.0/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.9/src/damo.egg-info/PKG-INFO` & `damo-2.3.0/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.9
+Version: 2.3.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.0/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.9/src/damo.egg-info/SOURCES.txt` & `damo-2.3.0/src/damo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
 src/damo/damo_record_info.py
 src/damo/damo_replay.py
 src/damo/damo_report.py
+src/damo/damo_report_footprint.py
 src/damo/damo_report_profile.py
 src/damo/damo_report_raw.py
 src/damo/damo_report_times.py
 src/damo/damo_schemes.py
 src/damo/damo_show.py
 src/damo/damo_start.py
 src/damo/damo_status.py
```

