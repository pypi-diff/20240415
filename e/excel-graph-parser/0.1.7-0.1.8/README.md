# Comparing `tmp/excel_graph_parser-0.1.7.tar.gz` & `tmp/excel_graph_parser-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel_graph_parser-0.1.7.tar", last modified: Tue Apr  2 14:25:24 2024, max compression
+gzip compressed data, was "excel_graph_parser-0.1.8.tar", last modified: Mon Apr 15 14:20:45 2024, max compression
```

## Comparing `excel_graph_parser-0.1.7.tar` & `excel_graph_parser-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.7/LICENSE
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-02-14 06:51:33.000000 excel_graph_parser-0.1.7/README.md
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.859020 excel_graph_parser-0.1.7/excel_graph_parser/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.7/excel_graph_parser/__init__.py
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13582 2024-04-02 14:24:07.000000 excel_graph_parser-0.1.7/excel_graph_parser/graph_parser.py
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/SOURCES.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/dependency_links.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/requires.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/top_level.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-04-02 14:24:07.000000 excel_graph_parser-0.1.7/pyproject.toml
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/setup.cfg
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.8/LICENSE
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-02-14 06:51:33.000000 excel_graph_parser-0.1.8/README.md
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/excel_graph_parser/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.8/excel_graph_parser/__init__.py
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13475 2024-04-15 14:17:41.000000 excel_graph_parser-0.1.8/excel_graph_parser/graph_parser.py
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/requires.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/top_level.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-04-15 14:18:44.000000 excel_graph_parser-0.1.8/pyproject.toml
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/setup.cfg
```

### Comparing `excel_graph_parser-0.1.7/LICENSE` & `excel_graph_parser-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.7/PKG-INFO` & `excel_graph_parser-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.7
+Version: 0.1.8
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
```

### Comparing `excel_graph_parser-0.1.7/README.md` & `excel_graph_parser-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.7/excel_graph_parser/graph_parser.py` & `excel_graph_parser-0.1.8/excel_graph_parser/graph_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,44 +133,41 @@
                     x_axis_title = chart.x_axis.title.tx.rich.p[0].r[-1].t
                 if chart.y_axis.title:
                     y_axis_title = chart.y_axis.title.tx.rich.p[0].r[-1].t
 
             # Get series data
             for i, serie in enumerate(chart.series):
                 if chart_type == "scatterChart":
-                    try:
-                        input_cat_range = serie.xVal.strRef.f
-                        input_cat_format = None
-                    except AttributeError:
-                        input_cat_range = serie.xVal.numRef.f
-                        input_cat_format = serie.xVal.numRef.numCache.formatCode
-                        input_cat_format = None if input_cat_format == "General" else input_cat_format
-                    try:
-                        input_val_range = serie.yVal.strRef.f
-                        input_val_format = None
-                    except AttributeError:
-                        input_val_range = serie.yVal.numRef.f
-                        input_val_format = serie.yVal.numRef.numCache.formatCode
-                        input_val_format = None if input_val_format == "General" else input_val_format
+                    if serie.xVal:
+                        if serie.xVal.strRef:
+                            input_cat_range = serie.xVal.strRef.f
+                            input_cat_format = None
+                        elif serie.xVal.numRef:
+                            input_cat_range = serie.xVal.numRef.f
+                            input_cat_format = serie.xVal.numRef.numCache.formatCode
+                            input_cat_format = None if input_cat_format == "General" else input_cat_format
+
+                    input_val_range = serie.yVal.numRef.f
+                    input_val_format = serie.yVal.numRef.numCache.formatCode
+                    input_val_format = None if input_val_format == "General" else input_val_format
 
                 else:
-                    try:
-                        input_cat_range = serie.cat.strRef.f
-                        input_cat_format = None
-                    except AttributeError:
-                        input_cat_range = serie.cat.numRef.f
-                        input_cat_format = serie.cat.numRef.numCache.formatCode
-                        input_cat_format = None if input_cat_format == "General" else input_cat_format
-                    try:
-                        input_val_range = serie.val.strRef.f
-                        input_val_format = None
-                    except AttributeError:
-                        input_val_range = serie.val.numRef.f
-                        input_val_format = serie.val.numRef.numCache.formatCode
-                        input_val_format = None if input_val_format == "General" else input_val_format
+                    if serie.cat:
+                        # if no category data in the sequence, use the one that was set for the previous sequence
+                        if serie.cat.strRef:
+                            input_cat_range = serie.cat.strRef.f
+                            input_cat_format = None
+                        elif serie.cat.numRef:
+                            input_cat_range = serie.cat.numRef.f
+                            input_cat_format = serie.cat.numRef.numCache.formatCode
+                            input_cat_format = None if input_cat_format == "General" else input_cat_format
+
+                    input_val_range = serie.val.numRef.f
+                    input_val_format = serie.val.numRef.numCache.formatCode
+                    input_val_format = None if input_val_format == "General" else input_val_format
 
                 chart_sheet_name = input_cat_range.replace('(', '').replace(')', '').replace("'", "").split(sep="!")[0]
 
                 chart_cat_range = input_cat_range.replace('(', '').replace(')', '').replace("'", "").replace(f"{chart_sheet_name}!", "").replace('$', "")
                 chart_cat_range = chart_cat_range.split(",")[0] + ":" + chart_cat_range.split(",")[-1] if "," in chart_cat_range else chart_cat_range
                 cat_data = []
                 for element in wb[chart_sheet_name][chart_cat_range]:
```

### Comparing `excel_graph_parser-0.1.7/excel_graph_parser.egg-info/PKG-INFO` & `excel_graph_parser-0.1.8/excel_graph_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.7
+Version: 0.1.8
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
```

### Comparing `excel_graph_parser-0.1.7/pyproject.toml` & `excel_graph_parser-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "excel_graph_parser"
-version = "0.1.7"
+version = "0.1.8"
 description = "Parser to translate excel graphs to Plotly figures"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "D. Sommers", email = "dsommers@viktor.ai" }
 ]
```

