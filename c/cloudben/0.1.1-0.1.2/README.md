# Comparing `tmp/cloudben-0.1.1.tar.gz` & `tmp/cloudben-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudben-0.1.1.tar", max compression
+gzip compressed data, was "cloudben-0.1.2.tar", max compression
```

## Comparing `cloudben-0.1.1.tar` & `cloudben-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2195 2024-04-14 22:43:08.041696 cloudben-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-13 13:57:16.103585 cloudben-0.1.1/cloudben/__init__.py
--rw-r--r--   0        0        0       47 2024-04-14 21:11:44.761628 cloudben-0.1.1/cloudben/__main__.py
--rw-r--r--   0        0        0     6485 2024-04-14 22:25:26.930853 cloudben-0.1.1/cloudben/main.py
--rw-r--r--   0        0        0      463 2024-04-14 22:43:09.751086 cloudben-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 cloudben-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2195 2024-04-15 01:27:04.786398 cloudben-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 01:27:04.786398 cloudben-0.1.2/cloudben/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-15 01:27:04.786398 cloudben-0.1.2/cloudben/__main__.py
+-rw-r--r--   0        0        0     6485 2024-04-15 01:27:04.786398 cloudben-0.1.2/cloudben/main.py
+-rw-r--r--   0        0        0      463 2024-04-15 01:27:04.786398 cloudben-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 cloudben-0.1.2/PKG-INFO
```

### Comparing `cloudben-0.1.1/README.md` & `cloudben-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudben-0.1.1/cloudben/main.py` & `cloudben-0.1.2/cloudben/main.py`

 * *Files identical despite different names*

### Comparing `cloudben-0.1.1/PKG-INFO` & `cloudben-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudben
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simply CLI tool to interact with the Cloudflare APIs.
 Author: Alberto Gallinaro
 Author-email: alberto.gallinaro@audienceview.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

