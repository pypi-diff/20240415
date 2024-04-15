# Comparing `tmp/test_option_deps-1.1.1.tar.gz` & `tmp/test_option_deps-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_option_deps-1.1.1.tar", max compression
+gzip compressed data, was "test_option_deps-2.0.0.tar", max compression
```

## Comparing `test_option_deps-1.1.1.tar` & `test_option_deps-2.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-14 07:46:47.460505 test_option_deps-1.1.1/README.md
--rw-r--r--   0        0        0      609 2024-04-15 04:44:06.908287 test_option_deps-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 07:47:11.009214 test_option_deps-1.1.1/test_option_deps/__init__.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 test_option_deps-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-14 07:46:47.460505 test_option_deps-2.0.0/README.md
+-rw-r--r--   0        0        0      534 2024-04-15 05:11:19.401480 test_option_deps-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-15 05:09:22.250707 test_option_deps-2.0.0/test_option_deps/__init__.py
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 test_option_deps-2.0.0/PKG-INFO
```

### Comparing `test_option_deps-1.1.1/PKG-INFO` & `test_option_deps-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-option-deps
-Version: 1.1.1
+Version: 2.0.0
 Summary: Testing optional dependencies
 Author: Saipraneeth
 Author-email: 2506664+msaipraneeth@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

