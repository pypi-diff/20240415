# Comparing `tmp/atomrdf-0.4.2.tar.gz` & `tmp/atomrdf-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomrdf-0.4.2.tar", last modified: Mon Apr 15 10:29:06 2024, max compression
+gzip compressed data, was "atomrdf-0.4.3.tar", last modified: Mon Apr 15 10:33:42 2024, max compression
```

## Comparing `atomrdf-0.4.2.tar` & `atomrdf-0.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 10:29:03.000000 atomrdf-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 10:29:03.000000 atomrdf-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:29:06.358624 atomrdf-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 10:29:03.000000 atomrdf-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.354624 atomrdf-0.4.2/atomrdf/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/atomrdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/json_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/atomrdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    37476 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/atomrdf/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/workflow/pyiron.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-15 10:29:03.000000 atomrdf-0.4.2/atomrdf/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/atomrdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 10:29:06.000000 atomrdf-0.4.2/atomrdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:29:06.358624 atomrdf-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 10:29:06.000000 atomrdf-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:29:06.358624 atomrdf-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 10:29:03.000000 atomrdf-0.4.2/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 10:29:03.000000 atomrdf-0.4.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 10:29:03.000000 atomrdf-0.4.2/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.303616 atomrdf-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 10:33:39.000000 atomrdf-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 10:33:39.000000 atomrdf-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:33:42.303616 atomrdf-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 10:33:39.000000 atomrdf-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.299616 atomrdf-0.4.3/atomrdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.299616 atomrdf-0.4.3/atomrdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/json_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.299616 atomrdf-0.4.3/atomrdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37476 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.303616 atomrdf-0.4.3/atomrdf/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/workflow/pyiron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-15 10:33:39.000000 atomrdf-0.4.3/atomrdf/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.303616 atomrdf-0.4.3/atomrdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 10:33:42.000000 atomrdf-0.4.3/atomrdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:33:42.303616 atomrdf-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 10:33:42.000000 atomrdf-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:42.303616 atomrdf-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 10:33:40.000000 atomrdf-0.4.3/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 10:33:40.000000 atomrdf-0.4.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 10:33:40.000000 atomrdf-0.4.3/tests/test_structuregraph.py
```

### Comparing `atomrdf-0.4.2/LICENSE` & `atomrdf-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/PKG-INFO` & `atomrdf-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.4.2
+Version: 0.4.3
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomrdf-0.4.2/README.md` & `atomrdf-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/data/asmo.owl` & `atomrdf-0.4.3/atomrdf/data/asmo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/data/cmso.owl` & `atomrdf-0.4.3/atomrdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/data/element.yml` & `atomrdf-0.4.3/atomrdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/data/pldo.owl` & `atomrdf-0.4.3/atomrdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/data/podo.owl` & `atomrdf-0.4.3/atomrdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/graph.py` & `atomrdf-0.4.3/atomrdf/graph.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/json_io.py` & `atomrdf-0.4.3/atomrdf/json_io.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/network/network.py` & `atomrdf-0.4.3/atomrdf/network/network.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/network/ontology.py` & `atomrdf-0.4.3/atomrdf/network/ontology.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/network/parser.py` & `atomrdf-0.4.3/atomrdf/network/parser.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/network/patch.py` & `atomrdf-0.4.3/atomrdf/network/patch.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/network/term.py` & `atomrdf-0.4.3/atomrdf/network/term.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/properties.py` & `atomrdf-0.4.3/atomrdf/properties.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/stores.py` & `atomrdf-0.4.3/atomrdf/stores.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/structure.py` & `atomrdf-0.4.3/atomrdf/structure.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/visualize.py` & `atomrdf-0.4.3/atomrdf/visualize.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/workflow/pyiron.py` & `atomrdf-0.4.3/atomrdf/workflow/pyiron.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf/workflow/workflow.py` & `atomrdf-0.4.3/atomrdf/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/atomrdf.egg-info/PKG-INFO` & `atomrdf-0.4.3/atomrdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.4.2
+Version: 0.4.3
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `atomrdf-0.4.2/atomrdf.egg-info/SOURCES.txt` & `atomrdf-0.4.3/atomrdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/setup.py` & `atomrdf-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='atomrdf',
-    version='0.4.2',
+    version='0.4.3',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['atomrdf', 'atomrdf.*']),
     zip_safe=False,
```

### Comparing `atomrdf-0.4.2/tests/test_encoder_and_write.py` & `atomrdf-0.4.3/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/tests/test_graph.py` & `atomrdf-0.4.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.2/tests/test_structuregraph.py` & `atomrdf-0.4.3/tests/test_structuregraph.py`

 * *Files identical despite different names*

