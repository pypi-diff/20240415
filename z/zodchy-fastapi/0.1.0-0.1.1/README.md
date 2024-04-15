# Comparing `tmp/zodchy_fastapi-0.1.0.tar.gz` & `tmp/zodchy_fastapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_fastapi-0.1.0.tar", max compression
+gzip compressed data, was "zodchy_fastapi-0.1.1.tar", max compression
```

## Comparing `zodchy_fastapi-0.1.0.tar` & `zodchy_fastapi-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.1.0/README.md
--rw-r--r--   0        0        0      411 2024-04-13 13:35:16.452894 zodchy_fastapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       58 2024-01-11 09:14:13.703189 zodchy_fastapi-0.1.0/zodchy_fastapi/__init__.py
--rw-r--r--   0        0        0      246 2024-04-02 15:23:42.896725 zodchy_fastapi-0.1.0/zodchy_fastapi/contracts/__init__.py
--rw-r--r--   0        0        0     3424 2024-04-13 13:35:16.455663 zodchy_fastapi-0.1.0/zodchy_fastapi/contracts/request.py
--rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.1.0/zodchy_fastapi/contracts/response.py
--rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.1.0/zodchy_fastapi/handlers.py
--rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.1.0/zodchy_fastapi/router.py
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 zodchy_fastapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.1.1/README.md
+-rw-r--r--   0        0        0      467 2024-04-15 11:01:18.147303 zodchy_fastapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-01-11 09:14:13.703189 zodchy_fastapi-0.1.1/zodchy_fastapi/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-02 15:23:42.896725 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/__init__.py
+-rw-r--r--   0        0        0     3424 2024-04-13 13:35:16.455663 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/request.py
+-rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/response.py
+-rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.1.1/zodchy_fastapi/handlers.py
+-rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.1.1/zodchy_fastapi/router.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.1.1/PKG-INFO
```

### Comparing `zodchy_fastapi-0.1.0/zodchy_fastapi/contracts/request.py` & `zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/request.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.0/zodchy_fastapi/contracts/response.py` & `zodchy_fastapi-0.1.1/zodchy_fastapi/contracts/response.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.0/zodchy_fastapi/handlers.py` & `zodchy_fastapi-0.1.1/zodchy_fastapi/handlers.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.1.0/zodchy_fastapi/router.py` & `zodchy_fastapi-0.1.1/zodchy_fastapi/router.py`

 * *Files identical despite different names*

