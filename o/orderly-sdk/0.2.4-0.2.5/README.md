# Comparing `tmp/orderly_sdk-0.2.4.tar.gz` & `tmp/orderly_sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orderly_sdk-0.2.4.tar", max compression
+gzip compressed data, was "orderly_sdk-0.2.5.tar", max compression
```

## Comparing `orderly_sdk-0.2.4.tar` & `orderly_sdk-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-12-07 06:04:42.890481 orderly_sdk-0.2.4/LICENSE
--rw-r--r--   0        0        0      417 2024-02-23 15:04:31.641139 orderly_sdk-0.2.4/README.md
--rw-r--r--   0        0        0      636 2024-02-23 15:04:41.659767 orderly_sdk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-07 06:04:42.893509 orderly_sdk-0.2.4/src/orderly_sdk/__init__.py
--rw-r--r--   0        0        0      808 2023-12-07 06:04:42.893971 orderly_sdk-0.2.4/src/orderly_sdk/exceptions.py
--rw-r--r--   0        0        0      628 2023-12-07 06:04:42.894332 orderly_sdk-0.2.4/src/orderly_sdk/helpers.py
--rw-r--r--   0        0        0      435 2023-12-07 06:04:42.894595 orderly_sdk-0.2.4/src/orderly_sdk/log.py
--rw-r--r--   0        0        0     9068 2024-02-23 15:05:56.289240 orderly_sdk-0.2.4/src/orderly_sdk/rest.py
--rw-r--r--   0        0        0     7264 2023-12-07 06:04:42.895254 orderly_sdk-0.2.4/src/orderly_sdk/ws.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 orderly_sdk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-07 06:04:42.890481 orderly_sdk-0.2.5/LICENSE
+-rw-r--r--   0        0        0      417 2024-02-23 15:04:31.641139 orderly_sdk-0.2.5/README.md
+-rw-r--r--   0        0        0      636 2024-04-15 17:53:58.092660 orderly_sdk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-07 06:04:42.893509 orderly_sdk-0.2.5/src/orderly_sdk/__init__.py
+-rw-r--r--   0        0        0      808 2023-12-07 06:04:42.893971 orderly_sdk-0.2.5/src/orderly_sdk/exceptions.py
+-rw-r--r--   0        0        0      628 2023-12-07 06:04:42.894332 orderly_sdk-0.2.5/src/orderly_sdk/helpers.py
+-rw-r--r--   0        0        0      436 2024-04-15 17:57:02.267850 orderly_sdk-0.2.5/src/orderly_sdk/log.py
+-rw-r--r--   0        0        0     9068 2024-02-23 15:05:56.289240 orderly_sdk-0.2.5/src/orderly_sdk/rest.py
+-rw-r--r--   0        0        0     7265 2024-04-15 17:57:02.268198 orderly_sdk-0.2.5/src/orderly_sdk/ws.py
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 orderly_sdk-0.2.5/PKG-INFO
```

### Comparing `orderly_sdk-0.2.4/LICENSE` & `orderly_sdk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `orderly_sdk-0.2.4/pyproject.toml` & `orderly_sdk-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "orderly-sdk"
-version = "0.2.4"
+version = "0.2.5"
 description = "Orderly Rest and Websocket SDK"
 authors = ["Akagi201 <akagi201@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "orderly_sdk", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 eth-keys = "^0.5.0"
 base58 = "^2.1.1"
-cryptography = "^42.0.4"
-aiohttp = "^3.9.3"
+cryptography = "^42.0.5"
+aiohttp = "^3.9.4"
 requests = "^2.31.0"
-types-requests = "^2.31.0.20240218"
+types-requests = "^2.31.0.20240406"
 websockets = "^12.0"
 loguru = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.2"
-mypy = "^1.8.0"
+ruff = "^0.3.7"
+mypy = "^1.9.0"
 pdoc = "^14.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orderly_sdk-0.2.4/src/orderly_sdk/exceptions.py` & `orderly_sdk-0.2.5/src/orderly_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `orderly_sdk-0.2.4/src/orderly_sdk/helpers.py` & `orderly_sdk-0.2.5/src/orderly_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `orderly_sdk-0.2.4/src/orderly_sdk/rest.py` & `orderly_sdk-0.2.5/src/orderly_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `orderly_sdk-0.2.4/src/orderly_sdk/ws.py` & `orderly_sdk-0.2.5/src/orderly_sdk/ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Orderly Async Websocket API Client
 """
+
 import asyncio
 import base64
 import datetime
 import json as jsonlib
 from collections import defaultdict
 from typing import DefaultDict, Dict, Optional
```

### Comparing `orderly_sdk-0.2.4/PKG-INFO` & `orderly_sdk-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: orderly-sdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Orderly Rest and Websocket SDK
 License: Apache-2.0
 Author: Akagi201
 Author-email: akagi201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
-Requires-Dist: cryptography (>=42.0.4,<43.0.0)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: eth-keys (>=0.5.0,<0.6.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: types-requests (>=2.31.0.20240218,<3.0.0.0)
+Requires-Dist: types-requests (>=2.31.0.20240406,<3.0.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # orderly-sdk-py
 
 [![PyPI version](https://badge.fury.io/py/orderly-sdk.svg)](https://badge.fury.io/py/orderly-sdk) [![Pdoc Badge](https://img.shields.io/badge/docs-orderly_sdk-green)](https://akagi201.github.io/orderly-sdk-py/)
```

