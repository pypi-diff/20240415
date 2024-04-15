# Comparing `tmp/trm_woodburn-0.0.5.tar.gz` & `tmp/trm_woodburn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.5.tar", last modified: Mon Apr 15 21:34:38 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.6.tar", last modified: Mon Apr 15 21:41:59 2024, max compression
```

## Comparing `trm_woodburn-0.0.5.tar` & `trm_woodburn-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.250509 trm_woodburn-0.0.5/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.5/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6965 2024-04-15 21:34:38.250453 trm_woodburn-0.0.5/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6486 2024-04-15 21:33:57.000000 trm_woodburn-0.0.5/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.5/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:34:38.250730 trm_woodburn-0.0.5/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.248693 trm_woodburn-0.0.5/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.249536 trm_woodburn-0.0.5/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.5/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.5/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.250281 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6965 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.236250 trm_woodburn-0.0.6/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.6/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     7308 2024-04-15 21:41:59.236194 trm_woodburn-0.0.6/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6829 2024-04-15 21:41:16.000000 trm_woodburn-0.0.6/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.6/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:41:59.236465 trm_woodburn-0.0.6/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.234597 trm_woodburn-0.0.6/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.235259 trm_woodburn-0.0.6/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.6/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.6/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:41:59.236020 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     7308 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:41:59.000000 trm_woodburn-0.0.6/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.5/LICENSE.txt` & `trm_woodburn-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.5/PKG-INFO` & `trm_woodburn-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -171,14 +171,14 @@
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
 
 
-[fig_heat_uni]: figures/fig_heat_uni.png
-[fig_heat_ascii]: figures/fig_heat_ascii.png
-[fig_plot]: figures/fig_plot.png
-[fig_plot_1]: figures/fig_plot_1.png
-[fig_plot_5]: figures/fig_plot_5.png
-[fig_sparsity_uni]: figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: figures/fig_sparsity_ascii.png
+[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
+[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
+[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
+[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
+[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
+[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
+[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

### Comparing `trm_woodburn-0.0.5/README.md` & `trm_woodburn-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -156,14 +156,14 @@
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
 
 
-[fig_heat_uni]: figures/fig_heat_uni.png
-[fig_heat_ascii]: figures/fig_heat_ascii.png
-[fig_plot]: figures/fig_plot.png
-[fig_plot_1]: figures/fig_plot_1.png
-[fig_plot_5]: figures/fig_plot_5.png
-[fig_sparsity_uni]: figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: figures/fig_sparsity_ascii.png
+[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
+[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
+[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
+[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
+[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
+[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
+[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

### Comparing `trm_woodburn-0.0.5/setup.cfg` & `trm_woodburn-0.0.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.5
+version = 0.0.6
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.5/src/trm/trm.py` & `trm_woodburn-0.0.6/src/trm/trm.py`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.5/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.6/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -171,14 +171,14 @@
 width of the current terminal window will be used.
 
 ```
  44% [/////////////////////----------------------------] -00:00:02.1
 ```
 
 
-[fig_heat_uni]: figures/fig_heat_uni.png
-[fig_heat_ascii]: figures/fig_heat_ascii.png
-[fig_plot]: figures/fig_plot.png
-[fig_plot_1]: figures/fig_plot_1.png
-[fig_plot_5]: figures/fig_plot_5.png
-[fig_sparsity_uni]: figures/fig_sparsity_uni.png
-[fig_sparsity_ascii]: figures/fig_sparsity_ascii.png
+[fig_heat_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_uni.png
+[fig_heat_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_heat_ascii.png
+[fig_plot]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot.png
+[fig_plot_1]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_1.png
+[fig_plot_5]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_plot_5.png
+[fig_sparsity_uni]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_uni.png
+[fig_sparsity_ascii]: https://gitlab.com/davidwoodburn/trm/-/blob/main/figures/fig_sparsity_ascii.png
```

