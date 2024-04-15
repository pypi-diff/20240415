# Comparing `tmp/transformer_embeddings-4.0.8.tar.gz` & `tmp/transformer_embeddings-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_embeddings-4.0.8.tar", max compression
+gzip compressed data, was "transformer_embeddings-4.0.9.tar", max compression
```

## Comparing `transformer_embeddings-4.0.8.tar` & `transformer_embeddings-4.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11334 2024-01-11 22:23:42.624389 transformer_embeddings-4.0.8/LICENSE
--rw-r--r--   0        0        0     5589 2024-01-11 22:23:42.624389 transformer_embeddings-4.0.8/README.md
--rw-r--r--   0        0        0     1873 2024-01-11 22:23:57.312228 transformer_embeddings-4.0.8/pyproject.toml
--rw-r--r--   0        0        0      192 2024-01-11 22:23:57.300228 transformer_embeddings-4.0.8/src/transformer_embeddings/__init__.py
--rw-r--r--   0        0        0     2100 2024-01-11 22:23:42.624389 transformer_embeddings-4.0.8/src/transformer_embeddings/helpers.py
--rw-r--r--   0        0        0    11657 2024-01-11 22:23:42.624389 transformer_embeddings-4.0.8/src/transformer_embeddings/model.py
--rw-r--r--   0        0        0     1828 2024-01-11 22:23:42.624389 transformer_embeddings-4.0.8/src/transformer_embeddings/poolers.py
--rw-r--r--   0        0        0     6679 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11334 2024-01-11 23:29:51.467579 transformer_embeddings-4.0.9/LICENSE
+-rw-r--r--   0        0        0     5589 2024-01-11 23:29:51.467579 transformer_embeddings-4.0.9/README.md
+-rw-r--r--   0        0        0     1873 2024-01-11 23:30:06.279353 transformer_embeddings-4.0.9/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-01-11 23:30:06.263354 transformer_embeddings-4.0.9/src/transformer_embeddings/__init__.py
+-rw-r--r--   0        0        0     2100 2024-01-11 23:29:51.467579 transformer_embeddings-4.0.9/src/transformer_embeddings/helpers.py
+-rw-r--r--   0        0        0    11657 2024-01-11 23:29:51.467579 transformer_embeddings-4.0.9/src/transformer_embeddings/model.py
+-rw-r--r--   0        0        0     1828 2024-01-11 23:29:51.467579 transformer_embeddings-4.0.9/src/transformer_embeddings/poolers.py
+-rw-r--r--   0        0        0     6679 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.9/PKG-INFO
```

### Comparing `transformer_embeddings-4.0.8/LICENSE` & `transformer_embeddings-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.8/README.md` & `transformer_embeddings-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.8/pyproject.toml` & `transformer_embeddings-4.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-embeddings"
-version = "4.0.8"
+version = "4.0.9"
 description = "Transformer Embeddings"
 authors = ["Headspace Health <transformer-embeddings@headspace.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/HeadspaceMeditation/transformer-embeddings"
 repository = "https://github.com/HeadspaceMeditation/transformer-embeddings"
 documentation = "https://github.com/HeadspaceMeditation/transformer-embeddings"
```

### Comparing `transformer_embeddings-4.0.8/src/transformer_embeddings/helpers.py` & `transformer_embeddings-4.0.9/src/transformer_embeddings/helpers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.8/src/transformer_embeddings/model.py` & `transformer_embeddings-4.0.9/src/transformer_embeddings/model.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.8/src/transformer_embeddings/poolers.py` & `transformer_embeddings-4.0.9/src/transformer_embeddings/poolers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.8/PKG-INFO` & `transformer_embeddings-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformer-embeddings
-Version: 4.0.8
+Version: 4.0.9
 Summary: Transformer Embeddings
 Home-page: https://github.com/HeadspaceMeditation/transformer-embeddings
 License: Apache-2.0
 Author: Headspace Health
 Author-email: transformer-embeddings@headspace.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

