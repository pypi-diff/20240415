# Comparing `tmp/setga-1.3.2.tar.gz` & `tmp/setga-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setga-1.3.2.tar", last modified: Mon Apr 15 13:00:05 2024, max compression
+gzip compressed data, was "setga-1.3.4.tar", last modified: Mon Apr 15 13:41:49 2024, max compression
```

## Comparing `setga-1.3.2.tar` & `setga-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 13:00:02.000000 setga-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 13:00:05.549740 setga-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:00:02.000000 setga-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/setga/
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-15 13:00:02.000000 setga-1.3.2/setga/select_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-15 13:00:02.000000 setga-1.3.2/setga/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/setga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 13:00:05.549740 setga-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 13:00:04.000000 setga-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:41:49.177020 setga-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 13:41:47.000000 setga-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:41:49.177020 setga-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:41:47.000000 setga-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:41:49.173020 setga-1.3.4/setga/
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-15 13:41:47.000000 setga-1.3.4/setga/select_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-15 13:41:47.000000 setga-1.3.4/setga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:41:49.177020 setga-1.3.4/setga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:41:49.000000 setga-1.3.4/setga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 13:41:49.000000 setga-1.3.4/setga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:41:49.000000 setga-1.3.4/setga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:41:49.000000 setga-1.3.4/setga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:41:49.000000 setga-1.3.4/setga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 13:41:49.177020 setga-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-15 13:41:48.000000 setga-1.3.4/setup.py
```

### Comparing `setga-1.3.2/LICENSE` & `setga-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `setga-1.3.2/PKG-INFO` & `setga-1.3.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.3.2
+Version: 1.3.4
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
+Project-URL: Documentation, https://readthedocs.org/projects/setminga/
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
```

### Comparing `setga-1.3.2/README.md` & `setga-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `setga-1.3.2/setga/select_subset.py` & `setga-1.3.4/setga/select_subset.py`

 * *Files identical despite different names*

### Comparing `setga-1.3.2/setga/utils.py` & `setga-1.3.4/setga/utils.py`

 * *Files identical despite different names*

### Comparing `setga-1.3.2/setga.egg-info/PKG-INFO` & `setga-1.3.4/setga.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.3.2
+Version: 1.3.4
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
+Project-URL: Documentation, https://readthedocs.org/projects/setminga/
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
```

### Comparing `setga-1.3.2/setup.py` & `setga-1.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,18 @@
   name = 'setga',         
   packages = ['setga'], 
   license='MIT',       
   description = 'library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.',   # Give a short description about your library
   author = 'Nikola Kalábová',              
   author_email = 'nikola@kalabova.eu',     
   url = 'https://github.com/lavakin/setga',  
-  version = "1.3.2",    
+  version = "1.3.4",    
   keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
   long_description = "library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.",
+  project_urls = {"Documentation" :"https://readthedocs.org/projects/setminga/"},
   install_requires=[          
           'numpy',
           'deap',
           "matplotlib",
       ],
 
   classifiers=[
```

