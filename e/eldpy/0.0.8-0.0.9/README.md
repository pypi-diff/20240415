# Comparing `tmp/eldpy-0.0.8.tar.gz` & `tmp/eldpy-0.0.9.tar.gz`

## Comparing `eldpy-0.0.8.tar` & `eldpy-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/__init__.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/annotation.py
--rw-r--r--   0        0        0    34761 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/archive.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/bulk.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/cldf2gb4e.py
--rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/colexify.py
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/collection.py
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/constants.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/delaman.py
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/download.py
--rw-r--r--   0        0        0    39466 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/elanfile.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/lod.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/paradisecconverter.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/resolver.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/testing.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/transitiveclosure.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 eldpy-0.0.8/eldpy/wikidatagraph.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 eldpy-0.0.8/executables/analyze_eafs.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/executables/annotation.py -> ../annotation.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/executables/constants.py -> ../../eldpy/constants.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/executables/elanfile.py -> /home/snordhoff/git/eldpy/elanfile.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/tests/annotation.py -> ../annotation.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/tests/constants.py -> ../constants.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.8/tests/elanfile.py -> ../elanfile.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 eldpy-0.0.8/tests/test_elan.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 eldpy-0.0.8/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 eldpy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 eldpy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/__init__.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/annotation.py
+-rw-r--r--   0        0        0    34761 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/archive.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/bulk.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/cldf2gb4e.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/colexify.py
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/collection.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/constants.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/delaman.py
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/download.py
+-rw-r--r--   0        0        0    39466 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/elanfile.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/lod.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/paradisecconverter.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/resolver.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/testing.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/transitiveclosure.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 eldpy-0.0.9/eldpy/wikidatagraph.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 eldpy-0.0.9/executables/analyze_eafs.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/executables/annotation.py -> ../annotation.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/executables/constants.py -> ../../eldpy/constants.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/executables/elanfile.py -> /home/snordhoff/git/eldpy/elanfile.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/tests/annotation.py -> ../annotation.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/tests/constants.py -> ../constants.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eldpy-0.0.9/tests/elanfile.py -> ../elanfile.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 eldpy-0.0.9/tests/test_elan.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 eldpy-0.0.9/README.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 eldpy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 eldpy-0.0.9/PKG-INFO
```

### Comparing `eldpy-0.0.8/eldpy/annotation.py` & `eldpy-0.0.9/eldpy/annotation.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/archive.py` & `eldpy-0.0.9/eldpy/archive.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/bulk.py` & `eldpy-0.0.9/eldpy/bulk.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/cldf2gb4e.py` & `eldpy-0.0.9/eldpy/cldf2gb4e.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         csv_reader = csv.DictReader(csv_file)
         for row in csv_reader:
             ID = row["ID"]
             gloss = row["Gloss"]
             primary_text = row["Primary_Text"]
             analyzed_word = row["Analyzed_Word"]
             translation = row["Translated_Text"]
-            comment = row["Comment"]
+            comment = row,get("Comment",'')
             matrix.append([ID,primary_text,analyzed_word,gloss,translation,comment])
     return matrix
 
 def get_tex_content_from_csv(filename,provided_title="", output_type="examples"):
     matrix = get_matrix_content_from_csv(filename,provided_title="")
     return get_tex_content(matrix,provided_title=provided_title,output_type=output_type)
```

### Comparing `eldpy-0.0.8/eldpy/colexify.py` & `eldpy-0.0.9/eldpy/colexify.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/collection.py` & `eldpy-0.0.9/eldpy/collection.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/constants.py` & `eldpy-0.0.9/eldpy/constants.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/delaman.py` & `eldpy-0.0.9/eldpy/delaman.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/download.py` & `eldpy-0.0.9/eldpy/download.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/elanfile.py` & `eldpy-0.0.9/eldpy/elanfile.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/lod.py` & `eldpy-0.0.9/eldpy/lod.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/paradisecconverter.py` & `eldpy-0.0.9/eldpy/paradisecconverter.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/resolver.py` & `eldpy-0.0.9/eldpy/resolver.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/testing.py` & `eldpy-0.0.9/eldpy/testing.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/transitiveclosure.py` & `eldpy-0.0.9/eldpy/transitiveclosure.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/eldpy/wikidatagraph.py` & `eldpy-0.0.9/eldpy/wikidatagraph.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/executables/analyze_eafs.py` & `eldpy-0.0.9/executables/analyze_eafs.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/tests/test_elan.py` & `eldpy-0.0.9/tests/test_elan.py`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/README.md` & `eldpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eldpy-0.0.8/pyproject.toml` & `eldpy-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "eldpy"
 description = "A Python package to download and analyze data from endangered language archives"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Sebastian Nordhoff", email = "sebastian.nordhoff@glottotopia.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 
 dependencies = [
```

### Comparing `eldpy-0.0.8/PKG-INFO` & `eldpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eldpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package to download and analyze data from endangered language archives
 Project-URL: Homepage, https://github.com/ZAS-QUEST/eldpy
 Project-URL: Bug Tracker, https://github.com/ZAS-QUEST/eldpy/issues
 Author-email: Sebastian Nordhoff <sebastian.nordhoff@glottotopia.de>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

