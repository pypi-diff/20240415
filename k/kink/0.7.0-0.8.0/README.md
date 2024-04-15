# Comparing `tmp/kink-0.7.0.tar.gz` & `tmp/kink-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kink-0.7.0.tar", max compression
+gzip compressed data, was "kink-0.8.0.tar", max compression
```

## Comparing `kink-0.7.0.tar` & `kink-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1083 2023-09-25 07:38:41.650778 kink-0.7.0/LICENSE
--rw-r--r--   0        0        0    11234 2023-09-25 07:38:41.650778 kink-0.7.0/README.md
--rw-r--r--   0        0        0       47 2023-09-25 07:38:41.650778 kink-0.7.0/kink/__init__.py
--rw-r--r--   0        0        0       22 2023-09-25 07:38:41.650778 kink-0.7.0/kink/__verstion__.py
--rw-r--r--   0        0        0     3509 2023-09-25 07:38:41.650778 kink-0.7.0/kink/container.py
--rw-r--r--   0        0        0      169 2023-09-25 07:38:41.650778 kink-0.7.0/kink/errors/__init__.py
--rw-r--r--   0        0        0       45 2023-09-25 07:38:41.650778 kink-0.7.0/kink/errors/conainer_error.py
--rw-r--r--   0        0        0       92 2023-09-25 07:38:41.650778 kink-0.7.0/kink/errors/execution_error.py
--rw-r--r--   0        0        0       91 2023-09-25 07:38:41.650778 kink-0.7.0/kink/errors/resolver_error.py
--rw-r--r--   0        0        0      100 2023-09-25 07:38:41.654778 kink-0.7.0/kink/errors/service_error.py
--rw-r--r--   0        0        0     6241 2023-09-25 07:38:41.654778 kink-0.7.0/kink/inject.py
--rw-r--r--   0        0        0        0 2023-09-25 07:38:41.654778 kink-0.7.0/kink/py.typed
--rw-r--r--   0        0        0      589 2023-09-25 07:38:41.654778 kink-0.7.0/kink/typing_support.py
--rw-r--r--   0        0        0      837 2023-09-25 07:38:41.654778 kink-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    12203 1970-01-01 00:00:00.000000 kink-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-15 05:30:00.179310 kink-0.8.0/LICENSE
+-rw-r--r--   0        0        0    11234 2024-04-15 05:30:00.179310 kink-0.8.0/README.md
+-rw-r--r--   0        0        0       47 2024-04-15 05:30:00.179310 kink-0.8.0/kink/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-15 05:30:00.179310 kink-0.8.0/kink/__verstion__.py
+-rw-r--r--   0        0        0     3493 2024-04-15 05:30:00.179310 kink-0.8.0/kink/container.py
+-rw-r--r--   0        0        0      169 2024-04-15 05:30:00.179310 kink-0.8.0/kink/errors/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-15 05:30:00.179310 kink-0.8.0/kink/errors/conainer_error.py
+-rw-r--r--   0        0        0       92 2024-04-15 05:30:00.179310 kink-0.8.0/kink/errors/execution_error.py
+-rw-r--r--   0        0        0       91 2024-04-15 05:30:00.179310 kink-0.8.0/kink/errors/resolver_error.py
+-rw-r--r--   0        0        0      100 2024-04-15 05:30:00.179310 kink-0.8.0/kink/errors/service_error.py
+-rw-r--r--   0        0        0     6318 2024-04-15 05:30:00.179310 kink-0.8.0/kink/inject.py
+-rw-r--r--   0        0        0        0 2024-04-15 05:30:00.179310 kink-0.8.0/kink/py.typed
+-rw-r--r--   0        0        0      589 2024-04-15 05:30:00.179310 kink-0.8.0/kink/typing_support.py
+-rw-r--r--   0        0        0      858 2024-04-15 05:30:00.179310 kink-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    12153 1970-01-01 00:00:00.000000 kink-0.8.0/PKG-INFO
```

### Comparing `kink-0.7.0/LICENSE` & `kink-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kink-0.7.0/README.md` & `kink-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `kink-0.7.0/kink/container.py` & `kink-0.8.0/kink/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,18 @@
             del self._memoized_services[List[target]]  # type: ignore
 
         if name not in self._aliases:
             self._aliases[name] = []
         self._aliases[name].append(target)
 
     @overload
-    def __getitem__(self, key: str) -> Any:
-        ...
+    def __getitem__(self, key: str) -> Any: ...
 
     @overload
-    def __getitem__(self, key: Type[T]) -> T:
-        ...
+    def __getitem__(self, key: Type[T]) -> T: ...
 
     def __getitem__(self, key):
         if key in self._factories:
             return self._factories[key](self)
 
         if is_optional(key):
             return self[unpack_optional(key)]
```

### Comparing `kink-0.7.0/kink/inject.py` & `kink-0.8.0/kink/inject.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import sys
 from abc import ABC
 from functools import wraps
 from inspect import Parameter as InspectParameter, isclass, signature
-from typing import Any, Callable, Dict, NewType, Tuple, Type, TypeVar, Union, ForwardRef  # type: ignore
+from typing import Any, Callable, Dict, NewType, Tuple, Type, TypeVar, Union, ForwardRef, Optional  # type: ignore
 
 from typing_extensions import Protocol
 
 from .container import di, Container
 from .errors import ExecutionError
 
 T = TypeVar("T")
@@ -97,17 +97,18 @@
 
     return resolved_kwargs
 
 
 def _decorate(binding: Dict[str, Any], service: ServiceDefinition, container: Container) -> ServiceResult:
 
     # ignore abstract class initialiser and protocol initialisers
-    if (
-        service in [ABC.__init__, _no_init] or service.__name__ == "_no_init"
-    ):  # FIXME: fix this when typing_extensions library gets fixed
+    if service in [ABC.__init__, _no_init] or service.__name__ in [
+        "_no_init",
+        "_no_init_or_replace_init",
+    ]:  # FIXME: fix this when typing_extensions library gets fixed
         return service
 
     # Add class definition to dependency injection
     parameters_name, parameters = _inspect_function_arguments(service)
 
     def _resolve_kwargs(args, kwargs) -> dict:
         # attach named arguments
@@ -162,17 +163,17 @@
     if asyncio.iscoroutinefunction(service):
         return _async_decorated
 
     return _decorated
 
 
 def inject(
-    _service: ServiceDefinition = None,
-    alias: Any = None,
-    bind: Dict[str, Any] = None,
+    _service: Optional[ServiceDefinition] = None,
+    alias: Optional[Any] = None,
+    bind: Optional[Dict[str, Any]] = None,
     container: Container = di,
     use_factory: bool = False,
 ) -> Union[ServiceResult, Callable[[ServiceDefinition], ServiceResult]]:
     def _decorator(_service: ServiceDefinition) -> ServiceResult:
         if isclass(_service):
             setattr(
                 _service,
```

### Comparing `kink-0.7.0/kink/typing_support.py` & `kink-0.8.0/kink/typing_support.py`

 * *Files identical despite different names*

### Comparing `kink-0.7.0/pyproject.toml` & `kink-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kink"
-version = "0.7.0"
+version = "0.8.0"
 description = "Dependency injection for python."
 authors = [
     "Dawid Kraczkowski <dawid.kraczkowski@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -19,21 +19,22 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 include = ["kink/py.typed"]
 
 # Requirements
 [tool.poetry.dependencies]
-python = "^3.7"
-typing_extensions = "^4.1.1"
+python = "^3.8"
+typing_extensions = "^4.9.0"
 
 
 [tool.poetry.dev-dependencies]
-isort = "^5.7.0"
-pytest = "^5.4.3"
-pytest-asyncio = "^0.14.0"
-pytest-cov = "^2.5"
+isort = "^5.13.2"
+pytest = "^8.0.0"
+pytest-asyncio = "^0.23.5"
+pytest-cov = "^4.1.0"
 requests = "^2.31.0"
-starlette = "^0.13.4"
-black = "^22.3.0"
-mypy = "^0.961"
+starlette = "^0.37.1"
+httpx = "^0.26.0"
+black = "^24.2.0"
+mypy = "^1.8.0"
```

### Comparing `kink-0.7.0/PKG-INFO` & `kink-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: kink
-Version: 0.7.0
+Version: 0.8.0
 Summary: Dependency injection for python.
 Home-page: https://github.com/kodemore/kink
 License: MIT
 Keywords: kink,dependency injection
 Author: Dawid Kraczkowski
 Author-email: dawid.kraczkowski@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: typing_extensions (>=4.1.1,<5.0.0)
+Requires-Dist: typing_extensions (>=4.9.0,<5.0.0)
 Project-URL: Documentation, https://github.com/kodemore/kink
 Project-URL: Repository, https://github.com/kodemore/kink
 Description-Content-Type: text/markdown
 
 # Kink ![PyPI](https://img.shields.io/pypi/v/kink) ![Linting and Tests](https://github.com/kodemore/kink/workflows/Linting%20and%20Tests/badge.svg?branch=master) [![codecov](https://codecov.io/gh/kodemore/kink/branch/master/graph/badge.svg)](https://codecov.io/gh/kodemore/kink) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 Dependency injection container made for python
```

