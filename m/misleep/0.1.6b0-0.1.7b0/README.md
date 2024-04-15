# Comparing `tmp/misleep-0.1.6b0.tar.gz` & `tmp/misleep-0.1.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.6b0.tar", last modified: Mon Apr 15 10:41:36 2024, max compression
+gzip compressed data, was "misleep-0.1.7b0.tar", last modified: Mon Apr 15 11:24:32 2024, max compression
```

## Comparing `misleep-0.1.6b0.tar` & `misleep-0.1.7b0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.409612 misleep-0.1.6b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.6b0/LICENSE
--rw-rw-rw-   0        0        0     2968 2024-04-15 10:41:36.409612 misleep-0.1.6b0/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2024-04-15 03:11:05.000000 misleep-0.1.6b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.387612 misleep-0.1.6b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.6b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      536 2024-04-15 10:40:35.000000 misleep-0.1.6b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.392612 misleep-0.1.6b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     6775 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    56115 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.394612 misleep-0.1.6b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.6b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.1.6b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.398613 misleep-0.1.6b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24854 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/save_data_dialog_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     3375 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.400613 misleep-0.1.6b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     6275 2024-04-15 10:39:05.000000 misleep-0.1.6b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     4785 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.401612 misleep-0.1.6b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.6b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.6b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.1.6b0/misleep/preprocessing/signals.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.6b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.403613 misleep-0.1.6b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.1.6b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.6b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.405612 misleep-0.1.6b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.6b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.6b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.6b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.6b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.389612 misleep-0.1.6b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     2968 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 10:41:36.000000 misleep-0.1.6b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 10:41:36.410612 misleep-0.1.6b0/setup.cfg
--rw-rw-rw-   0        0        0     2157 2024-04-15 10:40:45.000000 misleep-0.1.6b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:41:36.408613 misleep-0.1.6b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.6b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.1.6b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.6b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.6b0/test/test_show.py
--rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.1.6b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.6b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.6b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.435966 misleep-0.1.7b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.7b0/LICENSE
+-rw-rw-rw-   0        0        0     2968 2024-04-15 11:24:32.435966 misleep-0.1.7b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2024-04-15 03:11:05.000000 misleep-0.1.7b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.408966 misleep-0.1.7b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.7b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      523 2024-04-15 11:24:18.000000 misleep-0.1.7b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.415966 misleep-0.1.7b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.7b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     6697 2024-04-15 11:23:51.000000 misleep-0.1.7b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    56191 2024-04-15 11:22:51.000000 misleep-0.1.7b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.418966 misleep-0.1.7b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.7b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.1.7b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.421965 misleep-0.1.7b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.7b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    24854 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     3375 2024-04-15 10:35:14.000000 misleep-0.1.7b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.423965 misleep-0.1.7b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.7b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     6268 2024-04-15 11:24:05.000000 misleep-0.1.7b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     4785 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.425966 misleep-0.1.7b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.7b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.7b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.1.7b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.7b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.427966 misleep-0.1.7b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.7b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.1.7b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.7b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.429966 misleep-0.1.7b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.7b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.7b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.7b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.7b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.410966 misleep-0.1.7b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     2968 2024-04-15 11:24:32.000000 misleep-0.1.7b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2024-04-15 11:24:32.000000 misleep-0.1.7b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:24:32.000000 misleep-0.1.7b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-15 11:24:32.000000 misleep-0.1.7b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 11:24:32.000000 misleep-0.1.7b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:24:32.435966 misleep-0.1.7b0/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2024-04-15 11:24:23.000000 misleep-0.1.7b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:32.434966 misleep-0.1.7b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.7b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.1.7b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.7b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.7b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.1.7b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.7b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.7b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.6b0/LICENSE` & `misleep-0.1.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/PKG-INFO` & `misleep-0.1.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.6b0
+Version: 0.1.7b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.6b0/README.md` & `misleep-0.1.7b0/README.md`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/config.ini` & `misleep-0.1.7b0/misleep/config.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [gui]
-version = v0.1.6 Beta
+version = v0.1.7 Beta
 updatetime = 2024/04/01
 marker = ['pat', 'add water', 'third']
 startend = ['SWA', 'SWA', 'start end label', 'start end label', 'start end label', 'start end label', 'start end label']
 statemap = {"1": "NREM", "2": "REM", "3": "Wake", "4": "INIT"}
 statecolor = {"1": "orange", "2": "skyblue", "3": "red", "4": "white"}
 statecolorbgalpha = 0.1
 markerlinecolor = "red"
 startendlinecolor = "blue"
-openpath = E:/workplace/EEGProcessing/00_DATA/medusa/example_data/15_48_32_055/15_48_32_055_sleep.txt
+openpath = E:/workplace/EEGProcessing/00_DATA/medusa/example_data/15_48_32_055/label.txt
```

### Comparing `misleep-0.1.6b0/misleep/gui/about.py` & `misleep-0.1.7b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/dialog.py` & `misleep-0.1.7b0/misleep/gui/dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,14 @@
         
     def enable_time_editor(self):
         self.ACTimeEditor.setEnabled(True)
 
     def transfer(self, config, mianno, ac_time):
         """Transfer result to dataframe, triggered by okay button"""
 
-        self.ACTimeEditor.setDateTime(ac_time.strptime("%Y%m%d-%H:%M:%S"))
-
         if self.ResetTimeCheckBox.isChecked():
             ac_time = self.ACTimeEditor.dateTime().toPyDateTime()
         else:
             ac_time = datetime.datetime.strptime(ac_time, "%Y%m%d-%H:%M:%S")
         
         
         fd, _ = QFileDialog.getSaveFileName(self, "Save transfered result",
```

### Comparing `misleep-0.1.6b0/misleep/gui/main_window.py` & `misleep-0.1.7b0/misleep/gui/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1344,14 +1344,15 @@
     def tool_bar_dispatcher(self, signal):
         """Triggered by ToolBar action, transfer result"""
         if signal.text() == "Transfer Result":
             self.transfer_result()
 
     def transfer_result(self):
         """Transfer result into file"""
+        self.transfer_result_dialog.ACTimeEditor.setDateTime(self.ac_time)
         self.transfer_result_dialog.exec_()
         if self.label_dialog.closed:
             return
         self.transfer_result_dialog.transfer(config=self.config,
                                              mianno=self.mianno,
                                              ac_time=self.midata.time)
```

### Comparing `misleep-0.1.6b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.7b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/resources/logo.png` & `misleep-0.1.7b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/resources/misleep.py` & `misleep-0.1.7b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/spec_window.py` & `misleep-0.1.7b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/thread.py` & `misleep-0.1.7b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/save_data_dialog_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/save_data_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/uis/transfer_result_dialog_ui.py` & `misleep-0.1.7b0/misleep/gui/uis/transfer_result_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/gui/utils.py` & `misleep-0.1.7b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/io/annotation_io.py` & `misleep-0.1.7b0/misleep/io/annotation_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 @Project: MiSleep_v2 
 @File: annotation_io.py
 @Author: Xueqiang Wang
 @Date: 2024/3/6
 @Description:  Annotation io, default is for MiSleep annotation, `NAME.txt`
 """
 from misleep.io.base import MiAnnotation
-from misleep.utils.annotation import marker2mianno, start_end2mianno, lst2group, sleep_state2mianno, \
-    transfer_time, insert_row, temp_loop4below_row
+from misleep.utils.annotation import marker2mianno, start_end2mianno, lst2group, sleep_state2mianno, transfer_time, insert_row, temp_loop4below_row
 import pandas as pd
 
 
 def load_misleep_anno(file_path):
     """
     Load annotations from misleep annotation file
```

### Comparing `misleep-0.1.6b0/misleep/io/base.py` & `misleep-0.1.7b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/io/signal_io.py` & `misleep-0.1.7b0/misleep/io/signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/preprocessing/spectral.py` & `misleep-0.1.7b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/utils/annotation.py` & `misleep-0.1.7b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/utils/only4gui.py` & `misleep-0.1.7b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/utils/signals.py` & `misleep-0.1.7b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/viz/hypnogram.py` & `misleep-0.1.7b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/viz/signals.py` & `misleep-0.1.7b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep/viz/spectral.py` & `misleep-0.1.7b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/misleep.egg-info/PKG-INFO` & `misleep-0.1.7b0/misleep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.6b0
+Version: 0.1.7b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.6b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.7b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/setup.py` & `misleep-0.1.7b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.6 Beta"
+VERSION = "0.1.7 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.1.6b0/test/test_midata.py` & `misleep-0.1.7b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/test/test_signal_io.py` & `misleep-0.1.7b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/test/test_signals_viz.py` & `misleep-0.1.7b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.6b0/test/test_spectral_viz.py` & `misleep-0.1.7b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

