# Comparing `tmp/avaris-0.2.0.tar.gz` & `tmp/avaris-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avaris-0.2.0.tar", max compression
+gzip compressed data, was "avaris-0.2.1.tar", max compression
```

## Comparing `avaris-0.2.0.tar` & `avaris-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-11 14:16:41.287572 avaris-0.2.0/LICENSE
--rw-r--r--   0        0        0     5559 2024-04-11 14:16:41.287572 avaris-0.2.0/README.md
--rw-r--r--   0        0        0     1107 2024-04-11 14:16:41.287572 avaris-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      656 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/__init__.py
--rw-r--r--   0        0        0      187 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/__main__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/api/__init__.py
--rw-r--r--   0        0        0     4572 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/api/models.py
--rw-r--r--   0        0        0      540 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/api/output.py
--rw-r--r--   0        0        0     3425 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/cli.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/__init__.py
--rw-r--r--   0        0        0     2051 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/config_loader.py
--rw-r--r--   0        0        0     2746 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/config_manager.py
--rw-r--r--   0        0        0      468 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/error.py
--rw-r--r--   0        0        0      961 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/exception.py
--rw-r--r--   0        0        0      633 2024-04-11 14:16:41.287572 avaris-0.2.0/src/avaris/config/value_parser.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/datamanager.py
--rw-r--r--   0        0        0      383 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/models.py
--rw-r--r--   0        0        0      341 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/s3.py
--rw-r--r--   0        0        0      197 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/shipper.py
--rw-r--r--   0        0        0     7665 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/data/sql.py
--rw-r--r--   0        0        0     2444 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/defaults.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/engine/__init__.py
--rw-r--r--   0        0        0      114 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/engine/commands.py
--rw-r--r--   0        0        0     4099 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/engine/engine.py
--rw-r--r--   0        0        0      446 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/engine/listener.py
--rw-r--r--   0        0        0     7121 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/engine/start.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/__init__.py
--rw-r--r--   0        0        0      923 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/apicall.py
--rw-r--r--   0        0        0     1553 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/endpoint.py
--rw-r--r--   0        0        0     5301 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/executor.py
--rw-r--r--   0        0        0     2458 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/fetch_file.py
--rw-r--r--   0        0        0     2805 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/github_release.py
--rw-r--r--   0        0        0     2511 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/http_get.py
--rw-r--r--   0        0        0      970 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/executor/shell.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/handler/__init__.py
--rw-r--r--   0        0        0      688 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/handler/handler.py
--rw-r--r--   0        0        0      762 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/manage.py
--rw-r--r--   0        0        0      132 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/registry.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/service/__init__.py
--rw-r--r--   0        0        0      411 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/service/dataqueue.py
--rw-r--r--   0        0        0     7018 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/service/datasource.py
--rw-r--r--   0        0        0      312 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/service/service.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/__init__.py
--rw-r--r--   0        0        0     1073 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/plugins.py
--rw-r--r--   0        0        0     1131 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/task_registry.py
--rw-r--r--   0        0        0     7105 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/taskmaster.py
--rw-r--r--   0        0        0     3782 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/taskmaster_apscheduler.py
--rw-r--r--   0        0        0     1346 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/task/taskmaster_celery.py
--rw-r--r--   0        0        0        0 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/utils/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/utils/auth.py
--rw-r--r--   0        0        0     2188 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/utils/logging.py
--rw-r--r--   0        0        0      529 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/utils/management.py
--rw-r--r--   0        0        0     7339 2024-04-11 14:16:41.291572 avaris-0.2.0/src/avaris/utils/parse.py
--rw-r--r--   0        0        0     6921 1970-01-01 00:00:00.000000 avaris-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 12:08:38.722117 avaris-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7714 2024-04-15 12:08:38.722117 avaris-0.2.1/README.md
+-rw-r--r--   0        0        0     1107 2024-04-15 12:08:38.726117 avaris-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/api/__init__.py
+-rw-r--r--   0        0        0     4572 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/api/models.py
+-rw-r--r--   0        0        0      540 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/api/output.py
+-rw-r--r--   0        0        0     3425 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/cli.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/__init__.py
+-rw-r--r--   0        0        0     2051 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/config_loader.py
+-rw-r--r--   0        0        0     2746 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/config_manager.py
+-rw-r--r--   0        0        0      468 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/error.py
+-rw-r--r--   0        0        0      961 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/exception.py
+-rw-r--r--   0        0        0      633 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/config/value_parser.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/datamanager.py
+-rw-r--r--   0        0        0      383 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/models.py
+-rw-r--r--   0        0        0      341 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/s3.py
+-rw-r--r--   0        0        0      197 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/shipper.py
+-rw-r--r--   0        0        0     7755 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/data/sql.py
+-rw-r--r--   0        0        0     2444 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/engine/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/engine/commands.py
+-rw-r--r--   0        0        0     4099 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/engine/engine.py
+-rw-r--r--   0        0        0      446 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/engine/listener.py
+-rw-r--r--   0        0        0     7121 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/engine/start.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/apicall.py
+-rw-r--r--   0        0        0     1553 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/endpoint.py
+-rw-r--r--   0        0        0     5301 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/executor.py
+-rw-r--r--   0        0        0     2458 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/fetch_file.py
+-rw-r--r--   0        0        0     3011 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/github_release.py
+-rw-r--r--   0        0        0     2511 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/http_get.py
+-rw-r--r--   0        0        0      970 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/executor/shell.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/handler/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/handler/handler.py
+-rw-r--r--   0        0        0      762 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/manage.py
+-rw-r--r--   0        0        0      132 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/registry.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/service/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-15 12:08:38.726117 avaris-0.2.1/src/avaris/service/dataqueue.py
+-rw-r--r--   0        0        0     7111 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/service/datasource.py
+-rw-r--r--   0        0        0      312 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/plugins.py
+-rw-r--r--   0        0        0     1131 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/task_registry.py
+-rw-r--r--   0        0        0     7105 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/taskmaster.py
+-rw-r--r--   0        0        0     3782 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/taskmaster_apscheduler.py
+-rw-r--r--   0        0        0     1346 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/task/taskmaster_celery.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/utils/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/utils/auth.py
+-rw-r--r--   0        0        0     2188 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/utils/logging.py
+-rw-r--r--   0        0        0      529 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/utils/management.py
+-rw-r--r--   0        0        0     7339 2024-04-15 12:08:38.730117 avaris-0.2.1/src/avaris/utils/parse.py
+-rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 avaris-0.2.1/PKG-INFO
```

### Comparing `avaris-0.2.0/LICENSE` & `avaris-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/README.md` & `avaris-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -116,14 +116,86 @@
         # Implementation of your task
         try:
             return {}
         except Exception as e:
             self.logger.error(f"An error occurred while executing task: {e}")
             raise
 ```
+## Passing variables from the environment
+
+For a task parameter set that looks like this
+```python
+class HTTPGetParameters(BaseParameter):
+    __NAME__ = 'http_get'
+    url: str
+    username: Optional[str] = None
+    password: Optional[SecretStr] = None
+    response_format: Literal['json', 'text',
+                             'binary'] = 'text'
+```
+You can now instruct Avaris to get the secret from the environment directly like so.
+```yaml
+compendium:
+  name: get request
+  tasks:
+    - name: get example.com
+      schedule: "* * * * *"
+      executor:
+        task: http_get
+        parameters:
+          username: ${{ env.USERNAME }}
+          password: ${{ env.PASSWORD }}
+          url: https://example.com
+          response_format: text
+```
+
+Another way to specify secrets (legacy method) would be like so:
+```python
+from avaris.executor.executor import TaskExecutor
+from avaris.api.models import BaseParameter
+from avaris.task.task_registry import register_task_executor
+
+"""Define your parameter model with its identifier"""
+class MyParameters(BaseParameter):
+    __NAME__ = 'my_task_identifier_in_yaml'
+    my_param: str = ""
+
+@register_task_executor(MyParameters)
+class MyTask(TaskExecutor[MyParameters]) :
+
+    async def execute(self) -> dict:
+        try:
+            self.logger.info("Hello World!")
+            # Fetch secrets if any were mentioned explicity from the config. (will also load from env)
+            secrets = await self.load_secrets()
+            access_parameters_this_way = self.parameters.my_param
+            my_secret = secrets.get("MY_SECRET", None)
+            return {'my_key': self.parameters.my_param}
+        except Exception as e:
+            self.logger.error(
+                f"Error : {e}")
+            return {'error': str(e)}
+```
+And then in YAML you could instruct Avaris this way:
+```yaml
+compendium:
+  name: latest version jobs
+  tasks:
+    -  # more tasks...
+    - name: Example
+      schedule: "* * * * *"
+      executor:
+        task: my_task_identifier_in_yaml # task identifier
+        parameters:
+          my_param: "123"
+        secrets:
+          MY_SECRET: # implicity loading from env
+```
+
+
 
 # Default Configurations Summary
 
 ## Directories
 
 - **Home Directory**: `~/.avaris`
 - **Working Directory**: `$WORKINGDIR` or fallback to `~/.avaris` or current working directory
```

### Comparing `avaris-0.2.0/pyproject.toml` & `avaris-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avaris"
-version = "0.2.0"
+version = "0.2.1"
 description = "Task execution engine for data management and monitoring"
 authors = ["dennis <denngohis@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "avaris", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `avaris-0.2.0/src/avaris/__init__.py` & `avaris-0.2.1/src/avaris/__init__.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/api/models.py` & `avaris-0.2.1/src/avaris/api/models.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/api/output.py` & `avaris-0.2.1/src/avaris/api/output.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/cli.py` & `avaris-0.2.1/src/avaris/cli.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/config/config_loader.py` & `avaris-0.2.1/src/avaris/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/config/config_manager.py` & `avaris-0.2.1/src/avaris/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/config/exception.py` & `avaris-0.2.1/src/avaris/config/exception.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/config/value_parser.py` & `avaris-0.2.1/src/avaris/config/value_parser.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/data/datamanager.py` & `avaris-0.2.1/src/avaris/data/datamanager.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/data/sql.py` & `avaris-0.2.1/src/avaris/data/sql.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,38 +122,41 @@
                 await session.commit()
             except SQLAlchemyError as e:
                 await session.rollback()  # Ensure to roll back on other SQL errors
                 self.logger.error(
                     f"Failed to add or update task result for {execution_result.task} in the SQL database: {e}"
                 )
 
+
     async def get_filtered_tasks(self, **kwargs):
         async with self.SessionLocal() as session:
             query = select(SQLExecutionResult)
 
             conditions = []
             for key, value in kwargs.items():
                 if hasattr(SQLExecutionResult, key) and value is not None:
-                    # Use the '==' operator for most fields
-                    condition = getattr(SQLExecutionResult, key) == value
+                    if isinstance(value, list) and value:  # Check if the value is a non-empty list
+                        condition = getattr(SQLExecutionResult, key).in_(value)
+                    else:
+                        condition = getattr(SQLExecutionResult, key) == value
 
-                    # Special handling for date range queries
                     if key == "start_date":
                         condition = SQLExecutionResult.timestamp >= value
                     elif key == "end_date":
                         condition = SQLExecutionResult.timestamp <= value
 
                     conditions.append(condition)
 
             if conditions:
                 query = query.filter(and_(*conditions))
 
             results = await session.execute(query)
             return results.scalars().all()
 
+
     async def get_task_result(self, job_id: str):
         try:
             async with self.SessionLocal() as session:
                 query = select(SQLExecutionResult).filter(
                     SQLExecutionResult.id == job_id
                 )
                 result = await session.execute(query)
```

### Comparing `avaris-0.2.0/src/avaris/defaults.py` & `avaris-0.2.1/src/avaris/defaults.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/engine/engine.py` & `avaris-0.2.1/src/avaris/engine/engine.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/engine/start.py` & `avaris-0.2.1/src/avaris/engine/start.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/apicall.py` & `avaris-0.2.1/src/avaris/executor/apicall.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/endpoint.py` & `avaris-0.2.1/src/avaris/executor/endpoint.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/executor.py` & `avaris-0.2.1/src/avaris/executor/executor.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/fetch_file.py` & `avaris-0.2.1/src/avaris/executor/fetch_file.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/github_release.py` & `avaris-0.2.1/src/avaris/executor/github_release.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 
 
 class GitHubReleaseRequestParameters(BaseParameter):
     __NAME__ = "http_get_github_release"
     api_url: HttpUrl
     username: Optional[str] = None
     password: Optional[SecretStr] = None
+    github_token: Optional[SecretStr] = None
 
 
 @register_task_executor(GitHubReleaseRequestParameters)
 class GitHubReleaseExecutor(TaskExecutor[GitHubReleaseRequestParameters]):
+
     async def execute(self) -> dict:
         try:
-            secrets = await self.load_secrets()
-            github_token = secrets.get("GITHUB_TOKEN", None)
+            # Try to load secret from environment or explicitly
+            github_token = None
+            if self.parameters.github_token:
+                github_token = self.parameters.github_token.get_secret_value()
             headers = {"Accept": "application/vnd.github.v3+json"}
 
             url = self.parameters.api_url.unicode_string()
             async with httpx.AsyncClient() as client:
                 if github_token:
-                    headers[
-                        "Authorization"] = f"token {github_token.get_secret_value()}"
+                    headers["Authorization"] = f"token {github_token}"
                     response = await client.get(url, headers=headers)
                 elif self.parameters.username and self.parameters.password:
                     auth = (self.parameters.username,
                             self.parameters.password.get_secret_value())
                     response = await client.get(url,
                                                 headers=headers,
                                                 auth=auth)
@@ -57,9 +60,11 @@
 
             else:
                 self.logger.error(
                     f"Failed to fetch {self.parameters.api_url}: Status {response.status_code}"
                 )
                 return {"error": f"HTTP Error: Status {response.status_code}"}
         except Exception as e:
-            self.logger.error(f"Exception during fetch: {str(e)}")
-            raise
+            self.logger.error(
+                f"Exception during fetch '{self.parameters.api_url}': {str(e)}"
+            )
+            return {"error": f"Exception: {str(e)}"}
```

### Comparing `avaris-0.2.0/src/avaris/executor/http_get.py` & `avaris-0.2.1/src/avaris/executor/http_get.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/executor/shell.py` & `avaris-0.2.1/src/avaris/executor/shell.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/handler/handler.py` & `avaris-0.2.1/src/avaris/handler/handler.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/manage.py` & `avaris-0.2.1/src/avaris/manage.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/service/datasource.py` & `avaris-0.2.1/src/avaris/service/datasource.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from logging import Logger
 from avaris.service.service import Service
 from fastapi import FastAPI, Request, Depends
 from uvicorn import Config, Server
 from avaris.data.datamanager import DataManager
 from avaris.utils.logging import get_logger
 import multiprocessing
-from typing import List
+from typing import List, Optional
 from fastapi import Query
 from avaris.api.models import ExecutionResult, ListenerData
 from avaris.utils.parse import generate_task_id
 from avaris.utils.auth import validate_signature
 from avaris.defaults import Names
 import traceback
 
@@ -134,21 +134,28 @@
 
 
 
         @self.app.get("/health")
         async def health_check():
             return {"status": "ok"}
 
+
+
+
+
+
         @self.app.get("/tasks")
         async def get_filtered_tasks(
-            id: str = Query(None, description="Filter tasks by ID"),
-            name: str = Query(None, description="Filter tasks by name"),
-            task: str = Query(None, description="Filter tasks by task type"),
-            start_date: datetime = Query(None, description="Start date for task filter (ISO 8601 format)"),
-            end_date: datetime = Query(None, description="End date for task filter (ISO 8601 format)"),
+            id: Optional[str] = Query(None, description="Filter tasks by ID"),
+            name: Optional[str] = Query(None, description="Filter tasks by name"),
+            task: List[str] = Query([], description="Filter tasks by task type"),
+            start_date: Optional[datetime] = Query(
+                None, description="Start date for task filter (ISO 8601 format)"),
+            end_date: Optional[datetime] = Query(
+                None, description="End date for task filter (ISO 8601 format)"),
         ):
             # Prepare the filtering criteria as a dictionary
             filter_criteria = {
                 "id": id,
                 "name": name,
                 "task": task,
                 "start_date": start_date,
```

### Comparing `avaris-0.2.0/src/avaris/task/plugins.py` & `avaris-0.2.1/src/avaris/task/plugins.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/task/task_registry.py` & `avaris-0.2.1/src/avaris/task/task_registry.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/task/taskmaster.py` & `avaris-0.2.1/src/avaris/task/taskmaster.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/task/taskmaster_apscheduler.py` & `avaris-0.2.1/src/avaris/task/taskmaster_apscheduler.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/task/taskmaster_celery.py` & `avaris-0.2.1/src/avaris/task/taskmaster_celery.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/utils/auth.py` & `avaris-0.2.1/src/avaris/utils/auth.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/utils/logging.py` & `avaris-0.2.1/src/avaris/utils/logging.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/utils/management.py` & `avaris-0.2.1/src/avaris/utils/management.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/src/avaris/utils/parse.py` & `avaris-0.2.1/src/avaris/utils/parse.py`

 * *Files identical despite different names*

### Comparing `avaris-0.2.0/PKG-INFO` & `avaris-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avaris
-Version: 0.2.0
+Version: 0.2.1
 Summary: Task execution engine for data management and monitoring
 License: Apache-2.0
 Author: dennis
 Author-email: denngohis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -151,14 +151,86 @@
         # Implementation of your task
         try:
             return {}
         except Exception as e:
             self.logger.error(f"An error occurred while executing task: {e}")
             raise
 ```
+## Passing variables from the environment
+
+For a task parameter set that looks like this
+```python
+class HTTPGetParameters(BaseParameter):
+    __NAME__ = 'http_get'
+    url: str
+    username: Optional[str] = None
+    password: Optional[SecretStr] = None
+    response_format: Literal['json', 'text',
+                             'binary'] = 'text'
+```
+You can now instruct Avaris to get the secret from the environment directly like so.
+```yaml
+compendium:
+  name: get request
+  tasks:
+    - name: get example.com
+      schedule: "* * * * *"
+      executor:
+        task: http_get
+        parameters:
+          username: ${{ env.USERNAME }}
+          password: ${{ env.PASSWORD }}
+          url: https://example.com
+          response_format: text
+```
+
+Another way to specify secrets (legacy method) would be like so:
+```python
+from avaris.executor.executor import TaskExecutor
+from avaris.api.models import BaseParameter
+from avaris.task.task_registry import register_task_executor
+
+"""Define your parameter model with its identifier"""
+class MyParameters(BaseParameter):
+    __NAME__ = 'my_task_identifier_in_yaml'
+    my_param: str = ""
+
+@register_task_executor(MyParameters)
+class MyTask(TaskExecutor[MyParameters]) :
+
+    async def execute(self) -> dict:
+        try:
+            self.logger.info("Hello World!")
+            # Fetch secrets if any were mentioned explicity from the config. (will also load from env)
+            secrets = await self.load_secrets()
+            access_parameters_this_way = self.parameters.my_param
+            my_secret = secrets.get("MY_SECRET", None)
+            return {'my_key': self.parameters.my_param}
+        except Exception as e:
+            self.logger.error(
+                f"Error : {e}")
+            return {'error': str(e)}
+```
+And then in YAML you could instruct Avaris this way:
+```yaml
+compendium:
+  name: latest version jobs
+  tasks:
+    -  # more tasks...
+    - name: Example
+      schedule: "* * * * *"
+      executor:
+        task: my_task_identifier_in_yaml # task identifier
+        parameters:
+          my_param: "123"
+        secrets:
+          MY_SECRET: # implicity loading from env
+```
+
+
 
 # Default Configurations Summary
 
 ## Directories
 
 - **Home Directory**: `~/.avaris`
 - **Working Directory**: `$WORKINGDIR` or fallback to `~/.avaris` or current working directory
```

