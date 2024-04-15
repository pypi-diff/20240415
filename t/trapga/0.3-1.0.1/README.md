# Comparing `tmp/trapga-0.3.tar.gz` & `tmp/trapga-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trapga-0.3.tar", last modified: Wed Mar 13 12:36:02 2024, max compression
+gzip compressed data, was "trapga-1.0.1.tar", last modified: Mon Apr 15 14:38:13 2024, max compression
```

## Comparing `trapga-0.3.tar` & `trapga-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-03-13 12:36:02.358384 trapga-0.3/
--rw-r--r--   0 nkalabova  (2728)      350      615 2024-03-13 12:36:02.358271 trapga-0.3/PKG-INFO
--rw-r--r--   0 nkalabova  (2728)      350     3188 2024-02-29 13:41:44.000000 trapga-0.3/README.md
--rw-r--r--   0 nkalabova  (2728)      350       38 2024-03-13 12:36:02.358420 trapga-0.3/setup.cfg
--rw-r--r--   0 nkalabova  (2728)      350     1074 2024-03-13 12:32:41.000000 trapga-0.3/setup.py
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-03-13 12:36:02.357094 trapga-0.3/trapga/
--rw-r--r--   0 nkalabova  (2728)      350     4354 2024-03-13 12:35:34.000000 trapga-0.3/trapga/trapga.py
--rw-r--r--   0 nkalabova  (2728)      350     4302 2024-03-13 12:32:39.000000 trapga-0.3/trapga/utils.py
-drwxr-xr-x   0 nkalabova  (2728)      350        0 2024-03-13 12:36:02.358109 trapga-0.3/trapga.egg-info/
--rw-r--r--   0 nkalabova  (2728)      350      615 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/PKG-INFO
--rw-r--r--   0 nkalabova  (2728)      350      233 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/SOURCES.txt
--rw-r--r--   0 nkalabova  (2728)      350        1 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/dependency_links.txt
--rw-r--r--   0 nkalabova  (2728)      350       45 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/entry_points.txt
--rw-r--r--   0 nkalabova  (2728)      350       55 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/requires.txt
--rw-r--r--   0 nkalabova  (2728)      350        7 2024-03-13 12:36:02.000000 trapga-0.3/trapga.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:38:13.283395 trapga-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 14:38:13.283395 trapga-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-15 14:38:10.000000 trapga-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:38:13.283395 trapga-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-15 14:38:11.000000 trapga-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:38:13.283395 trapga-1.0.1/trapga/
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-15 14:38:10.000000 trapga-1.0.1/trapga/trapga.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-04-15 14:38:10.000000 trapga-1.0.1/trapga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:38:13.283395 trapga-1.0.1/trapga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 14:38:13.000000 trapga-1.0.1/trapga.egg-info/top_level.txt
```

### Comparing `trapga-0.3/PKG-INFO` & `trapga-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: trapga
-Version: 0.3
+Version: 1.0.1
 Summary: Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages
 Home-page: https://github.com/lavakin/trapga
-Download-URL: https://github.com/lavakin/trapga/archive/refs/tags/v0.3.tar.gz
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
+Project-URL: Documentation, https://trapga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+
+Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages
```

### Comparing `trapga-0.3/README.md` & `trapga-1.0.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-# TraP-GA 
-[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
-![Visitors](https://api.visitorbadge.io/api/visitors?path=https://github.com/lavakin/TraP-GA&label=Visitors&countColor=%23263759&style=flat)
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+.. image:: https://readthedocs.org/projects/trapga/badge/?version=latest
+    :target: https://trapga.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
 
-## Overview
+TraP-GA 
+=============
+
+Overview
+-------------------
 
 The TraP-GA is a Python library built upon SetMiG, designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages (for more information on how to get the gene ages, see [GeneEra](https://github.com/josuebarrera/GenEra)).
 
 The project features an algorithm designed to identify genes contributing to the observed hourglass pattern in developmental gene expression data. The hourglass pattern refers to a characteristic developmental pattern observed in various organisms, where the morphological and genetic similarities between individuals are most pronounced at a specific stage of development.
 
 This algorithm aims to identify a subset of genes that, if removed from the dataset, would significantly reduce the presence of the hourglass pattern. By employing a multi-objective genetic algorithm, it maximizes the removal of the hourglass pattern while minimizing the number of removed genes.
 
 The algorithm utilizes the DEAP (Distributed Evolutionary Algorithms in Python) library, which provides a flexible framework for implementing genetic algorithms. It offers various selection methods, mutation operators, and genetic operators to evolve populations of candidate solutions.
 
 Additionally, to enhance its search capability and avoid being trapped in local optima, the algorithm employs an island model. This approach involves maintaining multiple subpopulations, or "islands," that evolve independently. Periodic migration of individuals between islands allows for sharing of genetic information and prevents the algorithm from converging prematurely to suboptimal solutions. This utilization of the island model enhances the algorithm's ability to explore the solution space and discover more globally optimal solutions.
 
 https://github.com/lavakin/ga_for_hourglass/assets/76702901/5435d04b-151b-46da-b179-d48ca9a7e5ce
 
-## Features
+Features
+-------------------
 
 - **Gene Extraction:** Automatically identifies and extracts genes significant to development from transcriptomic data.
 - **Built on SetMiG:** Leveraging the capabilities of SetMiG, a library for extracting a minimal subset which optimizes a given function.
 
-## Installation
-```
-git clone https://github.com/lavakin/TraP-GA
-chmod +x DEAP_island.py
-```
-## Usage
-
-```
-./DEAP_island.py data.csv output_folder --save_plot
-```
+Installation
+-------------------
+
+.. code-block:: bash
+
+  git clone https://github.com/lavakin/TraP-GA
+
+.. code-block:: bash
+
+  chmod +x DEAP_island.py
+
+
+Usage
+-------------------
+
+.. code-block:: bash
+
+   ./DEAP_island.py data.csv output_folder --save_plot
+
+
 
 
-## Contributing
+Contributing
+-------------------
 
 Contributions to this project are welcome. If you have any ideas for improvements, new features, or bug fixes, please submit a pull request. For major changes, please open an issue to discuss the proposed modifications.
 
 
-## License
+License
+-------------------
 
 This project is licensed under the MIT License. Feel free to use and modify the code according to the terms of this license.
```

### Comparing `trapga-0.3/setup.py` & `trapga-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
+from distutils.core import setup
 
 setup(
     name='trapga',
-    version='0.3',
     py_modules=['trapga'],
     packages = ['trapga'],
     license='MIT',   
-    description = 'Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages',   # Give a short description about your library
+    description = 'Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages',  # Give a short description about your library
+    long_description = 'Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages', 
+    project_urls = {"Documentation" :"https://trapga.readthedocs.io/en/latest/genindex.html"},
     author = 'Nikola Kalábová',              
     author_email = 'nikola@kalabova.eu',     
-    url = 'https://github.com/lavakin/trapga',  
-    download_url = 'https://github.com/lavakin/trapga/archive/refs/tags/v0.3.tar.gz',    
+    url = 'https://github.com/lavakin/trapga', 
+    version = "1.0.1",      
     keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
-    install_requires=['numpy', 'scipy', 'pandas', 'argparse', 'scikit-learn', 'tqdm',"setminga"],
+    install_requires=['numpy', 'scipy', 'pandas', 'argparse', 'scikit-learn', 'tqdm',"setga"],
     entry_points={
         'console_scripts': [
             'trapga = trapga.trapga:cli'
         ]
         },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',  
     ] 
 )
-
```

### Comparing `trapga-0.3/trapga.egg-info/PKG-INFO` & `trapga-1.0.1/trapga.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: trapga
-Version: 0.3
+Version: 1.0.1
 Summary: Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages
 Home-page: https://github.com/lavakin/trapga
-Download-URL: https://github.com/lavakin/trapga/archive/refs/tags/v0.3.tar.gz
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
+Project-URL: Documentation, https://trapga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+
+Library designed for extracting genes that play a significant role in development. It utilizes transcriptomic data of genes, spanning multiple developmental stages and their respective gene ages
```

