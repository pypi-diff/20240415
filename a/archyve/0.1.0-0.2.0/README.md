# Comparing `tmp/archyve-0.1.0.tar.gz` & `tmp/archyve-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archyve-0.1.0.tar", max compression
+gzip compressed data, was "archyve-0.2.0.tar", max compression
```

## Comparing `archyve-0.1.0.tar` & `archyve-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      369 2024-04-14 21:46:33.101089 archyve-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1221 2024-04-14 14:29:28.118250 archyve-0.1.0/README.md
--rw-r--r--   0        0        0     9673 2024-04-14 21:32:47.189326 archyve-0.1.0/src/archyve.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 archyve-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9673 2024-04-14 21:32:47.189326 archyve-0.2.0/archyve.py
+-rw-r--r--   0        0        0      369 2024-04-14 22:25:07.771712 archyve-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1953 2024-04-14 22:23:51.671891 archyve-0.2.0/README.md
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 archyve-0.2.0/PKG-INFO
```

### Comparing `archyve-0.1.0/src/archyve.py` & `archyve-0.2.0/archyve.py`

 * *Files identical despite different names*

