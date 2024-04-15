# Comparing `tmp/lib-dt-state-estimation-0.0.6.tar.gz` & `tmp/lib-dt-state-estimation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib-dt-state-estimation-0.0.6.tar", last modified: Fri Sep 23 15:55:52 2022, max compression
+gzip compressed data, was "lib-dt-state-estimation-0.0.7.tar", last modified: Mon Apr 15 15:25:34 2024, max compression
```

## Comparing `lib-dt-state-estimation-0.0.6.tar` & `lib-dt-state-estimation-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      517 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2133 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       83 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      517 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      759 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       46 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2022-09-23 15:36:03.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8500 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/lane_filter.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4361 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/assets/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4852 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/assets/lane_filter_grid.png
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       94 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6169 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/rendering.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-09-23 15:55:52.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2411 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/types.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      198 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3787 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/wheel_odometer.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2022-09-23 15:29:06.000000 lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.073311 lib-dt-state-estimation-0.0.7/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      621 2024-04-15 15:25:34.073311 lib-dt-state-estimation-0.0.7/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-15 15:25:34.073311 lib-dt-state-estimation-0.0.7/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2133 2023-12-17 21:31:24.000000 lib-dt-state-estimation-0.0.7/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.069311 lib-dt-state-estimation-0.0.7/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.069311 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-15 15:25:25.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.069311 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       94 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.069311 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4852 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/assets/lane_filter_grid.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8500 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/lane_filter.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6169 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4361 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.069311 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2411 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      198 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3787 2023-04-19 19:49:23.000000 lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/wheel_odometer.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:25:34.073311 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      621 2024-04-15 15:25:33.000000 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      759 2024-04-15 15:25:34.000000 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-15 15:25:33.000000 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       83 2024-04-15 15:25:33.000000 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       46 2024-04-15 15:25:33.000000 lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lib-dt-state-estimation-0.0.6/setup.py` & `lib-dt-state-estimation-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # :==> Fill in your project data here
 # The package name is the name on PyPI
 # it is not the python module names.
 package_name = "dt-state-estimation"
 library_webpage = f"http://github.com/duckietown/lib-{package_name}"
 maintainer = "Andrea F. Daniele"
-maintainer_email = "afdaniele@duckietown.org"
+maintainer_email = "afdaniele@duckietown.com"
 short_description = "State estimation components of Duckietown's autonomy behavior."
 full_description = """
 State estimation components of the autonomous behavior pipeline running on Duckietown robots.
 """
 
 # Read version from the __init__ file
 def get_version_from_source(filename):
```

### Comparing `lib-dt-state-estimation-0.0.6/src/lib_dt_state_estimation.egg-info/SOURCES.txt` & `lib-dt-state-estimation-0.0.7/src/lib_dt_state_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/lane_filter.py` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/lane_filter.py`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/types.py` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/assets/lane_filter_grid.png` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/assets/lane_filter_grid.png`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/lane_filter/rendering.py` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/lane_filter/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/types.py` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-state-estimation-0.0.6/src/dt_state_estimation/wheel_odometry/wheel_odometer.py` & `lib-dt-state-estimation-0.0.7/src/dt_state_estimation/wheel_odometry/wheel_odometer.py`

 * *Files identical despite different names*

