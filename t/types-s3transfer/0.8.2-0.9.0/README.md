# Comparing `tmp/types_s3transfer-0.8.2.tar.gz` & `tmp/types_s3transfer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_s3transfer-0.8.2.tar", max compression
+gzip compressed data, was "types_s3transfer-0.9.0.tar", max compression
```

## Comparing `types_s3transfer-0.8.2.tar` & `types_s3transfer-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/LICENSE
--rw-r--r--   0        0        0     2329 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/README.md
--rw-r--r--   0        0        0     2668 2023-11-30 00:56:16.028966 types_s3transfer-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4648 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/__init__.pyi
--rw-r--r--   0        0        0     2533 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/bandwidth.pyi
--rw-r--r--   0        0        0      499 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/compat.pyi
--rw-r--r--   0        0        0      122 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/constants.pyi
--rw-r--r--   0        0        0      868 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/copies.pyi
--rw-r--r--   0        0        0     6491 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/crt.pyi
--rw-r--r--   0        0        0      187 2023-11-30 00:55:52.441003 types_s3transfer-0.8.2/s3transfer-stubs/delete.pyi
--rw-r--r--   0        0        0     5013 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/download.pyi
--rw-r--r--   0        0        0      396 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/exceptions.pyi
--rw-r--r--   0        0        0     4542 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/futures.pyi
--rw-r--r--   0        0        0     5138 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/manager.pyi
--rw-r--r--   0        0        0     5348 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/processpool.pyi
--rw-r--r--   0        0        0        0 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/py.typed
--rw-r--r--   0        0        0      689 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/subscribers.pyi
--rw-r--r--   0        0        0      748 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/tasks.pyi
--rw-r--r--   0        0        0     4446 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/upload.pyi
--rw-r--r--   0        0        0     5725 2023-11-30 00:55:52.445003 types_s3transfer-0.8.2/s3transfer-stubs/utils.pyi
--rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 types_s3transfer-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2329 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/README.md
+-rw-r--r--   0        0        0     2668 2023-12-14 00:56:08.120005 types_s3transfer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4648 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2533 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/bandwidth.pyi
+-rw-r--r--   0        0        0      499 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/compat.pyi
+-rw-r--r--   0        0        0      122 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/constants.pyi
+-rw-r--r--   0        0        0      868 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/copies.pyi
+-rw-r--r--   0        0        0     6491 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/crt.pyi
+-rw-r--r--   0        0        0      187 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/delete.pyi
+-rw-r--r--   0        0        0     5013 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/download.pyi
+-rw-r--r--   0        0        0      396 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     4542 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/futures.pyi
+-rw-r--r--   0        0        0     5138 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/manager.pyi
+-rw-r--r--   0        0        0     5348 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/processpool.pyi
+-rw-r--r--   0        0        0        0 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/py.typed
+-rw-r--r--   0        0        0      689 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/subscribers.pyi
+-rw-r--r--   0        0        0      748 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/tasks.pyi
+-rw-r--r--   0        0        0     4446 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/upload.pyi
+-rw-r--r--   0        0        0     5725 2023-12-14 00:55:44.075953 types_s3transfer-0.9.0/s3transfer-stubs/utils.pyi
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 types_s3transfer-0.9.0/PKG-INFO
```

### Comparing `types_s3transfer-0.8.2/LICENSE` & `types_s3transfer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/README.md` & `types_s3transfer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/pyproject.toml` & `types_s3transfer-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "types-s3transfer"
-version = "0.8.2"
+version = "0.9.0"
 description = "Type annotations and code completion for s3transfer"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/types-s3transfer"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/__init__.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/bandwidth.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/bandwidth.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/copies.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/copies.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/crt.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/download.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/download.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/futures.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/futures.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/manager.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/manager.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/processpool.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/processpool.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/subscribers.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/subscribers.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/tasks.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/tasks.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/upload.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/upload.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/s3transfer-stubs/utils.pyi` & `types_s3transfer-0.9.0/s3transfer-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types_s3transfer-0.8.2/PKG-INFO` & `types_s3transfer-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-s3transfer
-Version: 0.8.2
+Version: 0.9.0
 Summary: Type annotations and code completion for s3transfer
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: s3transfer,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
```

