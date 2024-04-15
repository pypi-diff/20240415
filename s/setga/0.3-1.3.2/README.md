# Comparing `tmp/setga-0.3.tar.gz` & `tmp/setga-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setga-0.3.tar", last modified: Fri Apr 12 16:46:04 2024, max compression
+gzip compressed data, was "setga-1.3.2.tar", last modified: Mon Apr 15 13:00:05 2024, max compression
```

## Comparing `setga-0.3.tar` & `setga-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-04-12 16:46:04.702378 setga-0.3/
--rw-r--r--   0 nkalabova  (2728)      350     1074 2024-03-12 12:02:17.000000 setga-0.3/LICENSE
--rw-r--r--   0 nkalabova  (2728)      350      644 2024-04-12 16:46:04.702302 setga-0.3/PKG-INFO
--rw-r--r--   0 nkalabova  (2728)      350     2561 2024-03-12 12:02:17.000000 setga-0.3/README.md
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-04-12 16:46:04.701239 setga-0.3/setga/
--rw-r--r--   0 nkalabova  (2728)      350     6682 2024-04-12 12:09:08.000000 setga-0.3/setga/select_subset.py
--rw-r--r--   0 nkalabova  (2728)      350    11329 2024-04-12 12:09:20.000000 setga-0.3/setga/utils.py
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-04-12 16:46:04.702102 setga-0.3/setga.egg-info/
--rw-r--r--   0 nkalabova  (2728)      350      644 2024-04-12 16:46:04.000000 setga-0.3/setga.egg-info/PKG-INFO
--rw-r--r--   0 nkalabova  (2728)      350      218 2024-04-12 16:46:04.000000 setga-0.3/setga.egg-info/SOURCES.txt
--rw-r--r--   0 nkalabova  (2728)      350        1 2024-04-12 16:46:04.000000 setga-0.3/setga.egg-info/dependency_links.txt
--rw-r--r--   0 nkalabova  (2728)      350       22 2024-04-12 16:46:04.000000 setga-0.3/setga.egg-info/requires.txt
--rw-r--r--   0 nkalabova  (2728)      350        6 2024-04-12 16:46:04.000000 setga-0.3/setga.egg-info/top_level.txt
--rw-r--r--   0 nkalabova  (2728)      350       79 2024-04-12 16:46:04.702586 setga-0.3/setup.cfg
--rw-r--r--   0 nkalabova  (2728)      350      875 2024-04-12 10:42:11.000000 setga-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 13:00:02.000000 setga-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 13:00:05.549740 setga-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:00:02.000000 setga-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/setga/
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-15 13:00:02.000000 setga-1.3.2/setga/select_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-15 13:00:02.000000 setga-1.3.2/setga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:00:05.549740 setga-1.3.2/setga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:00:05.000000 setga-1.3.2/setga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 13:00:05.549740 setga-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 13:00:04.000000 setga-1.3.2/setup.py
```

### Comparing `setga-0.3/LICENSE` & `setga-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `setga-0.3/README.md` & `setga-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `setga-0.3/setga/select_subset.py` & `setga-1.3.2/setga/select_subset.py`

 * *Files identical despite different names*

### Comparing `setga-0.3/setga/utils.py` & `setga-1.3.2/setga/utils.py`

 * *Files identical despite different names*

### Comparing `setga-0.3/setup.py` & `setga-1.3.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+
 from distutils.core import setup
 setup(
   name = 'setga',         
-  packages = ['setga'],   
-  version = '0.3',      
+  packages = ['setga'], 
   license='MIT',       
   description = 'library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.',   # Give a short description about your library
   author = 'Nikola Kalábová',              
   author_email = 'nikola@kalabova.eu',     
-  url = 'https://github.com/lavakin/setminga',  
-  download_url = 'https://github.com/lavakin/setminga/archive/refs/tags/v0.3.tar.gz',    
+  url = 'https://github.com/lavakin/setga',  
+  version = "1.3.2",    
   keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
+  long_description = "library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.",
   install_requires=[          
           'numpy',
           'deap',
           "matplotlib",
       ],
+
   classifiers=[
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: MIT License',  
   ],
 )
```

