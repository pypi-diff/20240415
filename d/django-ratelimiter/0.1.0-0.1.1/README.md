# Comparing `tmp/django_ratelimiter-0.1.0.tar.gz` & `tmp/django_ratelimiter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ratelimiter-0.1.0.tar", max compression
+gzip compressed data, was "django_ratelimiter-0.1.1.tar", max compression
```

## Comparing `django_ratelimiter-0.1.0.tar` & `django_ratelimiter-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-10 19:32:55.690451 django_ratelimiter-0.1.0/LICENSE
--rw-r--r--   0        0        0     1147 2024-04-11 07:11:10.911905 django_ratelimiter-0.1.0/README.md
--rw-r--r--   0        0        0      144 2024-04-11 07:11:10.912077 django_ratelimiter-0.1.0/django_ratelimiter/__init__.py
--rw-r--r--   0        0        0     2910 2024-04-11 07:11:10.912269 django_ratelimiter-0.1.0/django_ratelimiter/decorator.py
--rw-r--r--   0        0        0     1764 2024-04-11 07:11:10.912465 django_ratelimiter-0.1.0/django_ratelimiter/storage.py
--rw-r--r--   0        0        0      186 2024-04-11 07:11:10.912644 django_ratelimiter-0.1.0/django_ratelimiter/types.py
--rw-r--r--   0        0        0      565 2024-04-11 07:11:10.912896 django_ratelimiter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 django_ratelimiter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3722 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/README.md
+-rw-r--r--   0        0        0      144 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/__init__.py
+-rw-r--r--   0        0        0     3323 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/py.typed
+-rw-r--r--   0        0        0     1607 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/storage.py
+-rw-r--r--   0        0        0      315 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/types.py
+-rw-r--r--   0        0        0      668 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 django_ratelimiter-0.1.1/PKG-INFO
```

### Comparing `django_ratelimiter-0.1.0/LICENSE` & `django_ratelimiter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.1.0/django_ratelimiter/storage.py` & `django_ratelimiter-0.1.1/django_ratelimiter/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import time
-from typing import cast
+from typing import Union, Optional
 
-from django.conf import settings
 from django.core.cache import caches, BaseCache
 
 from limits.storage import Storage
 
 
 class CacheStorage(Storage):
 
     def __init__(
         self,
-        cache: str | None = None,
+        cache: str,
         wrap_exceptions: bool = False,
-        **options: float | str | bool,
+        **options: Union[float, str, bool],
     ) -> None:
-        self.cache_name = cache or cast(
-            str, getattr(settings, "DJANGO_RATELIMITER_CACHE", "default")
-        )
-        self.cache: BaseCache = caches[self.cache_name]
+        self.cache: BaseCache = caches[cache]
         super().__init__(uri=None, wrap_exceptions=wrap_exceptions, **options)
 
     @property
-    def base_exceptions(self) -> type[Exception] | tuple[type[Exception], ...]:
+    def base_exceptions(self) -> Union[type[Exception], tuple[type[Exception], ...]]:
         return Exception
 
     def get(self, key: str) -> int:
         return self.cache.get(key, 0)
 
     def incr(
         self, key: str, expiry: int, elastic_expiry: bool = False, amount: int = 1
@@ -48,12 +44,12 @@
     def check(self) -> bool:
         try:
             self.cache.get("django-ratelimiter-check")
             return True
         except:  # noqa: E722
             return False
 
-    def reset(self) -> int | None:
+    def reset(self) -> Optional[int]:
         raise NotImplementedError
 
     def clear(self, key: str) -> None:
         self.cache.delete(key)
```

### Comparing `django_ratelimiter-0.1.0/pyproject.toml` & `django_ratelimiter-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "django-ratelimiter"
-version = "0.1.0"
+version = "0.1.1"
 description = "Rate-limiting for django"
 authors = ["Andrii Kohut <kogut.andriy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.9"
 django = "*"
 limits = ">=3.10"
+typing-extensions = {version = "^4.11.0", python = "3.9"}
 
 
 [tool.poetry.group.dev.dependencies]
 django-stubs = "^4.2.7"
 mypy = "^1.9.0"
 black = "^24.3.0"
 ruff = "^0.3.5"
 pytest = "^8.1.1"
 freezegun = "^1.4.0"
 pymemcache = "^4.0.0"
 redis = "^5.0.3"
 pytest-cov = "^5.0.0"
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.17"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

