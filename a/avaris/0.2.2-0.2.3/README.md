# Comparing `tmp/avaris-0.2.2.tar.gz` & `tmp/avaris-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avaris-0.2.2.tar", max compression
+gzip compressed data, was "avaris-0.2.3.tar", max compression
```

## Comparing `avaris-0.2.2.tar` & `avaris-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-15 12:28:10.078377 avaris-0.2.2/LICENSE
--rw-r--r--   0        0        0     7714 2024-04-15 12:28:10.078377 avaris-0.2.2/README.md
--rw-r--r--   0        0        0     1107 2024-04-15 12:28:10.078377 avaris-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      656 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/__init__.py
--rw-r--r--   0        0        0      187 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/__main__.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/api/__init__.py
--rw-r--r--   0        0        0     4572 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/api/models.py
--rw-r--r--   0        0        0      540 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/api/output.py
--rw-r--r--   0        0        0     3425 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/cli.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/__init__.py
--rw-r--r--   0        0        0     2051 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/config_loader.py
--rw-r--r--   0        0        0     2746 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/config_manager.py
--rw-r--r--   0        0        0      468 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/error.py
--rw-r--r--   0        0        0      961 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/exception.py
--rw-r--r--   0        0        0      633 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/config/value_parser.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/data/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/data/datamanager.py
--rw-r--r--   0        0        0      383 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/data/models.py
--rw-r--r--   0        0        0      341 2024-04-15 12:28:10.078377 avaris-0.2.2/src/avaris/data/s3.py
--rw-r--r--   0        0        0      197 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/data/shipper.py
--rw-r--r--   0        0        0     8287 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/data/sql.py
--rw-r--r--   0        0        0     2444 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/defaults.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/engine/__init__.py
--rw-r--r--   0        0        0      114 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/engine/commands.py
--rw-r--r--   0        0        0     4099 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/engine/engine.py
--rw-r--r--   0        0        0      446 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/engine/listener.py
--rw-r--r--   0        0        0     7121 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/engine/start.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/__init__.py
--rw-r--r--   0        0        0      923 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/apicall.py
--rw-r--r--   0        0        0     1553 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/endpoint.py
--rw-r--r--   0        0        0     5301 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/executor.py
--rw-r--r--   0        0        0     2458 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/fetch_file.py
--rw-r--r--   0        0        0     3011 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/github_release.py
--rw-r--r--   0        0        0     2511 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/http_get.py
--rw-r--r--   0        0        0      970 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/executor/shell.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/handler/__init__.py
--rw-r--r--   0        0        0      688 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/handler/handler.py
--rw-r--r--   0        0        0      762 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/manage.py
--rw-r--r--   0        0        0      132 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/registry.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/service/__init__.py
--rw-r--r--   0        0        0      411 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/service/dataqueue.py
--rw-r--r--   0        0        0     7111 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/service/datasource.py
--rw-r--r--   0        0        0      312 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/service/service.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/__init__.py
--rw-r--r--   0        0        0     1073 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/plugins.py
--rw-r--r--   0        0        0     1131 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/task_registry.py
--rw-r--r--   0        0        0     7105 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/taskmaster.py
--rw-r--r--   0        0        0     3782 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/taskmaster_apscheduler.py
--rw-r--r--   0        0        0     1346 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/task/taskmaster_celery.py
--rw-r--r--   0        0        0        0 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/utils/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/utils/auth.py
--rw-r--r--   0        0        0     2188 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/utils/logging.py
--rw-r--r--   0        0        0      529 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/utils/management.py
--rw-r--r--   0        0        0     7339 2024-04-15 12:28:10.082377 avaris-0.2.2/src/avaris/utils/parse.py
--rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 avaris-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 16:18:55.103050 avaris-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7714 2024-04-15 16:18:55.103050 avaris-0.2.3/README.md
+-rw-r--r--   0        0        0     1107 2024-04-15 16:18:55.103050 avaris-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/api/__init__.py
+-rw-r--r--   0        0        0     4572 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/api/models.py
+-rw-r--r--   0        0        0      540 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/api/output.py
+-rw-r--r--   0        0        0     3425 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/cli.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/__init__.py
+-rw-r--r--   0        0        0     2051 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/config_loader.py
+-rw-r--r--   0        0        0     2746 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/config_manager.py
+-rw-r--r--   0        0        0      468 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/error.py
+-rw-r--r--   0        0        0      961 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/exception.py
+-rw-r--r--   0        0        0      633 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/config/value_parser.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.103050 avaris-0.2.3/src/avaris/data/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/data/datamanager.py
+-rw-r--r--   0        0        0      383 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/data/models.py
+-rw-r--r--   0        0        0      341 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/data/s3.py
+-rw-r--r--   0        0        0      197 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/data/shipper.py
+-rw-r--r--   0        0        0     8776 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/data/sql.py
+-rw-r--r--   0        0        0     2444 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/engine/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/engine/commands.py
+-rw-r--r--   0        0        0     4099 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/engine/engine.py
+-rw-r--r--   0        0        0      446 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/engine/listener.py
+-rw-r--r--   0        0        0     7121 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/engine/start.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/apicall.py
+-rw-r--r--   0        0        0     1553 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/endpoint.py
+-rw-r--r--   0        0        0     5301 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/executor.py
+-rw-r--r--   0        0        0     2458 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/fetch_file.py
+-rw-r--r--   0        0        0     3011 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/github_release.py
+-rw-r--r--   0        0        0     2511 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/http_get.py
+-rw-r--r--   0        0        0      970 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/executor/shell.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/handler/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/handler/handler.py
+-rw-r--r--   0        0        0      762 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/manage.py
+-rw-r--r--   0        0        0      132 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/registry.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/service/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/service/dataqueue.py
+-rw-r--r--   0        0        0     7111 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/service/datasource.py
+-rw-r--r--   0        0        0      312 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/plugins.py
+-rw-r--r--   0        0        0     1131 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/task_registry.py
+-rw-r--r--   0        0        0     7105 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/taskmaster.py
+-rw-r--r--   0        0        0     3713 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/taskmaster_apscheduler.py
+-rw-r--r--   0        0        0     1346 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/task/taskmaster_celery.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/utils/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/utils/auth.py
+-rw-r--r--   0        0        0     2188 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/utils/logging.py
+-rw-r--r--   0        0        0      529 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/utils/management.py
+-rw-r--r--   0        0        0     7339 2024-04-15 16:18:55.107050 avaris-0.2.3/src/avaris/utils/parse.py
+-rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 avaris-0.2.3/PKG-INFO
```

### Comparing `avaris-0.2.2/LICENSE` & `avaris-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/README.md` & `avaris-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/pyproject.toml` & `avaris-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avaris"
-version = "0.2.2"
+version = "0.2.3"
 description = "Task execution engine for data management and monitoring"
 authors = ["dennis <denngohis@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "avaris", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `avaris-0.2.2/src/avaris/__init__.py` & `avaris-0.2.3/src/avaris/__init__.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/api/models.py` & `avaris-0.2.3/src/avaris/api/models.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/api/output.py` & `avaris-0.2.3/src/avaris/api/output.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/cli.py` & `avaris-0.2.3/src/avaris/cli.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/config/config_loader.py` & `avaris-0.2.3/src/avaris/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/config/config_manager.py` & `avaris-0.2.3/src/avaris/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/config/exception.py` & `avaris-0.2.3/src/avaris/config/exception.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/config/value_parser.py` & `avaris-0.2.3/src/avaris/config/value_parser.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/data/datamanager.py` & `avaris-0.2.3/src/avaris/data/datamanager.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/data/sql.py` & `avaris-0.2.3/src/avaris/data/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,53 +84,62 @@
                 timestamp=result.timestamp,
                 result=result.result,
             )
             for result in sql_results
         ]
         return execution_results
 
-    async def add_task_result(self, execution_result: ExecutionResult):
+
+    async def add_task_result(self, execution_result: ExecutionResult) -> bool:
         async with self.SessionLocal() as session:
             try:
                 db_task_result = SQLExecutionResult(
                     id=execution_result.id,
                     name=execution_result.name,
                     task=execution_result.task,
                     result=execution_result.result,
                     timestamp=execution_result.timestamp,
                 )
                 session.add(db_task_result)
                 await session.commit()
                 self.logger.info(
                     f"Task result for {execution_result.task} added to the SQL database"
                 )
+                return True
             except IntegrityError:
                 await session.rollback()  # Roll back the failed transaction
                 self.logger.info(
                     f"Found existing {execution_result.task}[{execution_result.id}], updating record."
                 )
-                # Update the existing record
-                await session.execute(
-                    update(SQLExecutionResult)
-                    .where(SQLExecutionResult.id == execution_result.id)
-                    .values(
-                        name=execution_result.name,
-                        task=execution_result.task,
-                        result=execution_result.result,
-                        timestamp=execution_result.timestamp,
+                try:
+                    # Update the existing record
+                    await session.execute(
+                        update(SQLExecutionResult)
+                        .where(SQLExecutionResult.id == execution_result.id)
+                        .values(
+                            name=execution_result.name,
+                            task=execution_result.task,
+                            result=execution_result.result,
+                            timestamp=execution_result.timestamp,
+                        )
                     )
-                )
-                await session.commit()
+                    await session.commit()
+                    return True
+                except SQLAlchemyError as e:
+                    self.logger.error(
+                        f"Failed to update task result for {execution_result.task} in the SQL database: {e}"
+                    )
+                    await session.rollback()  # Ensure to roll back on update failure
+                    return False
             except SQLAlchemyError as e:
-                await session.rollback()  # Ensure to roll back on other SQL errors
                 self.logger.error(
-                    f"Failed to add or update task result for {execution_result.task} in the SQL database: {e}"
+                    f"Failed to add task result for {execution_result.task} in the SQL database: {e}"
                 )
-
-
+                await session.rollback()  # Ensure to roll back on other SQL errors
+                return False
 
 
     async def get_filtered_tasks(self, **kwargs):
         async with self.SessionLocal() as session:
             query = select(SQLExecutionResult)
 
             conditions = []
```

### Comparing `avaris-0.2.2/src/avaris/defaults.py` & `avaris-0.2.3/src/avaris/defaults.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/engine/engine.py` & `avaris-0.2.3/src/avaris/engine/engine.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/engine/start.py` & `avaris-0.2.3/src/avaris/engine/start.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/apicall.py` & `avaris-0.2.3/src/avaris/executor/apicall.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/endpoint.py` & `avaris-0.2.3/src/avaris/executor/endpoint.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/executor.py` & `avaris-0.2.3/src/avaris/executor/executor.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/fetch_file.py` & `avaris-0.2.3/src/avaris/executor/fetch_file.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/github_release.py` & `avaris-0.2.3/src/avaris/executor/github_release.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/http_get.py` & `avaris-0.2.3/src/avaris/executor/http_get.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/executor/shell.py` & `avaris-0.2.3/src/avaris/executor/shell.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/manage.py` & `avaris-0.2.3/src/avaris/manage.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/service/datasource.py` & `avaris-0.2.3/src/avaris/service/datasource.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/task/plugins.py` & `avaris-0.2.3/src/avaris/task/plugins.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/task/task_registry.py` & `avaris-0.2.3/src/avaris/task/task_registry.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/task/taskmaster.py` & `avaris-0.2.3/src/avaris/task/taskmaster.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/task/taskmaster_apscheduler.py` & `avaris-0.2.3/src/avaris/task/taskmaster_apscheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 from logging import Logger
 from typing import Callable, Dict, Type
 
 import pytz
 from apscheduler.executors.asyncio import AsyncIOExecutor
 from apscheduler.executors.pool import ThreadPoolExecutor
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
-from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.triggers.cron import CronTrigger
 
 from avaris.executor.executor import TaskExecutor
 from avaris.task.taskmaster import TaskMaster
 from avaris.utils.logging import get_logger
 
 
 class APSchedulerTaskMaster(TaskMaster):
-    scheduler: BackgroundScheduler
+    scheduler: AsyncIOScheduler
 
     def __init__(
         self,
         task_registry: Dict[str, Type[TaskExecutor]],
         logger: Logger = None,
         use_daemon=False,
         result_handler: Callable = None,
@@ -34,15 +33,15 @@
         """Create and return an AsyncIOScheduler instance."""
         executors = {
             "default": ThreadPoolExecutor(10),  # For synchronous tasks
             "asyncio": AsyncIOExecutor(),  # For asynchronous tasks
         }
         job_defaults = {
             "coalesce": False,
-            "max_instances": 3,
+            "max_instances": 1,
         }
         scheduler = AsyncIOScheduler(
             executors=executors, job_defaults=job_defaults, timezone="UTC"
         )
         return scheduler
 
     def start_scheduler(self):
```

### Comparing `avaris-0.2.2/src/avaris/task/taskmaster_celery.py` & `avaris-0.2.3/src/avaris/task/taskmaster_celery.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/utils/auth.py` & `avaris-0.2.3/src/avaris/utils/auth.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/utils/logging.py` & `avaris-0.2.3/src/avaris/utils/logging.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/utils/management.py` & `avaris-0.2.3/src/avaris/utils/management.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/src/avaris/utils/parse.py` & `avaris-0.2.3/src/avaris/utils/parse.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.2/PKG-INFO` & `avaris-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avaris
-Version: 0.2.2
+Version: 0.2.3
 Summary: Task execution engine for data management and monitoring
 License: Apache-2.0
 Author: dennis
 Author-email: denngohis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

