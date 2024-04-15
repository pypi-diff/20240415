# Comparing `tmp/testpack24-0.0.4.tar.gz` & `tmp/testpack24-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpack24-0.0.4.tar", max compression
+gzip compressed data, was "testpack24-0.0.5.tar", max compression
```

## Comparing `testpack24-0.0.4.tar` & `testpack24-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936958 testpack24-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904792 testpack24-0.0.4/README.md
--rw-r--r--   0        0        0      620 2024-04-15 12:24:15.484002 testpack24-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1147 2024-04-12 19:41:45.687388 testpack24-0.0.4/testpack24/__init__.py
--rw-r--r--   0        0        0     5210 2024-04-11 15:06:07.537776 testpack24-0.0.4/testpack24/cluster.py
--rw-r--r--   0        0        0     4500 2024-04-06 12:59:39.883072 testpack24-0.0.4/testpack24/isochrones.py
--rw-r--r--   0        0        0     3034 2024-04-06 12:59:39.867071 testpack24-0.0.4/testpack24/likelihood.py
--rw-r--r--   0        0        0        0 2017-08-07 21:46:26.427264 testpack24-0.0.4/testpack24/modules/__init__.py
--rw-r--r--   0        0        0     3725 2024-04-13 14:53:07.514535 testpack24-0.0.4/testpack24/modules/imfs.py
--rw-r--r--   0        0        0    17615 2024-04-06 12:59:40.319079 testpack24-0.0.4/testpack24/modules/isochrones_priv.py
--rw-r--r--   0        0        0     9947 2024-04-06 12:59:40.119075 testpack24-0.0.4/testpack24/modules/likelihood_priv.py
--rw-r--r--   0        0        0     7845 2024-04-13 14:53:07.526535 testpack24-0.0.4/testpack24/modules/mass_binary.py
--rw-r--r--   0        0        0    32517 2024-04-13 14:44:29.560876 testpack24-0.0.4/testpack24/modules/synth_cluster_priv.py
--rw-r--r--   0        0        0    17822 2024-04-14 13:07:56.970990 testpack24-0.0.4/testpack24/synthetic.py
--rw-r--r--   0        0        0        0 2024-04-15 12:05:55.219305 testpack24-0.0.4/testpack24/test_module.py~
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testpack24-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936958 testpack24-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904792 testpack24-0.0.5/README.md
+-rw-r--r--   0        0        0      620 2024-04-15 12:27:29.613163 testpack24-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1147 2024-04-12 19:41:45.687388 testpack24-0.0.5/testpack24/__init__.py
+-rw-r--r--   0        0        0     5210 2024-04-11 15:06:07.537776 testpack24-0.0.5/testpack24/cluster.py
+-rw-r--r--   0        0        0     4500 2024-04-06 12:59:39.883072 testpack24-0.0.5/testpack24/isochrones.py
+-rw-r--r--   0        0        0     3034 2024-04-06 12:59:39.867071 testpack24-0.0.5/testpack24/likelihood.py
+-rw-r--r--   0        0        0        0 2017-08-07 21:46:26.427264 testpack24-0.0.5/testpack24/modules/__init__.py
+-rw-r--r--   0        0        0     3725 2024-04-13 14:53:07.514535 testpack24-0.0.5/testpack24/modules/imfs.py
+-rw-r--r--   0        0        0    17615 2024-04-06 12:59:40.319079 testpack24-0.0.5/testpack24/modules/isochrones_priv.py
+-rw-r--r--   0        0        0     9947 2024-04-06 12:59:40.119075 testpack24-0.0.5/testpack24/modules/likelihood_priv.py
+-rw-r--r--   0        0        0     7845 2024-04-13 14:53:07.526535 testpack24-0.0.5/testpack24/modules/mass_binary.py
+-rw-r--r--   0        0        0    32517 2024-04-13 14:44:29.560876 testpack24-0.0.5/testpack24/modules/synth_cluster_priv.py
+-rw-r--r--   0        0        0    17822 2024-04-14 13:07:56.970990 testpack24-0.0.5/testpack24/synthetic.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:05:55.219305 testpack24-0.0.5/testpack24/test_module.py~
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testpack24-0.0.5/PKG-INFO
```

### Comparing `testpack24-0.0.4/LICENSE.txt` & `testpack24-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/README.md` & `testpack24-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/pyproject.toml` & `testpack24-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testpack24"
-version = "0.0.4"
+version = "0.0.5"
 description = "Stellar cluster analysis package"
 authors = ["Gabriel I Perren <gabrielperren@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluster", "astrophysics"]
 homepage = "https://asteca.github.io/"
 repository = "https://github.com/asteca/ASteCA"
```

### Comparing `testpack24-0.0.4/testpack24/__init__.py` & `testpack24-0.0.5/testpack24/__init__.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/cluster.py` & `testpack24-0.0.5/testpack24/cluster.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/isochrones.py` & `testpack24-0.0.5/testpack24/isochrones.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/likelihood.py` & `testpack24-0.0.5/testpack24/likelihood.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/modules/imfs.py` & `testpack24-0.0.5/testpack24/modules/imfs.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/modules/isochrones_priv.py` & `testpack24-0.0.5/testpack24/modules/isochrones_priv.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/modules/likelihood_priv.py` & `testpack24-0.0.5/testpack24/modules/likelihood_priv.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/modules/mass_binary.py` & `testpack24-0.0.5/testpack24/modules/mass_binary.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/modules/synth_cluster_priv.py` & `testpack24-0.0.5/testpack24/modules/synth_cluster_priv.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/testpack24/synthetic.py` & `testpack24-0.0.5/testpack24/synthetic.py`

 * *Files identical despite different names*

### Comparing `testpack24-0.0.4/PKG-INFO` & `testpack24-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpack24
-Version: 0.0.4
+Version: 0.0.5
 Summary: Stellar cluster analysis package
 Home-page: https://asteca.github.io/
 License: MIT
 Keywords: cluster,astrophysics
 Author: Gabriel I Perren
 Author-email: gabrielperren@gmail.com
 Requires-Python: >=3.11,<4.0
```

