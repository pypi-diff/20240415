# Comparing `tmp/sqlalchemy_schema_factory-0.1.1.tar.gz` & `tmp/sqlalchemy_schema_factory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_schema_factory-0.1.1.tar", max compression
+gzip compressed data, was "sqlalchemy_schema_factory-0.1.2.tar", max compression
```

## Comparing `sqlalchemy_schema_factory-0.1.1.tar` & `sqlalchemy_schema_factory-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.1.1/README.md
--rw-r--r--   0        0        0      443 2024-04-15 12:09:07.088914 sqlalchemy_schema_factory-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       80 2024-01-11 09:14:13.699175 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/__init__.py
--rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/auxiliary.py
--rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/conventions.py
--rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/factory.py
--rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/jsonb/__init__.py
--rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/jsonb/decoding.py
--rw-r--r--   0        0        0      669 2024-01-11 09:14:13.699968 sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/jsonb/encoding.py
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.1.2/README.md
+-rw-r--r--   0        0        0      511 2024-04-15 12:11:24.192670 sqlalchemy_schema_factory-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-01-11 09:14:13.699175 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/__init__.py
+-rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/auxiliary.py
+-rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/conventions.py
+-rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/factory.py
+-rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/__init__.py
+-rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/decoding.py
+-rw-r--r--   0        0        0      669 2024-01-11 09:14:13.699968 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/encoding.py
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.1.2/PKG-INFO
```

### Comparing `sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/auxiliary.py` & `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/auxiliary.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/conventions.py` & `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/conventions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/factory.py` & `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/factory.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/jsonb/decoding.py` & `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/decoding.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.1/sqlalchemy_schema_factory/jsonb/encoding.py` & `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/encoding.py`

 * *Files identical despite different names*

