# Comparing `tmp/waylay-sdk-core-0.1.0.tar.gz` & `tmp/waylay_sdk_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-core-0.1.0.tar", last modified: Mon Apr  8 12:37:57 2024, max compression
+gzip compressed data, was "waylay_sdk_core-0.2.0.tar", last modified: Mon Apr 15 07:40:21 2024, max compression
```

## Comparing `waylay-sdk-core-0.1.0.tar` & `waylay_sdk_core-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.991711 waylay-sdk-core-0.1.0/
--rw-r--r--   0 thomas     (502) staff       (20)      746 2024-03-26 09:30:45.000000 waylay-sdk-core-0.1.0/LICENSE.txt
--rw-r--r--   0 thomas     (502) staff       (20)     3886 2024-04-08 12:37:57.991318 waylay-sdk-core-0.1.0/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     1710 2024-04-08 12:34:55.000000 waylay-sdk-core-0.1.0/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1492 2024-04-08 12:34:55.000000 waylay-sdk-core-0.1.0/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-08 12:37:57.991791 waylay-sdk-core-0.1.0/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.908203 waylay-sdk-core-0.1.0/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.907416 waylay-sdk-core-0.1.0/src/waylay/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.910753 waylay-sdk-core-0.1.0/src/waylay/sdk/
--rw-r--r--   0 thomas     (502) staff       (20)      754 2024-03-27 11:50:39.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)       65 2024-04-08 12:34:55.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/_version.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.946667 waylay-sdk-core-0.1.0/src/waylay/sdk/api/
--rw-r--r--   0 thomas     (502) staff       (20)      661 2024-03-25 07:17:42.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     6130 2024-04-08 09:44:30.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/_models.py
--rw-r--r--   0 thomas     (502) staff       (20)     4423 2024-03-27 11:50:39.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/client.py
--rw-r--r--   0 thomas     (502) staff       (20)     2298 2024-03-15 07:16:26.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/exceptions.py
--rw-r--r--   0 thomas     (502) staff       (20)     2299 2024-03-25 07:17:42.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/http.py
--rw-r--r--   0 thomas     (502) staff       (20)    10842 2024-03-27 14:07:57.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/api/serialization.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.952664 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/
--rw-r--r--   0 thomas     (502) staff       (20)      523 2024-03-14 11:07:10.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)      882 2024-03-14 10:54:52.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/exceptions.py
--rw-r--r--   0 thomas     (502) staff       (20)     5972 2024-03-07 17:25:15.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/interactive.py
--rw-r--r--   0 thomas     (502) staff       (20)    11539 2024-03-07 17:25:15.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/model.py
--rw-r--r--   0 thomas     (502) staff       (20)      832 2024-03-07 17:25:15.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/parse.py
--rw-r--r--   0 thomas     (502) staff       (20)     4243 2024-03-07 17:25:15.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/auth/provider.py
--rw-r--r--   0 thomas     (502) staff       (20)     1880 2024-04-08 09:44:30.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/client.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.967277 waylay-sdk-core-0.1.0/src/waylay/sdk/config/
--rw-r--r--   0 thomas     (502) staff       (20)      341 2024-03-14 11:07:10.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/config/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     3106 2024-03-26 17:17:35.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/config/client.py
--rw-r--r--   0 thomas     (502) staff       (20)    13667 2024-03-07 17:25:15.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/config/model.py
--rw-r--r--   0 thomas     (502) staff       (20)     2809 2024-03-15 07:16:26.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/exceptions.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.974791 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/
--rw-r--r--   0 thomas     (502) staff       (20)      229 2024-03-14 11:07:10.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     4401 2024-03-25 07:17:42.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/base.py
--rw-r--r--   0 thomas     (502) staff       (20)     2373 2024-03-25 07:17:42.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/client.py
--rw-r--r--   0 thomas     (502) staff       (20)      206 2024-04-08 09:44:30.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/loader.py
--rw-r--r--   0 thomas     (502) staff       (20)     2480 2024-04-08 09:44:30.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/type_stubs.py
--rw-r--r--   0 thomas     (502) staff       (20)       80 2024-02-08 12:59:42.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.975839 waylay-sdk-core-0.1.0/src/waylay/sdk/services/
--rw-r--r--   0 thomas     (502) staff       (20)     4887 2024-04-08 09:44:30.000000 waylay-sdk-core-0.1.0/src/waylay/sdk/services/gateway.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-08 12:37:57.989668 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)     3886 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     1101 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       64 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/entry_points.txt
--rw-r--r--   0 thomas     (502) staff       (20)      330 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)        7 2024-04-08 12:37:57.000000 waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.099580 waylay_sdk_core-0.2.0/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-03-26 14:02:35.000000 waylay_sdk_core-0.2.0/LICENSE.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3967 2024-04-15 07:40:21.098954 waylay_sdk_core-0.2.0/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1710 2024-04-10 15:11:43.000000 waylay_sdk_core-0.2.0/README.md
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1541 2024-04-12 12:21:48.000000 waylay_sdk_core-0.2.0/pyproject.toml
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 07:40:21.099674 waylay_sdk_core-0.2.0/setup.cfg
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:20.999483 waylay_sdk_core-0.2.0/src/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:20.996684 waylay_sdk_core-0.2.0/src/waylay/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.044374 waylay_sdk_core-0.2.0/src/waylay/sdk/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      754 2024-03-28 08:55:26.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       65 2024-04-12 12:21:48.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/_version.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.065377 waylay_sdk_core-0.2.0/src/waylay/sdk/api/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      661 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     6130 2024-04-11 14:02:19.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/_models.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4423 2024-04-10 15:17:36.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       40 2024-04-12 12:21:10.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/constants.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2298 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/exceptions.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2299 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/http.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    14116 2024-04-12 12:21:10.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/serialization.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.078570 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      523 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/exceptions.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5972 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/interactive.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    11539 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/model.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/parse.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4243 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/provider.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1880 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/client.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.083365 waylay_sdk_core-0.2.0/src/waylay/sdk/config/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      341 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3106 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    13667 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/model.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2809 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/exceptions.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.090961 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      229 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4401 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/base.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2373 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      206 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/loader.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2480 2024-03-28 11:04:55.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/type_stubs.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       80 2024-02-13 14:44:08.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/py.typed
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.092512 waylay_sdk_core-0.2.0/src/waylay/sdk/services/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4887 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/services/gateway.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.097642 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3967 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1133 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       64 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      365 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/top_level.txt
```

### Comparing `waylay-sdk-core-0.1.0/LICENSE.txt` & `waylay_sdk_core-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/PKG-INFO` & `waylay_sdk_core-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -29,14 +29,15 @@
 Requires-Dist: python-jose
 Requires-Dist: python_dateutil
 Requires-Dist: typing_extensions>=4.10.0
 Requires-Dist: typeguard
 Requires-Dist: jsonpath-ng
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
+Requires-Dist: waylay-beta==9.9.9b9
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: pytest-httpx; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: starlette; extra == "dev"
@@ -44,14 +45,15 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
 Requires-Dist: types-appdirs; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: sse-starlette; extra == "dev"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk-core` package provides a basic SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

### Comparing `waylay-sdk-core-0.1.0/README.md` & `waylay_sdk_core-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/pyproject.toml` & `waylay_sdk_core-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-core"
-version = "0.1.0"
+version = "0.2.0"
 description = "Waylay Python SDK."
 requires-python = ">=3.9"
 keywords = ["waylay", "sdk"]
 readme = "README.md"
 authors = [{name = "Waylay", email = "info@waylay.io"}]
 license={file = "LICENSE.txt"}
 dependencies = [
@@ -17,14 +17,15 @@
     "python-jose",
     "python_dateutil",
     "typing_extensions >= 4.10.0",
     "typeguard",
     "jsonpath-ng",
     "pydantic >= 2.6.0",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
+    "waylay-beta==9.9.9b9",
 ]
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
 Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-py.git"
 
@@ -53,14 +54,15 @@
     "ruff",
     'mypy',
     'types-python-jose',
     'types-appdirs',
     'types-python-dateutil',
     'docformatter',
     'pre-commit',
+    'sse-starlette',
 ]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 include = ["pyproject.toml", "src/**/*.py", "test/**/*.py"]
```

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/__init__.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/__init__.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/_models.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/_models.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/client.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/exceptions.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/http.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/http.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/api/serialization.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/api/serialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """API client."""
 
 from __future__ import annotations
+import contextlib
+import json
 import logging
 import re
 import datetime
 from urllib.parse import quote
 from inspect import isclass
 from typing import (
     Any,
+    AsyncGenerator,
+    AsyncIterator,
     Mapping,
     Optional,
     AsyncIterable,
     Type,
+    TypeVar,
     Union,
     Iterable,
     Protocol,
+    cast,
     runtime_checkable,
 )
 from abc import abstractmethod
-import warnings
 
 from pydantic import BaseModel, ConfigDict, TypeAdapter, ValidationError
 from pydantic_core import to_jsonable_python
 from jsonpath_ng import parse as jsonpath_parse  # type: ignore[import-untyped]
 from httpx import USE_CLIENT_DEFAULT
 import httpx._client as httpxc
 
@@ -50,14 +55,21 @@
 
 _MODEL_TYPE_ADAPTER = TypeAdapter(Model)
 
 log = logging.getLogger(__name__)
 
 DEFAULT_SERIALIZATION_ARGS = {"by_alias": True, "exclude_none": True}
 
+TEXT_EVENT_STREAM_CONTENT_TYPE = "text/event-stream"
+NDJSON_EVENT_STREAM_CONTENT_TYPE = "application/x-ndjson"
+EVENT_STREAM_CONTENT_TYPES = [
+    TEXT_EVENT_STREAM_CONTENT_TYPE,
+    NDJSON_EVENT_STREAM_CONTENT_TYPE,
+]
+
 
 class WithSerializationSupport:
     """Serialization support for the SDK client."""
 
     base_url: str
     serialization_args = DEFAULT_SERIALIZATION_ARGS
 
@@ -169,57 +181,40 @@
         """Deserialize a http response into a python object.
 
         :param response_data: Response object to be deserialized.
         :param response_type: Response type to use for 2XX status codes,
             or a mapping per status code, including '2XX', '3XX', .. and
             '*' or 'default' wildcard keys.
         :param select_path: json path to be extracted from the json payload.
-        :return: An instance of the type specified in the mapping.
+        :param stream: Whether the response should be in streaming mode.
+            If the response is an event stream, this function will return an async iterator.
+        :return: An instance of the type specified in the mapping, or an async iterator for event stream responses when stream is True.
         """
-        if stream:
-            warnings.warn(
-                "Using `stream=True` is currently only supported with `raw_response=True`."
-            )
-            return response
         status_code = response.status_code
-        response_type = _response_type_for_status_code(status_code, response_type)
+        _response_type = _response_type_for_status_code(status_code, response_type)
 
-        # deserialize response data
-        return_data = None
-        try:
-            if response_type in _PRIMITIVE_BYTE_TYPES + tuple(
-                t.__name__ for t in _PRIMITIVE_BYTE_TYPES
-            ):
-                return_data = response.content
-            elif response_type is not None:
-                try:
-                    _data = response.json()
-                    if select_path:
-                        jsonpath_expr = jsonpath_parse(select_path)
-                        match_values = [
-                            match.value for match in jsonpath_expr.find(_data)
-                        ]
-                        _data = (
-                            match_values[0]
-                            if not re.search(r"\[(\*|.*:.*|.*,.*)\]", select_path)
-                            else match_values
-                        )
-                except ValueError:
-                    _data = response.text
-                if _data is not None:
-                    return_data = _deserialize(_data, response_type)
-                else:
-                    return_data = response.content
-        finally:
-            if not 200 <= status_code <= 299:
-                raise ApiError.from_response(
-                    response,
-                    return_data,
-                )
-        return return_data
+        if not 200 <= response.status_code <= 299:
+            raise ApiError.from_response(
+                response,
+                _deserialize_response(
+                    response, response_type=_response_type, select_path=select_path
+                ),
+            )
+        content_type = response.headers.get("content-type", "")
+        is_event_stream = any(
+            [content_type.startswith(ect) for ect in EVENT_STREAM_CONTENT_TYPES]
+        )
+        if stream and is_event_stream:
+            return _iter_event_stream(
+                response, response_type=_response_type, select_path=select_path
+            )
+        else:
+            return _deserialize_response(
+                response, response_type=_response_type, select_path=select_path
+            )
 
 
 _CHUNK_SIZE = 65_536
 
 
 @runtime_checkable
 class Readable(Protocol):
@@ -321,11 +316,116 @@
     status_code_key = str(status_code)
     rt_map = (
         {"2XX": response_type} if not isinstance(response_type, dict) else response_type
     )
     if rt_map is None:
         return _DEFAULT_RESPONSE_TYPE
     for key in [status_code_key, f"{status_code_key[0]}XX", "default", "*"]:
-        rt = rt_map.get(key)
+        rt: Type | None = rt_map.get(key)
         if rt is not None:
             return rt
     return _DEFAULT_RESPONSE_TYPE
+
+
+def _extract_selected(data, select_path: str):
+    if not select_path:
+        return data
+    jsonpath_expr = jsonpath_parse(select_path)
+    match_values = [match.value for match in jsonpath_expr.find(data)]
+    data = (
+        match_values[0]
+        if not re.search(r"\[(\*|.*:.*|.*,.*)\]", select_path)
+        else match_values
+    )
+    return data
+
+
+T = TypeVar("T")
+
+
+def _deserialize_response(
+    response: Response,
+    response_type: type[T],
+    select_path: str = "",
+) -> T:
+    return_data: T = None  # type: ignore
+    try:
+        if response_type in _PRIMITIVE_BYTE_TYPES + tuple(
+            t.__name__ for t in _PRIMITIVE_BYTE_TYPES
+        ):
+            _content = response.content
+            try:
+                return_data = cast(T, _content)
+            except (TypeError, ValueError):
+                return_data = _content  # type: ignore
+        elif response_type is not None:
+            try:
+                _data = response.json()
+                if select_path:
+                    _data = _extract_selected(_data, select_path)
+            except ValueError:
+                _data = response.text
+            if _data is not None:
+                try:
+                    return_data = _deserialize(_data, response_type)
+                except (TypeError, ValueError):
+                    return _data
+            else:
+                return_data = response.content  # type: ignore
+        elif response_type is None:
+            return_data = None
+    finally:
+        return return_data
+
+
+async def _iter_event_stream(
+    response: Response,
+    response_type: type[T],
+    select_path: str = "",
+) -> AsyncIterator[T]:
+    _response_type = _response_type_for_status_code(response.status_code, response_type)
+    content_type = response.headers.get("content-type", "")
+    try:
+        async for event_str in __iter_events_response(response, content_type):
+            event = __parse_event(event_str, content_type)
+            if not event:
+                continue
+            _deserialized_event = _deserialize(
+                _extract_selected(event, select_path), _response_type
+            )
+            yield _deserialized_event
+    finally:
+        await response.aclose()
+
+
+async def __iter_events_response(
+    response: Response, content_type: str
+) -> AsyncGenerator[str, None]:
+    if content_type.startswith(TEXT_EVENT_STREAM_CONTENT_TYPE):
+        async for event_str_batch in response.aiter_text():
+            for event_str in event_str_batch.split("\r\n\r"):
+                yield event_str
+    else:
+        async for event_str in response.aiter_lines():
+            yield event_str
+
+
+def __parse_event(event_str: str, content_type: str):
+    if content_type.startswith(TEXT_EVENT_STREAM_CONTENT_TYPE):
+        event = {}
+        for line in event_str.split("\n"):
+            keyword, *data = line.split(": ", 1)
+            keyword = keyword.strip()
+            _data = data[0].strip() if data else ""
+            with contextlib.suppress(ValueError, TypeError):
+                _data = json.loads(_data)
+            if keyword or data:
+                event[keyword] = _data
+        return event
+    elif content_type == NDJSON_EVENT_STREAM_CONTENT_TYPE:
+        try:
+            event = json.loads(event_str)
+        except (ValueError, TypeError):
+            log.warning("Cannot deserialize event\n%s", event_str, exc_info=True)
+    else:
+        return event_str
+    return event
```

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/__init__.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/exceptions.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/interactive.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/interactive.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/model.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/model.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/parse.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/parse.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/auth/provider.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/provider.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/client.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/config/client.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/config/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/config/model.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/config/model.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/exceptions.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/base.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/base.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/client.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/plugin/type_stubs.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/type_stubs.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay/sdk/services/gateway.py` & `waylay_sdk_core-0.2.0/src/waylay/sdk/services/gateway.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/PKG-INFO` & `waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -29,14 +29,15 @@
 Requires-Dist: python-jose
 Requires-Dist: python_dateutil
 Requires-Dist: typing_extensions>=4.10.0
 Requires-Dist: typeguard
 Requires-Dist: jsonpath-ng
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
+Requires-Dist: waylay-beta==9.9.9b9
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: pytest-httpx; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: starlette; extra == "dev"
@@ -44,14 +45,15 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
 Requires-Dist: types-appdirs; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: sse-starlette; extra == "dev"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk-core` package provides a basic SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

### Comparing `waylay-sdk-core-0.1.0/src/waylay_sdk_core.egg-info/SOURCES.txt` & `waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/waylay/sdk/_version.py
 src/waylay/sdk/client.py
 src/waylay/sdk/exceptions.py
 src/waylay/sdk/py.typed
 src/waylay/sdk/api/__init__.py
 src/waylay/sdk/api/_models.py
 src/waylay/sdk/api/client.py
+src/waylay/sdk/api/constants.py
 src/waylay/sdk/api/exceptions.py
 src/waylay/sdk/api/http.py
 src/waylay/sdk/api/serialization.py
 src/waylay/sdk/auth/__init__.py
 src/waylay/sdk/auth/exceptions.py
 src/waylay/sdk/auth/interactive.py
 src/waylay/sdk/auth/model.py
```

