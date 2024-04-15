# Comparing `tmp/pldag-0.6.1.tar.gz` & `tmp/pldag-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.6.1.tar", max compression
+gzip compressed data, was "pldag-0.6.3.tar", max compression
```

## Comparing `pldag-0.6.1.tar` & `pldag-0.6.3.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.1/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.6.1/README.md
--rw-r--r--   0        0        0    11616 2024-04-12 07:41:35.861024 pldag-0.6.1/pldag/__init__.py
--rw-r--r--   0        0        0      359 2024-04-12 08:02:28.327123 pldag-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.6.3/README.md
+-rw-r--r--   0        0        0    19894 2024-04-15 07:17:06.020286 pldag-0.6.3/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.3/pldag/solver/__init__.py
+-rw-r--r--   0        0        0      800 2024-04-12 11:08:55.426504 pldag-0.6.3/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-15 07:17:20.956358 pldag-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 pldag-0.6.3/PKG-INFO
```

### Comparing `pldag-0.6.1/LICENSE` & `pldag-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.6.1/README.md` & `pldag-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.6.1/PKG-INFO` & `pldag-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.6.1
+Version: 0.6.3
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: glpk
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prime Logic Directed Acyclic Graph
 "Prime Logic Directed Acyclic Graph" data structure, or "PL-DAG" for short, is fundamentally a Directed Acyclic Graph (DAG) where each node represents a logical relationship, and the leaf nodes correspond to literals. 
 Each node in the graph encapsulates information about how its incoming nodes or leafs are logically related. For instance, a node might represent an AND operation, meaning that if it evaluates to true, all its incoming nodes or leafs must also evaluate to true.
 What sets this structure apart is that each node and leaf is associated with a prime number, and each node computes a composite prime number based on the prime numbers of its incoming nodes or leafs. This prime-based system allows for efficient manipulation and traversal of the graph while preserving logical relationships.
```

