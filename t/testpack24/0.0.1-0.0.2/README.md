# Comparing `tmp/testpack24-0.0.1.tar.gz` & `tmp/testpack24-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpack24-0.0.1.tar", max compression
+gzip compressed data, was "testpack24-0.0.2.tar", max compression
```

## Comparing `testpack24-0.0.1.tar` & `testpack24-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      228 2024-04-15 12:08:32.897583 testpack24-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      908 2024-04-15 12:05:32.074931 testpack24-0.0.1/testpack24/__init__.py
--rw-r--r--   0        0        0       13 2024-04-15 12:06:11.739565 testpack24-0.0.1/testpack24/test_module.py
--rw-r--r--   0        0        0        0 2024-04-15 12:05:55.219305 testpack24-0.0.1/testpack24/test_module.py~
--rw-r--r--   0        0        0      215 1970-01-01 00:00:00.000000 testpack24-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-04-15 12:12:23.741540 testpack24-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1147 2024-04-12 19:41:45.687388 testpack24-0.0.2/testpack24/__init__.py
+-rw-r--r--   0        0        0     5210 2024-04-11 15:06:07.537776 testpack24-0.0.2/testpack24/cluster.py
+-rw-r--r--   0        0        0     4500 2024-04-06 12:59:39.883072 testpack24-0.0.2/testpack24/isochrones.py
+-rw-r--r--   0        0        0     3034 2024-04-06 12:59:39.867071 testpack24-0.0.2/testpack24/likelihood.py
+-rw-r--r--   0        0        0    17822 2024-04-14 13:07:56.970990 testpack24-0.0.2/testpack24/synthetic.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:05:55.219305 testpack24-0.0.2/testpack24/test_module.py~
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 testpack24-0.0.2/PKG-INFO
```

### Comparing `testpack24-0.0.1/testpack24/__init__.py` & `testpack24-0.0.2/testpack24/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+from .isochrones import isochrones
+from .synthetic import synthetic
+from .cluster import cluster
+from .likelihood import likelihood
+
+# # Pull version from pyproject.toml
+# __version__ = importlib.metadata.version(__package__ or __name__)
+
 from contextlib import suppress
 import importlib.metadata
 from pathlib import Path
 
 
 def extract_version() -> str:
     """Returns either the version of the installed package or the one
```

