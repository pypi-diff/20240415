# Comparing `tmp/flake8_no_else-0.1.0.tar.gz` & `tmp/flake8_no_else-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_no_else-0.1.0.tar", last modified: Sun Apr 14 14:33:54 2024, max compression
+gzip compressed data, was "flake8_no_else-0.1.1.tar", last modified: Mon Apr 15 05:18:43 2024, max compression
```

## Comparing `flake8_no_else-0.1.0.tar` & `flake8_no_else-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-14 14:33:54.846437 flake8_no_else-0.1.0/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       17 2024-04-14 14:10:46.000000 flake8_no_else-0.1.0/MANIFEST.in
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2986 2024-04-14 14:33:54.846437 flake8_no_else-0.1.0/PKG-INFO
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2071 2024-04-14 14:28:52.000000 flake8_no_else-0.1.0/README.md
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-14 14:33:54.846437 flake8_no_else-0.1.0/flake8_no_else.egg-info/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2986 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/PKG-INFO
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      317 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/SOURCES.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)        1 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/dependency_links.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       47 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/entry_points.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       63 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/requires.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       15 2024-04-14 14:33:54.000000 flake8_no_else-0.1.0/flake8_no_else.egg-info/top_level.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1342 2024-04-14 14:26:42.000000 flake8_no_else-0.1.0/flake8_no_else.py
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1059 2024-04-14 14:33:54.846437 flake8_no_else-0.1.0/setup.cfg
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       39 2024-04-14 14:23:47.000000 flake8_no_else-0.1.0/setup.py
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-14 14:33:54.846437 flake8_no_else-0.1.0/tests/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      701 2024-04-14 14:27:52.000000 flake8_no_else-0.1.0/tests/test_flake8_no_else.py
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-15 05:18:43.844137 flake8_no_else-0.1.1/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       17 2024-04-14 14:10:46.000000 flake8_no_else-0.1.1/MANIFEST.in
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2986 2024-04-15 05:18:43.844137 flake8_no_else-0.1.1/PKG-INFO
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2071 2024-04-14 14:28:52.000000 flake8_no_else-0.1.1/README.md
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-15 05:18:43.844137 flake8_no_else-0.1.1/flake8_no_else.egg-info/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2986 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/PKG-INFO
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      317 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/SOURCES.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)        1 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/dependency_links.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       47 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/entry_points.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       63 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/requires.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       15 2024-04-15 05:18:43.000000 flake8_no_else-0.1.1/flake8_no_else.egg-info/top_level.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1385 2024-04-15 05:16:35.000000 flake8_no_else-0.1.1/flake8_no_else.py
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1059 2024-04-15 05:18:43.844137 flake8_no_else-0.1.1/setup.cfg
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       39 2024-04-14 14:23:47.000000 flake8_no_else-0.1.1/setup.py
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-15 05:18:43.844137 flake8_no_else-0.1.1/tests/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      701 2024-04-15 05:11:31.000000 flake8_no_else-0.1.1/tests/test_flake8_no_else.py
```

### Comparing `flake8_no_else-0.1.0/PKG-INFO` & `flake8_no_else-0.1.1/flake8_no_else.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8_no_else
-Version: 0.1.0
+Name: flake8-no-else
+Version: 0.1.1
 Summary: A flake8 plugin to enforce object calisthenics rule "do not use ELSE"
 Home-page: https://git.nocyphr.com/flake8-plugins/flake8-no-else
 Author: Sebastian Guckes
 Author-email: nocyphr@outlook.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `flake8_no_else-0.1.0/README.md` & `flake8_no_else-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_no_else-0.1.0/flake8_no_else.egg-info/PKG-INFO` & `flake8_no_else-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8-no-else
-Version: 0.1.0
+Name: flake8_no_else
+Version: 0.1.1
 Summary: A flake8 plugin to enforce object calisthenics rule "do not use ELSE"
 Home-page: https://git.nocyphr.com/flake8-plugins/flake8-no-else
 Author: Sebastian Guckes
 Author-email: nocyphr@outlook.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `flake8_no_else-0.1.0/flake8_no_else.py` & `flake8_no_else-0.1.1/flake8_no_else.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,21 +14,21 @@
         self.errors = []
 
     def visit_If(self, node: If) -> Any:
         if not node.orelse:
             self.generic_visit(node)
             return
         if isinstance(node.orelse[0], If):
-            self.errors.append((node.lineno, node.col_offset, 'FNE101 ELIF found'))
+            self.errors.append((node.orelse[0].lineno, node.col_offset + 1, 'FNE101 ELIF found'))
         if not isinstance(node.orelse[0], If):
-            self.errors.append((node.lineno, node.col_offset, 'FNE100 ELSE found'))
+            self.errors.append((node.orelse[0].lineno - 1, node.col_offset + 1, 'FNE100 ELSE found'))
         self.generic_visit(node)
 
     def visit_IfExp(self, node: IfExp) -> Any:
-        self.errors.append((node.lineno, node.col_offset, 'FNE102 ternary ELSE found'))
+        self.errors.append((node.lineno, node.orelse.col_offset - 4, 'FNE102 ternary ELSE found'))
         self.generic_visit(node)
 
 
 class Plugin:
     name = __name__
     version = importlib_metadata.version(__name__)
```

### Comparing `flake8_no_else-0.1.0/setup.cfg` & `flake8_no_else-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8_no_else
-version = 0.1.0
+version = 0.1.1
 description = A flake8 plugin to enforce object calisthenics rule "do not use ELSE"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sebastian Guckes
 author_email = nocyphr@outlook.com
 url = https://git.nocyphr.com/flake8-plugins/flake8-no-else
 license = MIT
```

