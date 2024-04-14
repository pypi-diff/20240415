# Comparing `tmp/pysilico-server-0.20.0.tar.gz` & `tmp/pysilico_server-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysilico-server-0.20.0.tar", last modified: Mon May 30 13:15:46 2022, max compression
+gzip compressed data, was "pysilico_server-0.21.0.tar", last modified: Sun Apr 14 22:06:07 2024, max compression
```

## Comparing `pysilico-server-0.20.0.tar` & `pysilico_server-0.21.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.703376 pysilico-server-0.20.0/pysilico_server/calib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/calib/dark_frame/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/calib/dark_frame/none.fits
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/camera_controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/camera_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/camera_controller/camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/camera_controller/pysilico_run_camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     6957 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/camera_controller/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/conf/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/conf/pysilico_server.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/devices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/abstract_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/avtCamera.py
--rw-r--r--   0 runner    (1001) docker     (121)     4544 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/base_simulated_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/simulated_auxiliary_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     6515 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/devices/simulated_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/process_monitor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/process_monitor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      178 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/process_monitor/pysilico_run_process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/process_monitor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/scripts/pysilico_camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/scripts/pysilico_kill_processes.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/scripts/pysilico_process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/scripts/pysilico_stop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/utils/process_startup_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/pysilico_server/utils/starter_script_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/pysilico_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-30 13:15:46.000000 pysilico-server-0.20.0/pysilico_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/test/controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2822 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/controller/camera_controller_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/test/devices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7205 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/devices/avt_camera_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/devices/hw_avt_camera_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/devices/simulated_auxiliary_camera_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/devices/simulated_pyramid_wfs_camera_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/fake_time_mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.707376 pysilico-server-0.20.0/test/integration/calib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/test/integration/calib/dark_frame/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/integration/calib/dark_frame/none.fits
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 13:15:46.711376 pysilico-server-0.20.0/test/integration/conffiles/
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/integration/conffiles/pysilico_server.conf
--rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/integration/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    17142 2022-05-30 13:15:32.000000 pysilico-server-0.20.0/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.966076 pysilico_server-0.21.0/pysilico_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.966076 pysilico_server-0.21.0/pysilico_server/calib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/calib/dark_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/calib/dark_frame/none.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/camera_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/camera_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/camera_controller/camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/camera_controller/pysilico_run_camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/camera_controller/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/conf/pysilico_server.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/abstract_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/avtCamera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/base_simulated_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/basler_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/simulated_auxiliary_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/devices/simulated_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/process_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/process_monitor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/process_monitor/pysilico_run_process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/process_monitor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.970075 pysilico_server-0.21.0/pysilico_server/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/scripts/pysilico_camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/scripts/pysilico_kill_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/scripts/pysilico_process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/scripts/pysilico_stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/pysilico_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/utils/process_startup_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/pysilico_server/utils/starter_script_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/pysilico_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 22:06:07.000000 pysilico_server-0.21.0/pysilico_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/controller/camera_controller_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/devices/avt_camera_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/devices/hw_avt_camera_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/devices/simulated_auxiliary_camera_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/devices/simulated_pyramid_wfs_camera_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/fake_time_mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.966076 pysilico_server-0.21.0/test/integration/calib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/integration/calib/dark_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/integration/calib/dark_frame/none.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:06:07.974076 pysilico_server-0.21.0/test/integration/conffiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/integration/conffiles/pysilico_server.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/integration/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-04-14 22:05:58.000000 pysilico_server-0.21.0/test/test_helper.py
```

### Comparing `pysilico-server-0.20.0/LICENSE` & `pysilico_server-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/PKG-INFO` & `pysilico_server-0.21.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: pysilico-server
-Version: 0.20.0
+Version: 0.21.0
 Summary: AVT-Prosilica camera controller with PLICO
 Home-page: https://github.com/lbusoni/pysilico_server
 Author: Lorenzo Busoni
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: plico,Prosilica,AVT,camera,laboratory,instrumentation control
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: plico>=0.25
+Requires-Dist: pysilico>=0.19
+Requires-Dist: numpy
+Requires-Dist: psutil
+Requires-Dist: six
+Requires-Dist: rebin
 
 # PYSILICO server: Prosilica AVT camera controller for Plico
 
  ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico_server/workflows/Python%20package/badge.svg)
  [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server)
  [![Documentation Status](https://readthedocs.org/projects/pysilico_server/badge/?version=latest)](https://pysilico_server.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version][pypiversion]][pypiversionlink]
```

### Comparing `pysilico-server-0.20.0/README.md` & `pysilico_server-0.21.0/README.md`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/pysilico_server/camera_controller/camera_controller.py` & `pysilico_server-0.21.0/pysilico_server/camera_controller/camera_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         self._rpcHandler.sendCameraFrame(self._publisherSocket, correctedFrame)
         self._logger.debug('frame %d published' % correctedFrame.counter())
         self._publishForDisplay(correctedFrame)
 
     def _downsizeForDisplay(self, frame):
         DISPLAY_FRAME_SIZE = 256.
         minSize = np.min(frame.toNumpyArray().shape)
-        downsizeBy = np.int(np.ceil(
+        downsizeBy = int(np.ceil(
             minSize / DISPLAY_FRAME_SIZE))
         if downsizeBy > 1:
             array = self._downsizeBySampling(frame.toNumpyArray(),
                                              downsizeBy)
         else:
             array = frame.toNumpyArray()
         return CameraFrame.fromNumpyArray(np.float32(array),
```

### Comparing `pysilico-server-0.20.0/pysilico_server/camera_controller/runner.py` & `pysilico_server-0.21.0/pysilico_server/camera_controller/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import os
 import time
 from plico.utils.base_runner import BaseRunner
+from pysilico_server.devices.abstract_camera import CameraException
 from pysilico_server.devices.simulated_camera import \
     SimulatedPyramidWfsCamera
 from pysilico_server.devices.simulated_auxiliary_camera import \
     SimulatedAuxiliaryCamera
 from plico.utils.logger import Logger
 from plico.utils.control_loop import IntolerantControlLoop
 from plico.utils.decorator import override
 from pysilico_server.camera_controller.camera_controller import \
     CameraController
 from plico.rpc.zmq_ports import ZmqPorts
 import functools
-
-class CameraException(Exception):
-    '''Custom exception class in order to avoid
-       exposing the Vimba namespace outside the context wrapper'''
-    pass
+import traceback
 
 
 def ContextWrapper():
     def wrapperFunc(f):
         @functools.wraps(f)
         def wrapper_vimba(self, *args, **kwds):
             import vimba
@@ -68,14 +65,16 @@
         if cameraModel == 'simulatedPyramidWfsCamera':
             self._createSimulatedPyramidWfsCamera(cameraDeviceSection)
         elif cameraModel == 'simulatedAuxiliaryCamera':
             self._createSimulatedAuxiliaryCamera(cameraDeviceSection)
         elif cameraModel == 'avt':
             self._use_vimba_wrapper = True
             self._createAvtCamera(cameraDeviceSection)
+        elif cameraModel == 'basler':
+            self._createBaslerCamera(cameraDeviceSection)
         else:
             raise KeyError('Unsupported camera model %s' % cameraModel)
 
     def _createSimulatedPyramidWfsCamera(self, cameraDeviceSection):
         cameraName = self.configuration.deviceName(cameraDeviceSection)
         self._camera = SimulatedPyramidWfsCamera(cameraName)
         self._setBinning(cameraDeviceSection)
@@ -96,14 +95,22 @@
         cameraName = self.configuration.deviceName(cameraDeviceSection)
         with Vimba.get_instance() as v:
             self._vimbacamera = v.get_camera_by_id(ipAddress)
         self._camera = AvtCamera(self._vimbacamera, cameraName)
         self._camera.setStreamBytesPerSecond(streamBytesPerSecond)
         self._setBinning(cameraDeviceSection)
 
+    def _createBaslerCamera(self, cameraDeviceSection):
+        from pysilico_server.devices import basler_camera
+        ipAddress = self.configuration.getValue(cameraDeviceSection,
+                                                'ip_address')
+        cameraName = self.configuration.deviceName(cameraDeviceSection)
+        self._baslercamera = basler_camera.get_device_by_ip(ipAddress)
+        self._camera = basler_camera.BaslerCamera(self._baslercamera, cameraName)
+
     def _setBinning(self, cameraDeviceSection):
         try:
             binning = self.configuration.getValue(
                 cameraDeviceSection, 'binning', getint=True)
             self._camera.setBinning(binning)
         except Exception:
             self._logger.warn(
@@ -172,14 +179,15 @@
                 # Wait a little bit and try to reconnect
                 self._logger.warn(e)
                 if hasattr(self, '_vimbacamera'):
                     delattr(self, '_vimbacamera')
                 time.sleep(1)
             except Exception as e:
                 self._logger.fatal('Unhandled exception: '+str(e))
+                traceback.print_exc()
                 self._isTerminated = True
         return os.EX_OK
 
     @override
     def terminate(self, signal, frame):
         self._isTerminated = True
         if hasattr(self, '_controller'):
```

### Comparing `pysilico-server-0.20.0/pysilico_server/conf/pysilico_server.conf` & `pysilico_server-0.21.0/pysilico_server/conf/pysilico_server.conf`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 [deviceAuxCameraAvt]
 name= AVT Aux Camera
 model= avt
 ip_address= 192.168.29.157
 streambytespersecond= 50000000
 binning= 4
 
+[deviceBaslerCamera]
+name=Baslers Camera
+model= basler
+ip_address= 193.206.155.38
+
 [camera1]
 name= AVT 1 server
 log_level= info
 camera= deviceAuxCameraSimulated
 host= localhost
 port= 7100
```

### Comparing `pysilico-server-0.20.0/pysilico_server/devices/abstract_camera.py` & `pysilico_server-0.21.0/pysilico_server/devices/abstract_camera.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import numpy
 from plico.utils.decorator import returns
 
 
 __version__= "$Id: abstract_camera.py 268 2017-04-12 21:54:14Z lbusoni $"
 
 
+class CameraException(Exception):
+    '''Custom exception class in order to avoid
+       exposing the Vimba namespace outside the context wrapper'''
+    pass
+
 class AbstractCamera(with_metaclass(abc.ABCMeta, object)):
 
     @abc.abstractmethod
     def name(self):
         assert False
 
     @abc.abstractmethod
@@ -59,9 +64,17 @@
         assert False
 
     @abc.abstractmethod
     def getFrameCounter(self):
         assert False
 
     @abc.abstractmethod
+    def getFrameRate(self):
+        assert False
+
+    @abc.abstractmethod
+    def setFrameRate(self, frameRateInHz):
+        assert False
+
+    @abc.abstractmethod
     def deinitialize(self):
         assert False
```

### Comparing `pysilico-server-0.20.0/pysilico_server/devices/avtCamera.py` & `pysilico_server-0.21.0/pysilico_server/devices/avtCamera.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,17 +61,23 @@
         self._callbackList = []
         self._mutex = threading.RLock()
         self._lastValidFrame = CameraFrame(np.zeros((4, 4)), counter=0)
         self._initialize()
 
     @withVimba()
     def _initialize(self):
+        # Identify if the camera is one of the Alvium models
+        self._isAlvium = (self._camera.get_name().lower()[0:6] == 'alvium')
 
         # Limit data rate from camera as a default
-        self.setStreamBytesPerSecond(10000000)
+        if self._isAlvium:
+            # Alvium G1 has a higher min value for stream bps
+            self.setStreamBytesPerSecond(32375000)
+        else:
+            self.setStreamBytesPerSecond(10000000)
 
         self._resetBinningAndOffset()
 
         if self.pixelFormat() == PixelFormat.Mono12:
             self.BYTES_PER_PIXEL = 2
             self._dtype = np.uint16
         else:
@@ -106,16 +112,19 @@
 
         restartAcquistion = False
         if self._isContinuouslyAcquiring:
             self.stopAcquisition()
             restartAcquistion = True
 
         if self._isBinningAvailable():
-            self._camera.BinningHorizontal.set(self._binning)
+            # Vertical to be set before Horizontal binning because
+            # in some cameras the Horizontal binning value could have
+            # constraints given by the Vertical binning setting.
             self._camera.BinningVertical.set(self._binning)
+            self._camera.BinningHorizontal.set(self._binning)
         elif self._isDecimationAvailable():
             self._camera.DecimationHorizontal.set(self._binning)
             self._camera.DecimationVertical.set(self._binning)
         else:
             raise Exception("Neither binning nor decimation available")
 
         self._camera.OffsetX.set(0)
@@ -142,42 +151,51 @@
     def _logCameraInfo(self):
         self._logger.notice('Camera: %s at %s - ID: %s' % (
                             self.deviceModelName(),
                             self.ipAddress(),
                             self.deviceID()))
         self._logger.notice('Sensor is %d rows x %d cols, %d bits/pixel' % (
             self._camera.SensorHeight.get(),
-            self._camera.SensorWidth.get(), self._camera.SensorBits.get()))
+            self._camera.SensorWidth.get(), self.bpp()))
         self._logger.notice('Output format is %s' % self.pixelFormat())
         self._logger.notice('Exposure time is %f ms' % self.exposureTime())
 
     @synchronized("_mutex")
     @withCamera()
     def setStreamBytesPerSecond(self, streamBytesPerSecond):
         try:
             self._camera.StreamBytesPerSecond.set(streamBytesPerSecond)
         except AttributeError:
             try:
                 # Some cameras use a different name
                 self._camera.DeviceLinkThroughputLimit.set(streamBytesPerSecond)
+                self._camera.DeviceLinkThroughputLimitMode.set('On')
+                mode_entry = self._camera.DeviceLinkThroughputLimitMode.get()
+                self._logger.notice('Device Link Trhougput Mode set to: '+str(mode_entry))
             except AttributeError:
                 # If we can't set it, return silently and
                 # avoid the logging notice
+                self._logger.notice('No Attribute for setting StreamBytesPerSecond')
                 return
         self._logger.notice('Camera data rate set to %4.1f MB/s'
                              % (streamBytesPerSecond / 1e6))
 
     @synchronized("_mutex")
     @withCamera()
     def getStreamBytesPerSecond(self):
         try:
             return self._camera.StreamBytesPerSecond.get()
         except AttributeError:
-            # Some cameras do not have this attribute
-            return 0
+            try:
+                # Some cameras use a different name
+                self._camera.DeviceLinkThroughputLimit.get()
+            except AttributeError:
+                # Some cameras do not have this attribute.
+                # Zero is returned in this case.
+                return 0
 
     @override
     def setBinning(self, binning):
         self._binning = binning
         self._resetBinningAndOffset()
 
     @override
@@ -211,15 +229,29 @@
     @withCamera()
     def cols(self):
         return self._camera.Width.get()
 
     @synchronized("_mutex")
     @withCamera()
     def bpp(self):
-        return self._camera.SensorBits.get()
+        if self._isAlvium:
+            bpp_str = str(self._camera.SensorBitDepth.get())
+            # Alvium typ cameras return a str: Bpp8, Bpp10 or Bpp12
+            if bpp_str == 'Bpp8':
+                return 8
+            elif bpp_str == 'Bpp10':
+                return 10
+            elif bpp_str == 'Bpp12':
+                return 12
+            else:
+                # In case of Adaptive or other unsupported EnumEntry
+                raise Exception('Unsupported SesnorBitDepth setting: '+bpp_str)
+        else:
+            return self._camera.SensorBits.get()
+             
 
     @synchronized("_mutex")
     @withCamera()
     def pixelFormat(self):
         return self._camera.get_pixel_format()
 
     @override
@@ -258,23 +290,34 @@
             # Some cameras use AcquisitionFrameRate, others AcquisitionFrameRateAbs. We try both.
             return self._camera.AcquisitionFrameRate.get()
 
     @override
     @synchronized("_mutex")
     @withCamera()
     def setFrameRate(self, frameRate):
-        try:
-            self._camera.AcquisitionFrameRateAbs.set(np.minimum(
-                frameRate,
-                self._maximum_frame_rate()))
-        except AttributeError:
-            # Some cameras use AcquisitionFrameRate, others AcquisitionFrameRateAbs. We try both.
-            self._camera.AcquisitionFrameRate.set(np.minimum(
-                frameRate,
-                self._maximum_frame_rate()))
+        if self._isAlvium:
+            isFrameRateReadOnly = not self._camera.AcquisitionFrameRateEnable.get() 
+            if isFrameRateReadOnly:
+                expTimeInUs = 1e6/frameRate
+                expTimeRange = self._camera.ExposureTime.get_range()
+                expTimeInRange = np.min([expTimeInUs, expTimeRange[1]])
+                expTimeInRange = np.max([expTimeInRange, expTimeRange[0]])
+                self.setExposureTime(1e-3 * expTimeInRange)
+            else:
+                self._camera.AcquisitionFrameRate.set(frameRate)
+        else:
+            try:
+                self._camera.AcquisitionFrameRateAbs.set(np.minimum(
+                    frameRate,
+                    self._maximum_frame_rate()))
+            except AttributeError:
+                # Some cameras use AcquisitionFrameRate, others AcquisitionFrameRateAbs. We try both.
+                self._camera.AcquisitionFrameRate.set(np.minimum(
+                    frameRate,
+                    self._maximum_frame_rate()))
         self._logger.notice('Frame rate set to %g Hz - (requested %g Hz)'
                             % (self.getFrameRate(), frameRate))
 
     def readFrame(self, timeoutMilliSec=2000):
         pass
 
     def _notifyListenersAboutNewFrame(self):
@@ -283,18 +326,21 @@
 
     def _frame_callback(self, camera, frame):
         try:
             # self._logger.debug("Got frame %d at time %.3f" % (
             #    self._counter, frame.get_timestamp() /
             #    self._timeStampTickFrequency))
             if frame.get_status() == FrameStatus.Complete:
+                h, w = frame.get_height(), frame.get_width() 
                 frame_data = frame.get_buffer()
+                self._logger.debug('Frame size H x W: %g x %g' 
+                                   % (h, w))
                 img = np.ndarray(buffer=frame_data,
                                  dtype=self._dtype,
-                                 shape=(frame.get_height(), frame.get_width()))
+                                 shape=(h, w))
                 self._lastValidFrame = CameraFrame(img, counter=self._counter)
                 self._notifyListenersAboutNewFrame()
                 self._counter += 1
             else:
                 self._logger.warn(
                     "Frame status not complete. "
                     "Try to reduce streamBytesPerSecond value")
@@ -310,32 +356,46 @@
 
             while not self._camera.GVSPAdjustPacketSize.is_done():
                 pass
 
         except (AttributeError, VimbaFeatureError):
             pass
 
+
     def _maximum_frame_rate(self):
+        if self._isAlvium:
+            frame_rate_range = self._camera.AcquisitionFrameRate.get_range() 
+            self._logger.debug('_maximum_frame_rate: Framerate Range [Hz] (%g, %g)' 
+                                % frame_rate_range)
+            maxFrameRate = frame_rate_range[1]
+        else:
+            maxFrameRate =  self._camera.AcquisitionFrameRateLimit.get()
         aLittleBitSlower = 0.01
-        return self._camera.AcquisitionFrameRateLimit.get() - aLittleBitSlower
+        return maxFrameRate - aLittleBitSlower
+    
 
     @withCamera()
     def startAcquisition(self):
         self._adjust_packet_size()
         self._camera.TriggerSelector.set('FrameStart')
-        self._camera.TriggerSource.set('FixedRate')
+        if self._isAlvium:
+            self._camera.TriggerSource.set('Software')
+        else:
+            self._camera.TriggerSource.set('FixedRate')
         self._camera.AcquisitionMode.set('Continuous')
         self.setFrameRate(self._maximum_frame_rate())
         try:
             self._camera.SyncOutSelector.set('SyncOut1')
             self._camera.SyncOutSource.set('Exposing')
         except AttributeError:
             pass
         self._camera.start_streaming(
             handler=self._frame_callback, buffer_count=10)
+        if self._isAlvium:
+            self._camera.TriggerSoftware.run()
         self._logger.notice('Continuous acquisition started')
         self._isContinuouslyAcquiring = True
 
     @withCamera()
     def stopAcquisition(self):
         self._isContinuouslyAcquiring = False
         # self._stopAcquisitionAndFlushQueue()
```

### Comparing `pysilico-server-0.20.0/pysilico_server/devices/base_simulated_camera.py` & `pysilico_server-0.21.0/pysilico_server/devices/base_simulated_camera.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,195 +4,166 @@
 from pysilico_server.devices.abstract_camera import AbstractCamera
 from plico.utils.logger import Logger
 from plico.utils.concurrent_loop import ConcurrentLoop
 from plico.utils.convergeable import Convergeable
 from pysilico.types.camera_frame import CameraFrame
 
 
-__version__= "$Id: $"
-
-
-
 class SimulatedFrameProducer(Convergeable):
 
     def __init__(self, simulatedCamera):
-        self._camera= simulatedCamera
-
-        self._cycleCounter= 0
-        self._logger= Logger.of("SimulatedFrameProducer")
+        self._camera = simulatedCamera
 
+        self._cycleCounter = 0
+        self._logger = Logger.of("SimulatedFrameProducer")
 
     @override
     @returns(bool)
     def hasConverged(self):
         return False
 
-
     @override
     def performOneConvergenceStep(self):
         self._camera.produceFrame()
         self._cycleCounter += 1
 
-
     @override
     def measureConvergence(self):
         pass
 
 
-
-
 class BaseSimulatedCamera(AbstractCamera):
-    SENSOR_H= 1024
-    SENSOR_W= 1360
-    DTYPE= np.uint16
-    MAX_VALUE= 4096
-
+    SENSOR_H = 1024
+    SENSOR_W = 1360
+    DTYPE = np.uint16
+    MAX_VALUE = 4096
 
     def __init__(self, name='Simulated Camera'):
-        self._name= name
-        self._logger= Logger.of('SimulatedCamera')
-        self._counter= 0
-        self._delay= 0.00
-        self._exposureTimeMs= 10.0
-        self._frameRate= 1000./ self._exposureTimeMs
-        self._binning= 1
-        self._totalFluxPerMilliSecond= 2e6
-        self._noiseInCount= 10.
+        self._name = name
+        self._logger = Logger.of('SimulatedCamera')
+        self._counter = 0
+        self._delay = 0.00
+        self._exposureTimeMs = 10.0
+        self._frameRate = 1000. / self._exposureTimeMs
+        self._binning = 1
+        self._totalFluxPerMilliSecond = 2e6
+        self._noiseInCount = 10.
 
-        self._lastValidFrame= None
-        self._callbackList= []
+        self._lastValidFrame = None
+        self._callbackList = []
         self._buildFrameProducerLoop()
 
         self._logger.notice('Simulated camera initialized')
         self._logger.notice('Sensor size (H,W) %s %s' % (
             self.SENSOR_H, self.SENSOR_W))
-        self._raiseExceptionOnDeinitialize= False
-
+        self._raiseExceptionOnDeinitialize = False
 
     def raiseExceptionOnDeinitialize(self, trueOrFalse):
-        self._raiseExceptionOnDeinitialize= trueOrFalse
-
+        self._raiseExceptionOnDeinitialize = trueOrFalse
 
     def _buildFrameProducerLoop(self):
-        self._frameProducer= SimulatedFrameProducer(self)
-        self._frameProducerLoop= ConcurrentLoop(
-            "SimulatedFrameProducerLoop", self._frameProducer, 0.01,
+        self._frameProducer = SimulatedFrameProducer(self)
+        self._frameProducerLoop = ConcurrentLoop(
+            "SimulatedFrameProducerLoop", self._frameProducer, 0.0001,
             self._logger.error)
         self._frameProducerLoop.initialize()
 
-
     def _notifyListenersAboutNewFrame(self):
         for callback in self._callbackList:
             callback(self._lastValidFrame)
 
-
     def produceFrame(self):
-        frame= self._computeFrameFromWavefront()
-        self._lastValidFrame= CameraFrame(frame, self._counter)
+        self._logger.debug('Enter produceFrame')
+        frame = self._computeFrameFromWavefront()
+        self._counter += 1
+        self._lastValidFrame = CameraFrame(frame, self._counter)
         self._notifyListenersAboutNewFrame()
-        self._counter+= 1
-
+        self._logger.debug('Exit produceFrame. Counter: %d' % self._counter)
 
     @override
     def deinitialize(self):
         if self._raiseExceptionOnDeinitialize:
             raise Exception('Asked to fail on deinitialize')
         else:
             self._frameProducerLoop.deinitialize()
 
-
     @override
     def startAcquisition(self):
         self._frameProducerLoop.close()
 
-
     @override
     def stopAcquisition(self):
         self._frameProducerLoop.open()
 
+    def acquisitionIsStopped(self):
+        pass
 
     @override
     def registerCallback(self, callback):
         self._callbackList.append(callback)
 
-
     def frameCounter(self):
         return self._counter
 
-
     @override
     def name(self):
         return self._name
 
-
     @override
     def rows(self):
-        return int(float(self.SENSOR_H)/ self._binning)
-
+        return int(float(self.SENSOR_H) / self._binning)
 
     @override
     def cols(self):
-        return int(float(self.SENSOR_W)/ self._binning)
-
+        return int(float(self.SENSOR_W) / self._binning)
 
     @override
     def dtype(self):
         return self.DTYPE
 
-
     @override
     @returns(np.ndarray)
     def readFrame(self, timeoutMilliSec=2000):
         return self._computeFrameFromWavefront()
 
-
     def setNoiseInCount(self, noise):
-        self._noiseInCount= noise
-
+        self._noiseInCount = noise
 
     def setTotalFluxPerMilliSecond(self, totalFluxPerMilliSec):
-        self._totalFluxPerMilliSecond= totalFluxPerMilliSec
-
+        self._totalFluxPerMilliSecond = totalFluxPerMilliSec
 
     def _computeFrameFromWavefront(self):
         pixels = np.zeros((self.rows(), self.cols()),
                           dtype=np.float)
 
         self._counter += 1
-        time.sleep(1./ self.getFrameRate())
+        time.sleep(1. / self.getFrameRate())
         return pixels.astype(self.DTYPE)
 
-
     @override
     def setExposureTime(self, exposureTimeInMilliSeconds):
-        self._exposureTimeMs= exposureTimeInMilliSeconds
-
+        self._exposureTimeMs = exposureTimeInMilliSeconds
 
     @override
     def exposureTime(self):
         return self._exposureTimeMs
 
-
     @override
     def setBinning(self, binning):
         self._logger.notice("setting binning to %d" % binning)
-        self._binning= binning
-
+        self._binning = binning
 
     @override
     def getBinning(self):
         return self._binning
 
-
     @override
     def getFrameRate(self):
         return self._frameRate
 
-
     @override
     def setFrameRate(self, frameRate):
-        self._frameRate= frameRate
-
+        self._frameRate = frameRate
 
     @override
     def getFrameCounter(self):
         return self._counter
```

### Comparing `pysilico-server-0.20.0/pysilico_server/devices/simulated_auxiliary_camera.py` & `pysilico_server-0.21.0/pysilico_server/devices/simulated_auxiliary_camera.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python
 
 import numpy as np
 import time
-from rebin import rebin
 from pysilico_server.devices.base_simulated_camera import BaseSimulatedCamera
 
-__version__ = "$Id: simulated_camera.py 203 2017-01-16 11:30:46Z lbusoni $"
-
 
 class SimulatedAuxiliaryCamera(BaseSimulatedCamera):
 
     def __init__(self, name='SimulatedAuxiliaryCamera'):
         BaseSimulatedCamera.__init__(self, name)
         self._totalFluxPerMilliSecond = 1e5
         self.setFrameRate(3)
```

### Comparing `pysilico-server-0.20.0/pysilico_server/devices/simulated_camera.py` & `pysilico_server-0.21.0/pysilico_server/devices/simulated_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 import time
 from rebin import rebin
 from plico.utils.zernike_generator import ZernikeGenerator
 from plico.types.zernike_coefficients import ZernikeCoefficients
 from pysilico_server.devices.base_simulated_camera import BaseSimulatedCamera
+from plico.utils.decorator import logEnterAndExit
 
 __version__ = "$Id: simulated_camera.py 293 2017-06-21 17:10:57Z lbusoni $"
 
 
 class SimulatedPyramidWfsCamera(BaseSimulatedCamera):
     SENSOR_H = 1024
     SENSOR_W = 1360
@@ -18,61 +19,63 @@
 
     def __init__(self, name='Simulated Pyramid Wfs Camera'):
         BaseSimulatedCamera.__init__(self, name)
         self._pupilRadius = None
         pupilsSeparation = 520
         opticalAxis = (self.SENSOR_H / 2, self.SENSOR_W / 2)
         self._pupilsCenter = self._computeCenters(pupilsSeparation,
-                                                 opticalAxis)
+                                                  opticalAxis)
         self._tipTiltCoefficients = np.zeros(2)
         self._wavefront = None
         self._zernikeGenerator = None
 
         self.setPupilsRadiusInUnbinnedPixels(80)
         self.setScaleInMeterPerPixel(
             10e-3 / (2 * self.getPupilsRadiusInUnbinnedPixels()))
         self.setSlopeSaturationInRadians(40e-3)
 
         self._logger.notice('Pupil centers %s' % (self._pupilsCenter))
         self._logger.notice('Pupil radius %s' % (self._pupilRadius))
+        self.setFrameRate(3)
 
     def setPupilsRadiusInUnbinnedPixels(self, radius):
         self._pupilRadius = radius
-        self._wavefront = np.zeros((2 * self._pupilRadius, 2 * self._pupilRadius))
+        self._wavefront = np.zeros(
+            (2 * self._pupilRadius, 2 * self._pupilRadius))
         self._zernikeGenerator = ZernikeGenerator(2 * self._pupilRadius)
 
     def getPupilsRadiusInUnbinnedPixels(self):
         return self._pupilRadius
 
     def setTilt(self, tipTiltCoefficients):
         self._tipTiltCoefficients = tipTiltCoefficients
 
     def setWavefront(self, wavefront):
         self._wavefront = wavefront
 
     def _computeWavefrontFromZernikeCoefficients(self, coeff, zg):
-        wf = 0.* zg.getZernike(1)
+        wf = 0. * zg.getZernike(1)
         for y in coeff.zernikeIndexes():
             wf += coeff.getZ([y]) * zg.getZernike(y)
         return wf
 
     def setWavefrontFromZernikeVector(self, zernikeVector):
         wf = self._computeWavefrontFromZernikeCoefficients(
             ZernikeCoefficients.fromNumpyArray(np.array(zernikeVector)),
             self._zernikeGenerator)
         self.setWavefront(wf)
 
     def _computeCenters(self, pupilsSeparation, opticalAxis):
         pupDist = int(0.5 * pupilsSeparation)
         center = opticalAxis
         res = np.zeros((4, 2))
-        res[0,:] = [center[0] + pupDist, center[1] - pupDist]
-        res[1,:] = [center[0] + pupDist, center[1] + pupDist]
-        res[2,:] = [center[0] - pupDist, center[1] - pupDist]
-        res[3,:] = [center[0] - pupDist, center[1] + pupDist]
+        res[0, :] = [center[0] + pupDist, center[1] - pupDist]
+        res[1, :] = [center[0] + pupDist, center[1] + pupDist]
+        res[2, :] = [center[0] - pupDist, center[1] - pupDist]
+        res[3, :] = [center[0] - pupDist, center[1] + pupDist]
         return res
 
     def setPupilsCenterInUnbinnedPixels(self, centers):
         assert centers.shape == (4, 2)
         self._pupilsCenter = centers
 
     def getPupilsCenterInUnbinnedPixels(self):
@@ -90,39 +93,42 @@
             "tl,tr,bl,br %g,%g,%g,%g - z2,z3: %g,%g" %
             (tl, tr, bl, br, (tr + br - tl - bl) / tot,
              (tl + tr - bl - br) / tot))
         return tl, tr, bl, br
 
     def _pupilImagesFromWavefront(self, wavefront):
         Amat = np.array([[1., 0, 1, 0],
-                        [0., 1, 0, 1],
-                        [0., 0, 1, 1],
-                        [1., 1, 0, 0]])
+                         [0., 1, 0, 1],
+                         [0., 0, 1, 1],
+                         [1., 1, 0, 0]])
 
         (dyMap, dxMap) = np.gradient(wavefront / self._scaleInMeterPerPixel)
         dxMapClipped = dxMap.clip(min=-self._slopeSaturationInRad,
-                                 max=self._slopeSaturationInRad)
+                                  max=self._slopeSaturationInRad)
         dyMapClipped = dyMap.clip(min=-self._slopeSaturationInRad,
-                                 max=self._slopeSaturationInRad)
+                                  max=self._slopeSaturationInRad)
         dx = 2. / np.pi * np.arcsin(dxMapClipped / self._slopeSaturationInRad)
         dy = 2. / np.pi * np.arcsin(dyMapClipped / self._slopeSaturationInRad)
         (sz0, sz1) = dxMap.shape
-        totalIntensity = 1.* sz0 * sz1
+        totalIntensity = 1. * sz0 * sz1
         B = totalIntensity / (sz0 * sz1) / 2 * np.array(
             [1 - dx, 1 + dx, 1 - dy, 1 + dy])
 
         res = np.linalg.lstsq(Amat, B.reshape((4, sz0 * sz1)), rcond=-1)
         pupils = res[0].reshape((4, sz0, sz1))
 
         if isinstance(wavefront, np.ma.MaskedArray):
             for i in range(4):
                 pupils[i][wavefront.mask] = 0
 
         return pupils
 
+    @logEnterAndExit('Enter _computeFrameFromWavefront',
+                     'Exit _computeFrameFromWavefront',
+                     level='debug')
     def _computeFrameFromWavefront(self):
         radius = self._pupilRadius
         cc = self._pupilsCenter
         maxNoiseInCount = self._noiseInCount
 
         pupils = self._pupilImagesFromWavefront(self._wavefront)
         pixels = np.zeros((self.SENSOR_H, self.SENSOR_W),
@@ -147,15 +153,14 @@
                 maxNoiseInCount,
                 size=(self.SENSOR_H, self.SENSOR_W))
 
         if self._binning != 1:
             pixels = rebin(pixels, self._binning) * self._binning ** 2
         pixels = pixels.clip(min=0, max=self.MAX_VALUE)
 
-        self._counter += 1
         time.sleep(1. / self.getFrameRate())
         return pixels.astype(self.DTYPE)
 
     def setSlopeSaturationInRadians(self, slopeSaturationInRadians):
         self._slopeSaturationInRad = slopeSaturationInRadians
 
     def getSlopeSaturationInRadians(self):
```

### Comparing `pysilico-server-0.20.0/pysilico_server/process_monitor/runner.py` & `pysilico_server-0.21.0/pysilico_server/process_monitor/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,69 +10,58 @@
 from plico.utils.decorator import override
 from plico.utils.logger import Logger
 from pysilico_server.utils.process_startup_helper import \
     ProcessStartUpHelper
 from pysilico_server.utils.constants import Constants
 
 
-__version__ = "$Id: runner.py 31 2018-01-27 10:47:29Z lbusoni $"
-
-
-
 class Runner(BaseRunner):
 
     RUNNING_MESSAGE = "Monitor of processes is running."
 
     def __init__(self):
         BaseRunner.__init__(self)
 
-        self._logger= None
-        self._processes= []
-        self._timeToDie= False
-        self._psh= ProcessStartUpHelper()
-
+        self._logger = None
+        self._processes = []
+        self._timeToDie = False
+        self._psh = ProcessStartUpHelper()
 
     def _determineInstalledBinaryDir(self):
         try:
-            self._binFolder= self._configuration.getValue(
+            self._binFolder = self._configuration.getValue(
                 Constants.PROCESS_MONITOR_CONFIG_SECTION,
                 'binaries_installation_directory')
         except KeyError:
-            self._binFolder= None
-
+            self._binFolder = None
 
     def _logRunning(self):
         self._logger.notice(self.RUNNING_MESSAGE)
         sys.stdout.flush()
 
-
     def _setSignalIntHandler(self):
         signal.signal(signal.SIGINT, self._signalHandling)
 
-
     def _signalHandling(self, signalNumber, stackFrame):
         self._logger.notice("Received signal %d (%s)" %
                             (signalNumber, str(stackFrame)))
         if signalNumber == signal.SIGINT:
-            self._timeToDie= True
-
-
-
+            self._timeToDie = True
 
     def _terminateAll(self):
 
         def on_terminate(proc):
             self._logger.notice(
                 "process {} terminated with exit code {}".
                 format(proc, proc.returncode))
 
         self._logger.notice("Terminating all subprocesses using psutil")
         self._logger.notice("My pid %d" % os.getpid())
-        parent= psutil.Process(os.getpid())
-        processes= parent.children(recursive=True)
+        parent = psutil.Process(os.getpid())
+        processes = parent.children(recursive=True)
         for process in processes:
             try:
                 self._logger.notice(
                     "Killing pid %d %s" % (process.pid, process.cmdline()))
                 process.send_signal(signal.SIGTERM)
             except Exception as e:
                 self._logger.error("Failed killing process %s: %s" %
@@ -83,49 +72,44 @@
         if alive:
             for p in alive:
                 self._logger.notice(
                     "process %s survived SIGTERM; giving up" % str(p))
 
         self._logger.notice("terminated all")
 
-
-
     def _spawnController(self, name, section):
         if self._binFolder:
-            cmd= [os.path.join(self._binFolder, name)]
+            cmd = [os.path.join(self._binFolder, name)]
         else:
-            cmd= [name]
+            cmd = [name]
         cmd += [self._configuration._filename, section]
-        self._logger.notice("MirrorController cmd is %s" % cmd)
-        mirrorController= subprocess.Popen(cmd)
+        self._logger.notice("Controller cmd is %s" % cmd)
+        mirrorController = subprocess.Popen(cmd)
         self._processes.append(mirrorController)
         return mirrorController
 
-
     def _setup(self):
-        self._logger= Logger.of("Process monitor runner")
+        self._logger = Logger.of("Process monitor runner")
         self._setSignalIntHandler()
         self._logger.notice("Creating controller processes")
         self._determineInstalledBinaryDir()
-        sections = self._configuration.numberedSectionList(prefix='camera')
+        sections = self._configuration.numberedSectionList(
+            prefix=Constants.SERVER_CONFIG_SECTION_PREFIX)
         for section in sections:
             self._spawnController(Constants.SERVER_PROCESS_NAME, section)
 
     def _runLoop(self):
         self._logRunning()
         while self._timeToDie is False:
             time.sleep(1)
         self._terminateAll()
 
-
-
     @override
     def run(self):
         self._setup()
         self._runLoop()
         return os.EX_OK
 
-
     @override
     def terminate(self, signal, frame):
         self._logger.notice("Terminating..")
         self._terminateAll()
```

### Comparing `pysilico-server-0.20.0/pysilico_server/utils/process_startup_helper.py` & `pysilico_server-0.21.0/pysilico_server/utils/process_startup_helper.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/pysilico_server/utils/starter_script_creator.py` & `pysilico_server-0.21.0/pysilico_server/utils/starter_script_creator.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/pysilico_server.egg-info/PKG-INFO` & `pysilico_server-0.21.0/pysilico_server.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: pysilico-server
-Version: 0.20.0
+Version: 0.21.0
 Summary: AVT-Prosilica camera controller with PLICO
 Home-page: https://github.com/lbusoni/pysilico_server
 Author: Lorenzo Busoni
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: plico,Prosilica,AVT,camera,laboratory,instrumentation control
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: plico>=0.25
+Requires-Dist: pysilico>=0.19
+Requires-Dist: numpy
+Requires-Dist: psutil
+Requires-Dist: six
+Requires-Dist: rebin
 
 # PYSILICO server: Prosilica AVT camera controller for Plico
 
  ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico_server/workflows/Python%20package/badge.svg)
  [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server)
  [![Documentation Status](https://readthedocs.org/projects/pysilico_server/badge/?version=latest)](https://pysilico_server.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version][pypiversion]][pypiversionlink]
```

### Comparing `pysilico-server-0.20.0/pysilico_server.egg-info/SOURCES.txt` & `pysilico_server-0.21.0/pysilico_server.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pysilico_server/camera_controller/pysilico_run_camera_controller.py
 pysilico_server/camera_controller/runner.py
 pysilico_server/conf/pysilico_server.conf
 pysilico_server/devices/__init__.py
 pysilico_server/devices/abstract_camera.py
 pysilico_server/devices/avtCamera.py
 pysilico_server/devices/base_simulated_camera.py
+pysilico_server/devices/basler_camera.py
 pysilico_server/devices/simulated_auxiliary_camera.py
 pysilico_server/devices/simulated_camera.py
 pysilico_server/process_monitor/__init__.py
 pysilico_server/process_monitor/pysilico_run_process_monitor.py
 pysilico_server/process_monitor/runner.py
 pysilico_server/scripts/__init__.py
 pysilico_server/scripts/pysilico_camera_controller.py
```

### Comparing `pysilico-server-0.20.0/setup.py` & `pysilico_server-0.21.0/setup.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/controller/camera_controller_test.py` & `pysilico_server-0.21.0/test/controller/camera_controller_test.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/devices/avt_camera_test.py` & `pysilico_server-0.21.0/test/devices/avt_camera_test.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/devices/hw_avt_camera_test.py` & `pysilico_server-0.21.0/test/devices/hw_avt_camera_test.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/devices/simulated_auxiliary_camera_test.py` & `pysilico_server-0.21.0/test/devices/simulated_auxiliary_camera_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,63 +2,54 @@
 import unittest
 import numpy as np
 import logging
 from pysilico_server.devices.simulated_auxiliary_camera import \
     SimulatedAuxiliaryCamera
 from plico.utils.logger import Logger
 
-__version__ = "$Id: simulated_auxiliary_camera_test.py 271 2017-04-28 16:49:02Z lbusoni $"
-
 
 class SimulatedAuxiliaryCameraTest(unittest.TestCase):
 
     def setUp(self):
         self._setUpLogging()
         self._camera = SimulatedAuxiliaryCamera()
 
-
     def tearDown(self):
         self._camera.raiseExceptionOnDeinitialize(False)
         self._camera.deinitialize()
 
-
     def _setUpLogging(self):
-        FORMAT='%(asctime)s %(levelname)s %(message)s'
+        FORMAT = '%(asctime)s %(levelname)s %(message)s'
         logging.basicConfig(level=logging.DEBUG, format=FORMAT)
-        self._logger= Logger.of(self.__class__.__name__)
-
+        self._logger = Logger.of(self.__class__.__name__)
 
     def testReadFrameDimensionsAndType(self):
         self._camera.setBinning(1)
         f = self._camera.readFrame()
         self.assertEqual(f.shape, (self._camera.SENSOR_H,
                                    self._camera.SENSOR_W))
         self.assertEqual(f.dtype, self._camera.DTYPE)
 
-
     def testSetNoise(self):
         self._camera.setNoiseInCount(100.)
         f = self._camera.readFrame()
         self.assertAlmostEqual(100, np.std(f[0:100, 0:100]), delta=3)
 
-
     def testFluxIsProportionalToExposureTime(self):
         self._camera.setNoiseInCount(0)
         self._camera.setExposureTime(0.1)
-        ima1ms= self._camera.readFrame()
+        ima1ms = self._camera.readFrame()
         self._camera.setExposureTime(0.25)
-        ima2ms= self._camera.readFrame()
-        self.assertAlmostEqual(2.5* ima1ms.max(),
+        ima2ms = self._camera.readFrame()
+        self.assertAlmostEqual(2.5 * ima1ms.max(),
                                ima2ms.max(),
                                delta=3)
 
-
     def testFrameIsSaturatedIfFluxIsTooHigh(self):
         self._camera.setTotalFluxPerMilliSecond(1e9)
-        frame= self._camera.readFrame()
+        frame = self._camera.readFrame()
         self.assertEqual(self._camera.MAX_VALUE,
                          frame.max())
 
 
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysilico-server-0.20.0/test/devices/simulated_pyramid_wfs_camera_test.py` & `pysilico_server-0.21.0/test/devices/simulated_pyramid_wfs_camera_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import numpy as np
 import logging
 from test.test_helper import Poller, ExecutionProbe
 from plico.utils.logger import Logger
 from pysilico_server.devices.simulated_camera import \
     SimulatedPyramidWfsCamera
 
-__version__ = "$Id: simulated_camera_test.py 271 2017-04-28 16:49:02Z lbusoni $"
-
 
 class SimulatedPyramidWfsCameraTest(unittest.TestCase):
 
     def setUp(self):
         self._setUpLogging()
         self._camera = SimulatedPyramidWfsCamera()
 
@@ -53,21 +51,21 @@
         self.assertEqual(self._camera.MAX_VALUE,
                          frame.max())
 
     def testChangePupilsCenter(self):
         self._camera.setNoiseInCount(0)
         self._camera.setExposureTime(1.0)
         cp = 0.5 * np.array([self._camera.SENSOR_H,
-                           self._camera.SENSOR_W])
+                             self._camera.SENSOR_W])
         d = 0.1 * self._camera.SENSOR_H
         centers = np.zeros((4, 2))
-        centers[0,:] = [cp[0] - d, cp[1] - d]
-        centers[1,:] = [cp[0] + d, cp[1] - d]
-        centers[2,:] = [cp[0] - d, cp[1] + d]
-        centers[3,:] = [cp[0] + d, cp[1] + d]
+        centers[0, :] = [cp[0] - d, cp[1] - d]
+        centers[1, :] = [cp[0] + d, cp[1] - d]
+        centers[2, :] = [cp[0] - d, cp[1] + d]
+        centers[3, :] = [cp[0] + d, cp[1] + d]
         self._camera.setPupilsCenterInUnbinnedPixels(centers)
         self._camera.readFrame()
 
     def testWavefrontFromZernikeVector(self):
         tipPtV2Rms = 0.25
         ttCoeff = np.array([-1, 10]) * 1e-6
         self._camera.setNoiseInCount(0)
@@ -75,43 +73,52 @@
         self._camera.setSlopeSaturationInRadians(100e-3)
         self._camera.setWavefrontFromZernikeVector(ttCoeff)
         self._camera.setExposureTime(10)
         frame = self._camera.readFrame().astype(float)
         total = frame.sum()
         (sy, sx) = frame.shape
         dx = frame[:, -sx // 2:].sum() - frame[:, 0:sx // 2].sum()
-        dy = frame[-sy // 2:,:].sum() - frame[0:sy // 2,:].sum()
+        dy = frame[-sy // 2:, :].sum() - frame[0:sy // 2, :].sum()
         ttFromFlux = np.sin(np.pi / 2 * np.array([dx / total, dy / total])) * \
             self._camera.getSlopeSaturationInRadians() * \
             self._camera.getScaleInMeterPerPixel() * \
             self._camera.getPupilsRadiusInUnbinnedPixels() * 2 * \
             tipPtV2Rms
         self.assertTrue(np.allclose(ttCoeff, ttFromFlux, rtol=0.05),
                         "Wanted %s, got %s" % (ttCoeff, ttFromFlux))
 
     def _callback(self, frame):
-        print ('callback %d' % frame.counter())
+        self._logger.debug('callback. Counter: %d' % frame.counter())
         self._lastFrameCounter = frame.counter()
 
     def testCallbackStartAndStop(self):
-        print('testcallback')
+        self._logger.notice('testcallback')
         self._lastFrameCounter = 0
         self._camera.registerCallback(self._callback)
+        self._camera.setFrameRate(1000)
 
         def _frameCounterIncreased(self, originalFrameCounter):
             if self._lastFrameCounter <= originalFrameCounter:
-                raise Exception("last %d - original %d" % (
+                raise Exception("last %d <= wanted %d" % (
                     self._lastFrameCounter, originalFrameCounter))
 
+        self._logger.notice('starting acquisition')
         self._camera.startAcquisition()
         Poller(2).check(ExecutionProbe(_frameCounterIncreased, '', self, 0))
+        self._logger.notice('stopping acquisition')
         self._camera.stopAcquisition()
         currentFrameCnt = self._lastFrameCounter
+        self._logger.notice('current frame counter %d' %
+                            self._lastFrameCounter)
+        # Acquisition is stopped. But there may be one last frame being
+        # acquired. Assert that lastFrameCounter is not bigger than
+        # currentFrameCnt + 1
         self.assertRaises(
             RuntimeError,
-            Poller(2).check,
-            ExecutionProbe(_frameCounterIncreased, '', self, currentFrameCnt)
+            Poller(1, reportPeriodSec=0.5).check,
+            ExecutionProbe(_frameCounterIncreased, '',
+                           self, currentFrameCnt + 1)
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysilico-server-0.20.0/test/fake_time_mod.py` & `pysilico_server-0.21.0/test/fake_time_mod.py`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/integration/conffiles/pysilico_server.conf` & `pysilico_server-0.21.0/test/integration/conffiles/pysilico_server.conf`

 * *Files identical despite different names*

### Comparing `pysilico-server-0.20.0/test/integration/integration_test.py` & `pysilico_server-0.21.0/test/integration/integration_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,15 +30,22 @@
 
     TEST_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                             "./tmp/")
     LOG_DIR = os.path.join(TEST_DIR, "log")
     CONF_FILE = 'test/integration/conffiles/pysilico_server.conf'
     CALIB_FOLDER = 'test/integration/calib'
     CONF_SECTION = Constants.PROCESS_MONITOR_CONFIG_SECTION
-    SERVER_LOG_PATH = os.path.join(LOG_DIR, "%s.log" % CONF_SECTION)
+    PROCESS_MONITOR_LOG_PATH = os.path.join(LOG_DIR, "%s.log" % CONF_SECTION)
+    SERVER_1_LOG_PATH = os.path.join(
+        LOG_DIR, '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 1))
+    SERVER_2_LOG_PATH = os.path.join(
+        LOG_DIR, '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 2))
+    SERVER_3_LOG_PATH = os.path.join(
+        LOG_DIR, '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 3))
+
     BIN_DIR = os.path.join(TEST_DIR, "apps", "bin")
     SOURCE_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                               "../..")
 
     def setUp(self):
         self._setUpBasicLogging()
         self.server = None
@@ -67,55 +74,50 @@
                         calibTempFolder)
 
     def _removeTestFolderIfItExists(self):
         if os.path.exists(self.TEST_DIR):
             shutil.rmtree(self.TEST_DIR)
 
     def tearDown(self):
-        TestHelper.dumpFileToStdout(self.SERVER_LOG_PATH)
+        TestHelper.dumpFileToStdout(self.PROCESS_MONITOR_LOG_PATH)
+        TestHelper.dumpFileToStdout(self.SERVER_1_LOG_PATH)
+        TestHelper.dumpFileToStdout(self.SERVER_2_LOG_PATH)
+        TestHelper.dumpFileToStdout(self.SERVER_3_LOG_PATH)
 
         if self.server is not None:
             TestHelper.terminateSubprocess(self.server)
 
         if self._wasSuccessful:
             self._removeTestFolderIfItExists()
 
     def _createStarterScripts(self):
         ssc = StarterScriptCreator()
         ssc.setInstallationBinDir(self.BIN_DIR)
         ssc.setPythonPath(self.SOURCE_DIR)
         ssc.setConfigFileDestination(self.CONF_FILE)
-        numCameras = len(self.configuration.numberedSectionList(Constants.SERVER_CONFIG_SECTION_PREFIX))
+        numCameras = len(self.configuration.numberedSectionList(
+            Constants.SERVER_CONFIG_SECTION_PREFIX))
         ssc.installExecutables(numCameras)
 
     def _startProcesses(self):
         psh = ProcessStartUpHelper()
         self.server = subprocess.Popen(
             [psh.processProcessMonitorStartUpScriptPath(),
              self.CONF_FILE,
              self.CONF_SECTION])
         Poller(5).check(MessageInFileProbe(
-            ProcessMonitorRunner.RUNNING_MESSAGE, self.SERVER_LOG_PATH))
+            ProcessMonitorRunner.RUNNING_MESSAGE, self.PROCESS_MONITOR_LOG_PATH))
 
     def _testProcessesActuallyStarted(self):
-        controllerLogFile = os.path.join(
-            self.LOG_DIR,
-            '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 1))
         Poller(5).check(MessageInFileProbe(
-            Runner.RUNNING_MESSAGE, controllerLogFile))
-        controller2LogFile = os.path.join(
-            self.LOG_DIR,
-            '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 2))
+            Runner.RUNNING_MESSAGE, self.SERVER_1_LOG_PATH))
         Poller(5).check(MessageInFileProbe(
-            Runner.RUNNING_MESSAGE, controller2LogFile))
-        controller3LogFile = os.path.join(
-            self.LOG_DIR,
-            '%s%d.log' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 3))
+            Runner.RUNNING_MESSAGE, self.SERVER_2_LOG_PATH))
         Poller(5).check(MessageInFileProbe(
-            Runner.RUNNING_MESSAGE, controller3LogFile))
+            Runner.RUNNING_MESSAGE, self.SERVER_3_LOG_PATH))
 
     def _buildClients(self):
         ports1 = ZmqPorts.fromConfiguration(
             self.configuration,
             '%s%d' % (Constants.SERVER_CONFIG_SECTION_PREFIX, 1))
         self.client1 = CameraClient(
             self.rpc, Sockets(ports1, self.rpc))
@@ -224,15 +226,14 @@
         disp = self.client1.getFrameForDisplay().toNumpyArray().shape
         full = self.client1.getFutureFrames(1).toNumpyArray().shape
         Poller(3).check(ExecutionProbe(
             lambda: self.assertEqual(
                 full,
                 self.client1.getFrameForDisplay().toNumpyArray().shape)))
 
-
     def testMain(self):
         self._buildClients()
         self._createStarterScripts()
         self._startProcesses()
         self._testProcessesActuallyStarted()
         self._testCameraGetFrame()
         self._testCameraGetFutureFrames()
```

### Comparing `pysilico-server-0.20.0/test/test_helper.py` & `pysilico_server-0.21.0/test/test_helper.py`

 * *Files identical despite different names*

