# Comparing `tmp/pydantic_changedetect-0.6.5.tar.gz` & `tmp/pydantic_changedetect-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_changedetect-0.6.5.tar", max compression
+gzip compressed data, was "pydantic_changedetect-0.6.6.tar", max compression
```

## Comparing `pydantic_changedetect-0.6.5.tar` & `pydantic_changedetect-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/LICENSE
--rw-r--r--   0        0        0     5576 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/README.md
--rw-r--r--   0        0        0       47 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pydantic_changedetect/__init__.py
--rw-r--r--   0        0        0     1337 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pydantic_changedetect/_compat.py
--rw-r--r--   0        0        0    28056 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pydantic_changedetect/changedetect.py
--rw-r--r--   0        0        0        0 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pydantic_changedetect/py.typed
--rw-r--r--   0        0        0     2654 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pydantic_changedetect/utils.py
--rw-r--r--   0        0        0     1052 2024-03-28 17:38:10.828132 pydantic_changedetect-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     6394 1970-01-01 00:00:00.000000 pydantic_changedetect-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/LICENSE
+-rw-r--r--   0        0        0     5576 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/README.md
+-rw-r--r--   0        0        0       47 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/pydantic_changedetect/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/pydantic_changedetect/_compat.py
+-rw-r--r--   0        0        0    31972 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/changedetect.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/py.typed
+-rw-r--r--   0        0        0     2654 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/utils.py
+-rw-r--r--   0        0        0     1052 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     6394 1970-01-01 00:00:00.000000 pydantic_changedetect-0.6.6/PKG-INFO
```

### Comparing `pydantic_changedetect-0.6.5/LICENSE` & `pydantic_changedetect-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.5/README.md` & `pydantic_changedetect-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.5/pydantic_changedetect/_compat.py` & `pydantic_changedetect-0.6.6/pydantic_changedetect/_compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pydantic
 from pydantic.fields import FieldInfo
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 PYDANTIC_V1 = PYDANTIC_VERSION.startswith("1.")
 PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
+PYDANTIC_VERSION_TUPLE = tuple(map(int, PYDANTIC_VERSION.split('.')))
 
 if PYDANTIC_V1:  # pragma: no cover
     class PydanticCompat:  # type: ignore
         obj: pydantic.BaseModel
 
         def __init__(
             self,
```

### Comparing `pydantic_changedetect-0.6.5/pydantic_changedetect/changedetect.py` & `pydantic_changedetect-0.6.6/pydantic_changedetect/changedetect.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     cast,
     no_type_check,
     overload,
 )
 
 import pydantic
 
-from ._compat import PYDANTIC_V1, PYDANTIC_V2, PydanticCompat
+from ._compat import PYDANTIC_V1, PYDANTIC_V2, PYDANTIC_VERSION_TUPLE, PydanticCompat
 from .utils import is_pydantic_change_detect_annotation
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic import PrivateAttr
     from pydantic.typing import AbstractSetIntStr, MappingIntStrAny
     if PYDANTIC_V1:
         from pydantic.typing import DictStrAny, SetStr
@@ -432,85 +432,166 @@
                 super().__deepcopy__(memo=memo),
             )
             object.__setattr__(clone, "model_original", self.model_original.copy())
             object.__setattr__(clone, "model_self_changed_fields", self.model_self_changed_fields.copy())
             object.__setattr__(clone, "model_changed_markers", self.model_changed_markers.copy())
             return clone
 
-        def model_dump(
-            self,
-            *,
-            mode: Union[Literal['json', 'python'], str] = 'python',
-            include: "IncEx" = None,
-            exclude: "IncEx" = None,
-            by_alias: bool = False,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,
-            exclude_unchanged: bool = False,
-            round_trip: bool = False,
-            warnings: bool = True,
-        ) -> Dict[str, Any]:
-            """
-            Generate a dictionary representation of the model, optionally specifying
-            which fields to include or exclude.
-
-            Extends normal pydantic method to also allow to use `exclude_unchanged`.
-            """
-
-            return super().model_dump(
-                **self._get_changed_export_includes(
-                    mode=mode,
-                    include=include,
-                    exclude=exclude,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    exclude_defaults=exclude_defaults,
-                    exclude_none=exclude_none,
-                    exclude_unchanged=exclude_unchanged,
-                    round_trip=round_trip,
-                    warnings=warnings,
-                ),
-            )
+        if PYDANTIC_VERSION_TUPLE >= (2, 7, 0):
+            def model_dump(  # pyright: ignore [reportRedeclaration]
+                self,
+                *,
+                mode: Union[Literal['json', 'python'], str] = 'python',
+                include: "IncEx" = None,
+                exclude: "IncEx" = None,
+                context: Optional[Dict[str, Any]] = None,  # Available since 2.7
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                exclude_unchanged: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
+                serialize_as_any: bool = False,  # Available since 2.7
+            ) -> Dict[str, Any]:
+                """
+                Generate a dictionary representation of the model, optionally specifying
+                which fields to include or exclude.
+
+                Extends normal pydantic method to also allow to use `exclude_unchanged`.
+                """
+
+                return super().model_dump(
+                    **self._get_changed_export_includes(
+                        mode=mode,
+                        include=include,
+                        exclude=exclude,
+                        context=context,
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        exclude_none=exclude_none,
+                        exclude_unchanged=exclude_unchanged,
+                        round_trip=round_trip,
+                        warnings=warnings,
+                        serialize_as_any=serialize_as_any,
+                    ),
+                )
 
-        def model_dump_json(
-            self,
-            *,
-            indent: Optional[int] = None,
-            include: "IncEx" = None,
-            exclude: "IncEx" = None,
-            by_alias: bool = False,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,
-            exclude_unchanged: bool = False,
-            round_trip: bool = False,
-            warnings: bool = True,
-        ) -> str:
-            """
-            Generates a JSON representation of the model using Pydantic's `to_json`
-            method.
-
-            Extends normal pydantic method to also allow to use `exclude_unchanged`.
-            """
-
-            return super().model_dump_json(
-                **self._get_changed_export_includes(
-                    indent=indent,
-                    include=include,
-                    exclude=exclude,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    exclude_defaults=exclude_defaults,
-                    exclude_none=exclude_none,
-                    exclude_unchanged=exclude_unchanged,
-                    round_trip=round_trip,
-                    warnings=warnings,
-                ),
-            )
+            def model_dump_json(  # pyright: ignore [reportRedeclaration]
+                self,
+                *,
+                indent: Optional[int] = None,
+                include: "IncEx" = None,
+                exclude: "IncEx" = None,
+                context: Optional[Dict[str, Any]] = None,  # Available since 2.7
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                exclude_unchanged: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
+                serialize_as_any: bool = False,  # Available since 2.7
+            ) -> str:
+                """
+                Generates a JSON representation of the model using Pydantic's `to_json`
+                method.
+
+                Extends normal pydantic method to also allow to use `exclude_unchanged`.
+                """
+
+                return super().model_dump_json(
+                    **self._get_changed_export_includes(
+                        indent=indent,
+                        include=include,
+                        exclude=exclude,
+                        context=context,
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        exclude_none=exclude_none,
+                        exclude_unchanged=exclude_unchanged,
+                        round_trip=round_trip,
+                        warnings=warnings,
+                        serialize_as_any=serialize_as_any,
+                    ),
+                )
+        else:  # Version 2.x < 2.7.0
+            def model_dump(  # pyright: ignore [reportIncompatibleMethodOverride]
+                self,
+                *,
+                mode: Union[Literal['json', 'python'], str] = 'python',
+                include: "IncEx" = None,
+                exclude: "IncEx" = None,
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                exclude_unchanged: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
+            ) -> Dict[str, Any]:
+                """
+                Generate a dictionary representation of the model, optionally specifying
+                which fields to include or exclude.
+
+                Extends normal pydantic method to also allow to use `exclude_unchanged`.
+                """
+
+                return super().model_dump(
+                    **self._get_changed_export_includes(
+                        mode=mode,
+                        include=include,
+                        exclude=exclude,
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        exclude_none=exclude_none,
+                        exclude_unchanged=exclude_unchanged,
+                        round_trip=round_trip,
+                        warnings=warnings,
+                    ),
+                )
+
+            def model_dump_json(  # pyright: ignore [reportIncompatibleMethodOverride]
+                self,
+                *,
+                indent: Optional[int] = None,
+                include: "IncEx" = None,
+                exclude: "IncEx" = None,
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                exclude_unchanged: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
+            ) -> str:
+                """
+                Generates a JSON representation of the model using Pydantic's `to_json`
+                method.
+
+                Extends normal pydantic method to also allow to use `exclude_unchanged`.
+                """
+
+                return super().model_dump_json(
+                    **self._get_changed_export_includes(
+                        indent=indent,
+                        include=include,
+                        exclude=exclude,
+                        by_alias=by_alias,
+                        exclude_unset=exclude_unset,
+                        exclude_defaults=exclude_defaults,
+                        exclude_none=exclude_none,
+                        exclude_unchanged=exclude_unchanged,
+                        round_trip=round_trip,
+                        warnings=warnings,
+                    ),
+                )
 
     # Compatibility for pydantic 2.0 compatibility methods to support pydantic 1.0 migration 🙈
 
     def copy(
         self: "Model",
         *,
         include: "Union[AbstractSetIntStr, MappingIntStrAny, None]" = None,
@@ -534,15 +615,15 @@
         )
         object.__setattr__(clone, "model_original", self.model_original.copy())
         object.__setattr__(clone, "model_self_changed_fields", self.model_self_changed_fields.copy())
         object.__setattr__(clone, "model_changed_markers", self.model_changed_markers.copy())
         return clone
 
     if PYDANTIC_V2:
-        # The following methods are SLIGHTLY different fpr v1 and v2, so we need to keep
+        # The following methods are SLIGHTLY different for v1 and v2, so we need to keep
         # them separate
 
         def dict(  # type: ignore
             self,
             *,
             include: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
             exclude: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
```

### Comparing `pydantic_changedetect-0.6.5/pydantic_changedetect/utils.py` & `pydantic_changedetect-0.6.6/pydantic_changedetect/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.5/pyproject.toml` & `pydantic_changedetect-0.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-changedetect"
-version = "0.6.5"
+version = "0.6.6"
 description = "Extend pydantic models to also detect and record changes made to the model attributes."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-changedetect"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_changedetect-0.6.5/PKG-INFO` & `pydantic_changedetect-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-changedetect
-Version: 0.6.5
+Version: 0.6.6
 Summary: Extend pydantic models to also detect and record changes made to the model attributes.
 Home-page: https://github.com/team23/pydantic-changedetect
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

