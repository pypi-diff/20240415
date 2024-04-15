# Comparing `tmp/caustic.lexer-1.2.1.tar.gz` & `tmp/caustic.lexer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.lexer-1.2.1.tar", last modified: Mon Apr 15 01:43:31 2024, max compression
+gzip compressed data, was "caustic.lexer-1.2.2.tar", last modified: Mon Apr 15 03:48:43 2024, max compression
```

## Comparing `caustic.lexer-1.2.1.tar` & `caustic.lexer-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.840969 caustic.lexer-1.2.1/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.2.1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     7504 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     6572 2024-04-15 01:36:25.000000 caustic.lexer-1.2.1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-15 01:43:15.000000 caustic.lexer-1.2.1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-15 01:43:31.840969 caustic.lexer-1.2.1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.830969 caustic.lexer-1.2.1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.830969 caustic.lexer-1.2.1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.2.1/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.2.1/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.2.1/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1382 2024-04-15 01:40:52.000000 caustic.lexer-1.2.1/src/caustic/lexer/grammar.cag
--rw-r--r--   0 shae      (1000) shae      (1000)    14142 2024-04-12 23:45:20.000000 caustic.lexer-1.2.1/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3281 2024-04-15 01:43:29.000000 caustic.lexer-1.2.1/src/caustic/lexer/precompiled_nodes.pkl
--rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.2.1/src/caustic/lexer/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.2.1/src/caustic/lexer/util.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     7504 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 03:48:43.754054 caustic.lexer-1.2.2/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.2.2/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     7607 2024-04-15 03:48:43.754054 caustic.lexer-1.2.2/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     6675 2024-04-15 02:09:50.000000 caustic.lexer-1.2.2/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-15 02:00:48.000000 caustic.lexer-1.2.2/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-15 03:48:43.754054 caustic.lexer-1.2.2/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 03:48:43.747387 caustic.lexer-1.2.2/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 03:48:43.747387 caustic.lexer-1.2.2/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 03:48:43.750720 caustic.lexer-1.2.2/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.2.2/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.2.2/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.2.2/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1382 2024-04-15 01:40:52.000000 caustic.lexer-1.2.2/src/caustic/lexer/grammar.cag
+-rw-r--r--   0 shae      (1000) shae      (1000)    14143 2024-04-15 02:06:07.000000 caustic.lexer-1.2.2/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3281 2024-04-15 03:48:41.000000 caustic.lexer-1.2.2/src/caustic/lexer/precompiled_nodes.pkl
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.2.2/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.2.2/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 03:48:43.754054 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     7607 2024-04-15 03:48:43.000000 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-15 03:48:43.000000 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-15 03:48:43.000000 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-15 03:48:43.000000 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-15 03:48:43.000000 caustic.lexer-1.2.2/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic.lexer-1.2.1/LICENSE` & `caustic.lexer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/PKG-INFO` & `caustic.lexer-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -218,7 +218,11 @@
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
 
 ## 1.2.1
 - Fixed several nodes improperly stripping whitespace
+
+## 1.2.2
+- Fixed unpacking never triggering
+- Fixed `NodeRange`s raising exceptions upon backtracking
```

### Comparing `caustic.lexer-1.2.1/README.md` & `caustic.lexer-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -194,7 +194,11 @@
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
 
 ## 1.2.1
 - Fixed several nodes improperly stripping whitespace
+
+## 1.2.2
+- Fixed unpacking never triggering
+- Fixed `NodeRange`s raising exceptions upon backtracking
```

### Comparing `caustic.lexer-1.2.1/pyproject.toml` & `caustic.lexer-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
```

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/__init__.py` & `caustic.lexer-1.2.2/src/caustic/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/basic_compiler.py` & `caustic.lexer-1.2.2/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/compiler.py` & `caustic.lexer-1.2.2/src/caustic/lexer/compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/grammar.cag` & `caustic.lexer-1.2.2/src/caustic/lexer/grammar.cag`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/nodes.py` & `caustic.lexer-1.2.2/src/caustic/lexer/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 assert not stealer
                 bm.load_pos(save)
                 return NO_MATCH
             # Check how we should return results
             if n.name is None: # not assigned a name ("[name]:<node>")
                 if isinstance(results, dict): continue # don't add it
                 if not single_result: results.append(res)
-            elif n.name == b'^': # unpack name
+            elif n.name == '^': # unpack name
                 if single_result:
                     te = TypeError(f'Conflicting return types: unpack result cannot be added to single result')
                     te.add_note(str(n))
                     te.add_note(f'In {self}')
                     raise te
                 if isinstance(res, dict):
                     if not isinstance(results, dict):
@@ -216,15 +216,15 @@
         results = []
         save = bm.save_pos()
         for _ in range(self.min):
             try: results.append(self.node(bm, stealer=stealer))
             except NodeSyntaxError as nse:
                 raise NodeSyntaxError(self, bm, f'Expected at least {self.min} of {self.node}') from nse
             if results[-1] is NO_MATCH:
-                self.load_pos()
+                bm.load_pos(save)
                 return NO_MATCH
             if not self.keep_whitespace:
                 bm.match(WHITESPACE_PATT)
         if self.max is None:
             while (res := self.node(bm)) is not NO_MATCH:
                 results.append(res)
                 if not self.keep_whitespace:
```

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/precompiled_nodes.pkl` & `caustic.lexer-1.2.2/src/caustic/lexer/precompiled_nodes.pkl`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/serialize.py` & `caustic.lexer-1.2.2/src/caustic/lexer/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic/lexer/util.py` & `caustic.lexer-1.2.2/src/caustic/lexer/util.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.1/src/caustic.lexer.egg-info/PKG-INFO` & `caustic.lexer-1.2.2/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -218,7 +218,11 @@
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
 
 ## 1.2.1
 - Fixed several nodes improperly stripping whitespace
+
+## 1.2.2
+- Fixed unpacking never triggering
+- Fixed `NodeRange`s raising exceptions upon backtracking
```

