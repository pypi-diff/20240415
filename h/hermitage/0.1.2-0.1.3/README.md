# Comparing `tmp/hermitage-0.1.2.tar.gz` & `tmp/hermitage-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.2.tar", max compression
+gzip compressed data, was "hermitage-0.1.3.tar", max compression
```

## Comparing `hermitage-0.1.2.tar` & `hermitage-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage-0.1.2/README.md
--rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.2/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.2/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.2/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.2/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1020 2024-04-13 13:50:37.613982 hermitage-0.1.2/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.2/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.2/hermitage/parsers/query.py
--rw-r--r--   0        0        0      356 2024-04-13 13:47:50.456971 hermitage-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 hermitage-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.3/README.md
+-rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.3/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.3/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.3/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.3/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1020 2024-04-13 13:50:37.613982 hermitage-0.1.3/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.3/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.3/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      389 2024-04-15 11:34:27.345218 hermitage-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 hermitage-0.1.3/PKG-INFO
```

### Comparing `hermitage-0.1.2/hermitage/definition/contracts.py` & `hermitage-0.1.3/hermitage/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.2/hermitage/mappers/invoice.py` & `hermitage-0.1.3/hermitage/mappers/invoice.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.2/hermitage/parsers/query.py` & `hermitage-0.1.3/hermitage/parsers/query.py`

 * *Files identical despite different names*

