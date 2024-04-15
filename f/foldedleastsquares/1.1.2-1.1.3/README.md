# Comparing `tmp/foldedleastsquares-1.1.2.tar.gz` & `tmp/foldedleastsquares-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldedleastsquares-1.1.2.tar", last modified: Fri Dec 29 20:31:24 2023, max compression
+gzip compressed data, was "foldedleastsquares-1.1.3.tar", last modified: Sat Jan 13 09:16:37 2024, max compression
```

## Comparing `foldedleastsquares-1.1.2.tar` & `foldedleastsquares-1.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:24.318555 foldedleastsquares-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2023-12-29 20:31:24.318555 foldedleastsquares-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:24.314555 foldedleastsquares-1.1.2/foldedleastsquares/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27409 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:24.314555 foldedleastsquares-1.1.2/foldedleastsquares/template_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/template_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17706 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/template_generator/default_transit_template_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/template_generator/tailed_transit_template_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/template_generator/transit_template_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:24.318555 foldedleastsquares-1.1.2/foldedleastsquares/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_FAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_cleaned_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_duration_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_multi_planet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_multi_planet_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_period_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_stats_gap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_transit_depth_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/tls_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/foldedleastsquares/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:31:24.314555 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2023-12-29 20:31:24.000000 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-12-29 20:31:24.000000 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 20:31:24.000000 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-29 20:31:24.000000 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-29 20:31:24.000000 foldedleastsquares-1.1.2/foldedleastsquares.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 20:31:24.318555 foldedleastsquares-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-29 20:31:16.000000 foldedleastsquares-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:37.448502 foldedleastsquares-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-01-13 09:16:37.448502 foldedleastsquares-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:37.444502 foldedleastsquares-1.1.3/foldedleastsquares/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:37.444502 foldedleastsquares-1.1.3/foldedleastsquares/template_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/template_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/template_generator/default_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/template_generator/tailed_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/template_generator/transit_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:37.448502 foldedleastsquares-1.1.3/foldedleastsquares/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_FAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_cleaned_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_duration_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_multi_planet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_multi_planet_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_period_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_stats_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_transit_depth_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/tls_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/foldedleastsquares/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 09:16:37.444502 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-01-13 09:16:37.000000 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-13 09:16:37.000000 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 09:16:37.000000 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-13 09:16:37.000000 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-13 09:16:37.000000 foldedleastsquares-1.1.3/foldedleastsquares.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 09:16:37.448502 foldedleastsquares-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-01-13 09:16:28.000000 foldedleastsquares-1.1.3/setup.py
```

### Comparing `foldedleastsquares-1.1.2/LICENSE` & `foldedleastsquares-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/PKG-INFO` & `foldedleastsquares-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.1.2
+Version: 1.1.3
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/martindevora/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
         ### An optimized transit-fitting algorithm to search for periodic transits of small planets
```

### Comparing `foldedleastsquares-1.1.2/README.md` & `foldedleastsquares-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/__init__.py` & `foldedleastsquares-1.1.3/foldedleastsquares/__init__.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/catalog.py` & `foldedleastsquares-1.1.3/foldedleastsquares/catalog.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/command_line.py` & `foldedleastsquares-1.1.3/foldedleastsquares/command_line.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/core.py` & `foldedleastsquares-1.1.3/foldedleastsquares/core.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/gpu.py` & `foldedleastsquares-1.1.3/foldedleastsquares/gpu.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/grid.py` & `foldedleastsquares-1.1.3/foldedleastsquares/grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/helpers.py` & `foldedleastsquares-1.1.3/foldedleastsquares/helpers.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/interpolation.py` & `foldedleastsquares-1.1.3/foldedleastsquares/interpolation.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/main.py` & `foldedleastsquares-1.1.3/foldedleastsquares/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         )
 
         # Python 2 multiprocessing with "partial" doesn't work
         # For now, only single-threading in Python 2 is supported
         if sys.version_info[0] < 3:
             self.use_threads = 1
             warnings.warn("This TLS version supports no multithreading on Python 2")
-        use_cpu = not self.use_gpu or gpu.get_device_count() == 0
+        use_cpu = not self.use_gpu or 'gpu' not in sys.modules or gpu.get_device_count() == 0
         if use_cpu:
             if self.use_threads == multiprocessing.cpu_count():
                 print("Using all " + str(self.use_threads) + " CPU threads")
             else:
                 print(
                     "Using "
                     + str(self.use_threads)
```

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/results.py` & `foldedleastsquares-1.1.3/foldedleastsquares/results.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/stats.py` & `foldedleastsquares-1.1.3/foldedleastsquares/stats.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/template_generator/default_transit_template_generator.py` & `foldedleastsquares-1.1.3/foldedleastsquares/template_generator/default_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/template_generator/tailed_transit_template_generator.py` & `foldedleastsquares-1.1.3/foldedleastsquares/template_generator/tailed_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/template_generator/transit_template_generator.py` & `foldedleastsquares-1.1.3/foldedleastsquares/template_generator/transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_catalog_data.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_catalog_data.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_cleaned_array.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_cleaned_array.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_duration_grid.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_duration_grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_multi_planet.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_multi_planet.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_multi_planet_gpu.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_multi_planet_gpu.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_period_grid.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_period_grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_resample.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_shapes.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_stats_gap.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_stats_gap.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_synthetic.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_transit_depth_min.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_transit_depth_min.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_uncertainties.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tests/test_validation.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/tls_constants.py` & `foldedleastsquares-1.1.3/foldedleastsquares/tls_constants.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares/validate.py` & `foldedleastsquares-1.1.3/foldedleastsquares/validate.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares.egg-info/PKG-INFO` & `foldedleastsquares-1.1.3/foldedleastsquares.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.1.2
+Version: 1.1.3
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/martindevora/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
         ### An optimized transit-fitting algorithm to search for periodic transits of small planets
```

### Comparing `foldedleastsquares-1.1.2/foldedleastsquares.egg-info/SOURCES.txt` & `foldedleastsquares-1.1.3/foldedleastsquares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.1.2/setup.py` & `foldedleastsquares-1.1.3/setup.py`

 * *Files identical despite different names*

