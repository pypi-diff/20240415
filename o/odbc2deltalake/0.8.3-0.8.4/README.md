# Comparing `tmp/odbc2deltalake-0.8.3.tar.gz` & `tmp/odbc2deltalake-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.3.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.4.tar", max compression
```

## Comparing `odbc2deltalake-0.8.3.tar` & `odbc2deltalake-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1081 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/README.md
--rw-r--r--   0        0        0      126 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    42665 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0     3714 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/delta_logger.py
--rw-r--r--   0        0        0       38 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5458 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     7195 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1961 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     4908 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-04-08 12:35:24.154336 odbc2deltalake-0.8.3/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     4757 2024-04-08 12:35:24.158336 odbc2deltalake-0.8.3/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-04-08 12:35:24.158336 odbc2deltalake-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/README.md
+-rw-r--r--   0        0        0      126 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    42950 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0     3809 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/delta_logger.py
+-rw-r--r--   0        0        0       38 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5458 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     7195 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1961 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4932 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1373 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.4/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.3/LICENSE` & `odbc2deltalake-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/README.md` & `odbc2deltalake-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.4/odbc2deltalake/db_to_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,17 +210,26 @@
         json.dumps(
             [c.model_dump() if is_pydantic_2 else c.dict() for c in cols], indent=4
         )
     )
     if source.local_delta_table_exists(
         destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
     ):
-        last_version_pk = source.get_local_delta_ops(
-            destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
-        ).version()
+        try:
+            last_version_pk = source.get_local_delta_ops(
+                destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
+            ).version()
+        except Exception as e:
+            import traceback
+
+            dest_logger.warning(
+                f"Could not get last version: {e}",
+                error_trackback=traceback.format_exc(),
+            )
+            last_version_pk = None
     else:
         last_version_pk = None
     lock_file_path = destination / "meta/lock.txt"
 
     try:
         if (
             lock_file_path.exists()
```

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/delta_logger.py` & `odbc2deltalake-0.8.4/odbc2deltalake/delta_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,25 @@
     def warning(
         self,
         message: str,
         *,
         load: str | None = None,
         sql: str | None = None,
         sub_load: str | None = None,
+        error_trackback: str | None = None,
     ):
         self._pending_logs.append(
             LogMessage(
                 message=message,
                 type="warn",
                 date=datetime.now(tz=timezone.utc),
                 load=load,
                 sql=sql,
                 sub_load=sub_load,
+                error_trackback=error_trackback,
             )
         )
         if self.base_logger:
             self.base_logger.warning(
                 message if isinstance(message, str) else json.dumps(message)
             )
         if len(self._pending_logs) > 10:
```

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.4/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.4/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.4/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.4/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.4/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.4/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.4/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/query.py` & `odbc2deltalake-0.8.4/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.4/odbc2deltalake/reader/odbc_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.4/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.4/odbc2deltalake/reader/spark_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return [row.asDict() for row in rows]
 
     def local_delta_table_exists(
         self, delta_path: Destination, extended_check=False
     ) -> bool:
         from delta import DeltaTable
 
-        if DeltaTable.isDeltaTable(self.spark, str(delta_path)):
+        if delta_path.exists() and DeltaTable.isDeltaTable(self.spark, str(delta_path)):
             if extended_check:
                 return (
                     len(
                         self.spark.sql(
                             f"select * from delta.`{str(delta_path)}` limit 0"
                         ).columns
                     )
```

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.4/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.4/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.4/odbc2deltalake/write_utils/restore_pk.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.3/pyproject.toml` & `odbc2deltalake-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.3"
+version = "0.8.4"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `odbc2deltalake-0.8.3/PKG-INFO` & `odbc2deltalake-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

