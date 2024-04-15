# Comparing `tmp/fango-0.0.18.tar.gz` & `tmp/fango-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fango-0.0.18.tar", max compression
+gzip compressed data, was "fango-0.0.19.tar", max compression
```

## Comparing `fango-0.0.18.tar` & `fango-0.0.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      620 2024-02-24 18:07:20.033525 fango-0.0.18/README.md
--rw-r--r--   0        0        0     7456 2024-04-14 16:48:43.151576 fango-0.0.18/fango/adapters/pydantic.py
--rw-r--r--   0        0        0      848 2024-04-14 16:48:43.152107 fango-0.0.18/fango/adapters/types.py
--rw-r--r--   0        0        0     2681 2024-04-14 16:48:43.152538 fango-0.0.18/fango/auth.py
--rw-r--r--   0        0        0     4845 2024-04-14 16:48:43.152929 fango-0.0.18/fango/filters.py
--rw-r--r--   0        0        0      310 2024-04-14 16:48:43.153250 fango-0.0.18/fango/generics.py
--rw-r--r--   0        0        0     1907 2024-04-14 16:48:43.153595 fango-0.0.18/fango/log.py
--rw-r--r--   0        0        0        0 2024-04-14 16:48:43.154606 fango-0.0.18/fango/middleware/__init__.py
--rw-r--r--   0        0        0      997 2024-04-14 16:48:43.156087 fango-0.0.18/fango/middleware/common.py
--rw-r--r--   0        0        0     6639 2024-04-14 16:48:43.156526 fango-0.0.18/fango/pagination.py
--rw-r--r--   0        0        0     2447 2024-04-14 16:48:43.156924 fango-0.0.18/fango/permissions.py
--rw-r--r--   0        0        0      440 2024-04-14 16:48:43.157427 fango-0.0.18/fango/routing.py
--rw-r--r--   0        0        0     2123 2024-04-14 16:48:43.157748 fango-0.0.18/fango/schemas.py
--rw-r--r--   0        0        0      284 2024-04-14 16:48:43.163550 fango-0.0.18/fango/tests/client.py
--rw-r--r--   0        0        0      723 2024-04-14 16:48:43.163843 fango-0.0.18/fango/tests/fixtures.py
--rw-r--r--   0        0        0     3518 2024-04-14 16:48:43.164120 fango-0.0.18/fango/utils.py
--rw-r--r--   0        0        0     7253 2024-04-14 16:51:53.948819 fango-0.0.18/fango/viewsets.py
--rw-r--r--   0        0        0      536 2024-04-14 16:53:16.859589 fango-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 fango-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0      620 2024-02-24 18:07:20.033525 fango-0.0.19/README.md
+-rw-r--r--   0        0        0     7456 2024-04-14 23:03:25.730166 fango-0.0.19/fango/adapters/pydantic.py
+-rw-r--r--   0        0        0      848 2024-04-14 23:03:25.731065 fango-0.0.19/fango/adapters/types.py
+-rw-r--r--   0        0        0     2681 2024-04-14 23:03:25.731578 fango-0.0.19/fango/auth.py
+-rw-r--r--   0        0        0     4845 2024-04-14 23:03:25.731979 fango-0.0.19/fango/filters.py
+-rw-r--r--   0        0        0      310 2024-04-14 23:03:25.732278 fango-0.0.19/fango/generics.py
+-rw-r--r--   0        0        0     1907 2024-04-14 23:03:25.732567 fango-0.0.19/fango/log.py
+-rw-r--r--   0        0        0        0 2024-04-14 23:03:25.733144 fango-0.0.19/fango/middleware/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-14 23:03:25.734606 fango-0.0.19/fango/middleware/common.py
+-rw-r--r--   0        0        0     6639 2024-04-14 23:03:25.735056 fango-0.0.19/fango/pagination.py
+-rw-r--r--   0        0        0     2447 2024-04-14 23:03:25.735385 fango-0.0.19/fango/permissions.py
+-rw-r--r--   0        0        0      440 2024-04-14 23:03:25.735661 fango-0.0.19/fango/routing.py
+-rw-r--r--   0        0        0     2427 2024-04-14 23:03:40.441267 fango-0.0.19/fango/schemas.py
+-rw-r--r--   0        0        0      284 2024-04-14 23:03:25.741040 fango-0.0.19/fango/tests/client.py
+-rw-r--r--   0        0        0      723 2024-04-14 23:03:25.741322 fango-0.0.19/fango/tests/fixtures.py
+-rw-r--r--   0        0        0     3116 2024-04-14 23:03:25.741600 fango-0.0.19/fango/utils.py
+-rw-r--r--   0        0        0     7253 2024-04-14 23:03:25.742114 fango-0.0.19/fango/viewsets.py
+-rw-r--r--   0        0        0      536 2024-04-14 23:03:19.644259 fango-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 fango-0.0.19/PKG-INFO
```

### Comparing `fango-0.0.18/README.md` & `fango-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/adapters/pydantic.py` & `fango-0.0.19/fango/adapters/pydantic.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/adapters/types.py` & `fango-0.0.19/fango/adapters/types.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/auth.py` & `fango-0.0.19/fango/auth.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/filters.py` & `fango-0.0.19/fango/filters.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/log.py` & `fango-0.0.19/fango/log.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/middleware/common.py` & `fango-0.0.19/fango/middleware/common.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/pagination.py` & `fango-0.0.19/fango/pagination.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/permissions.py` & `fango-0.0.19/fango/permissions.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/schemas.py` & `fango-0.0.19/fango/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from enum import Enum
 from typing import Generic, TypedDict, TypeVar, get_args
 
 from django.db.models import Manager
 from pydantic import BaseModel, ConfigDict, field_validator
 from typing_extensions import NotRequired
 
 from fango.adapters.types import PK
@@ -56,24 +57,34 @@
     name: str | None
 
 
 class FormModel(BaseModel):
     model_config = ConfigDict(from_attributes=True)
 
     @field_validator("*", mode="before")
-    def validate_complex_fields(cls, value, info):
+    def query_relation_manager(cls, value):
+        if isinstance(value, Manager):
+            return value.all()
+        return value
+
+    @field_validator("*", mode="after")
+    def use_choices_label(cls, value, info):
         from fango.utils import get_choices_label
 
-        for type_ in get_args(cls.model_fields[info.field_name].annotation):
-            if metadata := getattr(type_, "__pydantic_generic_metadata__", None):
-                if value is not None and metadata["origin"] is ChoicesItem:
-                    return {"id": value, "name": get_choices_label(metadata["args"][0], value)}
+        annotation = cls.model_fields[info.field_name].annotation
+        types = get_args(annotation)
 
-        if isinstance(value, Manager):
-            return value.all()
+        if value is not None:
+            for type_ in types:
+                if issubclass(type_, Enum):
+                    return get_choices_label(type_, value)
+
+                if metadata := getattr(type_, "__pydantic_generic_metadata__", None):
+                    if metadata["origin"] is ChoicesItem:
+                        return {"id": value, "name": get_choices_label(metadata["args"][0], value)}
 
         return value
 
 
 class Multiselect(FormModel):
     id: int
     name: str | None = None
```

### Comparing `fango-0.0.18/fango/tests/fixtures.py` & `fango-0.0.19/fango/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/fango/utils.py` & `fango-0.0.19/fango/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 from typing import Any, Callable
 
 from django.conf import settings
 from django.core.cache import cache
 from django.db.models import Choices
 from django.db.models.enums import ChoicesMeta
 from fastapi.concurrency import run_in_threadpool
-from fastapi.routing import APIRoute
 
-from base.main import app
-from base.urls import router
 from fango.generics import MethodT
 from fango.schemas import ChoicesItem
 
 __all__ = [
     "ttl_cache",
     "reverse_ordering",
     "replace_proto",
     "run_async",
     "run_sync",
     "get_choices_as_data",
     "copy_instance_method",
     "get_choices_label",
-    "get_all_routes_basenames",
 ]
 
 
 def ttl_cache(ttl=None) -> Any:
     """
     Decorator for TTL caching.
 
@@ -121,19 +117,7 @@
 
 def get_choices_label(enum: type[Choices], value: int) -> str:
     """
     Function returns choices text.
 
     """
     return enum.choices[value][1]
-
-
-def get_all_routes_basenames() -> set:
-    """
-    Function returns set of all routes basenames
-
-    """
-
-    fastapi = {x.tags[0] for x in app.routes if isinstance(x, APIRoute) and x.tags}
-    django = {x.name.split("-")[0] for x in router.urls}
-
-    return fastapi | django
```

### Comparing `fango-0.0.18/fango/viewsets.py` & `fango-0.0.19/fango/viewsets.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.18/pyproject.toml` & `fango-0.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fango"
-version = "0.0.18"
+version = "0.0.19"
 description = "Metaframework for web with combined FastAPI and Django"
 repository = "https://github.com/egorgam/fango"
 keywords = ["fastapi", "django", "fango"]
 authors = ["Egor Gamazin <egorgamazin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fango-0.0.18/PKG-INFO` & `fango-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fango
-Version: 0.0.18
+Version: 0.0.19
 Summary: Metaframework for web with combined FastAPI and Django
 Home-page: https://github.com/egorgam/fango
 License: MIT
 Keywords: fastapi,django,fango
 Author: Egor Gamazin
 Author-email: egorgamazin@yandex.ru
 Requires-Python: >=3.10,<4.0
```

