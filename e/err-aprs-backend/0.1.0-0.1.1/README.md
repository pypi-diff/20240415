# Comparing `tmp/err_aprs_backend-0.1.0.tar.gz` & `tmp/err_aprs_backend-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "err_aprs_backend-0.1.0.tar", max compression
+gzip compressed data, was "err_aprs_backend-0.1.1.tar", max compression
```

## Comparing `err_aprs_backend-0.1.0.tar` & `err_aprs_backend-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/LICENSE
--rw-r--r--   0        0        0     4541 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/README.md
--rw-r--r--   0        0        0       57 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/__init__.py
--rw-r--r--   0        0        0       81 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/aprs.plug
--rw-r--r--   0        0        0    15477 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/aprs.py
--rw-r--r--   0        0        0      104 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/clients/__init__.py
--rw-r--r--   0        0        0     5152 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/clients/aprsis.py
--rw-r--r--   0        0        0      132 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/clients/kiss.py
--rw-r--r--   0        0        0       48 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      151 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/exceptions/client/__init__.py
--rw-r--r--   0        0        0      311 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/exceptions/client/aprsis.py
--rw-r--r--   0        0        0      113 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/exceptions/packets/__init__.py
--rw-r--r--   0        0        0      112 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/exceptions/packets/parser.py
--rw-r--r--   0        0        0      742 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/message.py
--rw-r--r--   0        0        0     5420 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/packets/__init__.py
--rw-r--r--   0        0        0    10018 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/packets/parser.py
--rw-r--r--   0        0        0      748 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/person.py
--rw-r--r--   0        0        0       83 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/room.py
--rw-r--r--   0        0        0      500 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/utils/__init__.py
--rw-r--r--   0        0        0      601 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/utils/counter.py
--rw-r--r--   0        0        0       26 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/aprs_backend/utils/version.py
--rw-r--r--   0        0        0     1334 2024-04-15 03:36:37.473536 err_aprs_backend-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 err_aprs_backend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4541 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/README.md
+-rw-r--r--   0        0        0       57 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/aprs.plug
+-rw-r--r--   0        0        0    15477 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/aprs.py
+-rw-r--r--   0        0        0      104 2024-04-15 03:45:26.800880 err_aprs_backend-0.1.1/aprs_backend/clients/__init__.py
+-rw-r--r--   0        0        0     5152 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/clients/aprsis.py
+-rw-r--r--   0        0        0       82 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/clients/kiss.py
+-rw-r--r--   0        0        0       48 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/client/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/client/aprsis.py
+-rw-r--r--   0        0        0      113 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/packets/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/exceptions/packets/parser.py
+-rw-r--r--   0        0        0      742 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/message.py
+-rw-r--r--   0        0        0     5420 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/packets/__init__.py
+-rw-r--r--   0        0        0    10018 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/packets/parser.py
+-rw-r--r--   0        0        0      748 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/person.py
+-rw-r--r--   0        0        0       83 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/room.py
+-rw-r--r--   0        0        0      500 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/counter.py
+-rw-r--r--   0        0        0       26 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/aprs_backend/utils/version.py
+-rw-r--r--   0        0        0     1334 2024-04-15 03:45:26.804880 err_aprs_backend-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 err_aprs_backend-0.1.1/PKG-INFO
```

### Comparing `err_aprs_backend-0.1.0/LICENSE` & `err_aprs_backend-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/README.md` & `err_aprs_backend-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/aprs.py` & `err_aprs_backend-0.1.1/aprs_backend/aprs.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/clients/aprsis.py` & `err_aprs_backend-0.1.1/aprs_backend/clients/aprsis.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/message.py` & `err_aprs_backend-0.1.1/aprs_backend/message.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/packets/__init__.py` & `err_aprs_backend-0.1.1/aprs_backend/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/packets/parser.py` & `err_aprs_backend-0.1.1/aprs_backend/packets/parser.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/person.py` & `err_aprs_backend-0.1.1/aprs_backend/person.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/aprs_backend/utils/counter.py` & `err_aprs_backend-0.1.1/aprs_backend/utils/counter.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.1.0/pyproject.toml` & `err_aprs_backend-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "err-aprs-backend"
-version = "0.1.0"
+version = "0.1.1"
 description = "Errbot APRS backend plugin"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aprs_backend"}]
 include = ["*.plug"]
```

### Comparing `err_aprs_backend-0.1.0/PKG-INFO` & `err_aprs_backend-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: err-aprs-backend
-Version: 0.1.0
+Version: 0.1.1
 Summary: Errbot APRS backend plugin
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

