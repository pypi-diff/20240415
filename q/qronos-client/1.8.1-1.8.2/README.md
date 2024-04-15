# Comparing `tmp/qronos-client-1.8.1.tar.gz` & `tmp/qronos_client-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qronos-client-1.8.1.tar", last modified: Mon Dec 12 15:33:12 2022, max compression
+gzip compressed data, was "qronos_client-1.8.2.tar", last modified: Mon Apr 15 14:24:32 2024, max compression
```

## Comparing `qronos-client-1.8.1.tar` & `qronos_client-1.8.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:33:12.305724 qronos-client-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-12 15:33:04.000000 qronos-client-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-12 15:33:04.000000 qronos-client-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2022-12-12 15:33:12.305724 qronos-client-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2022-12-12 15:33:04.000000 qronos-client-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:33:12.305724 qronos-client-1.8.1/qronos/
--rw-r--r--   0 runner    (1001) docker     (123)    18225 2022-12-12 15:33:04.000000 qronos-client-1.8.1/qronos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:33:12.305724 qronos-client-1.8.1/qronos_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2022-12-12 15:33:12.000000 qronos-client-1.8.1/qronos_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-12 15:33:12.000000 qronos-client-1.8.1/qronos_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 15:33:12.000000 qronos-client-1.8.1/qronos_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-12 15:33:12.000000 qronos-client-1.8.1/qronos_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-12 15:33:12.000000 qronos-client-1.8.1/qronos_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2022-12-12 15:33:12.305724 qronos-client-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 15:33:04.000000 qronos-client-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:32.093372 qronos_client-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 14:24:18.000000 qronos_client-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 14:24:18.000000 qronos_client-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-15 14:24:32.093372 qronos_client-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-15 14:24:18.000000 qronos_client-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:32.093372 qronos_client-1.8.2/qronos/
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-15 14:24:18.000000 qronos_client-1.8.2/qronos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:32.093372 qronos_client-1.8.2/qronos_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-15 14:24:32.000000 qronos_client-1.8.2/qronos_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-15 14:24:32.000000 qronos_client-1.8.2/qronos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:24:32.000000 qronos_client-1.8.2/qronos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 14:24:32.000000 qronos_client-1.8.2/qronos_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 14:24:32.000000 qronos_client-1.8.2/qronos_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-15 14:24:32.093372 qronos_client-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:24:18.000000 qronos_client-1.8.2/setup.py
```

### Comparing `qronos-client-1.8.1/PKG-INFO` & `qronos_client-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qronos-client
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python Client for QRonos
 Home-page: https://github.com/QuickRelease/qronos-client.git
 Author: Nick Solly
 Author-email: nick.solly@quickrelease.co.uk
 License: All Rights Reserved
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: python-dateutil>=2.8.0
 
 # qronos-client
 Python client for QRonos
 
 ## Installation
 
 This package can be installed via pip:
```

### Comparing `qronos-client-1.8.1/README.md` & `qronos_client-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qronos-client-1.8.1/qronos/__init__.py` & `qronos_client-1.8.2/qronos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-__version__ = "1.8.1"
+__version__ = "1.8.2"
 
 import logging
 from urllib.parse import urlparse, parse_qs
 import dateutil.parser
 import requests
 
 logger = logging.getLogger(__name__)
 
 
 class QRonosError(Exception):
     """Generic exception for QRonos"""
     def __init__(self, msg):
-        super().__init__()
+        super().__init__(msg)
         logger.error(f"[QRONOS API] - {msg}")
 
 
 class QRonosClient(object):
     urls = {}
     headers = {}
```

### Comparing `qronos-client-1.8.1/qronos_client.egg-info/PKG-INFO` & `qronos_client-1.8.2/qronos_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qronos-client
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python Client for QRonos
 Home-page: https://github.com/QuickRelease/qronos-client.git
 Author: Nick Solly
 Author-email: nick.solly@quickrelease.co.uk
 License: All Rights Reserved
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: python-dateutil>=2.8.0
 
 # qronos-client
 Python client for QRonos
 
 ## Installation
 
 This package can be installed via pip:
```

### Comparing `qronos-client-1.8.1/setup.cfg` & `qronos_client-1.8.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qronos-client
-version = 1.8.1
+version = 1.8.2
 description = Python Client for QRonos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/QuickRelease/qronos-client.git
 author = Nick Solly
 author_email = nick.solly@quickrelease.co.uk
 license = All Rights Reserved
```

