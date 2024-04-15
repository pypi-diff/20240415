# Comparing `tmp/drf_error_handler-0.14.3.tar.gz` & `tmp/drf_error_handler-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_error_handler-0.14.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drf_error_handler-0.15.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drf_error_handler-0.14.3.tar` & `drf_error_handler-0.15.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.14.3/LICENSE
--rw-r--r--   0        0        0     5329 2024-04-15 01:32:53.845345 drf_error_handler-0.14.3/README.md
--rw-r--r--   0        0        0       68 2024-04-15 01:45:09.518369 drf_error_handler-0.14.3/drf_error_handler/__init__.py
--rw-r--r--   0        0        0      149 2024-04-12 00:44:51.157506 drf_error_handler-0.14.3/drf_error_handler/apps.py
--rw-r--r--   0        0        0     3272 2024-04-15 01:26:12.311564 drf_error_handler-0.14.3/drf_error_handler/exceptions.py
--rw-r--r--   0        0        0     4633 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/formatter.py
--rw-r--r--   0        0        0     7281 2024-04-12 01:26:22.505100 drf_error_handler-0.14.3/drf_error_handler/handler.py
--rw-r--r--   0        0        0    14833 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi.py
--rw-r--r--   0        0        0    10597 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_hooks.py
--rw-r--r--   0        0        0     3435 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_serializers.py
--rw-r--r--   0        0        0    18810 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_utils.py
--rw-r--r--   0        0        0     8811 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/openapi_validation_errors.py
--rw-r--r--   0        0        0        0 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/py.typed
--rw-r--r--   0        0        0     3645 2024-04-12 00:44:51.160840 drf_error_handler-0.14.3/drf_error_handler/settings.py
--rw-r--r--   0        0        0     1244 2024-04-12 01:25:54.807778 drf_error_handler-0.14.3/drf_error_handler/types.py
--rw-r--r--   0        0        0     2143 2024-04-15 01:45:36.778852 drf_error_handler-0.14.3/pyproject.toml
--rw-r--r--   0        0        0     7163 1970-01-01 00:00:00.000000 drf_error_handler-0.14.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.15.1/LICENSE
+-rw-r--r--   0        0        0     5329 2024-04-15 01:32:53.845345 drf_error_handler-0.15.1/README.md
+-rw-r--r--   0        0        0       68 2024-04-15 04:16:50.854198 drf_error_handler-0.15.1/drf_error_handler/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-12 00:44:51.157506 drf_error_handler-0.15.1/drf_error_handler/apps.py
+-rw-r--r--   0        0        0     3272 2024-04-15 01:26:12.311564 drf_error_handler-0.15.1/drf_error_handler/exceptions.py
+-rw-r--r--   0        0        0     4633 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/formatter.py
+-rw-r--r--   0        0        0     7281 2024-04-12 01:26:22.505100 drf_error_handler-0.15.1/drf_error_handler/handler.py
+-rw-r--r--   0        0        0    14833 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/openapi.py
+-rw-r--r--   0        0        0    10597 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/openapi_hooks.py
+-rw-r--r--   0        0        0     3435 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/openapi_serializers.py
+-rw-r--r--   0        0        0    18810 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/openapi_utils.py
+-rw-r--r--   0        0        0     8811 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/openapi_validation_errors.py
+-rw-r--r--   0        0        0        0 2024-04-12 00:44:51.160840 drf_error_handler-0.15.1/drf_error_handler/py.typed
+-rw-r--r--   0        0        0     3645 2024-04-15 03:15:59.566810 drf_error_handler-0.15.1/drf_error_handler/settings.py
+-rw-r--r--   0        0        0     1178 2024-04-15 02:55:19.492892 drf_error_handler-0.15.1/drf_error_handler/types.py
+-rw-r--r--   0        0        0     2142 2024-04-15 04:17:04.787672 drf_error_handler-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0     7162 1970-01-01 00:00:00.000000 drf_error_handler-0.15.1/PKG-INFO
```

### Comparing `drf_error_handler-0.14.3/LICENSE` & `drf_error_handler-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/README.md` & `drf_error_handler-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/exceptions.py` & `drf_error_handler-0.15.1/drf_error_handler/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/formatter.py` & `drf_error_handler-0.15.1/drf_error_handler/formatter.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/handler.py` & `drf_error_handler-0.15.1/drf_error_handler/handler.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/openapi.py` & `drf_error_handler-0.15.1/drf_error_handler/openapi.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/openapi_hooks.py` & `drf_error_handler-0.15.1/drf_error_handler/openapi_hooks.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/openapi_serializers.py` & `drf_error_handler-0.15.1/drf_error_handler/openapi_serializers.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/openapi_utils.py` & `drf_error_handler-0.15.1/drf_error_handler/openapi_utils.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/openapi_validation_errors.py` & `drf_error_handler-0.15.1/drf_error_handler/openapi_validation_errors.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/settings.py` & `drf_error_handler-0.15.1/drf_error_handler/settings.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.3/drf_error_handler/types.py` & `drf_error_handler-0.15.1/drf_error_handler/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
-from dataclasses import dataclass, field, make_dataclass
+
+from dataclasses import dataclass, make_dataclass
 from enum import Enum
-from typing import List, Optional, TypedDict, cast
+from typing import List, Optional, Type, TypedDict, cast
 
-from drf_error_handler.settings import DEFAULTS, IMPORT_STRINGS, PackageSettings
 from rest_framework.request import Request
 from rest_framework.views import APIView
 
+from drf_error_handler.settings import DEFAULTS, IMPORT_STRINGS, PackageSettings
+
 package_settings = PackageSettings(DEFAULTS, IMPORT_STRINGS)
 
 
 class ExceptionHandlerContext(TypedDict):
     view: APIView
     args: tuple
     kwargs: dict
@@ -22,28 +24,20 @@
 
 class ErrorType(str, Enum):
     VALIDATION_ERROR = "validation_error"
     CLIENT_ERROR = "client_error"
     SERVER_ERROR = "server_error"
 
 
-Error = make_dataclass("Error", [("detail", str), ("attr", type[Optional[str]]), (BUSINESS_CODE_NAME, int)])
-
-
-@dataclass
-class Error:
-    detail: str
-    attr: Optional[str]
-    BUSINESS_CODE_NAME: Optional[int]
-
+Error = make_dataclass("Error", [("detail", str), ("attr", Type[Optional[str]]), (BUSINESS_CODE_NAME, int)])
 
 @dataclass
 class ErrorResponse:
     type: ErrorType
-    errors: List[Error]
+    errors: List[Error] # type: ignore[reportInvalidTypeForm]
 
 
 class SetValidationErrorsKwargs(TypedDict):
     error_codes: List[str]
     field_name: Optional[str]
     actions: Optional[List[str]]
     methods: Optional[List[str]]
```

### Comparing `drf_error_handler-0.14.3/pyproject.toml` & `drf_error_handler-0.15.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
-    "django >=3.2",
-    "djangorestframework >=3.12",
+    "django >=2.2",
+    "djangorestframework >=3.9",
 ]
 
 [project.urls]
 Homepage = "https://github.com/korchizhinskiy/drf-error-handler"
 Documentation = "https://drf-error-handler.readthedocs.io/en/latest/"
 Code = "https://github.com/korchizhinskiy/drf-error-handler"
 Issues = "https://github.com/korchizhinskiy/drf-error-handler/issues"
@@ -61,15 +61,15 @@
     "drf-spectacular>=0.27.0",
     "inflection",
 ]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.14.3"
+current = "0.15.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `drf_error_handler-0.14.3/PKG-INFO` & `drf_error_handler-0.15.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: drf-error-handler
-Version: 0.14.3
+Version: 0.15.1
 Summary: Standardize your API error responses.
 Keywords: standardized errors,errors formatter,django rest framework,exception handler
 Author: Ghazi Abbassi, Nazar Korchizhinskiy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: django >=3.2
-Requires-Dist: djangorestframework >=3.12
+Requires-Dist: django >=2.2
+Requires-Dist: djangorestframework >=3.9
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: sphinx!=5.2.0.post0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme>=1.1.0 ; extra == "doc"
 Requires-Dist: myst-parser ; extra == "doc"
 Requires-Dist: drf-spectacular>=0.27.0 ; extra == "openapi"
 Requires-Dist: inflection ; extra == "openapi"
```

