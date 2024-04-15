# Comparing `tmp/fastapi_query-0.1a0.tar.gz` & `tmp/fastapi_query-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_query-0.1a0.tar", max compression
+gzip compressed data, was "fastapi_query-0.1a1.tar", max compression
```

## Comparing `fastapi_query-0.1a0.tar` & `fastapi_query-0.1a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1074 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/LICENSE
--rw-r--r--   0        0        0        0 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/README.md
--rw-r--r--   0        0        0        0 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/fastapi_query/__init__.py
--rw-r--r--   0        0        0     3578 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/fastapi_query/_compat.py
--rw-r--r--   0        0        0        0 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/fastapi_query/ext/__init__.py
--rw-r--r--   0        0        0      218 2024-02-23 14:28:12.088815 fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5988 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/filtering.py
--rw-r--r--   0        0        0     2119 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/ordering.py
--rw-r--r--   0        0        0     4718 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/pagination.py
--rw-r--r--   0        0        0      181 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/tortoise/__init__.py
--rw-r--r--   0        0        0     5700 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/tortoise/filtering.py
--rw-r--r--   0        0        0     1280 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/tortoise/ordering.py
--rw-r--r--   0        0        0     2223 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/tortoise/pagination.py
--rw-r--r--   0        0        0     1306 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/ext/tortoise/utils.py
--rw-r--r--   0        0        0      150 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/filtering/__init__.py
--rw-r--r--   0        0        0     1177 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/filtering/base_params.py
--rw-r--r--   0        0        0     1136 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/filtering/deps.py
--rw-r--r--   0        0        0      399 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/filtering/enums.py
--rw-r--r--   0        0        0     6426 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/filtering/utils.py
--rw-r--r--   0        0        0      199 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/pagination/__init__.py
--rw-r--r--   0        0        0      149 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/pagination/deps.py
--rw-r--r--   0        0        0      487 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/pagination/schemas.py
--rw-r--r--   0        0        0      766 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/pagination/utils.py
--rw-r--r--   0        0        0      548 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/fastapi_query/utils.py
--rw-r--r--   0        0        0     2713 2024-02-23 14:28:12.092815 fastapi_query-0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 fastapi_query-0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/__init__.py
+-rw-r--r--   0        0        0     3578 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/_compat.py
+-rw-r--r--   0        0        0        0 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5931 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/filtering.py
+-rw-r--r--   0        0        0     2119 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/ordering.py
+-rw-r--r--   0        0        0     4718 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/pagination.py
+-rw-r--r--   0        0        0      181 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/tortoise/__init__.py
+-rw-r--r--   0        0        0     5700 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/tortoise/filtering.py
+-rw-r--r--   0        0        0     1280 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/tortoise/ordering.py
+-rw-r--r--   0        0        0     2223 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/tortoise/pagination.py
+-rw-r--r--   0        0        0     1306 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/ext/tortoise/utils.py
+-rw-r--r--   0        0        0      150 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/filtering/__init__.py
+-rw-r--r--   0        0        0     1177 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/filtering/base_params.py
+-rw-r--r--   0        0        0     1136 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/filtering/deps.py
+-rw-r--r--   0        0        0      399 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/filtering/enums.py
+-rw-r--r--   0        0        0     6426 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/filtering/utils.py
+-rw-r--r--   0        0        0      199 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/pagination/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/pagination/deps.py
+-rw-r--r--   0        0        0      487 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/pagination/schemas.py
+-rw-r--r--   0        0        0      766 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/pagination/utils.py
+-rw-r--r--   0        0        0      548 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/fastapi_query/utils.py
+-rw-r--r--   0        0        0     2714 2024-04-15 18:56:02.019701 fastapi_query-0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 fastapi_query-0.1a1/PKG-INFO
```

### Comparing `fastapi_query-0.1a0/LICENSE` & `fastapi_query-0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/_compat.py` & `fastapi_query-0.1a1/fastapi_query/_compat.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/filtering.py` & `fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     return or_(*res)
 
 
 def _get_orm_filters(
         model_class: Any,
         filters: BaseFilterParams
 ) -> List[Any]:
-    columns: Dict[str, Column] = dict(inspect(model_class).columns)
     relationships: Dict[str, Relationship] = dict(inspect(model_class).relationships)
 
     res = []
     filter_fields = _model_dump(filters, exclude_none=True)
 
     for field_name, value in filter_fields.items():
         if "__" in field_name:
@@ -113,18 +112,14 @@
                 model_class=model_class,
                 search_query=value,
                 searchable_fields=filters.Settings.searchable_fields
             )
             if criteria is not None:
                 res.append(criteria)
 
-        elif field_name in columns:
-            model_field = getattr(model_class, field_name)
-            res.append(getattr(model_field, operator)(value))
-
         elif (
                 isinstance(value, dict) and
                 field_name in relationships and
                 relationships[field_name]
         ):
 
             is_many = relationships[field_name].uselist
@@ -139,14 +134,18 @@
                     model_field.any(and_(*nested_orm_filters))
                 )
             else:
                 res.append(
                     model_field.has(and_(*nested_orm_filters))
                 )
 
+        elif hasattr(model_class, field_name):
+            model_field = getattr(model_class, field_name)
+            res.append(getattr(model_field, operator)(value))
+
         elif value:
             raise ValueError(
                 f"Invalid {model_class.__name__} Field - {field_name}"
             )
 
     return res
```

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/ordering.py` & `fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/ordering.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/sqlalchemy/pagination.py` & `fastapi_query-0.1a1/fastapi_query/ext/sqlalchemy/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/tortoise/filtering.py` & `fastapi_query-0.1a1/fastapi_query/ext/tortoise/filtering.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/tortoise/ordering.py` & `fastapi_query-0.1a1/fastapi_query/ext/tortoise/ordering.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/tortoise/pagination.py` & `fastapi_query-0.1a1/fastapi_query/ext/tortoise/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/ext/tortoise/utils.py` & `fastapi_query-0.1a1/fastapi_query/ext/tortoise/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/filtering/base_params.py` & `fastapi_query-0.1a1/fastapi_query/filtering/base_params.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/filtering/deps.py` & `fastapi_query-0.1a1/fastapi_query/filtering/deps.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/filtering/utils.py` & `fastapi_query-0.1a1/fastapi_query/filtering/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/pagination/utils.py` & `fastapi_query-0.1a1/fastapi_query/pagination/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/fastapi_query/utils.py` & `fastapi_query-0.1a1/fastapi_query/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_query-0.1a0/pyproject.toml` & `fastapi_query-0.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fastapi-query"
-version = "0.1-alpha"
+version = "0.1-alpha1"
 description = "FastAPI Library for Filtering, Ordering, and Pagination"
 authors = ["Lazar Stamenkovic <lazarstamenkovic96@hotmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/lazarst96/fastapi-query"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `fastapi_query-0.1a0/PKG-INFO` & `fastapi_query-0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-query
-Version: 0.1a0
+Version: 0.1a1
 Summary: FastAPI Library for Filtering, Ordering, and Pagination
 Home-page: https://github.com/lazarst96/fastapi-query
 License: MIT
 Author: Lazar Stamenkovic
 Author-email: lazarstamenkovic96@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
```

