# Comparing `tmp/polyapi_python-0.2.3.dev8.tar.gz` & `tmp/polyapi_python-0.2.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.3.dev8.tar", last modified: Mon Apr 15 14:48:41 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.3.dev9.tar", last modified: Mon Apr 15 18:36:58 2024, max compression
```

## Comparing `polyapi_python-0.2.3.dev8.tar` & `polyapi_python-0.2.3.dev9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-15 14:48:41.000000 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-15 14:48:41.000000 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:48:41.000000 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 14:48:41.000000 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 14:48:41.000000 polyapi_python-0.2.3.dev8/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:48:41.700705 polyapi_python-0.2.3.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 14:48:37.000000 polyapi_python-0.2.3.dev8/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-15 18:36:58.000000 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-15 18:36:58.000000 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:36:58.000000 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 18:36:58.000000 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 18:36:58.000000 polyapi_python-0.2.3.dev9/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:36:58.795206 polyapi_python-0.2.3.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 18:36:55.000000 polyapi_python-0.2.3.dev9/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.3.dev8/LICENSE` & `polyapi_python-0.2.3.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/PKG-INFO` & `polyapi_python-0.2.3.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev8
+Version: 0.2.3.dev9
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.3.dev8/README.md` & `polyapi_python-0.2.3.dev9/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/api.py` & `polyapi_python-0.2.3.dev9/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/auth.py` & `polyapi_python-0.2.3.dev9/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/cli.py` & `polyapi_python-0.2.3.dev9/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/client.py` & `polyapi_python-0.2.3.dev9/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/config.py` & `polyapi_python-0.2.3.dev9/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/error_handler.py` & `polyapi_python-0.2.3.dev9/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/execute.py` & `polyapi_python-0.2.3.dev9/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/function_cli.py` & `polyapi_python-0.2.3.dev9/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/generate.py` & `polyapi_python-0.2.3.dev9/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/schema.py` & `polyapi_python-0.2.3.dev9/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/server.py` & `polyapi_python-0.2.3.dev9/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/typedefs.py` & `polyapi_python-0.2.3.dev9/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/utils.py` & `polyapi_python-0.2.3.dev9/polyapi/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import os
+import logging
 from typing import Tuple, List
 from colorama import Fore, Style
 from polyapi.constants import BASIC_PYTHON_TYPES
 from polyapi.typedefs import PropertySpecification, PropertyType
 from polyapi.schema import generate_schema_types, clean_title, map_primitive_types
 
 
@@ -87,15 +88,19 @@
             return map_primitive_types(value), ""
     elif type_spec["kind"] == "primitive":
         return map_primitive_types(type_spec["type"]), ""
     elif type_spec["kind"] == "array":
         if type_spec.get("items"):
             items = type_spec["items"]
             if items.get("$ref"):
-                return "ResponseType", generate_schema_types(type_spec, root="ResponseType")  # type: ignore
+                try:
+                    return "ResponseType", generate_schema_types(type_spec, root="ResponseType")  # type: ignore
+                except:
+                    logging.exception(f"Error when generating schema type: {type_spec}")
+                    return "Dict", ""
             else:
                 item_type, _ = get_type_and_def(items)
                 title = f"List[{item_type}]"
                 title = clean_title(title)
                 return title, ""
         else:
             return "List", ""
@@ -104,30 +109,39 @@
     elif type_spec["kind"] == "object":
         if type_spec.get("schema"):
             schema = type_spec["schema"]
             title = schema.get("title", "")
             if title:
                 assert isinstance(title, str)
                 title = clean_title(title)
-                return title, generate_schema_types(schema, root=title)  # type: ignore
+                try:
+                    return title, generate_schema_types(schema, root=title)  # type: ignore
+                except:
+                    logging.exception(f"Error when generating schema type: {schema}")
+                    return "Dict", ""
+
             elif schema.get("items"):
                 # fallback to schema $ref name if no explicit title
                 items = schema.get("items")  # type: ignore
                 title = items.get("title", "")  # type: ignore
                 if not title:
                     # title is actually a reference to another schema
                     title = items.get("$ref", "")  # type: ignore
 
                 title = title.rsplit("/", 1)[-1]
                 title = clean_title(title)
                 if not title:
                     return "List", ""
 
                 title = f"List[{title}]"
-                return title, generate_schema_types(schema, root=title)
+                try:
+                    return title, generate_schema_types(schema, root=title)
+                except:
+                    logging.exception(f"Error when generating schema type: {schema}")
+                    return "List", ""
             else:
                 return "Any", ""
         else:
             return "Dict", ""
     elif type_spec["kind"] == "any":
         return "Any", ""
     else:
```

### Comparing `polyapi_python-0.2.3.dev8/polyapi/variables.py` & `polyapi_python-0.2.3.dev9/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi/webhook.py` & `polyapi_python-0.2.3.dev9/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.3.dev9/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev8
+Version: 0.2.3.dev9
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.3.dev8/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.3.dev9/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/pyproject.toml` & `polyapi_python-0.2.3.dev9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.3.dev8"
+version = "0.2.3.dev9"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.3.dev8/tests/test_api.py` & `polyapi_python-0.2.3.dev9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/tests/test_auth.py` & `polyapi_python-0.2.3.dev9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/tests/test_function_cli.py` & `polyapi_python-0.2.3.dev9/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/tests/test_server.py` & `polyapi_python-0.2.3.dev9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/tests/test_utils.py` & `polyapi_python-0.2.3.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.3.dev8/tests/test_variables.py` & `polyapi_python-0.2.3.dev9/tests/test_variables.py`

 * *Files identical despite different names*

