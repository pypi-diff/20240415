# Comparing `tmp/cyclophaser-1.7.2.tar.gz` & `tmp/cyclophaser-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclophaser-1.7.2.tar", last modified: Sun Apr 14 02:37:49 2024, max compression
+gzip compressed data, was "cyclophaser-1.7.3.tar", last modified: Mon Apr 15 11:35:40 2024, max compression
```

## Comparing `cyclophaser-1.7.2.tar` & `cyclophaser-1.7.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/cyclophaser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/cyclophaser/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17504 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/cyclophaser/determine_periods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/cyclophaser/find_stages.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/cyclophaser/lanczos_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12837 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/cyclophaser/plots.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/cyclophaser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-14 02:37:49.000000 cyclophaser-1.7.2/cyclophaser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-14 02:37:49.000000 cyclophaser-1.7.2/cyclophaser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-14 02:37:49.000000 cyclophaser-1.7.2/cyclophaser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-14 02:37:49.000000 cyclophaser-1.7.2/cyclophaser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-14 02:37:49.111341 cyclophaser-1.7.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-04-14 02:37:48.000000 cyclophaser-1.7.2/tests/test_determine_periods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/cyclophaser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17504 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser/determine_periods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser/find_stages.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser/lanczos_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12837 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser/plots.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/cyclophaser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/cyclophaser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 11:35:40.794832 cyclophaser-1.7.3/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-04-15 11:35:40.000000 cyclophaser-1.7.3/tests/test_determine_periods.py
```

### Comparing `cyclophaser-1.7.2/PKG-INFO` & `cyclophaser-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.7.2
+Version: 1.7.3
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.7.2/README.md` & `cyclophaser-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.2/cyclophaser/determine_periods.py` & `cyclophaser-1.7.3/cyclophaser/determine_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    determine_periods.py                               :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: daniloceano <danilo.oceano@gmail.com>      +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/05/19 19:06:47 by danilocs          #+#    #+#              #
-#    Updated: 2024/04/13 23:35:55 by daniloceano      ###   ########.fr        #
+#    Updated: 2024/04/15 08:31:27 by daniloceano      ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import os
 import csv
 
 import xarray as xr
@@ -270,15 +270,15 @@
                               'dz_dt_smoothed2': dz_dt_smoothed2,
                               'dz_dt2_smoothed2': dz_dt2_smoothed2})
 
     return da 
 
 def get_periods(vorticity,  plot=False, plot_steps=False, export_dict=False, periods_args=None):
     default_args = {
-        'threshold_intensification_length': 0.125,
+        'threshold_intensification_length': 0.075,
         'threshold_intensification_gap': 0.075,
         'threshold_mature_distance': 0.125,
         'threshold_mature_length': 0.03,
         'threshold_decay_length': 0.075,
         'threshold_decay_gap': 0.075,
         'threshold_incipient_length': 0.4
     }
```

### Comparing `cyclophaser-1.7.2/cyclophaser/find_stages.py` & `cyclophaser-1.7.3/cyclophaser/find_stages.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.2/cyclophaser/lanczos_filter.py` & `cyclophaser-1.7.3/cyclophaser/lanczos_filter.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.2/cyclophaser/plots.py` & `cyclophaser-1.7.3/cyclophaser/plots.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.2/cyclophaser.egg-info/PKG-INFO` & `cyclophaser-1.7.3/cyclophaser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.7.2
+Version: 1.7.3
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.7.2/setup.py` & `cyclophaser-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '1.7.2'
+VERSION = '1.7.3'
 DESCRIPTION = 'Determine phases from extratropical cyclone life cycle'
 # LONG_DESCRIPTION = 'This script processes vorticity data, identifies different phases of the cyclone \
     # and plots the identified periods on periods.png and periods_didatic.png'
 
 setup(
     name="cyclophaser",
     version=VERSION,
```

### Comparing `cyclophaser-1.7.2/tests/test_determine_periods.py` & `cyclophaser-1.7.3/tests/test_determine_periods.py`

 * *Files identical despite different names*

