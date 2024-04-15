# Comparing `tmp/acmetric_plotting-1.3.1.tar.gz` & `tmp/acmetric_plotting-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acmetric_plotting-1.3.1.tar", last modified: Thu Apr 11 14:29:25 2024, max compression
+gzip compressed data, was "acmetric_plotting-1.3.2.tar", last modified: Mon Apr 15 06:40:43 2024, max compression
```

## Comparing `acmetric_plotting-1.3.1.tar` & `acmetric_plotting-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-11 14:29:25.993252 acmetric_plotting-1.3.1/
--rw-r--r--   0 jakob      (501) staff       (20)        0 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.1/LICENCE
--rw-r--r--   0 jakob      (501) staff       (20)       22 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.1/MANIFEST.in
--rw-r--r--   0 jakob      (501) staff       (20)     2724 2024-04-11 14:29:25.992959 acmetric_plotting-1.3.1/PKG-INFO
--rw-r--r--   0 jakob      (501) staff       (20)     2062 2024-04-11 14:29:12.000000 acmetric_plotting-1.3.1/README.md
--rw-r--r--   0 jakob      (501) staff       (20)      835 2024-04-11 14:28:57.000000 acmetric_plotting-1.3.1/pyproject.toml
--rw-r--r--   0 jakob      (501) staff       (20)       38 2024-04-11 14:29:25.993312 acmetric_plotting-1.3.1/setup.cfg
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-11 14:29:25.984505 acmetric_plotting-1.3.1/src/
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-11 14:29:25.990373 acmetric_plotting-1.3.1/src/acmetric_plotting/
--rw-r--r--   0 jakob      (501) staff       (20)    63900 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/Oswald-Regular.ttf
--rw-r--r--   0 jakob      (501) staff       (20)     1076 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/__init__.py
--rw-r--r--   0 jakob      (501) staff       (20)      659 2024-04-11 09:47:53.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/colors.py
--rw-r--r--   0 jakob      (501) staff       (20)      336 2024-04-11 14:25:22.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/fonts.py
--rw-r--r--   0 jakob      (501) staff       (20)     3129 2024-04-11 14:25:39.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/params.py
--rw-r--r--   0 jakob      (501) staff       (20)    19807 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.1/src/acmetric_plotting/plots.py
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-11 14:29:25.992597 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/
--rw-r--r--   0 jakob      (501) staff       (20)     2724 2024-04-11 14:29:25.000000 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/PKG-INFO
--rw-r--r--   0 jakob      (501) staff       (20)      469 2024-04-11 14:29:25.000000 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/SOURCES.txt
--rw-r--r--   0 jakob      (501) staff       (20)        1 2024-04-11 14:29:25.000000 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/dependency_links.txt
--rw-r--r--   0 jakob      (501) staff       (20)       74 2024-04-11 14:29:25.000000 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/requires.txt
--rw-r--r--   0 jakob      (501) staff       (20)       18 2024-04-11 14:29:25.000000 acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/top_level.txt
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-15 06:40:43.091847 acmetric_plotting-1.3.2/
+-rw-r--r--   0 jakob      (501) staff       (20)        0 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.2/LICENCE
+-rw-r--r--   0 jakob      (501) staff       (20)       31 2024-04-11 15:08:50.000000 acmetric_plotting-1.3.2/MANIFEST.in
+-rw-r--r--   0 jakob      (501) staff       (20)     2724 2024-04-15 06:40:43.091591 acmetric_plotting-1.3.2/PKG-INFO
+-rw-r--r--   0 jakob      (501) staff       (20)     2062 2024-04-15 05:54:45.000000 acmetric_plotting-1.3.2/README.md
+-rw-r--r--   0 jakob      (501) staff       (20)      835 2024-04-15 05:54:57.000000 acmetric_plotting-1.3.2/pyproject.toml
+-rw-r--r--   0 jakob      (501) staff       (20)       38 2024-04-15 06:40:43.091901 acmetric_plotting-1.3.2/setup.cfg
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-15 06:40:43.082937 acmetric_plotting-1.3.2/src/
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-15 06:40:43.088406 acmetric_plotting-1.3.2/src/acmetric_plotting/
+-rw-r--r--   0 jakob      (501) staff       (20)    63900 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/Oswald-Regular.ttf
+-rw-r--r--   0 jakob      (501) staff       (20)     1076 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/__init__.py
+-rw-r--r--   0 jakob      (501) staff       (20)      659 2024-04-11 09:47:53.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/colors.py
+-rw-r--r--   0 jakob      (501) staff       (20)      336 2024-04-11 14:25:22.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/fonts.py
+-rw-r--r--   0 jakob      (501) staff       (20)     3120 2024-04-15 05:53:10.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/params.py
+-rw-r--r--   0 jakob      (501) staff       (20)    19807 2024-04-11 09:45:22.000000 acmetric_plotting-1.3.2/src/acmetric_plotting/plots.py
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2024-04-15 06:40:43.091263 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/
+-rw-r--r--   0 jakob      (501) staff       (20)     2724 2024-04-15 06:40:43.000000 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/PKG-INFO
+-rw-r--r--   0 jakob      (501) staff       (20)      469 2024-04-15 06:40:43.000000 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob      (501) staff       (20)        1 2024-04-15 06:40:43.000000 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob      (501) staff       (20)       74 2024-04-15 06:40:43.000000 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/requires.txt
+-rw-r--r--   0 jakob      (501) staff       (20)       18 2024-04-15 06:40:43.000000 acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/top_level.txt
```

### Comparing `acmetric_plotting-1.3.1/PKG-INFO` & `acmetric_plotting-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acmetric_plotting
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to easily build ACMetric branded plots
 Author-email: Ivan <ivan@acmetric.com>, Jakob <jakob@acmetric.com>
 Project-URL: Homepage, https://github.com/ACMetric/acmetric_package
 Project-URL: Bug Tracker, https://github.com/ACMetric/acmetric_package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,15 +14,15 @@
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.7.0
 
 <a href='https://acmetric.com/' target='_blank'><img src='https://i.postimg.cc/ZnscgcFb/Acmetric-Social-3.jpg' height="100" border='0' alt='Acmetric-Social-3'/></a> 
 # Introducing ACMetric package!
-### Current version: `1.3.1`
+### Current version: `1.3.2`
 
 This package is created to help you use ACMetric's brand colors and build plots without hours of tuning. Enjoy!
 
 ## Installing on Google Colab 
 Setting up in Google Colab is described [here](https://github.com/ACMetric/acmetric_package/blob/master/colab_setup.md).
 
 ## Importing
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: acmetric_plotting Version: 1.3.1 Summary: A package
+Metadata-Version: 2.1 Name: acmetric_plotting Version: 1.3.2 Summary: A package
 to easily build ACMetric branded plots Author-email: Ivan
 acmetric.com>, Jakob
 acmetric.com> Project-URL: Homepage, https://github.com/ACMetric/
 acmetric_package Project-URL: Bug Tracker, https://github.com/ACMetric/
 acmetric_package/issues Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENCE Requires-Dist:
 cycler>=0.11.0 Requires-Dist: matplotlib>=3.5 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: numpy>=1.20.0 Requires-Dist: scipy>=1.7.0 _[_A_c_m_e_t_r_i_c_-_S_o_c_i_a_l_-_3_]#
-Introducing ACMetric package! ### Current version: `1.3.1` This package is
+Introducing ACMetric package! ### Current version: `1.3.2` This package is
 created to help you use ACMetric's brand colors and build plots without hours
 of tuning. Enjoy! ## Installing on Google Colab Setting up in Google Colab is
 described [here](https://github.com/ACMetric/acmetric_package/blob/master/
 colab_setup.md). ## Importing We recommend importing it along with `matplotlib`
 and `seaborn`. ```python3 %matplotlib inline # display plots in the notebook
 right away %config InlineBackend.figure_format='retina' # high resolution
 import matplotlib.pyplot as plt import seaborn as sns import acmetric_plotting
```

### Comparing `acmetric_plotting-1.3.1/README.md` & `acmetric_plotting-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href='https://acmetric.com/' target='_blank'><img src='https://i.postimg.cc/ZnscgcFb/Acmetric-Social-3.jpg' height="100" border='0' alt='Acmetric-Social-3'/></a> 
 # Introducing ACMetric package!
-### Current version: `1.3.1`
+### Current version: `1.3.2`
 
 This package is created to help you use ACMetric's brand colors and build plots without hours of tuning. Enjoy!
 
 ## Installing on Google Colab 
 Setting up in Google Colab is described [here](https://github.com/ACMetric/acmetric_package/blob/master/colab_setup.md).
 
 ## Importing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-_[_A_c_m_e_t_r_i_c_-_S_o_c_i_a_l_-_3_]# Introducing ACMetric package! ### Current version: `1.3.1`
+_[_A_c_m_e_t_r_i_c_-_S_o_c_i_a_l_-_3_]# Introducing ACMetric package! ### Current version: `1.3.2`
 This package is created to help you use ACMetric's brand colors and build plots
 without hours of tuning. Enjoy! ## Installing on Google Colab Setting up in
 Google Colab is described [here](https://github.com/ACMetric/acmetric_package/
 blob/master/colab_setup.md). ## Importing We recommend importing it along with
 `matplotlib` and `seaborn`. ```python3 %matplotlib inline # display plots in
 the notebook right away %config InlineBackend.figure_format='retina' # high
 resolution import matplotlib.pyplot as plt import seaborn as sns import
```

### Comparing `acmetric_plotting-1.3.1/pyproject.toml` & `acmetric_plotting-1.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acmetric_plotting"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Ivan", email="ivan@acmetric.com" },
   { name="Jakob", email="jakob@acmetric.com" }
 
 ]
 description = "A package to easily build ACMetric branded plots"
 readme = "README.md"
```

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting/Oswald-Regular.ttf` & `acmetric_plotting-1.3.2/src/acmetric_plotting/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting/__init__.py` & `acmetric_plotting-1.3.2/src/acmetric_plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting/colors.py` & `acmetric_plotting-1.3.2/src/acmetric_plotting/colors.py`

 * *Files identical despite different names*

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting/params.py` & `acmetric_plotting-1.3.2/src/acmetric_plotting/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import fonts
 
 __all__ = ['palette', 'cmap', 'fonts']
 
 palette = color_palette(colors.color_dict.values(), desat=1)
 
 cmap = LinearSegmentedColormap.from_list(
-    'acmetric_plotting', [colors.sun, colors.coral], N=100)
+    'acmetric', [colors.sun, colors.coral], N=100)
 
 rcParams['axes.edgecolor'] = colors.stone
 rcParams['axes.labelcolor'] = colors.stone
 rcParams['axes.spines.top'] = False
 rcParams['axes.spines.right'] = False
 rcParams['axes.titlecolor'] = colors.stone
 rcParams['axes.titlesize'] = 16
```

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting/plots.py` & `acmetric_plotting-1.3.2/src/acmetric_plotting/plots.py`

 * *Files identical despite different names*

### Comparing `acmetric_plotting-1.3.1/src/acmetric_plotting.egg-info/PKG-INFO` & `acmetric_plotting-1.3.2/src/acmetric_plotting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acmetric_plotting
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to easily build ACMetric branded plots
 Author-email: Ivan <ivan@acmetric.com>, Jakob <jakob@acmetric.com>
 Project-URL: Homepage, https://github.com/ACMetric/acmetric_package
 Project-URL: Bug Tracker, https://github.com/ACMetric/acmetric_package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,15 +14,15 @@
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.7.0
 
 <a href='https://acmetric.com/' target='_blank'><img src='https://i.postimg.cc/ZnscgcFb/Acmetric-Social-3.jpg' height="100" border='0' alt='Acmetric-Social-3'/></a> 
 # Introducing ACMetric package!
-### Current version: `1.3.1`
+### Current version: `1.3.2`
 
 This package is created to help you use ACMetric's brand colors and build plots without hours of tuning. Enjoy!
 
 ## Installing on Google Colab 
 Setting up in Google Colab is described [here](https://github.com/ACMetric/acmetric_package/blob/master/colab_setup.md).
 
 ## Importing
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: acmetric_plotting Version: 1.3.1 Summary: A package
+Metadata-Version: 2.1 Name: acmetric_plotting Version: 1.3.2 Summary: A package
 to easily build ACMetric branded plots Author-email: Ivan
 acmetric.com>, Jakob
 acmetric.com> Project-URL: Homepage, https://github.com/ACMetric/
 acmetric_package Project-URL: Bug Tracker, https://github.com/ACMetric/
 acmetric_package/issues Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENCE Requires-Dist:
 cycler>=0.11.0 Requires-Dist: matplotlib>=3.5 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: numpy>=1.20.0 Requires-Dist: scipy>=1.7.0 _[_A_c_m_e_t_r_i_c_-_S_o_c_i_a_l_-_3_]#
-Introducing ACMetric package! ### Current version: `1.3.1` This package is
+Introducing ACMetric package! ### Current version: `1.3.2` This package is
 created to help you use ACMetric's brand colors and build plots without hours
 of tuning. Enjoy! ## Installing on Google Colab Setting up in Google Colab is
 described [here](https://github.com/ACMetric/acmetric_package/blob/master/
 colab_setup.md). ## Importing We recommend importing it along with `matplotlib`
 and `seaborn`. ```python3 %matplotlib inline # display plots in the notebook
 right away %config InlineBackend.figure_format='retina' # high resolution
 import matplotlib.pyplot as plt import seaborn as sns import acmetric_plotting
```

