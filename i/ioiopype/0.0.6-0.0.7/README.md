# Comparing `tmp/ioiopype-0.0.6.tar.gz` & `tmp/ioiopype-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioiopype-0.0.6.tar", last modified: Thu Mar 21 18:52:22 2024, max compression
+gzip compressed data, was "ioiopype-0.0.7.tar", last modified: Mon Apr 15 10:55:48 2024, max compression
```

## Comparing `ioiopype-0.0.6.tar` & `ioiopype-0.0.7.tar`

### file list

```diff
@@ -1,68 +1,75 @@
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.984576 ioiopype-0.0.6/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1061 2024-03-13 16:32:39.000000 ioiopype-0.0.6/LICENSE
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     4494 2024-03-21 18:52:22.984513 ioiopype-0.0.6/PKG-INFO
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     3905 2024-03-21 15:42:19.000000 ioiopype-0.0.6/README.md
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.973210 ioiopype-0.0.6/ioiopype/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1616 2024-03-21 18:14:28.000000 ioiopype-0.0.6/ioiopype/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      189 2024-03-21 18:51:50.000000 ioiopype-0.0.6/ioiopype/__version__.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.974093 ioiopype-0.0.6/ioiopype/common/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:37:23.000000 ioiopype-0.0.6/ioiopype/common/__init__.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.974869 ioiopype-0.0.6/ioiopype/common/i_nodes/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/common/i_nodes/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1045 2024-03-17 11:24:21.000000 ioiopype-0.0.6/ioiopype/common/i_nodes/console_log.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2159 2024-03-20 17:25:20.000000 ioiopype-0.0.6/ioiopype/common/i_nodes/csv_logger.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1324 2024-03-17 11:24:12.000000 ioiopype-0.0.6/ioiopype/common/i_nodes/to_workspace.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.977288 ioiopype-0.0.6/ioiopype/common/io_nodes/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2373 2024-03-17 10:56:37.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/buffer.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2582 2024-03-17 11:23:19.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/butterworth_filter.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1954 2024-03-17 11:23:22.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/butterworth_filtfilt.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1519 2024-03-17 11:23:27.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/downsample.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1144 2024-03-17 10:33:08.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/framer.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2507 2024-03-17 11:23:32.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/offset_correction.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2080 2024-03-17 11:31:36.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/pwelch.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1411 2024-03-17 11:23:41.000000 ioiopype-0.0.6/ioiopype/common/io_nodes/to_sample.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.977990 ioiopype-0.0.6/ioiopype/common/o_devices/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/common/o_devices/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)    12683 2024-03-16 09:20:58.000000 ioiopype-0.0.6/ioiopype/common/o_devices/unicorn.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     6030 2024-03-20 16:48:56.000000 ioiopype-0.0.6/ioiopype/common/o_devices/unicorn_simulator.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.978912 ioiopype-0.0.6/ioiopype/common/o_nodes/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/common/o_nodes/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2214 2024-03-21 18:26:58.000000 ioiopype-0.0.6/ioiopype/common/o_nodes/csv_reader.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2284 2024-03-17 11:23:51.000000 ioiopype-0.0.6/ioiopype/common/o_nodes/data_generator.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      933 2024-03-17 11:24:01.000000 ioiopype-0.0.6/ioiopype/common/o_nodes/frame.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.980127 ioiopype-0.0.6/ioiopype/common/utilities/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/common/utilities/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1512 2024-03-09 21:49:14.000000 ioiopype-0.0.6/ioiopype/common/utilities/butterworth.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      126 2024-02-28 17:31:42.000000 ioiopype-0.0.6/ioiopype/common/utilities/filter_types.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1446 2024-03-21 15:37:55.000000 ioiopype-0.0.6/ioiopype/common/utilities/overriding_buffer.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1509 2024-02-29 16:44:00.000000 ioiopype-0.0.6/ioiopype/common/utilities/realtime_clock.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.980407 ioiopype-0.0.6/ioiopype/desktop/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/desktop/__init__.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.980951 ioiopype-0.0.6/ioiopype/desktop/i_nodes/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/desktop/i_nodes/__init__.py
--rwx------   0 martinwalchshoferwalchshofer   (501) staff       (20)     2421 2024-03-21 14:32:05.000000 ioiopype-0.0.6/ioiopype/desktop/i_nodes/frame_plot.py
--rwx------   0 martinwalchshoferwalchshofer   (501) staff       (20)     3702 2024-03-21 14:58:58.000000 ioiopype-0.0.6/ioiopype/desktop/i_nodes/sample_plot.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.982840 ioiopype-0.0.6/ioiopype/pattern/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/pattern/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     3041 2024-02-29 18:49:09.000000 ioiopype-0.0.6/ioiopype/pattern/i_node.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      990 2024-03-05 21:42:12.000000 ioiopype-0.0.6/ioiopype/pattern/i_stream.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      295 2024-02-22 06:28:38.000000 ioiopype-0.0.6/ioiopype/pattern/io_node.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      596 2024-03-13 15:52:52.000000 ioiopype-0.0.6/ioiopype/pattern/o_device.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1337 2024-02-29 09:04:10.000000 ioiopype-0.0.6/ioiopype/pattern/o_node.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1190 2024-03-20 15:43:34.000000 ioiopype-0.0.6/ioiopype/pattern/o_stream.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      624 2024-03-17 10:54:21.000000 ioiopype-0.0.6/ioiopype/pattern/stream_info.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.983169 ioiopype-0.0.6/ioiopype/utilities/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.6/ioiopype/utilities/__init__.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1096 2024-02-22 16:02:45.000000 ioiopype-0.0.6/ioiopype/utilities/system.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.984261 ioiopype-0.0.6/ioiopype.egg-info/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     4494 2024-03-21 18:52:22.000000 ioiopype-0.0.6/ioiopype.egg-info/PKG-INFO
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1735 2024-03-21 18:52:22.000000 ioiopype-0.0.6/ioiopype.egg-info/SOURCES.txt
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        1 2024-03-21 18:52:22.000000 ioiopype-0.0.6/ioiopype.egg-info/dependency_links.txt
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        9 2024-03-21 18:52:22.000000 ioiopype-0.0.6/ioiopype.egg-info/top_level.txt
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)       74 2024-03-21 18:52:22.984796 ioiopype-0.0.6/setup.cfg
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1335 2024-03-15 20:23:49.000000 ioiopype-0.0.6/setup.py
-drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-21 18:52:22.983846 ioiopype-0.0.6/test/
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2769 2024-03-15 19:33:50.000000 ioiopype-0.0.6/test/test_filter.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1203 2024-03-17 11:24:28.000000 ioiopype-0.0.6/test/test_json.py
--rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2081 2024-03-16 08:42:27.000000 ioiopype-0.0.6/test/test_realtime_pipe1.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.187626 ioiopype-0.0.7/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1061 2024-03-13 16:32:39.000000 ioiopype-0.0.7/LICENSE
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     4946 2024-04-15 10:55:48.187557 ioiopype-0.0.7/PKG-INFO
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     4357 2024-04-14 15:07:42.000000 ioiopype-0.0.7/README.md
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.174986 ioiopype-0.0.7/ioiopype/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2044 2024-04-14 15:05:09.000000 ioiopype-0.0.7/ioiopype/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      189 2024-04-15 10:54:29.000000 ioiopype-0.0.7/ioiopype/__version__.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.175781 ioiopype-0.0.7/ioiopype/common/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:37:23.000000 ioiopype-0.0.7/ioiopype/common/__init__.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.176560 ioiopype-0.0.7/ioiopype/common/i_nodes/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/common/i_nodes/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1045 2024-03-17 11:24:21.000000 ioiopype-0.0.7/ioiopype/common/i_nodes/console_log.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2159 2024-03-20 17:25:20.000000 ioiopype-0.0.7/ioiopype/common/i_nodes/csv_logger.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1324 2024-03-17 11:24:12.000000 ioiopype-0.0.7/ioiopype/common/i_nodes/to_workspace.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.180012 ioiopype-0.0.7/ioiopype/common/io_nodes/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2373 2024-03-17 10:56:37.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/buffer.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2582 2024-03-17 11:23:19.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/butterworth_filter.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1954 2024-03-17 11:23:22.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/butterworth_filtfilt.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1519 2024-03-17 11:23:27.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/downsample.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1144 2024-03-17 10:33:08.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/framer.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1987 2024-03-24 18:54:24.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/log.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1931 2024-04-05 21:34:10.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/mux.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2507 2024-03-17 11:23:32.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/offset_correction.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2415 2024-04-14 15:04:31.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/operation.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2082 2024-03-24 18:12:24.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/pwelch.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1534 2024-03-24 07:41:13.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/sqrt.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1538 2024-03-23 12:42:29.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/square.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1411 2024-03-17 11:23:41.000000 ioiopype-0.0.7/ioiopype/common/io_nodes/to_sample.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.180689 ioiopype-0.0.7/ioiopype/common/o_devices/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/common/o_devices/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)    12683 2024-03-16 09:20:58.000000 ioiopype-0.0.7/ioiopype/common/o_devices/unicorn.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     6030 2024-03-20 16:48:56.000000 ioiopype-0.0.7/ioiopype/common/o_devices/unicorn_simulator.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.182197 ioiopype-0.0.7/ioiopype/common/o_nodes/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1390 2024-04-14 09:57:44.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/constant.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2214 2024-03-21 18:26:58.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/csv_reader.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      933 2024-03-17 11:24:01.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/frame.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1522 2024-04-14 09:38:21.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/noise_generator.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     3905 2024-04-14 09:36:40.000000 ioiopype-0.0.7/ioiopype/common/o_nodes/signal_generator.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.183260 ioiopype-0.0.7/ioiopype/common/utilities/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/common/utilities/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1512 2024-03-09 21:49:14.000000 ioiopype-0.0.7/ioiopype/common/utilities/butterworth.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      126 2024-02-28 17:31:42.000000 ioiopype-0.0.7/ioiopype/common/utilities/filter_types.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1446 2024-03-21 15:37:55.000000 ioiopype-0.0.7/ioiopype/common/utilities/overriding_buffer.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1509 2024-02-29 16:44:00.000000 ioiopype-0.0.7/ioiopype/common/utilities/realtime_clock.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.183518 ioiopype-0.0.7/ioiopype/desktop/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/desktop/__init__.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.183985 ioiopype-0.0.7/ioiopype/desktop/i_nodes/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/desktop/i_nodes/__init__.py
+-rwx------   0 martinwalchshoferwalchshofer   (501) staff       (20)     2549 2024-03-21 22:09:05.000000 ioiopype-0.0.7/ioiopype/desktop/i_nodes/frame_plot.py
+-rwx------   0 martinwalchshoferwalchshofer   (501) staff       (20)     3743 2024-04-12 19:51:59.000000 ioiopype-0.0.7/ioiopype/desktop/i_nodes/sample_plot.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.185705 ioiopype-0.0.7/ioiopype/pattern/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/pattern/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     3041 2024-02-29 18:49:09.000000 ioiopype-0.0.7/ioiopype/pattern/i_node.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1034 2024-04-05 21:39:30.000000 ioiopype-0.0.7/ioiopype/pattern/i_stream.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      295 2024-02-22 06:28:38.000000 ioiopype-0.0.7/ioiopype/pattern/io_node.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      583 2024-03-22 08:32:12.000000 ioiopype-0.0.7/ioiopype/pattern/o_device.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1337 2024-02-29 09:04:10.000000 ioiopype-0.0.7/ioiopype/pattern/o_node.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1190 2024-03-20 15:43:34.000000 ioiopype-0.0.7/ioiopype/pattern/o_stream.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)      624 2024-03-17 10:54:21.000000 ioiopype-0.0.7/ioiopype/pattern/stream_info.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.186044 ioiopype-0.0.7/ioiopype/utilities/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-03-15 20:35:18.000000 ioiopype-0.0.7/ioiopype/utilities/__init__.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1096 2024-02-22 16:02:45.000000 ioiopype-0.0.7/ioiopype/utilities/system.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.187167 ioiopype-0.0.7/ioiopype.egg-info/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     4946 2024-04-15 10:55:48.000000 ioiopype-0.0.7/ioiopype.egg-info/PKG-INFO
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1986 2024-04-15 10:55:48.000000 ioiopype-0.0.7/ioiopype.egg-info/SOURCES.txt
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        1 2024-04-15 10:55:48.000000 ioiopype-0.0.7/ioiopype.egg-info/dependency_links.txt
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)        9 2024-04-15 10:55:48.000000 ioiopype-0.0.7/ioiopype.egg-info/top_level.txt
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)       74 2024-04-15 10:55:48.187844 ioiopype-0.0.7/setup.cfg
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1335 2024-03-15 20:23:49.000000 ioiopype-0.0.7/setup.py
+drwxr-xr-x   0 martinwalchshoferwalchshofer   (501) staff       (20)        0 2024-04-15 10:55:48.186874 ioiopype-0.0.7/test/
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     2769 2024-03-15 19:33:50.000000 ioiopype-0.0.7/test/test_filter.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1203 2024-03-17 11:24:28.000000 ioiopype-0.0.7/test/test_json.py
+-rw-r--r--   0 martinwalchshoferwalchshofer   (501) staff       (20)     1961 2024-04-05 19:04:55.000000 ioiopype-0.0.7/test/test_realtime_pipe1.py
```

### Comparing `ioiopype-0.0.6/LICENSE` & `ioiopype-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/PKG-INFO` & `ioiopype-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioiopype
-Version: 0.0.6
+Version: 0.0.7
 Summary: A realtime processing framework for python
 Home-page: https://github.com/MartinWalchshofer/ioiopype
 Author: Martin Walchshofer
 Author-email: mwalchshoferyt@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -32,17 +32,24 @@
 ## IONodes
 - Buffer - Buffers data with a defined window size and overlap
 - PWelch - Calculates a Pwelch spectrum from a frame
 - Downsample - Samples a data frame down by a given factor
 - OffsetCorrection - Removes the offset from a data frame
 - ButterworthFilter - Applies a butterworth filter to a sample based signal
 - ToSample - Slices and forwards a data frame into samples
+- Log - Applies a logarithm to the input signal (ln, log10, 10*log10)
+- Square - Squares the input signal
+- Sqrt - Calsulates the square root of the input signal
+- Mux - Concatenates multiple signals into one
+- Operation - Adds, Subtracts, Multiplies, Divides or applies a matrix multiplication
 
 ## ONodes
-- DataGenerator - Generates sample based time series data with configurable frequency and amplitude
+- Constant - forwards constant data with a defined sampling rate
+- NoiseGenerator - Generates gaussian noise as a timeseries signal.
+- SignalGenerator - Generates sample based timeseries signals. Sine, Square, Sawtooth and Triangle signals can be generated
 - Frame - Allows to send a data frame to INodes
 
 ## Supported platforms
 
 | Windows    | Linux    | Mac  |
 | :--------- |:---------| :----|
```

### Comparing `ioiopype-0.0.6/README.md` & `ioiopype-0.0.7/ioiopype.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: ioiopype
+Version: 0.0.7
+Summary: A realtime processing framework for python
+Home-page: https://github.com/MartinWalchshofer/ioiopype
+Author: Martin Walchshofer
+Author-email: mwalchshoferyt@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # IOIOpype
  IOIOpype is processing framework for realtime applications written in python. Data is propergated between Nodes that can be connected via Streams. Nodes can be input nodes 'INode', output nodes 'ONode' or input and output nodes 'IONode'. Algorithms and signal processing pipelines can be prototyped easily by combining multiple nodes.
 
 ## Supported Devices
 - Unicorn Hybrid Black (g.tec medical engineering GmbH)
 - Unicorn Hybrid Black Simulator
 
@@ -15,17 +32,24 @@
 ## IONodes
 - Buffer - Buffers data with a defined window size and overlap
 - PWelch - Calculates a Pwelch spectrum from a frame
 - Downsample - Samples a data frame down by a given factor
 - OffsetCorrection - Removes the offset from a data frame
 - ButterworthFilter - Applies a butterworth filter to a sample based signal
 - ToSample - Slices and forwards a data frame into samples
+- Log - Applies a logarithm to the input signal (ln, log10, 10*log10)
+- Square - Squares the input signal
+- Sqrt - Calsulates the square root of the input signal
+- Mux - Concatenates multiple signals into one
+- Operation - Adds, Subtracts, Multiplies, Divides or applies a matrix multiplication
 
 ## ONodes
-- DataGenerator - Generates sample based time series data with configurable frequency and amplitude
+- Constant - forwards constant data with a defined sampling rate
+- NoiseGenerator - Generates gaussian noise as a timeseries signal.
+- SignalGenerator - Generates sample based timeseries signals. Sine, Square, Sawtooth and Triangle signals can be generated
 - Frame - Allows to send a data frame to INodes
 
 ## Supported platforms
 
 | Windows    | Linux    | Mac  |
 | :--------- |:---------| :----|
 
@@ -88,8 +112,8 @@
 ```
 
 ![Unicorn Hybrid Black - Acquisition and data visualization example](https://github.com/MartinWalchshofer/ioiopype/blob/main/img/example1.png)
 
 ## Contact
 Support this project: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/MartinWalchshofer)<br>
 Join IOIOPype on [Discord](https://discord.gg/pKEumyD9)<br>
-Contact: ```mwalchsoferyt at gmail dot com```
+Contact: ```mwalchsoferyt at gmail dot com```
```

### Comparing `ioiopype-0.0.6/ioiopype/__init__.py` & `ioiopype-0.0.7/ioiopype/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,24 +23,33 @@
 
 #inodes
 from .common.i_nodes.csv_logger import CSVLogger
 from .common.i_nodes.console_log import ConsoleLog
 from .common.i_nodes.to_workspace import ToWorkspace
 
 #onodes
-from .common.o_nodes.data_generator import DataGenerator
+from .common.o_nodes.constant import Constant
+from .common.o_nodes.noise_generator import NoiseGenerator
+from .common.o_nodes.signal_generator import SignalGenerator
 from .common.o_nodes.frame import Frame
 from .common.o_nodes.csv_reader import CSVReader
 
 #ionodes
 from .common.io_nodes.buffer import Buffer
-from .common.io_nodes.pwelch import PWelch
+from .common.io_nodes.butterworth_filter import ButterworthFilter
+from .common.io_nodes.butterworth_filtfilt import ButterworthFiltFilt
 from .common.io_nodes.downsample import Downsample
+from .common.io_nodes.operation import Operation
+#from .common.io_nodes.framer import Framer
+from .common.io_nodes.log import Log
+from .common.io_nodes.mux import Mux
 from .common.io_nodes.offset_correction import OffsetCorrection
-from .common.io_nodes.butterworth_filter import ButterworthFilter
+from .common.io_nodes.pwelch import PWelch
+from .common.io_nodes.sqrt import Sqrt
+from .common.io_nodes.square import Square
 from .common.io_nodes.to_sample import ToSample
 
 #pattern
 from .pattern.i_node import INode
 from .pattern.o_node import ONode
 from .pattern.io_node import IONode
 from .pattern.i_stream import IStream
```

### Comparing `ioiopype-0.0.6/ioiopype/common/i_nodes/console_log.py` & `ioiopype-0.0.7/ioiopype/common/i_nodes/console_log.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/i_nodes/csv_logger.py` & `ioiopype-0.0.7/ioiopype/common/i_nodes/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/i_nodes/to_workspace.py` & `ioiopype-0.0.7/ioiopype/common/i_nodes/to_workspace.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/buffer.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/buffer.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/butterworth_filter.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/butterworth_filter.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/butterworth_filtfilt.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/butterworth_filtfilt.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/downsample.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/downsample.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/framer.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/framer.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/offset_correction.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/offset_correction.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/pwelch.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/pwelch.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,10 @@
             data = self.InputStreams[0].read()
         if data is not None:
             rows = data.shape[0]
             columns = data.shape[1]
             if self.spectrum is None:
                 self.spectrum = np.zeros((rows// 2 + 1, columns))
             frequencies, self.spectrum = sp.welch(data, fs=self.samplingRate, window='hann' ,nperseg=rows, average='median', scaling='spectrum', axis=0)
-            self.spectrum = np.sqrt(self.spectrum)
+            self.spectrum = np.sqrt(self.spectrum*2)
             self.write(0, self.spectrum)   
             self.write(1, frequencies)
```

### Comparing `ioiopype-0.0.6/ioiopype/common/io_nodes/to_sample.py` & `ioiopype-0.0.7/ioiopype/common/io_nodes/to_sample.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/o_devices/unicorn.py` & `ioiopype-0.0.7/ioiopype/common/o_devices/unicorn.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/o_devices/unicorn_simulator.py` & `ioiopype-0.0.7/ioiopype/common/o_devices/unicorn_simulator.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/o_nodes/csv_reader.py` & `ioiopype-0.0.7/ioiopype/common/o_nodes/csv_reader.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/o_nodes/frame.py` & `ioiopype-0.0.7/ioiopype/common/o_nodes/frame.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/utilities/butterworth.py` & `ioiopype-0.0.7/ioiopype/common/utilities/butterworth.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/utilities/overriding_buffer.py` & `ioiopype-0.0.7/ioiopype/common/utilities/overriding_buffer.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/common/utilities/realtime_clock.py` & `ioiopype-0.0.7/ioiopype/common/utilities/realtime_clock.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/desktop/i_nodes/frame_plot.py` & `ioiopype-0.0.7/ioiopype/desktop/i_nodes/frame_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 from ...pattern.i_stream import IStream
 from ...pattern.stream_info import StreamInfo
 from PySide6.QtCore import QObject, Signal, Slot 
 import pyqtgraph as pg
 import numpy as np
 import time
 
-class QTFramePlot(QObject):
-    updateSignal = Signal(np.ndarray)
+class FramePlot(INode):
+    UpdateRateHz = 20
 
-    def __init__(self, samplingRate=1, displayedAmplitude=[]):
-        super(QTFramePlot, self).__init__()
+    class QTFramePlot(QObject):
+        updateSignal = Signal(np.ndarray)
 
-        self.samplingRate = samplingRate
-        self.plotWidget = pg.plot(title="frame plot")
-        if len(displayedAmplitude) == 2:
-            self.plotWidget.setYRange(displayedAmplitude[0], displayedAmplitude[1], 0)
-        elif len(displayedAmplitude) == 1:
-            self.plotWidget.setYRange(-displayedAmplitude[0], displayedAmplitude[0], 0)
-
-        self.x = None
-        self.numberOfChannels = 0
-        self.items = []
-
-        self.updateSignal.connect(self.update_plot)
-
-    @Slot(np.ndarray)
-    def update_plot(self, y):
-        if y is not None:
-            if self.x is None or self.x.shape[0] != y.shape[0]:
-                self.x = np.linspace(1, y.shape[0], y.shape[0])
-                self.x = np.divide(self.x,self.samplingRate)
+        def __init__(self, samplingRate=1, displayedAmplitude=[]):
+            super(FramePlot.QTFramePlot, self).__init__()
 
-            self.numberOfChannels = y.shape[1]
-            if len(self.items) is not self.numberOfChannels:
+            self.samplingRate = samplingRate
+            self.plotWidget = pg.plot(title="frame plot")
+            if len(displayedAmplitude) == 2:
+                self.plotWidget.setYRange(displayedAmplitude[0], displayedAmplitude[1], 0)
+            elif len(displayedAmplitude) == 1:
+                self.plotWidget.setYRange(-displayedAmplitude[0], displayedAmplitude[0], 0)
+
+            self.x = None
+            self.numberOfChannels = 0
+            self.items = []
+
+            self.updateSignal.connect(self.update_plot)
+
+        @Slot(np.ndarray)
+        def update_plot(self, y):
+            if y is not None:
+                if self.x is None or self.x.shape[0] != y.shape[0]:
+                    self.x = np.linspace(1, y.shape[0], y.shape[0])
+                    self.x = np.divide(self.x,self.samplingRate)
+
+                self.numberOfChannels = y.shape[1]
+                if len(self.items) is not self.numberOfChannels:
+                    for i in range(0, self.numberOfChannels):
+                        self.items.append(pg.PlotCurveItem())
+                        self.plotWidget.addItem(self.items[i])
                 for i in range(0, self.numberOfChannels):
-                    self.items.append(pg.PlotCurveItem())
-                    self.plotWidget.addItem(self.items[i])
-            for i in range(0, self.numberOfChannels):
-                self.items[i].setData(x=self.x, y= y[:,i])
-
-class FramePlot(INode):
-    UpdateRateHz = 20
+                    self.items[i].setData(x=self.x, y= y[:,i])
 
     def __init__(self, samplingRate=1, displayedAmplitude=[]):
         super().__init__()
         self.add_i_stream(IStream(StreamInfo(0, 'data', StreamInfo.Datatype.Frame)))
         
         self.__timestamp = 0
         self.__dT = 0
         self.dTS = 1/self.UpdateRateHz
-        self.qto = QTFramePlot(samplingRate, displayedAmplitude)
+        self.qto = FramePlot.QTFramePlot(samplingRate, displayedAmplitude)
 
     def __del__(self):
         super().__del__()
 
     def update(self):
         data = None
         if self.InputStreams[0].DataCount > 0:
```

### Comparing `ioiopype-0.0.6/ioiopype/desktop/i_nodes/sample_plot.py` & `ioiopype-0.0.7/ioiopype/desktop/i_nodes/sample_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
             for i in range(0, self.numberOfChannels):
                 if i % 2 == 0:
                     self.offsets.append(amplitude * (numberOfChannels/2) - amplitude/2 - i*amplitude)
                 else:
                     self.offsets.append(amplitude * ((numberOfChannels/2)-0.5) - i*amplitude)
 
             self.plotWidget = pg.plot(title="sample plot")
-            self.plotWidget.getPlotItem().hideAxis('left')
+            if numberOfChannels > 1:
+                self.plotWidget.getPlotItem().hideAxis('left')
             self.items = []
             for i in range(0, self.numberOfChannels):
                 self.items.append(pg.PlotCurveItem())
                 self.plotWidget.addItem(self.items[i])
 
             minMaxAmplitude = 0
             if self.numberOfChannels % 2 == 0:
```

### Comparing `ioiopype-0.0.6/ioiopype/pattern/i_node.py` & `ioiopype-0.0.7/ioiopype/pattern/i_node.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/pattern/i_stream.py` & `ioiopype-0.0.7/ioiopype/pattern/i_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,24 @@
         self.DataCount : int = 0
         self.StreamInfo = streamInfo
         self.IsConnected = False
         self.__eventHandler : function
         self.__readCnt = 0
     
     def write(self, data):
-        self.__queue.put(data)
+        self.__queue.put(data, block=True, timeout=None)
         self.DataCount = self.__queue.qsize()
         if self.__eventHandler is not None:
             self.__eventHandler()
 
     def read(self):
-        if self.__queue.qsize() > 0:
+        if self.DataCount > 0:
             try:
                 self.__readCnt += 1
-                return self.__queue.get()
+                return self.__queue.get(block=True, timeout=None)
             except:
                 return None
         else:
             return None 
 
     def set_data_available_eventhandler(self, handler):
         self.__eventHandler = handler
```

### Comparing `ioiopype-0.0.6/ioiopype/pattern/o_device.py` & `ioiopype-0.0.7/ioiopype/pattern/o_device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #Copyright © 2024 Martin Walchshofer
 
 from .o_node import ONode
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 
 class ODevice( ONode):
     def __init__(self):
         super().__init__()
 
     def __del__(self):
         super().__del__()
 
     @staticmethod
     @abstractmethod
-    def start_scanning(self):
+    def start_scanning():
         pass
 
     @staticmethod
     @abstractmethod
-    def stop_scanning(self):
+    def stop_scanning():
         pass
 
     @staticmethod
     @abstractmethod
     def add_devices_discovered_eventhandler(handler):
         pass
```

### Comparing `ioiopype-0.0.6/ioiopype/pattern/o_node.py` & `ioiopype-0.0.7/ioiopype/pattern/o_node.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/pattern/o_stream.py` & `ioiopype-0.0.7/ioiopype/pattern/o_stream.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/pattern/stream_info.py` & `ioiopype-0.0.7/ioiopype/pattern/stream_info.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype/utilities/system.py` & `ioiopype-0.0.7/ioiopype/utilities/system.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/ioiopype.egg-info/SOURCES.txt` & `ioiopype-0.0.7/ioiopype.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,31 @@
 ioiopype/common/i_nodes/to_workspace.py
 ioiopype/common/io_nodes/__init__.py
 ioiopype/common/io_nodes/buffer.py
 ioiopype/common/io_nodes/butterworth_filter.py
 ioiopype/common/io_nodes/butterworth_filtfilt.py
 ioiopype/common/io_nodes/downsample.py
 ioiopype/common/io_nodes/framer.py
+ioiopype/common/io_nodes/log.py
+ioiopype/common/io_nodes/mux.py
 ioiopype/common/io_nodes/offset_correction.py
+ioiopype/common/io_nodes/operation.py
 ioiopype/common/io_nodes/pwelch.py
+ioiopype/common/io_nodes/sqrt.py
+ioiopype/common/io_nodes/square.py
 ioiopype/common/io_nodes/to_sample.py
 ioiopype/common/o_devices/__init__.py
 ioiopype/common/o_devices/unicorn.py
 ioiopype/common/o_devices/unicorn_simulator.py
 ioiopype/common/o_nodes/__init__.py
+ioiopype/common/o_nodes/constant.py
 ioiopype/common/o_nodes/csv_reader.py
-ioiopype/common/o_nodes/data_generator.py
 ioiopype/common/o_nodes/frame.py
+ioiopype/common/o_nodes/noise_generator.py
+ioiopype/common/o_nodes/signal_generator.py
 ioiopype/common/utilities/__init__.py
 ioiopype/common/utilities/butterworth.py
 ioiopype/common/utilities/filter_types.py
 ioiopype/common/utilities/overriding_buffer.py
 ioiopype/common/utilities/realtime_clock.py
 ioiopype/desktop/__init__.py
 ioiopype/desktop/i_nodes/__init__.py
```

### Comparing `ioiopype-0.0.6/setup.py` & `ioiopype-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/test/test_filter.py` & `ioiopype-0.0.7/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/test/test_json.py` & `ioiopype-0.0.7/test/test_json.py`

 * *Files identical despite different names*

### Comparing `ioiopype-0.0.6/test/test_realtime_pipe1.py` & `ioiopype-0.0.7/test/test_realtime_pipe1.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,64 +2,60 @@
 
 import sys
 import os
 
 dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.dirname(dir))
 
+from PySide6.QtWidgets import QApplication
 import ioiopype as ioio
 
+app = QApplication(sys.argv)
+
 #initialize nodes
 samplingRate = 250
 numberOfChannels = 8
 signalAmplitude = 10
-signalFrequency = 10
+signalFrequency = 2.7
 signalOffset = 100
-signalNoise = 5
 timesSamplingRate = 4
 bufferSizeInSamples = samplingRate * timesSamplingRate
 bufferOverlapInSamples = samplingRate * timesSamplingRate - 25
-displayedTimeRangeS = 6
+displayedTimeRangeS = 6.5
 displayedAmplitude = 100
 
 #define nodes
-dg = ioio.DataGenerator(samplingRate, numberOfChannels, signalAmplitude=signalAmplitude, signalFrequencyHz=signalFrequency, signalOffset=signalOffset, signalNoise=signalNoise)
+dg = ioio.SignalGenerator(samplingRate, numberOfChannels, ioio.SignalGenerator.SignalMode.Sine, signalAmplitude=signalAmplitude, signalFrequencyHz=signalFrequency, signalOffset=signalOffset)
 buf = ioio.Buffer(numberOfChannels, bufferSizeInSamples, bufferOverlapInSamples)
 oc = ioio.OffsetCorrection(100, mode=ioio.OffsetCorrection.OffsetCorrectionMode.Linear)
 pw = ioio.PWelch(samplingRate)
-fp1 = ioio.FramePlot(samplingRate=4, displayedAmplitude=[0, 10])
+fp1 = ioio.FramePlot(samplingRate=4, displayedAmplitude=[0, 12])
 fp2 = ioio.FramePlot(samplingRate=samplingRate, displayedAmplitude=[-50, 50] )
 sp = ioio.SamplePlot(numberOfChannels, samplingRate, displayedTimeRangeS, displayedAmplitude)
 cl1 = ioio.ConsoleLog()
-cl2 = ioio.ConsoleLog()
-cl3 = ioio.ConsoleLog()
 
 #connect nodes
 dg.connect(0, buf.InputStreams[0])
 buf.connect(0, cl1.InputStreams[0])
 buf.connect(0, oc.InputStreams[0])
 oc.connect(0, pw.InputStreams[0])
 pw.connect(0, fp1.InputStreams[0])
 oc.connect(0, fp2.InputStreams[0])
 dg.connect(0, sp.InputStreams[0])
-dg.connect(1, cl2.InputStreams[0]) 
-dg.connect(1, cl3.InputStreams[0]) 
 
 #start data generation
 dg.start()
 
 print('Press ENTER to terminate the script')
-input()
+app.exec()
 
 #disconnect nodes
 dg.disconnect(0, buf.InputStreams[0])
 buf.disconnect(0, cl1.InputStreams[0])
 buf.disconnect(0, oc.InputStreams[0])
 oc.disconnect(0, pw.InputStreams[0])
 pw.disconnect(0, fp1.InputStreams[0])
 oc.disconnect(0, fp2.InputStreams[0])
 dg.disconnect(0, sp.InputStreams[0])
-dg.disconnect(1, cl2.InputStreams[0]) 
-dg.disconnect(1, cl3.InputStreams[0]) 
 
 #stop data generation
 dg.stop()
```

