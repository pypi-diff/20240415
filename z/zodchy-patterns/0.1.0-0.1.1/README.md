# Comparing `tmp/zodchy_patterns-0.1.0.tar.gz` & `tmp/zodchy_patterns-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_patterns-0.1.0.tar", max compression
+gzip compressed data, was "zodchy_patterns-0.1.1.tar", max compression
```

## Comparing `zodchy_patterns-0.1.0.tar` & `zodchy_patterns-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       15 2024-04-11 15:49:10.635624 zodchy_patterns-0.1.0/README.md
--rw-r--r--   0        0        0      378 2024-04-13 13:26:29.840672 zodchy_patterns-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      205 2024-04-11 07:57:07.720094 zodchy_patterns-0.1.0/zodchy_patterns/__init__.py
--rw-r--r--   0        0        0      172 2024-04-11 07:57:07.720291 zodchy_patterns-0.1.0/zodchy_patterns/events/__init__.py
--rw-r--r--   0        0        0     1470 2024-04-13 13:25:25.515788 zodchy_patterns-0.1.0/zodchy_patterns/events/http.py
--rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.1.0/zodchy_patterns/mapping.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 zodchy_patterns-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.1.1/README.md
+-rw-r--r--   0        0        0      435 2024-04-15 10:14:19.227330 zodchy_patterns-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-04-11 07:57:07.720094 zodchy_patterns-0.1.1/zodchy_patterns/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-11 07:57:07.720291 zodchy_patterns-0.1.1/zodchy_patterns/events/__init__.py
+-rw-r--r--   0        0        0     1470 2024-04-13 13:25:25.515788 zodchy_patterns-0.1.1/zodchy_patterns/events/http.py
+-rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.1.1/zodchy_patterns/mapping.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.1.1/PKG-INFO
```

### Comparing `zodchy_patterns-0.1.0/zodchy_patterns/events/http.py` & `zodchy_patterns-0.1.1/zodchy_patterns/events/http.py`

 * *Files identical despite different names*

