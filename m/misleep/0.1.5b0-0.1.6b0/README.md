# Comparing `tmp/misleep-0.1.5b0.tar.gz` & `tmp/misleep-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.5b0.tar", last modified: Fri Apr 12 08:03:00 2024, max compression
+gzip compressed data, was "misleep-0.1.6b0.tar", last modified: Mon Apr 15 10:41:36 2024, max compression
```

## Comparing `misleep-0.1.5b0.tar` & `misleep-0.1.6b0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.909968 misleep-0.1.5b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.5b0/LICENSE
--rw-rw-rw-   0        0        0     2968 2024-04-12 08:03:00.908969 misleep-0.1.5b0/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2024-04-10 04:00:34.000000 misleep-0.1.5b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.885968 misleep-0.1.5b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.5b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.5b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      532 2024-04-12 08:02:53.000000 misleep-0.1.5b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.891968 misleep-0.1.5b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-12 06:13:32.000000 misleep-0.1.5b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0    10976 2024-04-12 06:57:35.000000 misleep-0.1.5b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    55821 2024-04-12 08:01:54.000000 misleep-0.1.5b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.893968 misleep-0.1.5b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.5b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.5b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.5b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-12 06:40:33.000000 misleep-0.1.5b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.5b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.896969 misleep-0.1.5b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24854 2024-04-12 06:48:24.000000 misleep-0.1.5b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.5b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     3048 2024-04-12 06:16:09.000000 misleep-0.1.5b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     3441 2024-04-12 06:27:56.000000 misleep-0.1.5b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.898969 misleep-0.1.5b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.5b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.5b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.900969 misleep-0.1.5b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.5b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.5b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.5b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.903969 misleep-0.1.5b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.5b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.905968 misleep-0.1.5b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.5b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.5b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.887968 misleep-0.1.5b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     2968 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 08:03:00.909968 misleep-0.1.5b0/setup.cfg
--rw-rw-rw-   0        0        0     2157 2024-04-12 08:02:06.000000 misleep-0.1.5b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.908969 misleep-0.1.5b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.5b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.5b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.5b0/test/test_show.py
--rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.5b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.409612 misleep-0.1.6b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.6b0/LICENSE
+-rw-rw-rw-   0        0        0     2968 2024-04-15 10:41:36.409612 misleep-0.1.6b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2024-04-15 03:11:05.000000 misleep-0.1.6b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.387612 misleep-0.1.6b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.6b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      536 2024-04-15 10:40:35.000000 misleep-0.1.6b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.392612 misleep-0.1.6b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     6775 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    56115 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.394612 misleep-0.1.6b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.6b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.1.6b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.398613 misleep-0.1.6b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    24854 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     3375 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.400613 misleep-0.1.6b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     6275 2024-04-15 10:39:05.000000 misleep-0.1.6b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     4785 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.401612 misleep-0.1.6b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.6b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.6b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.6b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.403613 misleep-0.1.6b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.405612 misleep-0.1.6b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.6b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.6b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.389612 misleep-0.1.6b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     2968 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:41:36.410612 misleep-0.1.6b0/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2024-04-15 10:40:45.000000 misleep-0.1.6b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.408613 misleep-0.1.6b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.6b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.1.6b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.6b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.6b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.1.6b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.6b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.6b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.5b0/LICENSE` & `misleep-0.1.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/PKG-INFO` & `misleep-0.1.6b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.5b0/README.md` & `misleep-0.1.6b0/README.md`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/config.ini` & `misleep-0.1.6b0/misleep/config.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [gui]
-version = v0.1.5 Beta
+version = v0.1.6 Beta
 updatetime = 2024/04/01
 marker = ['pat', 'add water', 'third']
 startend = ['SWA', 'SWA', 'start end label', 'start end label', 'start end label', 'start end label', 'start end label']
 statemap = {"1": "NREM", "2": "REM", "3": "Wake", "4": "INIT"}
 statecolor = {"1": "orange", "2": "skyblue", "3": "red", "4": "white"}
 statecolorbgalpha = 0.1
 markerlinecolor = "red"
 startendlinecolor = "blue"
-openpath = E:/workplace/EEGProcessing/00_DATA/20240117_0700_WXQ_3mice_24h/mouse2/mouse2_label.txt
+openpath = E:/workplace/EEGProcessing/00_DATA/medusa/example_data/15_48_32_055/15_48_32_055_sleep.txt
```

### Comparing `misleep-0.1.5b0/misleep/gui/about.py` & `misleep-0.1.6b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/main_window.py` & `misleep-0.1.6b0/misleep/gui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from PyQt5.QtWidgets import QMainWindow, QFileDialog, QMessageBox, QAction, QShortcut
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 from misleep.preprocessing.spectral import spectrogram
 from misleep.io.base import MiData, MiAnnotation
 from misleep.io.signal_io import load_mat, load_edf
-from misleep.io.annotation_io import load_misleep_anno
+from misleep.io.annotation_io import load_misleep_anno, load_bio_anno
 from misleep.gui.utils import create_new_mianno
 from misleep.utils.annotation import lst2group
 from misleep.gui.about import about_dialog
 from misleep.gui.dialog import label_dialog, transferResult_dialog
 from misleep.gui.spec_window import SpecWindow
 from misleep.gui.uis.main_window_ui import Ui_MiSleep
 from misleep.preprocessing.spectral import spectrogram, spectrum, band_power
@@ -337,15 +337,19 @@
 
         if anno_path == "":
             return
         self.anno_path = anno_path
 
         if self.anno_path.endswith((".txt", ".TXT")):
             try:
-                self.mianno = load_misleep_anno(self.anno_path)
+                file = open(self.anno_path, 'r').read()
+                if file[:5] == 'Start':
+                    self.mianno = load_bio_anno(self.anno_path)
+                else:
+                    self.mianno = load_misleep_anno(self.anno_path)
             except AssertionError as e:
                 if e.args[0] == "Empty":
                     if isinstance(self.midata, MiData):
                         self.mianno = create_new_mianno(self.midata.duration)
                     else:
                         QMessageBox.about(
                             self,
@@ -778,15 +782,15 @@
         self.hypo_ax.step(
             range(self.mianno.anno_length),
             self.mianno.sleep_state,
             where="mid",
             linewidth=1,
         )
 
-        self.hypo_ax.set_ylim(0, len(list(self.state_map_dict.keys())))
+        self.hypo_ax.set_ylim(0, len(list(self.state_map_dict.keys()))+0.5)
         self.hypo_ax.set_xlim(0, self.total_seconds)
         self.hypo_ax.yaxis.set_ticks(list(self.state_map_dict.keys()), 
                                      list(self.state_map_dict.values()))
         if self.StartEndRadio.isChecked():
             for each in self.start_end_ms:
                 self.hypo_ax.axvline(each, color="lime", alpha=1)
 
@@ -1329,15 +1333,15 @@
             self.load_anno()
         if signal.text() == "Show":
             self.check_show()
 
     def save_bar_dispatcher(self, signal):
         """Triggered by SaveBar action, save data, save annotation"""
         if signal.text() == "Save Data":
-            pass
+            self.save_data()
         if signal.text() == "Save Annotation":
             self.save_anno()
 
     def tool_bar_dispatcher(self, signal):
         """Triggered by ToolBar action, transfer result"""
         if signal.text() == "Transfer Result":
             self.transfer_result()
@@ -1356,14 +1360,18 @@
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
         saved = save_thread.save_anno()
         if saved:
             self.is_saved = True
             QMessageBox.about(self, "Info", "Annotation saved")
         save_thread.quit()
+
+    def save_data(self):
+        """Save data into file"""
+        
     
     def auto_save(self):
         """Auto save every 5 mins"""
         if not self.is_saved:
             self.save_anno()
         self.save_timer.start(5*60*1000)
```

### Comparing `misleep-0.1.5b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.6b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/resources/logo.png` & `misleep-0.1.6b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/resources/misleep.py` & `misleep-0.1.6b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/spec_window.py` & `misleep-0.1.6b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/thread.py` & `misleep-0.1.6b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.6b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.6b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.6b0/misleep/gui/uis/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.6b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/gui/uis/transfer_result_dialog_ui.py` & `misleep-0.1.6b0/misleep/gui/uis/transfer_result_dialog_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,28 @@
         TransferResultDialog.resize(324, 193)
         self.verticalLayout = QtWidgets.QVBoxLayout(TransferResultDialog)
         self.verticalLayout.setObjectName("verticalLayout")
         self.groupBox = QtWidgets.QGroupBox(TransferResultDialog)
         self.groupBox.setObjectName("groupBox")
         self.gridLayout = QtWidgets.QGridLayout(self.groupBox)
         self.gridLayout.setObjectName("gridLayout")
+        self.ResetTimeCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.ResetTimeCheckBox.setObjectName("ResetTimeCheckBox")
+        self.gridLayout.addWidget(self.ResetTimeCheckBox, 0, 0, 1, 1)
         self.ACTimeEditor = QtWidgets.QDateTimeEdit(self.groupBox)
         self.ACTimeEditor.setObjectName("ACTimeEditor")
         self.gridLayout.addWidget(self.ACTimeEditor, 1, 0, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem, 1, 1, 1, 1)
         self.ContainEventsCheckBox = QtWidgets.QCheckBox(self.groupBox)
         self.ContainEventsCheckBox.setObjectName("ContainEventsCheckBox")
-        self.gridLayout.addWidget(self.ContainEventsCheckBox, 2, 0, 1, 1)
-        self.ResetTimeCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.ResetTimeCheckBox.setObjectName("ResetTimeCheckBox")
-        self.gridLayout.addWidget(self.ResetTimeCheckBox, 0, 0, 1, 1)
+        self.gridLayout.addWidget(self.ContainEventsCheckBox, 3, 0, 1, 1)
+        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.gridLayout.addItem(spacerItem, 1, 1, 1, 1)
+        self.RejectArtifactCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.RejectArtifactCheckBox.setObjectName("RejectArtifactCheckBox")
+        self.gridLayout.addWidget(self.RejectArtifactCheckBox, 2, 0, 1, 1)
         self.verticalLayout.addWidget(self.groupBox)
         self.buttonBox = QtWidgets.QDialogButtonBox(TransferResultDialog)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout.addWidget(self.buttonBox)
 
@@ -44,10 +47,11 @@
         self.buttonBox.rejected.connect(TransferResultDialog.reject) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(TransferResultDialog)
 
     def retranslateUi(self, TransferResultDialog):
         _translate = QtCore.QCoreApplication.translate
         TransferResultDialog.setWindowTitle(_translate("TransferResultDialog", "Dialog"))
         self.groupBox.setTitle(_translate("TransferResultDialog", "Transfer result options"))
+        self.ResetTimeCheckBox.setText(_translate("TransferResultDialog", "Reset acquisition time"))
         self.ACTimeEditor.setDisplayFormat(_translate("TransferResultDialog", "yyyy/MM/dd HH:mm:ss"))
         self.ContainEventsCheckBox.setText(_translate("TransferResultDialog", "Contain Start-End events"))
-        self.ResetTimeCheckBox.setText(_translate("TransferResultDialog", "Reset acquisition time"))
+        self.RejectArtifactCheckBox.setText(_translate("TransferResultDialog", "Reject artifact"))
```

### Comparing `misleep-0.1.5b0/misleep/gui/utils.py` & `misleep-0.1.6b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/io/base.py` & `misleep-0.1.6b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/io/signal_io.py` & `misleep-0.1.6b0/misleep/io/signal_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,19 @@
             sf = [305. for _ in range(raw_data.shape[0])]
             time = datetime.datetime.now().strftime("%Y%m%d-%H:%M:%S")
             return MiData(signals=signals, channels=channels, sf=sf, time=time)
 
         raw_data = raw_data[0][0]
         # Whether saved by python
         if 'save' in names:
-            pass
+            channels = list(raw_data['channels'])
+            sf = [float(each) for each in raw_data['sf'][0]]
+            signals = [raw_data[each][0] for each in channels]
+            time = raw_data['time'][0]
+            return MiData(signals=signals, channels=channels, sf=sf, time=time)
 
         # Saved by matlab
         channels = [each for item in raw_data['channels'][0] for each in item]
         sf = [float(each[0]) for item in raw_data['sf'][0] for each in item]
         signals = [raw_data[each][0] for each in channels]
         time = raw_data['time'][0]
         
@@ -132,12 +136,13 @@
 
     Returns
     -------
     midata : MiData
         MiSleep data format data
     """
 
-    signals, signal_headers, _ = pyedflib.highlevel.read_edf(edf_file=data_path)
+    signals, signal_headers, meta = pyedflib.highlevel.read_edf(edf_file=data_path)
 
     return MiData(signals=signals,
                   channels=[each['label'] for each in signal_headers],
-                  sf=[each['sample_frequency'] for each in signal_headers])
+                  sf=[each['sample_frequency'] for each in signal_headers],
+                  time=meta['startdate'].strftime('%Y%m%d-%H:%M:%S'))
```

### Comparing `misleep-0.1.5b0/misleep/preprocessing/spectral.py` & `misleep-0.1.6b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/utils/only4gui.py` & `misleep-0.1.6b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/utils/signals.py` & `misleep-0.1.6b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/viz/hypnogram.py` & `misleep-0.1.6b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/viz/signals.py` & `misleep-0.1.6b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep/viz/spectral.py` & `misleep-0.1.6b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/misleep.egg-info/PKG-INFO` & `misleep-0.1.6b0/misleep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.5b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.6b0/misleep.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 misleep/gui/resources/logo.png
 misleep/gui/resources/misleep.py
 misleep/gui/resources/misleep.qrc
 misleep/gui/uis/__init__.py
 misleep/gui/uis/about_ui.py
 misleep/gui/uis/label_dialog_ui.py
 misleep/gui/uis/main_window_ui.py
+misleep/gui/uis/save_data_dialog_ui.py
 misleep/gui/uis/spec_window_ui.py
 misleep/gui/uis/transfer_result_dialog_ui.py
 misleep/io/__init__.py
 misleep/io/annotation_io.py
 misleep/io/base.py
 misleep/io/signal_io.py
 misleep/preprocessing/__init__.py
 misleep/preprocessing/channel.py
+misleep/preprocessing/signals.py
 misleep/preprocessing/spectral.py
 misleep/utils/__init__.py
 misleep/utils/annotation.py
 misleep/utils/only4gui.py
 misleep/utils/others.py
 misleep/utils/signals.py
 misleep/viz/__init__.py
```

### Comparing `misleep-0.1.5b0/setup.py` & `misleep-0.1.6b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.5 Beta"
+VERSION = "0.1.6 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.1.5b0/test/test_midata.py` & `misleep-0.1.6b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/test/test_signal_io.py` & `misleep-0.1.6b0/test/test_signal_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 @Project: misleep
 @File: test_signal_io.py
 @Author: Xueqiang Wang
 @Date: 2024/2/22
 @Description:
 """
 
-import unittest
+import pytest
 from misleep.io.signal_io import load_mat, load_edf, write_mat
 from time import time
 
 
-class TestSignalIO(unittest.TestCase):
+class TestSignalIO():
     def test_load_mat_write_mat(self):
         """Test load_mat and write_mat"""
-        mat_path = r'../datasets/mat_from_mat_.mat'
+        mat_path = r'E:\workplace\EEGProcessing\00_DATA\20231117_test+vid_6pin\data_mini_saved_python.mat'
         s = time()
         midata = load_mat(data_path=mat_path)
         e = time()
         print(f"Load data from .mat file, cost {e-s} seconds\n"
               f"Signals shape {len(midata.signals)}, channels: {midata.channels}, sampling frequency: {midata.sf}")
 
-        write_mat(midata.signals, midata.channels, midata.sf, midata.time, r'../datasets/mat_from_mat.mat')
+        write_mat(midata.signals, midata.channels, midata.sf, midata.time, 
+                  r'E:\workplace\EEGProcessing\00_DATA\20231117_test+vid_6pin\data_mini_saved_python.mat')
         print('Saved to .mat successfully')
 
     def test_load_edf_write_mat(self):
         """Test load_edf and write_mat"""
         edf_path = r'../datasets/learn-nsrr01.edf'
         s = time()
         signals, channels, sf = load_edf(data_path=edf_path)
```

### Comparing `misleep-0.1.5b0/test/test_signals_viz.py` & `misleep-0.1.6b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.5b0/test/test_spectral_viz.py` & `misleep-0.1.6b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

