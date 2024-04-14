# Comparing `tmp/ttemtoolbox-1.0.0.tar.gz` & `tmp/ttemtoolbox-4.14.2024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttemtoolbox-1.0.0.tar", last modified: Sun Apr 14 23:17:40 2024, max compression
+gzip compressed data, was "ttemtoolbox-4.14.2024.tar", last modified: Sun Apr 14 23:12:46 2024, max compression
```

## Comparing `ttemtoolbox-1.0.0.tar` & `ttemtoolbox-4.14.2024.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.355238 ttemtoolbox-1.0.0/
--rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)    35149 2024-04-14 20:29:28.000000 ttemtoolbox-1.0.0/LICENSE
--rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      818 2024-04-14 23:17:40.350238 ttemtoolbox-1.0.0/PKG-INFO
--rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       97 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/Readme.md
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)      805 2024-04-14 23:17:13.000000 ttemtoolbox-1.0.0/pyproject.toml
--rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       38 2024-04-14 23:17:40.356238 ttemtoolbox-1.0.0/setup.cfg
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.169246 ttemtoolbox-1.0.0/src/
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.192245 ttemtoolbox-1.0.0/src/tTEM_toolbox/
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       37 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/__init__.py
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.249242 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     2218 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/Rock_trans.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       91 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/__init__.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    10187 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/bootstrap.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     7627 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/main.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    14604 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/plot.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     6126 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_gamma.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    11059 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_ttem.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    22222 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_well.py
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.264242 ttemtoolbox-1.0.0/src/tTEM_toolbox/defaults/
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       23 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/defaults/__init__.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)      910 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/defaults/constants.py
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.297241 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       20 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/__init__.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     7541 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/canny_edge_detection.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/datafilter.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     1510 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/tools.py
--rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     9746 2024-04-14 23:04:50.000000 ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/visualize_surface_kansas.py
-drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:17:40.340239 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/
--rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      818 2024-04-14 23:17:40.000000 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      814 2024-04-14 23:17:40.000000 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)        1 2024-04-14 23:17:40.000000 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       49 2024-04-14 23:17:40.000000 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/requires.txt
--rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       13 2024-04-14 23:17:40.000000 ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:46.113631 ttemtoolbox-4.14.2024/
+-rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)    35149 2024-04-14 20:29:28.000000 ttemtoolbox-4.14.2024/LICENSE
+-rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      821 2024-04-14 23:12:46.108631 ttemtoolbox-4.14.2024/PKG-INFO
+-rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       97 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/Readme.md
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)      809 2024-04-14 23:12:28.000000 ttemtoolbox-4.14.2024/pyproject.toml
+-rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       38 2024-04-14 23:12:46.115630 ttemtoolbox-4.14.2024/setup.cfg
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:45.881640 ttemtoolbox-4.14.2024/src/
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:45.926638 ttemtoolbox-4.14.2024/src/tTEM_toolbox/
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       37 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/__init__.py
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:46.013635 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     2218 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/Rock_trans.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       91 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/__init__.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    10187 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/bootstrap.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     7627 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/main.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    14604 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/plot.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     6126 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_gamma.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    11059 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_ttem.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)    22222 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_well.py
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:46.027634 ttemtoolbox-4.14.2024/src/tTEM_toolbox/defaults/
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       23 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/defaults/__init__.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)      910 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/defaults/constants.py
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:46.061633 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)       20 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/__init__.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     7541 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/canny_edge_detection.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/datafilter.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     1510 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/tools.py
+-rwxr-xr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)     9746 2024-04-14 23:04:50.000000 ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/visualize_surface_kansas.py
+drwxrwxr-x   0 jiawei.li (1727140043) jiawei.li (1727140043)        0 2024-04-14 23:12:46.100631 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/
+-rw-r--r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      821 2024-04-14 23:12:45.000000 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)      814 2024-04-14 23:12:45.000000 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)        1 2024-04-14 23:12:45.000000 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       48 2024-04-14 23:12:45.000000 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/requires.txt
+-rw-rw-r--   0 jiawei.li (1727140043) jiawei.li (1727140043)       13 2024-04-14 23:12:45.000000 ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/top_level.txt
```

### Comparing `ttemtoolbox-1.0.0/LICENSE` & `ttemtoolbox-4.14.2024/LICENSE`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/PKG-INFO` & `ttemtoolbox-4.14.2024/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ttemtoolbox
-Version: 1.0.0
+Version: 4.14.2024
 Summary: A tool box to use for post processing of ttem files generated by Aarhus workbench
 Author-email: Jiawei Li <Jiaweiliwork@outlook.com>
 Project-URL: Homepage, https://github.com/Kosaksruri/ttemtoolbox
 Project-URL: Issues, https://github.com/Kosaksruri/ttemtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: pyproj
+Requires-Dist: pyroj
 Requires-Dist: scipy
 Requires-Dist: xarray
 Requires-Dist: plotly
 Requires-Dist: requests
 Requires-Dist: pandas
 
 # ttemtoolbox
```

### Comparing `ttemtoolbox-1.0.0/pyproject.toml` & `ttemtoolbox-4.14.2024/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 [project]
 name= "ttemtoolbox"
-version = '1.0.0'
+version = '04.14.2024'
 authors = [{name="Jiawei Li", email="Jiaweiliwork@outlook.com"}]
 description = "A tool box to use for post processing of ttem files generated by Aarhus workbench"
 readme = 'Readme.md'
-dependencies = ["numpy", "pyproj", "scipy", "xarray", "plotly", "requests", "pandas"]
+dependencies = ["numpy", "pyroj", "scipy", "xarray", "plotly", "requests", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 
 ]
```

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/Rock_trans.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/Rock_trans.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/bootstrap.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/main.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/main.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/plot.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/plot.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_gamma.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_gamma.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_ttem.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_ttem.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/core/process_well.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/core/process_well.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/defaults/constants.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/defaults/constants.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/canny_edge_detection.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/canny_edge_detection.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/tools.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/tools.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/tTEM_toolbox/utils/visualize_surface_kansas.py` & `ttemtoolbox-4.14.2024/src/tTEM_toolbox/utils/visualize_surface_kansas.py`

 * *Files identical despite different names*

### Comparing `ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/PKG-INFO` & `ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ttemtoolbox
-Version: 1.0.0
+Version: 4.14.2024
 Summary: A tool box to use for post processing of ttem files generated by Aarhus workbench
 Author-email: Jiawei Li <Jiaweiliwork@outlook.com>
 Project-URL: Homepage, https://github.com/Kosaksruri/ttemtoolbox
 Project-URL: Issues, https://github.com/Kosaksruri/ttemtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: pyproj
+Requires-Dist: pyroj
 Requires-Dist: scipy
 Requires-Dist: xarray
 Requires-Dist: plotly
 Requires-Dist: requests
 Requires-Dist: pandas
 
 # ttemtoolbox
```

### Comparing `ttemtoolbox-1.0.0/src/ttemtoolbox.egg-info/SOURCES.txt` & `ttemtoolbox-4.14.2024/src/ttemtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

