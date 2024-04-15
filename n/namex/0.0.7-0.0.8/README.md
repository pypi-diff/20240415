# Comparing `tmp/namex-0.0.7.tar.gz` & `tmp/namex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namex-0.0.7.tar", last modified: Mon Feb 27 23:03:18 2023, max compression
+gzip compressed data, was "namex-0.0.8.tar", last modified: Mon Apr 15 04:03:46 2024, max compression
```

## Comparing `namex-0.0.7.tar` & `namex-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-02-27 23:03:18.925519 namex-0.0.7/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      548 2023-02-03 23:53:19.000000 namex-0.0.7/LICENSE
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      245 2023-02-27 23:03:18.925285 namex-0.0.7/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5904 2023-02-05 02:45:57.000000 namex-0.0.7/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-02-27 23:03:18.924220 namex-0.0.7/namex/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      121 2023-02-05 02:32:20.000000 namex-0.0.7/namex/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3039 2023-02-14 20:13:45.000000 namex-0.0.7/namex/convert.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2221 2023-02-04 08:02:30.000000 namex-0.0.7/namex/export.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5767 2023-02-15 21:48:46.000000 namex-0.0.7/namex/generate.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-02-27 23:03:18.925027 namex-0.0.7/namex.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      245 2023-02-27 23:03:18.000000 namex-0.0.7/namex.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      211 2023-02-27 23:03:18.000000 namex-0.0.7/namex.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-02-27 23:03:18.000000 namex-0.0.7/namex.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2023-02-27 23:03:18.000000 namex-0.0.7/namex.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-02-27 23:03:18.925609 namex-0.0.7/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2023-02-27 23:02:29.000000 namex-0.0.7/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 04:03:46.991929 namex-0.0.8/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      548 2023-02-03 23:53:19.000000 namex-0.0.8/LICENSE
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      245 2024-04-15 04:03:46.991739 namex-0.0.8/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5904 2023-02-05 02:45:57.000000 namex-0.0.8/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 04:03:46.990292 namex-0.0.8/namex/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      121 2024-04-15 04:03:27.000000 namex-0.0.8/namex/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3039 2023-02-14 20:13:45.000000 namex-0.0.8/namex/convert.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2221 2023-02-04 08:02:30.000000 namex-0.0.8/namex/export.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5960 2024-04-15 04:03:03.000000 namex-0.0.8/namex/generate.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 04:03:46.991490 namex-0.0.8/namex.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      245 2024-04-15 04:03:46.000000 namex-0.0.8/namex.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      211 2024-04-15 04:03:46.000000 namex-0.0.8/namex.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-15 04:03:46.000000 namex-0.0.8/namex.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-15 04:03:46.000000 namex-0.0.8/namex.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-15 04:03:46.991979 namex-0.0.8/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-15 04:03:36.000000 namex-0.0.8/setup.py
```

### Comparing `namex-0.0.7/LICENSE` & `namex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `namex-0.0.7/README.md` & `namex-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `namex-0.0.7/namex/convert.py` & `namex-0.0.8/namex/convert.py`

 * *Files identical despite different names*

### Comparing `namex-0.0.7/namex/export.py` & `namex-0.0.8/namex/export.py`

 * *Files identical despite different names*

### Comparing `namex-0.0.7/namex/generate.py` & `namex-0.0.8/namex/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 since your modifications would be overwritten.
 """
 
 
 '''
 
 
-def generate_api_files(package, code_directory="src", verbose=False):
+def generate_api_files(package, code_directory="src", verbose=False, target_directory=None):
     """Writes out API export `__init__.py` files.
 
     Given a codebase structured as such:
 
     ```
     package/
     ...src/
@@ -91,14 +91,16 @@
     # Generate __init__ files content.
     init_files_content = {}
     for symbol in all_symbols:
         if verbose:
             print(f"...processing symbol '{symbol.__name__}'")
         for export_path in to_list(symbol._api_export_path):
             export_modules = export_path.split(".")
+            if export_modules[0] == package and target_directory is not None:
+                export_modules = [export_modules[0], target_directory] + export_modules[1:]
             export_name = export_modules[-1]
             parent_path = os.path.join(*export_modules[:-1])
             if parent_path not in init_files_content:
                 init_files_content[parent_path] = []
             init_files_content[parent_path].append(
                 {"symbol": symbol, "export_name": export_name}
             )
```

