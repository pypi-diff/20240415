# Comparing `tmp/archyve-0.2.2.tar.gz` & `tmp/archyve-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archyve-0.2.2.tar", max compression
+gzip compressed data, was "archyve-0.2.3.tar", max compression
```

## Comparing `archyve-0.2.2.tar` & `archyve-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     9667 2024-04-14 22:32:36.500069 archyve-0.2.2/archyve.py
--rw-r--r--   0        0        0      369 2024-04-14 22:33:22.581922 archyve-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1953 2024-04-14 22:23:51.671891 archyve-0.2.2/README.md
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 archyve-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     9667 2024-04-14 22:32:36.500069 archyve-0.2.3/archyve.py
+-rw-r--r--   0        0        0      369 2024-04-14 22:41:47.070884 archyve-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1953 2024-04-14 22:23:51.671891 archyve-0.2.3/README.md
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 archyve-0.2.3/PKG-INFO
```

### Comparing `archyve-0.2.2/archyve.py` & `archyve-0.2.3/archyve.py`

 * *Files identical despite different names*

### Comparing `archyve-0.2.2/README.md` & `archyve-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `archyve-0.2.2/PKG-INFO` & `archyve-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archyve
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python toolkit for the mass management and analysis of files.
 Author: Alistair Kellaway
 Author-email: ali.kellaway139@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
```

