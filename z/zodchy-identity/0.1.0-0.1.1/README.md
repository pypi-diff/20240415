# Comparing `tmp/zodchy_identity-0.1.0.tar.gz` & `tmp/zodchy_identity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_identity-0.1.0.tar", max compression
+gzip compressed data, was "zodchy_identity-0.1.1.tar", max compression
```

## Comparing `zodchy_identity-0.1.0.tar` & `zodchy_identity-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_identity-0.1.0/README.md
--rw-r--r--   0        0        0      394 2024-04-13 13:43:37.851263 zodchy_identity-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       50 2024-04-05 16:44:15.845279 zodchy_identity-0.1.0/zodchy_identity/__init__.py
--rw-r--r--   0        0        0      630 2024-04-02 15:23:42.896231 zodchy_identity-0.1.0/zodchy_identity/uuids.py
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 zodchy_identity-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_identity-0.1.1/README.md
+-rw-r--r--   0        0        0      452 2024-04-15 11:08:51.233041 zodchy_identity-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-05 16:44:15.845279 zodchy_identity-0.1.1/zodchy_identity/__init__.py
+-rw-r--r--   0        0        0      630 2024-04-02 15:23:42.896231 zodchy_identity-0.1.1/zodchy_identity/uuids.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 zodchy_identity-0.1.1/PKG-INFO
```

### Comparing `zodchy_identity-0.1.0/zodchy_identity/uuids.py` & `zodchy_identity-0.1.1/zodchy_identity/uuids.py`

 * *Files identical despite different names*

