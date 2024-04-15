# Comparing `tmp/that_depends-1.4.0.tar.gz` & `tmp/that_depends-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.4.0.tar", max compression
+gzip compressed data, was "that_depends-1.5.0.tar", max compression
```

## Comparing `that_depends-1.4.0.tar` & `that_depends-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3794 2024-03-20 20:02:14.016047 that_depends-1.4.0/README.md
--rw-r--r--   0        0        0     1482 2024-04-11 11:53:40.084417 that_depends-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.4.0/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.4.0/that_depends/container.py
--rw-r--r--   0        0        0     1016 2024-03-18 09:24:54.496625 that_depends-1.4.0/that_depends/injection.py
--rw-r--r--   0        0        0     4915 2024-04-11 11:51:20.009689 that_depends-1.4.0/that_depends/providers.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.4.0/that_depends/py.typed
--rw-r--r--   0        0        0     4274 1970-01-01 00:00:00.000000 that_depends-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6086 2024-04-15 19:22:41.395455 that_depends-1.5.0/README.md
+-rw-r--r--   0        0        0     1482 2024-04-15 19:22:41.390100 that_depends-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.5.0/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.5.0/that_depends/container.py
+-rw-r--r--   0        0        0     1016 2024-03-18 09:24:54.496625 that_depends-1.5.0/that_depends/injection.py
+-rw-r--r--   0        0        0     5545 2024-04-15 18:25:35.357555 that_depends-1.5.0/that_depends/providers.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.5.0/that_depends/py.typed
+-rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 that_depends-1.5.0/PKG-INFO
```

### Comparing `that_depends-1.4.0/pyproject.toml` & `that_depends-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.4.0"
+version = "1.5.0"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.4.0/that_depends/container.py` & `that_depends-1.5.0/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.4.0/that_depends/injection.py` & `that_depends-1.5.0/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.4.0/that_depends/providers.py` & `that_depends-1.5.0/that_depends/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,31 @@
 
         return self._factory(
             *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
             **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
         )
 
 
+class AsyncFactory(AbstractProvider[T]):
+    def __init__(self, factory: typing.Callable[P, typing.Awaitable[T]], *args: P.args, **kwargs: P.kwargs) -> None:
+        self._factory = factory
+        self._args = args
+        self._kwargs = kwargs
+        self._override = None
+
+    async def resolve(self) -> T:
+        if self._override:
+            return typing.cast(T, self._override)
+
+        return await self._factory(
+            *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
+            **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+        )
+
+
 class List(AbstractProvider[T]):
     def __init__(self, *providers: AbstractProvider[T]) -> None:
         self._providers = providers
 
     async def resolve(self) -> list[T]:  # type: ignore[override]
         return [await x.resolve() for x in self._providers]
```

