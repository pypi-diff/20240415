# Comparing `tmp/waylay-sdk-registry-2.13.0b0.post0.tar.gz` & `tmp/waylay-sdk-registry-2.13.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-registry-2.13.0b0.post0.tar", last modified: Fri Mar 29 12:36:57 2024, max compression
+gzip compressed data, was "waylay-sdk-registry-2.13.0rc0.tar", last modified: Fri Mar 29 13:21:52 2024, max compression
```

## Comparing `waylay-sdk-registry-2.13.0b0.post0.tar` & `waylay-sdk-registry-2.13.0rc0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.411841 waylay-sdk-registry-2.13.0b0.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-29 12:36:57.411841 waylay-sdk-registry-2.13.0b0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:36:57.411841 waylay-sdk-registry-2.13.0b0.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.403842 waylay-sdk-registry-2.13.0b0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.403842 waylay-sdk-registry-2.13.0b0.post0/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.403842 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.403842 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.407842 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   167061 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   174919 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/plugs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/runtimes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/schemas_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   168300 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/webscripts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.411841 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/service/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-29 12:36:53.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:36:57.411841 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 12:36:57.000000 waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167061 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174919 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168300 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/top_level.txt
```

### Comparing `waylay-sdk-registry-2.13.0b0.post0/LICENSE.txt` & `waylay-sdk-registry-2.13.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b0.post0
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay-sdk-registry-2.13.0b0.post0/README.md` & `waylay-sdk-registry-2.13.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/pyproject.toml` & `waylay-sdk-registry-2.13.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-registry"
-version = "2.13.0-beta.0-0"
+version = "2.13.0rc0"
 description = "Waylay Function Registry"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Function Registry"]
 requires-python = ">= 3.9"
 dependencies = [
```

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/default_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/jobs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/models_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/plugs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/runtimes_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/schemas_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/api/webscripts_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay/services/registry/service/service.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b0.post0
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay-sdk-registry-2.13.0b0.post0/src/waylay_sdk_registry.egg-info/SOURCES.txt` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

