# Comparing `tmp/prosperity2bt-0.4.4.tar.gz` & `tmp/prosperity2bt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.4.4.tar", last modified: Sat Apr 13 14:26:03 2024, max compression
+gzip compressed data, was "prosperity2bt-0.5.0.tar", last modified: Mon Apr 15 11:32:55 2024, max compression
```

## Comparing `prosperity2bt-0.4.4.tar` & `prosperity2bt-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.904474 prosperity2bt-0.4.4/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.908474 prosperity2bt-0.4.4/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.908474 prosperity2bt-0.4.4/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.912474 prosperity2bt-0.4.4/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.912474 prosperity2bt-0.4.4/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 14:26:01.000000 prosperity2bt-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.416466 prosperity2bt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.392466 prosperity2bt-0.5.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.396466 prosperity2bt-0.5.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.396466 prosperity2bt-0.5.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.404466 prosperity2bt-0.5.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-15 11:32:50.000000 prosperity2bt-0.5.0/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:32:55.412466 prosperity2bt-0.5.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 11:32:55.000000 prosperity2bt-0.5.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-15 11:32:53.000000 prosperity2bt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:32:55.416466 prosperity2bt-0.5.0/setup.cfg
```

### Comparing `prosperity2bt-0.4.4/LICENSE` & `prosperity2bt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/PKG-INFO` & `prosperity2bt-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.4
+Version: 0.5.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.4.4/README.md` & `prosperity2bt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/__main__.py` & `prosperity2bt-0.5.0/prosperity2bt/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/data.py` & `prosperity2bt-0.5.0/prosperity2bt/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from prosperity2bt.datamodel import Symbol, Trade
 from prosperity2bt.file_reader import FileReader
 from typing import Optional
 
 LIMITS = {
     "AMETHYSTS": 20,
     "STARFRUIT": 20,
+    "ORCHIDS": 100,
+    "CHOCOLATE": 250,
+    "STRAWBERRIES": 350,
+    "ROSES": 60,
+    "GIFT_BASKET": 60,
 }
 
 @dataclass
 class PriceRow:
     day: int
     timestamp: int
     product: Symbol
```

### Comparing `prosperity2bt-0.4.4/prosperity2bt/datamodel.py` & `prosperity2bt-0.5.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/file_reader.py` & `prosperity2bt-0.5.0/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/models.py` & `prosperity2bt-0.5.0/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.5.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt/runner.py` & `prosperity2bt-0.5.0/prosperity2bt/runner.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.4/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.5.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.4
+Version: 0.5.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.4.4/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.5.0/prosperity2bt.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,8 +20,15 @@
 prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
 prosperity2bt/resources/round1/__init__.py
 prosperity2bt/resources/round1/prices_round_1_day_-1.csv
 prosperity2bt/resources/round1/prices_round_1_day_-2.csv
 prosperity2bt/resources/round1/prices_round_1_day_0.csv
 prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
 prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
-prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+prosperity2bt/resources/round3/__init__.py
+prosperity2bt/resources/round3/prices_round_3_day_0.csv
+prosperity2bt/resources/round3/prices_round_3_day_1.csv
+prosperity2bt/resources/round3/prices_round_3_day_2.csv
+prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
```

### Comparing `prosperity2bt-0.4.4/pyproject.toml` & `prosperity2bt-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.4.4"
+version = "0.5.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

