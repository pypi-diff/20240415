# Comparing `tmp/reprompt-0.0.7.1.tar.gz` & `tmp/reprompt-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.1.tar` & `reprompt-0.0.7.2.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7.1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7.1/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-04 23:08:33.474206 reprompt-0.0.7.1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7.1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-04 23:08:33.474462 reprompt-0.0.7.1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7.1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7.1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7.1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7.1/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7.1/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-07 21:52:20.071934 reprompt-0.0.7.1/README.md
--rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7.1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7.1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7.1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7.1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7.1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7.1/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7.1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7.1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7.1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7.1/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7.1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7.1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7.1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7.1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7.1/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-07 21:52:20.072547 reprompt-0.0.7.1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476873 reprompt-0.0.7.1/src/README.md
--rw-r--r--   0        0        0     1480 2024-04-08 17:45:55.556657 reprompt-0.0.7.1/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7.1/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      166 2024-04-08 17:02:10.738220 reprompt-0.0.7.1/src/reprompt/config.py
--rw-r--r--   0        0        0     2119 2024-04-07 23:19:14.207089 reprompt-0.0.7.1/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0     2338 2024-04-07 23:50:31.283965 reprompt-0.0.7.1/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7.1/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7.1/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7.1/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7.1/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17737 1970-01-01 00:00:00.000000 reprompt-0.0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7.2/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7.2/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-04 23:08:33.474206 reprompt-0.0.7.2/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7.2/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-04 23:08:33.474462 reprompt-0.0.7.2/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7.2/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7.2/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7.2/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7.2/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 21:52:20.071934 reprompt-0.0.7.2/README.md
+-rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7.2/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7.2/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7.2/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7.2/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7.2/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7.2/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7.2/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7.2/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7.2/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7.2/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7.2/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7.2/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7.2/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7.2/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-07 21:52:20.072547 reprompt-0.0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476873 reprompt-0.0.7.2/src/README.md
+-rw-r--r--   0        0        0     1241 2024-04-15 21:41:32.721094 reprompt-0.0.7.2/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7.2/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      166 2024-04-08 17:02:10.738220 reprompt-0.0.7.2/src/reprompt/config.py
+-rw-r--r--   0        0        0     3347 2024-04-15 21:39:48.952401 reprompt-0.0.7.2/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7.2/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7.2/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7.2/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17737 1970-01-01 00:00:00.000000 reprompt-0.0.7.2/PKG-INFO
```

### Comparing `reprompt-0.0.7.1/.devcontainer/devcontainer.json` & `reprompt-0.0.7.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.2/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/.gitignore` & `reprompt-0.0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/.pre-commit-config.yaml` & `reprompt-0.0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/.vscode/settings.json` & `reprompt-0.0.7.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/LICENSE` & `reprompt-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/README.md` & `reprompt-0.0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/docs/Makefile` & `reprompt-0.0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/docs/conf.py` & `reprompt-0.0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/docs/make.bat` & `reprompt-0.0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/docs/pylint.md` & `reprompt-0.0.7.2/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/pyproject.toml` & `reprompt-0.0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/src/reprompt/__init__.py` & `reprompt-0.0.7.2/src/reprompt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 """Reprompt"""
 
 from __future__ import annotations
 
 import logging
 
 from . import config
-from .custom_httpx import setup_monkey_patch
-from .tracing import FunctionTrace, write_traces
+from .tracing import FunctionTrace, write_traces, get_edits
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.1"
+__version__ = "0.0.7.2"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
-__all__ = ["init", "FunctionTrace", "write_traces"]
+__all__ = ["init", "FunctionTrace", "write_traces", "get_edits"]
 
 
-def init(api_base_url: str = None, api_key: str = None, autocapture: bool = False):
+def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
+    if debug:
+        logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(logging.INFO)
     """
     Initializes the reprompt SDK with the given API base URL and API key.
     If api_base_url or api_key is not None in the arguments, we override the global variable.
     """
     if api_base_url is not None:
         config.api_base_url = api_base_url
     if api_key is not None:
         config.api_key = api_key
 
-    logger.info(api_key)
     if not config.api_key:
         logger.error("API key is required but was not provided. Monkey patching will not be applied.")
         return
 
-    if autocapture:
-        try:
-            # Apply the monkey patch
-            setup_monkey_patch()
-            logger.info("All HTTPX calls will now be intercepted and logged by Reprompt.")
-        except ImportError as e:
-            logger.error(f"Required module not found: {e}. Monkey patching not applied.")
-
-    logger.info(f"reprompt initialized with API Base URL: {config.api_base_url} and API Key: {config.api_key}")
+    logger.debug(
+        f"reprompt v{__version__} initialized with API Base URL: {config.api_base_url} and API Key: {config.api_key}"
+    )
```

### Comparing `reprompt-0.0.7.1/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.2/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/src/reprompt/tracing.py` & `reprompt-0.0.7.2/src/reprompt/tracing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,92 @@
 from __future__ import annotations
 
 from datetime import datetime
 
 import aiohttp
 import asyncio
 
+import logging
+
 from . import config
 
 from .background_task_manager import BackgroundTaskManager
 from functools import partial
 
+logger = logging.getLogger(__name__)
+
 
 async def write_traces_task(traces):
-    print("writing traces TASK")
     timestamp = datetime.now().isoformat()
     data = {"traces": [{"function_calls": traces, "timestamp": timestamp}]}
     if config.api_key is None:
         print("API key is required to upload traces")
         return
     try:
         async with aiohttp.ClientSession() as session:
+            logger.debug(f"Uploading traces asynchronously")
             async with session.post(
                 f"{config.api_base_url}/api/tracer/upload_batch",
                 json=data,
                 headers={"Content-Type": "application/json", "apiKey": config.api_key},
             ) as response:
                 if response.status != 200:
-                    print("Failed to upload batch")
+                    logger.error(f"Failed to upload batch: {response.status}")
                 else:
-                    print("Batch uploaded successfully")
+                    logger.debug("Batch uploaded successfully")
     except aiohttp.ClientError:
-        print("Cannot connect to tracer")
+        logger.error("Cannot connect to reprompt to upload traces")
 
 
 def write_traces(traces):
     loop = asyncio.get_event_loop()
     if loop.is_running():
         loop.create_task(write_traces_task([trace.get_trace_info() for trace in traces]))
     else:
         # Handling the case where loop is not running is tricky
         # It's usually not recommended to try to start the loop yourself in a library function
         print("Event loop is not running. Can't schedule write_traces_task.")
 
 
 class FunctionTrace:
     def __init__(self, func_name, func_inputs):
+        logger.debug(f"Creating trace for function {func_name}")
         self.func_name = func_name
         self.start_time = datetime.now()
         self.end_time = None
         self.duration = None
         self.func_inputs = func_inputs
         self.func_outputs = None
 
     def end_trace(self, func_outputs):
+        logger.debug(f"Ending trace for function {self.func_name}")
         self.func_outputs = func_outputs
         self.end_time = datetime.now()
         self.duration = (self.end_time - self.start_time).total_seconds()
 
     def get_trace_info(self):
         return {
             "function_name": self.func_name,
             "start_time": self.start_time.isoformat(),
             "end_time": self.end_time.isoformat() if self.end_time else None,
             "duration_seconds": self.duration,
             "function_inputs": self.func_inputs,
             "function_outputs": self.func_outputs,
         }
+
+
+async def get_edits(input: str) -> dict:
+    try:
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                f"{config.api_base_url}/api/overrides/get_example_overrides",
+                json={"input": input},
+                headers={"Content-Type": "application/json"},
+            ) as response:
+                if response.status != 200:
+                    logger.error(f"Failed to fetch edits: {response.status}")
+                    return None
+                else:
+                    logger.debug("fetched example overrides")
+                    return await response.json()
+    except aiohttp.ClientError:
+        logger.error("Cannot connect to reprompt to fetch edits")
```

### Comparing `reprompt-0.0.7.1/tests/conftest.py` & `reprompt-0.0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/tests/test_openai_tracing.py` & `reprompt-0.0.7.2/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.1/PKG-INFO` & `reprompt-0.0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

