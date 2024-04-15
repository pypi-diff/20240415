# Comparing `tmp/lib-dt-motion-planning-0.0.1.tar.gz` & `tmp/lib-dt-motion-planning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-motion-planning-0.0.1.tar", last modified: Mon Mar 14 06:17:03 2022, max compression
+gzip compressed data, was "lib-dt-motion-planning-0.0.2.tar", last modified: Mon Apr 15 15:26:08 2024, max compression
```

## Comparing `lib-dt-motion-planning-0.0.1.tar` & `lib-dt-motion-planning-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      577 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1930 2022-03-14 06:05:36.000000 lib-dt-motion-planning-0.0.1/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2022-03-14 06:17:01.000000 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/lane_controller/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      378 2022-03-14 06:03:35.000000 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/lane_controller/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10384 2022-03-14 06:03:35.000000 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/lane_controller/lane_controller.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      481 2022-03-13 23:14:16.000000 lib-dt-motion-planning-0.0.1/src/dt_motion_planning/lane_controller/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-03-14 06:17:03.647723 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      577 2022-03-14 06:17:03.000000 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      449 2022-03-14 06:17:03.000000 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2022-03-14 06:17:03.000000 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       14 2022-03-14 06:17:03.000000 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       44 2022-03-14 06:17:03.000000 lib-dt-motion-planning-0.0.1/src/lib_dt_motion_planning.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:26:08.466143 lib-dt-motion-planning-0.0.2/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      485 2024-04-15 15:26:08.466143 lib-dt-motion-planning-0.0.2/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-15 15:26:08.466143 lib-dt-motion-planning-0.0.2/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1930 2023-12-17 21:31:24.000000 lib-dt-motion-planning-0.0.2/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:26:08.462143 lib-dt-motion-planning-0.0.2/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:26:08.462143 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-15 15:26:03.000000 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:26:08.466143 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/lane_controller/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      378 2023-04-19 19:49:22.000000 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/lane_controller/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10384 2023-04-19 19:49:22.000000 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/lane_controller/lane_controller.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      481 2023-04-19 19:49:22.000000 lib-dt-motion-planning-0.0.2/src/dt_motion_planning/lane_controller/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-15 15:26:08.466143 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      485 2024-04-15 15:26:08.000000 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      449 2024-04-15 15:26:08.000000 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-15 15:26:08.000000 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       14 2024-04-15 15:26:08.000000 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       44 2024-04-15 15:26:08.000000 lib-dt-motion-planning-0.0.2/src/lib_dt_motion_planning.egg-info/top_level.txt
```

### Comparing `lib-dt-motion-planning-0.0.1/setup.py` & `lib-dt-motion-planning-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # :==> Fill in your project data here
 # The package name is the name on PyPI
 # it is not the python module names.
 package_name = "dt-motion-planning"
 library_webpage = f"http://github.com/duckietown/lib-{package_name}"
 maintainer = "Andrea F. Daniele"
-maintainer_email = "afdaniele@duckietown.org"
+maintainer_email = "afdaniele@duckietown.com"
 short_description = "Motion Planning components of Duckietown's autonomy behavior."
 full_description = """
 Motion Planning components of the autonomous behavior pipeline running on Duckietown robots.
 """
 
 # Read version from the __init__ file
 def get_version_from_source(filename):
```

### Comparing `lib-dt-motion-planning-0.0.1/src/dt_motion_planning/lane_controller/lane_controller.py` & `lib-dt-motion-planning-0.0.2/src/dt_motion_planning/lane_controller/lane_controller.py`

 * *Files identical despite different names*

