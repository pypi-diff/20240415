# Comparing `tmp/sql_athame-0.4.0a2.tar.gz` & `tmp/sql_athame-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a2.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a3.tar", max compression
```

## Comparing `sql_athame-0.4.0a2.tar` & `sql_athame-0.4.0a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/LICENSE
--rw-r--r--   0        0        0    12086 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/README.md
--rw-r--r--   0        0        0      751 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/__init__.py
--rw-r--r--   0        0        0    10350 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/base.py
--rw-r--r--   0        0        0    19697 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      743 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/py.typed
--rw-r--r--   0        0        0     1305 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      412 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/LICENSE
+-rw-r--r--   0        0        0    12086 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/README.md
+-rw-r--r--   0        0        0      751 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10350 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/base.py
+-rw-r--r--   0        0        0    19751 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      743 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/py.typed
+-rw-r--r--   0        0        0     1305 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      412 2024-04-14 23:49:14.829694 sql_athame-0.4.0a3/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a3/PKG-INFO
```

### Comparing `sql_athame-0.4.0a2/LICENSE` & `sql_athame-0.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a2/README.md` & `sql_athame-0.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a2/pyproject.toml` & `sql_athame-0.4.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-2"
+version = "0.4.0-alpha-3"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a2/sql_athame/base.py` & `sql_athame-0.4.0a3/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a2/sql_athame/dataclasses.py` & `sql_athame-0.4.0a3/sql_athame/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,9 +591,11 @@
         if deleted:
             await cls.delete_multiple(connection, deleted)
 
         return created, updated_triples, deleted
 
 
 def chunked(lst, n):
+    if type(lst) is not list:
+        lst = list(lst)
     for i in range(0, len(lst), n):
         yield lst[i : i + n]
```

### Comparing `sql_athame-0.4.0a2/sql_athame/escape.py` & `sql_athame-0.4.0a3/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a2/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a3/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a2/PKG-INFO` & `sql_athame-0.4.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

