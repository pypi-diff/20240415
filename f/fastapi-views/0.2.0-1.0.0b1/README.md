# Comparing `tmp/fastapi_views-0.2.0.tar.gz` & `tmp/fastapi_views-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_views-0.2.0.tar", max compression
+gzip compressed data, was "fastapi_views-1.0.0b1.tar", max compression
```

## Comparing `fastapi_views-0.2.0.tar` & `fastapi_views-1.0.0b1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-04-15 15:53:58.446512 fastapi_views-0.2.0/LICENSE
--rw-r--r--   0        0        0     2160 2024-04-15 15:53:58.446512 fastapi_views-0.2.0/README.md
--rw-r--r--   0        0        0      598 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/__init__.py
--rw-r--r--   0        0        0       22 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/_version.py
--rw-r--r--   0        0        0     1400 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/cli.py
--rw-r--r--   0        0        0     1701 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/config.py
--rw-r--r--   0        0        0        0 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/errors/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/errors/exceptions.py
--rw-r--r--   0        0        0     1648 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/errors/handlers.py
--rw-r--r--   0        0        0     4556 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/errors/models.py
--rw-r--r--   0        0        0     1647 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/healthcheck.py
--rw-r--r--   0        0        0      348 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/openapi.py
--rw-r--r--   0        0        0      586 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/opentelemetry.py
--rw-r--r--   0        0        0      663 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/prometheus.py
--rw-r--r--   0        0        0        0 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/py.typed
--rw-r--r--   0        0        0      526 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/response.py
--rw-r--r--   0        0        0      421 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/routers.py
--rw-r--r--   0        0        0      774 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/schemas.py
--rw-r--r--   0        0        0      789 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/serializer.py
--rw-r--r--   0        0        0     1997 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/settings.py
--rw-r--r--   0        0        0     1438 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/types.py
--rw-r--r--   0        0        0      170 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/__init__.py
--rw-r--r--   0        0        0    19102 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/api.py
--rw-r--r--   0        0        0     2599 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/functools.py
--rw-r--r--   0        0        0    12770 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/generics.py
--rw-r--r--   0        0        0     2120 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/mixins.py
--rw-r--r--   0        0        0     4355 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/fastapi_views/views/viewsets.py
--rw-r--r--   0        0        0     3109 2024-04-15 15:53:58.450512 fastapi_views-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 fastapi_views-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2166 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/README.md
+-rw-r--r--   0        0        0      598 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/__init__.py
+-rw-r--r--   0        0        0       29 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/_version.py
+-rw-r--r--   0        0        0     1701 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/config.py
+-rw-r--r--   0        0        0        0 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/errors/__init__.py
+-rw-r--r--   0        0        0     1335 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/errors/exceptions.py
+-rw-r--r--   0        0        0     2067 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/errors/handlers.py
+-rw-r--r--   0        0        0     4256 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/errors/models.py
+-rw-r--r--   0        0        0     1647 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/healthcheck.py
+-rw-r--r--   0        0        0      331 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/openapi.py
+-rw-r--r--   0        0        0      586 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/opentelemetry.py
+-rw-r--r--   0        0        0      663 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/prometheus.py
+-rw-r--r--   0        0        0        0 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/py.typed
+-rw-r--r--   0        0        0      446 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/response.py
+-rw-r--r--   0        0        0      421 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/routers.py
+-rw-r--r--   0        0        0      774 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/schemas.py
+-rw-r--r--   0        0        0      789 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/serializer.py
+-rw-r--r--   0        0        0     1997 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/settings.py
+-rw-r--r--   0        0        0     1438 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/types.py
+-rw-r--r--   0        0        0      170 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/__init__.py
+-rw-r--r--   0        0        0    18696 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/api.py
+-rw-r--r--   0        0        0     2599 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/functools.py
+-rw-r--r--   0        0        0    12770 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/generics.py
+-rw-r--r--   0        0        0     2120 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/mixins.py
+-rw-r--r--   0        0        0     4355 2024-02-05 22:16:47.082917 fastapi_views-1.0.0b1/fastapi_views/views/viewsets.py
+-rw-r--r--   0        0        0     2805 2024-02-05 22:16:47.086917 fastapi_views-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 fastapi_views-1.0.0b1/PKG-INFO
```

### Comparing `fastapi_views-0.2.0/LICENSE` & `fastapi_views-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/README.md` & `fastapi_views-1.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.2.0 
+Version: 1.0.0-beta.1
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
```

### Comparing `fastapi_views-0.2.0/fastapi_views/__init__.py` & `fastapi_views-1.0.0b1/fastapi_views/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/config.py` & `fastapi_views-1.0.0b1/fastapi_views/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/errors/exceptions.py` & `fastapi_views-1.0.0b1/fastapi_views/errors/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
         self.headers = headers
         self.kwargs = kwargs
 
     def get_status(self) -> int:
         return self.model.model_fields["status"].get_default()
 
     def as_model(self, **kwargs) -> ErrorDetails:
-        kwargs = {**self.kwargs, **kwargs}
-        return self.model(detail=self.detail, **kwargs)
+        return self.model(detail=self.detail, **self.kwargs, **kwargs)
 
 
 class NotFound(APIError):
     model = NotFoundErrorDetails
 
 
 class UnprocessableEntity(APIError):
```

### Comparing `fastapi_views-0.2.0/fastapi_views/errors/handlers.py` & `fastapi_views-1.0.0b1/fastapi_views/errors/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from logging import getLogger
 
 from fastapi import Request
-from fastapi.encoders import jsonable_encoder
-from fastapi.exceptions import RequestValidationError
+from fastapi.exceptions import RequestValidationError, ResponseValidationError
 from starlette.status import HTTP_500_INTERNAL_SERVER_ERROR
 
 from ..response import JsonResponse
 from .exceptions import APIError
 from .models import InternalServerErrorDetails, UnprocessableEntityErrorDetails
 
 logger = getLogger("exceptions.handler")
@@ -23,30 +22,42 @@
     )
 
 
 def request_validation_handler(request: Request, exc: RequestValidationError):
     model = UnprocessableEntityErrorDetails(
         detail="Validation error",
         instance=request.url.path,
-        errors=jsonable_encoder(exc.errors()),
+        errors=exc.errors(),
     )
     return JsonResponse(
         status_code=model.status,
         content=model.model_dump_json(),
     )
 
 
+def response_validation_handler(request: Request, exc: ResponseValidationError):
+    logger.exception("Response validation failed", exc_info=exc)
+    return JsonResponse(
+        status_code=HTTP_500_INTERNAL_SERVER_ERROR,
+        content=InternalServerErrorDetails(
+            detail="Response validation failed",
+            instance=request.url.path,
+        ).model_dump_json(),
+    )
+
+
 def exception_handler(request: Request, exc: Exception):
-    logger.exception("Unhandled exception", exc_info=exc)
+    logger.warning("Unhandled exception", exc_info=exc)
     return JsonResponse(
         status_code=HTTP_500_INTERNAL_SERVER_ERROR,
         content=InternalServerErrorDetails(
-            detail="Unhandled server error",
+            detail=str(exc),
             instance=request.url.path,
         ).model_dump_json(),
     )
 
 
 def add_error_handlers(app):
     app.add_exception_handler(APIError, api_error_handler)
     app.add_exception_handler(RequestValidationError, request_validation_handler)
+    app.add_exception_handler(ResponseValidationError, response_validation_handler)
     app.add_exception_handler(Exception, exception_handler)
```

### Comparing `fastapi_views-0.2.0/fastapi_views/errors/models.py` & `fastapi_views-1.0.0b1/fastapi_views/errors/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, ClassVar, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field, create_model, field_validator
+from pydantic import BaseModel, ConfigDict, Field, field_validator
+from pydantic.fields import FieldInfo
 from pydantic_core import Url
 from starlette.status import (
     HTTP_400_BAD_REQUEST,
     HTTP_401_UNAUTHORIZED,
     HTTP_403_FORBIDDEN,
     HTTP_404_NOT_FOUND,
     HTTP_409_CONFLICT,
@@ -18,19 +19,24 @@
 
 
 class ErrorDetails(BaseModel):
     """
     Base Model for https://www.rfc-editor.org/rfc/rfc9457.html
     """
 
-    _registry: ClassVar[dict[int, type["ErrorDetails"]]] = {}
-
     def __init_subclass__(cls, **kwargs):
+        for k in ("status", "title", "type"):
+            if field := kwargs.get(k):
+                cls.model_fields[k] = FieldInfo(
+                    default=field, annotation=Literal[field]
+                )
         cls._registry[cls.get_status()] = cls
 
+    _registry: ClassVar[dict[int, type["ErrorDetails"]]] = {}
+
     type: Union[Url, Literal["about:blank"]] = Field(
         "about:blank",
         description="Error type",
     )
     title: Optional[str] = Field("Bad Request", description="Error title")
     status: int = Field(HTTP_400_BAD_REQUEST, description="Error status")
     detail: str = Field(
@@ -68,80 +74,86 @@
         return super().model_dump_json(**kwargs)
 
     model_config = ConfigDict(
         use_enum_values=True, populate_by_name=True, extra="allow"
     )
 
 
-def create_error_model(name: str, type: str, title: str, status: int):
-    return create_model(
-        name,
-        __base__=ErrorDetails,
-        type=(Literal[type], Field(type, description="Error type")),
-        title=(Literal[title], Field(title, description="Error title")),
-        status=(Literal[status], Field(status, description="Error status")),
-    )
-
-
-NotFoundErrorDetails = create_error_model(
-    "NotFoundErrorDetails",
+class NotFoundErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.5.4",
     title="Not Found",
     status=HTTP_404_NOT_FOUND,
-)
+):
+    pass
+
 
-UnprocessableEntityErrorDetails = create_error_model(
-    "UnprocessableEntityErrorDetails",
+class UnprocessableEntityErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc4918#section-11.2",
     title="Unprocessable Entity",
     status=HTTP_422_UNPROCESSABLE_ENTITY,
-)
+):
+    pass
 
 
-BadRequestErrorDetails = create_error_model(
-    "BadRequestErrorDetails",
+class BadRequestErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.5.1",
     title="Bad Request",
     status=HTTP_400_BAD_REQUEST,
-)
+):
+    pass
+
 
-UnauthorizedErrorDetails = create_error_model(
-    "UnauthorizedErrorDetails",
+class UnauthorizedErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7235#section-3.1",
     title="Unauthorized",
     status=HTTP_401_UNAUTHORIZED,
-)
+):
+    pass
+
 
-ForbiddenErrorDetails = create_error_model(
-    "ForbiddenErrorDetails",
+class ForbiddenErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.5.3",
     title="Forbidden",
     status=HTTP_403_FORBIDDEN,
-)
+):
+    pass
 
-TooManyRequestsErrorDetails = create_error_model(
-    "TooManyRequestsErrorDetails",
+
+class TooManyRequestsErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc6585#section-4",
     title="Too many requests",
     status=HTTP_429_TOO_MANY_REQUESTS,
-)
+):
+    pass
+
 
-ConflictErrorDetails = create_error_model(
-    "ConflictErrorDetails",
+class ConflictErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.5.8",
     title="Conflict",
     status=HTTP_409_CONFLICT,
-)
+):
+    pass
+
 
-ServiceUnavailableErrorDetails = create_error_model(
-    "ServiceUnavailableErrorDetails",
+class ServiceUnavailableErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.6.4",
     title="Service Unavailable",
     status=HTTP_503_SERVICE_UNAVAILABLE,
-)
+):
+    pass
 
-InternalServerErrorDetails = create_error_model(
-    "InternalServerErrorDetails",
+
+class InternalServerErrorDetails(
+    ErrorDetails,
     type="https://datatracker.ietf.org/doc/html/rfc7231#section-6.6.1",
     title="Internal Server Error",
     status=HTTP_500_INTERNAL_SERVER_ERROR,
-)
+):
+    pass
```

### Comparing `fastapi_views-0.2.0/fastapi_views/healthcheck.py` & `fastapi_views-1.0.0b1/fastapi_views/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/opentelemetry.py` & `fastapi_views-1.0.0b1/fastapi_views/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/prometheus.py` & `fastapi_views-1.0.0b1/fastapi_views/prometheus.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 
 
 def add_prometheus_middleware(
     app: FastAPI, endpoint: str = "/metrics", **kwargs: Any
 ) -> None:
     from starlette_exporter import PrometheusMiddleware, handle_metrics
 
-    kwargs.setdefault("group_paths", True)
     kwargs.setdefault("app_name", app.title.lower().replace(" ", "_"))
     kwargs.setdefault("skip_paths", ["/healthz", "/docs", "/openapi.json", "/metrics"])
+    kwargs.setdefault("group_paths", True)
     kwargs.setdefault("labels", {"server": socket.gethostname()})
     kwargs.setdefault("always_use_int_status", True)
     app.add_middleware(PrometheusMiddleware, **kwargs)
     app.add_route(endpoint, handle_metrics)
```

### Comparing `fastapi_views-0.2.0/fastapi_views/schemas.py` & `fastapi_views-1.0.0b1/fastapi_views/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/serializer.py` & `fastapi_views-1.0.0b1/fastapi_views/serializer.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/settings.py` & `fastapi_views-1.0.0b1/fastapi_views/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/types.py` & `fastapi_views-1.0.0b1/fastapi_views/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/views/api.py` & `fastapi_views-1.0.0b1/fastapi_views/views/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
-import functools
 import inspect
 from abc import ABC, abstractmethod
 from collections.abc import Awaitable, Generator
-from typing import TYPE_CHECKING, Any, Callable, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Generic, Optional, TypeVar, Union
 
 from fastapi import Depends, Request, Response
 from starlette.status import HTTP_200_OK, HTTP_201_CREATED, HTTP_204_NO_CONTENT
 
 from ..errors.exceptions import APIError, Conflict, NotFound, UnprocessableEntity
 from ..response import JsonResponse
 from ..serializer import TypeSerializer
 from ..types import Action, SerializerOptions
 from .functools import VIEWSET_ROUTE_FLAG, errors
 from .mixins import DetailViewMixin, ErrorHandlerMixin
 
+S = TypeVar("S", bound=type[Any])
+
 Endpoint = Callable[..., Union[Response, Awaitable[Response]]]
 
 
 class View(ABC):
     """
     Basic View Class
     Usage:
@@ -51,33 +52,26 @@
 
     @classmethod
     def get_api_actions(cls, prefix: str = ""):
         yield from cls.get_custom_api_actions(prefix)
 
     @classmethod
     def get_custom_endpoint(cls, func):
-        options = getattr(func, "kwargs", {})
-        status_code = options.get("status_code", None)
-        response_class = options.get("response_class", None)
-
         async def _async_endpoint(self, *args, **kwargs):
             res = await func(self, *args, **kwargs)
-            return self.get_response(
-                content=res, status_code=status_code, response_class=response_class
-            )
+            return self.get_response(content=res)
 
         def _sync_endpoint(self, *args, **kwargs):
             res = func(self, *args, **kwargs)
-            return self.get_response(
-                content=res, status_code=status_code, response_class=response_class
-            )
+            return self.get_response(content=res)
 
-        endpoint = (
-            _async_endpoint if asyncio.iscoroutinefunction(func) else _sync_endpoint
-        )
+        if asyncio.iscoroutinefunction(func):
+            endpoint = _async_endpoint
+        else:
+            endpoint = _sync_endpoint
 
         cls._patch_endpoint_signature(endpoint, func)
         return endpoint
 
     @classmethod
     def get_custom_api_actions(cls, prefix: str = ""):
         for _, route_endpoint in inspect.getmembers(
@@ -124,65 +118,62 @@
             parameter.replace(kind=inspect.Parameter.KEYWORD_ONLY)
             for parameter in old_parameters[1:]
         ]
         new_signature = old_signature.replace(parameters=new_parameters)
         endpoint.__signature__ = new_signature
         cls._patch_metadata(endpoint, method)
 
-    def get_response(
-        self,
-        content: Any,
-        status_code: Optional[int] = None,
-        response_class: Optional[type[Response]] = None,
-    ) -> Response:
+    def get_response(self, content: Any, status_code: Optional[int] = None) -> Response:
         if isinstance(content, Response):
             return content
-        response_class = response_class or self.default_response_class
-        return response_class(
+        return self.default_response_class(
             content=content,
             status_code=status_code or self.response.status_code or HTTP_200_OK,
             headers=dict(self.response.headers),
         )
 
 
-class APIView(View, ErrorHandlerMixin):
+class APIView(View, ErrorHandlerMixin, Generic[S]):
     """
     View with build-in json serialization via
     `serializer` and error handling
     """
 
-    response_schema: Any
+    response_schema: S
     serializer_options: SerializerOptions = {"by_alias": True, "from_attributes": True}
 
+    _serializers: dict[str, TypeSerializer[S]] = {}
+
     @classmethod
-    def get_response_schema(cls, action: Action) -> Any:
+    def get_response_schema(cls, action: Action) -> S:
         return cls.response_schema
 
     @classmethod
-    @functools.lru_cache(maxsize=None, typed=True)
-    def get_serializer(cls, action: Action) -> TypeSerializer:
-        response_schema = cls.get_response_schema(action)
-        return TypeSerializer(response_schema)
+    def get_serializer(cls, action: Action) -> TypeSerializer[S]:
+        if action not in cls._serializers:
+            response_schema = cls.get_response_schema(action)
+            cls._serializers[action] = TypeSerializer(response_schema)
+        return cls._serializers[action]
 
     def serialize_response(
         self, action: Action, content: Any, status_code: int = HTTP_200_OK
     ):
-        if content and not isinstance(content, bytes):
+        if content:
             serializer = self.get_serializer(action)
             content = serializer.serialize(content, **self.serializer_options)
         if self.response.status_code is None:
             self.response.status_code = status_code
         return self.get_response(content)
 
 
-class BaseListAPIView(APIView):
+class BaseListAPIView(APIView[S]):
     response_schema_as_list: bool = True
 
     @classmethod
-    def get_response_schema(cls, action: Action) -> Any:
+    def get_response_schema(cls, action: Action) -> S:
         if action == "list" and cls.response_schema_as_list:
             return list[cls.response_schema]  # type: ignore
         return cls.response_schema
 
     @classmethod
     @abstractmethod
     def get_list_endpoint(cls) -> Endpoint:
@@ -253,15 +244,15 @@
     @classmethod
     def get_api_actions(cls, prefix: str = ""):
         yield cls.get_api_action(
             prefix=prefix,
             endpoint=cls.get_retrieve_endpoint(),
             path=cls.get_detail_route(action="retrieve"),
             methods=["GET"],
-            responses=errors(NotFound, UnprocessableEntity),
+            responses=errors(NotFound),
             response_model=cls.get_response_schema(action="retrieve"),
             name=f"Get {cls.get_name()}",
             operation_id=f"get_{cls.get_slug_name()}",
         )
         yield from super().get_api_actions(prefix)
 
 
@@ -537,15 +528,14 @@
     def get_api_actions(cls, prefix: str = "") -> Generator:
         yield cls.get_api_action(
             prefix=prefix,
             path=cls.get_detail_route(action="destroy"),
             endpoint=cls.get_destroy_endpoint(),
             methods=["DELETE"],
             response_class=Response,
-            responses=errors(UnprocessableEntity),
             status_code=HTTP_204_NO_CONTENT,
             name=f"Delete {cls.get_name()}",
             operation_id=f"delete_{cls.get_slug_name()}",
         )
         yield from super().get_api_actions(prefix)
 
     @classmethod
```

### Comparing `fastapi_views-0.2.0/fastapi_views/views/functools.py` & `fastapi_views-1.0.0b1/fastapi_views/views/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/views/generics.py` & `fastapi_views-1.0.0b1/fastapi_views/views/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/views/mixins.py` & `fastapi_views-1.0.0b1/fastapi_views/views/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/fastapi_views/views/viewsets.py` & `fastapi_views-1.0.0b1/fastapi_views/views/viewsets.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.2.0/pyproject.toml` & `fastapi_views-1.0.0b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 [tool.poetry]
 name = "fastapi-views"
-version = "0.2.0"
+version = "1.0.0-beta.1"
 description = "FastAPI Class Views and utilities"
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
-packages = [{ include = "fastapi_views" }]
-
-[tool.poetry.scripts]
-fastapi-views = "fastapi_views.cli:cli"
+packages = [{include = "fastapi_views"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-typer = "^0.9.0"
-fastapi = "^0.110.1"
+fastapi = "^0.109.2"
 pydantic = ">=2.0,<3.0"
 pydantic-settings = ">=2.0,<3.0"
 orjson = "^3.9.10"
-opentelemetry-instrumentation-fastapi = { version = "*", optional = true }
-starlette-exporter = { version = "^0.21.0", optional = true }
-uvloop = { version = "^0.19.0", optional = true }
-uvicorn = { version = "^0.27.1", optional = true }
+opentelemetry-instrumentation-fastapi = {version = "*", optional = true}
+starlette-exporter = {version = "^0.17.1", optional = true}
+uvloop = {version = "^0.19.0", optional = true}
+
 
 [tool.poetry.extras]
-all = ["uvloop", "starlette-exporter", "uvicorn", "opentelemetry-instrumentation-fastapi"]
+all = ["uvloop", "starlette-exporter", "opentelemetry-instrumentation-fastapi"]
 uvloop = ["uvloop"]
 prometheus = ["starlette-exporter"]
-uvicorn = ["uvicorn"]
 opentelemetry = ["opentelemetry-instrumentation-fastapi"]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 ruff = "^0.1.11"
 deptry = "^0.12.0"
 bandit = "^1.7.4"
-python-semantic-release = "^7.33.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.2.1,<9.0.0"
+pytest = "^7.2.1"
 pytest-asyncio = "^0.20.2"
 pytest-cov = "^4.0.0"
-pytest-sugar = ">=0.9.7,<1.1.0"
+pytest-sugar = "^0.9.7"
 pytest-repeat = "^0.9.3"
 httpx = "^0.24.0"
 asgi-lifespan = "^2.1.0"
+uvicorn = "^0.25.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.2.1"
 mkdocs-autorefs = "^0.4.1"
 mkdocs-gen-files = ">=0.4,<0.6"
-mkdocstrings = { version = ">=0.18", extras = ["python"] }
-watchdog = ">=2.0,<4.0"
+mkdocstrings = {version = ">=0.18", extras = ["python"]}
 
 [tool.pytest.ini_options]
 addopts = "--cov=./fastapi_views --count=3"
-testpaths = ["./tests"]
+testpaths = [
+   "./tests"
+]
 asyncio_mode = "auto"
 
 [tool.mypy]
 python_version = 3.9
 ignore_missing_imports = true
 no_site_packages = true
 
@@ -66,25 +62,25 @@
 target-version = "py39"
 
 line-length = 88
 indent-width = 4
 
 [tool.ruff.lint]
 select = [
-    "E",   # pycodestyle errors
-    "W",   # pycodestyle warnings
-    "F",   # pyflakes
-    "I",   # isort
-    "C",   # flake8-comprehensions
-    "B",   # flake8-bugbear
-    "UP",  # pyupgrade
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # pyflakes
+    "I",  # isort
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+    "UP", # pyupgrade
     "SIM", # flake8-simplify
 ]
 ignore = [
-    "B008", # do not perform function calls in argument defaults
+    "B008",  # do not perform function calls in argument defaults
     "E501", # line too long
 ]
 fixable = ["ALL"]
 unfixable = []
 
 [tool.ruff.format]
 quote-style = "double"
@@ -94,24 +90,25 @@
 docstring-code-line-length = "dynamic"
 line-ending = "auto"
 
 [tool.ruff.mccabe]
 max-complexity = 8
 
 [tool.deptry.per_rule_ignores]
-DEP001 = ["opentelemetry", "yaml"]
 DEP003 = ["fastapi_views", "pydantic_core", "starlette", "typing_extensions"]
-DEP002 = ["uvloop", "uvicorn", "opentelemetry-instrumentation-fastapi"]
+DEP002 = ["uvloop"]
 
 [tool.semantic_release]
-version_variable = ['fastapi_views/_version.py:__version__']
+version_variable = [
+    'fastapi_views/_version.py:__version__',
+]
 version_toml = 'pyproject.toml:tool.poetry.version'
 version_pattern = [
     'docs/index.md:Version: (\d+\.\d+\.\d+)',
-    'README.md:Version: (\d+\.\d+\.\d+)',
+    'README.md:Version: (\d+\.\d+\.\d+)'
 ]
 upload_to_repository = false
 major_on_zero = true
 hvcs = "github"
 commit_message = "Bump version: {version}"
 tag_commit = false
```

### Comparing `fastapi_views-0.2.0/PKG-INFO` & `fastapi_views-1.0.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: fastapi-views
-Version: 0.2.0
+Version: 1.0.0b1
 Summary: FastAPI Class Views and utilities
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: opentelemetry
 Provides-Extra: prometheus
-Provides-Extra: uvicorn
 Provides-Extra: uvloop
-Requires-Dist: fastapi (>=0.110.1,<0.111.0)
+Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: opentelemetry-instrumentation-fastapi ; extra == "all" or extra == "opentelemetry"
 Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pydantic-settings (>=2.0,<3.0)
-Requires-Dist: starlette-exporter (>=0.21.0,<0.22.0) ; extra == "all" or extra == "prometheus"
-Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: uvicorn (>=0.27.1,<0.28.0) ; extra == "all" or extra == "uvicorn"
+Requires-Dist: starlette-exporter (>=0.17.1,<0.18.0) ; extra == "all" or extra == "prometheus"
 Requires-Dist: uvloop (>=0.19.0,<0.20.0) ; extra == "all" or extra == "uvloop"
 Description-Content-Type: text/markdown
 
 # fastapi-views
 
 ![CI](https://github.com/performancemedia/fastapi-views/workflows/CI/badge.svg)
 ![Build](https://github.com/performancemedia/fastapi-views/workflows/Publish/badge.svg)
@@ -37,15 +34,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.2.0 
+Version: 1.0.0-beta.1
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
```

