# Comparing `tmp/wrapchain-0.0.1.tar.gz` & `tmp/wrapchain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapchain-0.0.1.tar", max compression
+gzip compressed data, was "wrapchain-0.0.2.tar", max compression
```

## Comparing `wrapchain-0.0.1.tar` & `wrapchain-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       14 2024-04-15 12:31:24.938306 wrapchain-0.0.1/README.md
--rw-r--r--   0        0        0      342 2024-04-15 12:56:54.516397 wrapchain-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       58 2024-04-15 12:54:02.130204 wrapchain-0.0.1/wrapchain/__init__.py
--rw-r--r--   0        0        0      435 2024-04-15 13:22:08.860436 wrapchain-0.0.1/wrapchain/main.py
--rw-r--r--   0        0        0     1217 2024-04-15 13:21:54.570632 wrapchain-0.0.1/wrapchain/wrapchain.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 wrapchain-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-04-15 12:31:24.938306 wrapchain-0.0.2/README.md
+-rw-r--r--   0        0        0      351 2024-04-15 13:34:13.802776 wrapchain-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-04-15 12:54:02.130204 wrapchain-0.0.2/wrapchain/__init__.py
+-rw-r--r--   0        0        0      435 2024-04-15 13:22:08.860436 wrapchain-0.0.2/wrapchain/main.py
+-rw-r--r--   0        0        0     1217 2024-04-15 13:21:54.570632 wrapchain-0.0.2/wrapchain/wrapchain.py
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 wrapchain-0.0.2/PKG-INFO
```

### Comparing `wrapchain-0.0.1/wrapchain/wrapchain.py` & `wrapchain-0.0.2/wrapchain/wrapchain.py`

 * *Files identical despite different names*

