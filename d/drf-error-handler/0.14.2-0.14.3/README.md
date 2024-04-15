# Comparing `tmp/drf_error_handler-0.14.2.tar.gz` & `tmp/drf_error_handler-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_error_handler-0.14.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drf_error_handler-0.14.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drf_error_handler-0.14.2.tar` & `drf_error_handler-0.14.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.14.2/LICENSE
--rw-r--r--   0        0        0     3946 2024-04-11 09:40:24.445050 drf_error_handler-0.14.2/README.md
--rw-r--r--   0        0        0       68 2024-04-12 01:29:11.308952 drf_error_handler-0.14.2/drf_error_handler/__init__.py
--rw-r--r--   0        0        0      149 2024-04-12 00:44:51.157506 drf_error_handler-0.14.2/drf_error_handler/apps.py
--rw-r--r--   0        0        0     3272 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/exceptions.py
--rw-r--r--   0        0        0     4633 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/formatter.py
--rw-r--r--   0        0        0     7281 2024-04-12 01:26:22.505100 drf_error_handler-0.14.2/drf_error_handler/handler.py
--rw-r--r--   0        0        0    14833 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/openapi.py
--rw-r--r--   0        0        0    10597 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/openapi_hooks.py
--rw-r--r--   0        0        0     3435 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/openapi_serializers.py
--rw-r--r--   0        0        0    18810 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/openapi_utils.py
--rw-r--r--   0        0        0     8811 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/openapi_validation_errors.py
--rw-r--r--   0        0        0        0 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/py.typed
--rw-r--r--   0        0        0     3645 2024-04-12 00:44:51.160840 drf_error_handler-0.14.2/drf_error_handler/settings.py
--rw-r--r--   0        0        0     1244 2024-04-12 01:25:54.807778 drf_error_handler-0.14.2/drf_error_handler/types.py
--rw-r--r--   0        0        0     2143 2024-04-12 01:29:05.808830 drf_error_handler-0.14.2/pyproject.toml
--rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 drf_error_handler-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.14.3/LICENSE
+-rw-r--r--   0        0        0     5329 2024-04-15 01:32:53.845345 drf_error_handler-0.14.3/README.md
+-rw-r--r--   0        0        0       68 2024-04-15 01:45:09.518369 drf_error_handler-0.14.3/drf_error_handler/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-12 00:44:51.157506 drf_error_handler-0.14.3/drf_error_handler/apps.py
+-rw-r--r--   0        0        0     3272 2024-04-15 01:26:12.311564 drf_error_handler-0.14.3/drf_error_handler/exceptions.py
+-rw-r--r--   0        0        0     4633 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/formatter.py
+-rw-r--r--   0        0        0     7281 2024-04-12 01:26:22.505100 drf_error_handler-0.14.3/drf_error_handler/handler.py
+-rw-r--r--   0        0        0    14833 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi.py
+-rw-r--r--   0        0        0    10597 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_hooks.py
+-rw-r--r--   0        0        0     3435 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_serializers.py
+-rw-r--r--   0        0        0    18810 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_utils.py
+-rw-r--r--   0        0        0     8811 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_validation_errors.py
+-rw-r--r--   0        0        0        0 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/py.typed
+-rw-r--r--   0        0        0     3645 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/settings.py
+-rw-r--r--   0        0        0     1244 2024-04-12 01:25:54.807778 drf_error_handler-0.14.3/drf_error_handler/types.py
+-rw-r--r--   0        0        0     2143 2024-04-15 01:45:36.778852 drf_error_handler-0.14.3/pyproject.toml
+-rw-r--r--   0        0        0     7163 1970-01-01 00:00:00.000000 drf_error_handler-0.14.3/PKG-INFO
```

### Comparing `drf_error_handler-0.14.2/LICENSE` & `drf_error_handler-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/exceptions.py` & `drf_error_handler-0.14.3/drf_error_handler/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/formatter.py` & `drf_error_handler-0.14.3/drf_error_handler/formatter.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/handler.py` & `drf_error_handler-0.14.3/drf_error_handler/handler.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/openapi.py` & `drf_error_handler-0.14.3/drf_error_handler/openapi.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/openapi_hooks.py` & `drf_error_handler-0.14.3/drf_error_handler/openapi_hooks.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/openapi_serializers.py` & `drf_error_handler-0.14.3/drf_error_handler/openapi_serializers.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/openapi_utils.py` & `drf_error_handler-0.14.3/drf_error_handler/openapi_utils.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/openapi_validation_errors.py` & `drf_error_handler-0.14.3/drf_error_handler/openapi_validation_errors.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/settings.py` & `drf_error_handler-0.14.3/drf_error_handler/settings.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/drf_error_handler/types.py` & `drf_error_handler-0.14.3/drf_error_handler/types.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.2/pyproject.toml` & `drf_error_handler-0.14.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "drf-spectacular>=0.27.0",
     "inflection",
 ]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.14.2"
+current = "0.14.3"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

