# Comparing `tmp/isbtchot-1.1.0.tar.gz` & `tmp/isbtchot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isbtchot-1.1.0.tar", last modified: Sat Apr 13 10:49:43 2024, max compression
+gzip compressed data, was "isbtchot-1.1.1.tar", last modified: Mon Apr 15 08:40:15 2024, max compression
```

## Comparing `isbtchot-1.1.0.tar` & `isbtchot-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 10:49:36.000000 isbtchot-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 10:49:43.844064 isbtchot-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-13 10:49:36.000000 isbtchot-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-13 10:49:36.000000 isbtchot-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:49:43.844064 isbtchot-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.840064 isbtchot-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.840064 isbtchot-1.1.0/src/isbtchot/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/src/isbtchot/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/schemas/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/src/isbtchot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:40:15.598988 isbtchot-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:40:11.000000 isbtchot-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-15 08:40:15.598988 isbtchot-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-15 08:40:11.000000 isbtchot-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 08:40:11.000000 isbtchot-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:40:15.598988 isbtchot-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:40:15.594988 isbtchot-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:40:15.598988 isbtchot-1.1.1/src/isbtchot/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:40:15.598988 isbtchot-1.1.1/src/isbtchot/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/schemas/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-15 08:40:11.000000 isbtchot-1.1.1/src/isbtchot/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:40:15.598988 isbtchot-1.1.1/src/isbtchot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-15 08:40:15.000000 isbtchot-1.1.1/src/isbtchot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-15 08:40:15.000000 isbtchot-1.1.1/src/isbtchot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:40:15.000000 isbtchot-1.1.1/src/isbtchot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 08:40:15.000000 isbtchot-1.1.1/src/isbtchot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 08:40:15.000000 isbtchot-1.1.1/src/isbtchot.egg-info/top_level.txt
```

### Comparing `isbtchot-1.1.0/LICENSE` & `isbtchot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isbtchot-1.1.0/PKG-INFO` & `isbtchot-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: isbtchot
-Version: 1.1.0
+Version: 1.1.1
 Summary: TBD
 Author-email: Daniel <dakixr@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: requests
+Requires-Dist: scikit-learn
 
 # isbtchot: BTC Hotness Index Dashboard
 
 The `isbtchot` package provides a minimalist terminal dashboard for visualizing Bitcoin's (BTC) hotness index. It utilizes historical BTC data to generate visualizations of BTC's price alongside the Hotness Index, directly in your terminal.
 
 ## Features:
 
@@ -40,25 +41,25 @@
 - `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
 | Argument       | Short Form | Description                                                                     | Default   |
 |----------------|------------|---------------------------------------------------------------------------------|-----------|
 | `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
-| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--time`        | `-t`       | Candlestick time to use (e.g., M for Monthly, W for Weekly).                   | W         |
 | `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
 
 ## Demo
 
 ### Hotness Index Dashboard
 Historically very reliable for bull market tops:
 ![BTC Hotness Index Dashboard Demo](media/demo.png)
 
 ### Power Law Delta Dashboard
-Historically very reliable for bull market bottoms:
+Historically very reliable for bear market bottoms:
 ![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
 - For optimal visualization, maximize your terminal window.
 - Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
```

### Comparing `isbtchot-1.1.0/README.md` & `isbtchot-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 - `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
 | Argument       | Short Form | Description                                                                     | Default   |
 |----------------|------------|---------------------------------------------------------------------------------|-----------|
 | `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
-| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--time`        | `-t`       | Candlestick time to use (e.g., M for Monthly, W for Weekly).                   | W         |
 | `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
 
 ## Demo
 
 ### Hotness Index Dashboard
 Historically very reliable for bull market tops:
 ![BTC Hotness Index Dashboard Demo](media/demo.png)
 
 ### Power Law Delta Dashboard
-Historically very reliable for bull market bottoms:
+Historically very reliable for bear market bottoms:
 ![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
 - For optimal visualization, maximize your terminal window.
 - Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
```

### Comparing `isbtchot-1.1.0/src/isbtchot/__main__.py` & `isbtchot-1.1.1/src/isbtchot/__main__.py`

 * *Files identical despite different names*

### Comparing `isbtchot-1.1.0/src/isbtchot/controller.py` & `isbtchot-1.1.1/src/isbtchot/controller.py`

 * *Files identical despite different names*

### Comparing `isbtchot-1.1.0/src/isbtchot/model.py` & `isbtchot-1.1.1/src/isbtchot/model.py`

 * *Files identical despite different names*

### Comparing `isbtchot-1.1.0/src/isbtchot/view.py` & `isbtchot-1.1.1/src/isbtchot/view.py`

 * *Files identical despite different names*

### Comparing `isbtchot-1.1.0/src/isbtchot.egg-info/PKG-INFO` & `isbtchot-1.1.1/src/isbtchot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: isbtchot
-Version: 1.1.0
+Version: 1.1.1
 Summary: TBD
 Author-email: Daniel <dakixr@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: requests
+Requires-Dist: scikit-learn
 
 # isbtchot: BTC Hotness Index Dashboard
 
 The `isbtchot` package provides a minimalist terminal dashboard for visualizing Bitcoin's (BTC) hotness index. It utilizes historical BTC data to generate visualizations of BTC's price alongside the Hotness Index, directly in your terminal.
 
 ## Features:
 
@@ -40,25 +41,25 @@
 - `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
 | Argument       | Short Form | Description                                                                     | Default   |
 |----------------|------------|---------------------------------------------------------------------------------|-----------|
 | `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
-| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--time`        | `-t`       | Candlestick time to use (e.g., M for Monthly, W for Weekly).                   | W         |
 | `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
 
 ## Demo
 
 ### Hotness Index Dashboard
 Historically very reliable for bull market tops:
 ![BTC Hotness Index Dashboard Demo](media/demo.png)
 
 ### Power Law Delta Dashboard
-Historically very reliable for bull market bottoms:
+Historically very reliable for bear market bottoms:
 ![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
 - For optimal visualization, maximize your terminal window.
 - Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
```

