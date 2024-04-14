# Comparing `tmp/sql_athame-0.4.0a1.tar.gz` & `tmp/sql_athame-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a1.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a2.tar", max compression
```

## Comparing `sql_athame-0.4.0a1.tar` & `sql_athame-0.4.0a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/LICENSE
--rw-r--r--   0        0        0    12086 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/README.md
--rw-r--r--   0        0        0      751 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/__init__.py
--rw-r--r--   0        0        0    10350 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/base.py
--rw-r--r--   0        0        0    17370 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      743 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/py.typed
--rw-r--r--   0        0        0     1305 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      412 2024-02-14 21:35:37.710590 sql_athame-0.4.0a1/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/LICENSE
+-rw-r--r--   0        0        0    12086 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/README.md
+-rw-r--r--   0        0        0      751 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10350 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/base.py
+-rw-r--r--   0        0        0    19697 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      743 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/py.typed
+-rw-r--r--   0        0        0     1305 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      412 2024-04-14 23:40:40.982872 sql_athame-0.4.0a2/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a2/PKG-INFO
```

### Comparing `sql_athame-0.4.0a1/LICENSE` & `sql_athame-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a1/README.md` & `sql_athame-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a1/pyproject.toml` & `sql_athame-0.4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-1"
+version = "0.4.0-alpha-2"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a1/sql_athame/base.py` & `sql_athame-0.4.0a2/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a1/sql_athame/dataclasses.py` & `sql_athame-0.4.0a2/sql_athame/dataclasses.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,20 +96,32 @@
 
 
 class ModelBase(Mapping[str, Any]):
     _column_info: Optional[Dict[str, ColumnInfo]]
     _cache: Dict[tuple, Any]
     table_name: str
     primary_key_names: Tuple[str, ...]
+    array_safe_insert: bool
 
     def __init_subclass__(
-        cls, *, table_name: str, primary_key: Union[FieldNames, str] = (), **kwargs: Any
+        cls,
+        *,
+        table_name: str,
+        primary_key: Union[FieldNames, str] = (),
+        insert_multiple_mode: str = "unnest",
+        **kwargs: Any,
     ):
         cls._cache = {}
         cls.table_name = table_name
+        if insert_multiple_mode == "array_safe":
+            cls.array_safe_insert = True
+        elif insert_multiple_mode == "unnest":
+            cls.array_safe_insert = False
+        else:
+            raise ValueError("Unknown `insert_multiple_mode`")
         if isinstance(primary_key, str):
             cls.primary_key_names = (primary_key,)
         else:
             cls.primary_key_names = tuple(primary_key)
 
     @classmethod
     def _fields(cls):
@@ -403,28 +415,78 @@
             unnest=sql.unnest(
                 (row.field_values() for row in rows),
                 (cls.column_info(name).type for name in cls.field_names()),
             ),
         )
 
     @classmethod
-    async def insert_multiple(
+    def insert_multiple_array_safe_sql(cls: Type[T], rows: Iterable[T]) -> Fragment:
+        return sql(
+            "INSERT INTO {table} ({fields}) VALUES {values}",
+            table=cls.table_name_sql(),
+            fields=sql.list(cls.field_names_sql()),
+            values=sql.list(
+                sql("({})", sql.list(row.field_values_sql(default_none=True)))
+                for row in rows
+            ),
+        )
+
+    @classmethod
+    async def insert_multiple_unnest(
         cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         return await connection_or_pool.execute(*cls.insert_multiple_sql(rows))
 
     @classmethod
-    async def upsert_multiple(
+    async def insert_multiple_array_safe(
+        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+    ) -> str:
+        for chunk in chunked(rows, 100):
+            last = await connection_or_pool.execute(
+                *cls.insert_multiple_array_safe_sql(chunk)
+            )
+        return last
+
+    @classmethod
+    async def insert_multiple(
+        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+    ) -> str:
+        if cls.array_safe_insert:
+            return await cls.insert_multiple_array_safe(connection_or_pool, rows)
+        else:
+            return await cls.insert_multiple_unnest(connection_or_pool, rows)
+
+    @classmethod
+    async def upsert_multiple_unnest(
         cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         return await connection_or_pool.execute(
             *cls.upsert_sql(cls.insert_multiple_sql(rows))
         )
 
     @classmethod
+    async def upsert_multiple_array_safe(
+        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+    ) -> str:
+        for chunk in chunked(rows, 100):
+            last = await connection_or_pool.execute(
+                *cls.upsert_sql(cls.insert_multiple_array_safe_sql(chunk))
+            )
+        return last
+
+    @classmethod
+    async def upsert_multiple(
+        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+    ) -> str:
+        if cls.array_safe_insert:
+            return await cls.upsert_multiple_array_safe(connection_or_pool, rows)
+        else:
+            return await cls.upsert_multiple_unnest(connection_or_pool, rows)
+
+    @classmethod
     def _get_equal_ignoring_fn(
         cls: Type[T], ignore: FieldNamesSet = ()
     ) -> Callable[[T, T], bool]:
         env: Dict[str, Any] = dict()
         func = ["def equal_ignoring(a, b):"]
         for f in cls._fields():
             if f.name not in ignore:
@@ -526,7 +588,12 @@
             await cls.upsert_multiple(
                 connection, (*created, *(t[1] for t in updated_triples))
             )
         if deleted:
             await cls.delete_multiple(connection, deleted)
 
         return created, updated_triples, deleted
+
+
+def chunked(lst, n):
+    for i in range(0, len(lst), n):
+        yield lst[i : i + n]
```

### Comparing `sql_athame-0.4.0a1/sql_athame/escape.py` & `sql_athame-0.4.0a2/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a1/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a2/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a1/PKG-INFO` & `sql_athame-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

