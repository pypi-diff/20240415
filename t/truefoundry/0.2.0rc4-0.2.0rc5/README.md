# Comparing `tmp/truefoundry-0.2.0rc4.tar.gz` & `tmp/truefoundry-0.2.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc4.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc5.tar", max compression
```

## Comparing `truefoundry-0.2.0rc4.tar` & `truefoundry-0.2.0rc5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      871 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/README.md
--rw-r--r--   0        0        0     1147 2024-04-12 09:17:42.678230 truefoundry-0.2.0rc4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4428 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2348 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    10929 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0      435 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      854 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5890 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5076 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0     1585 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-12 09:17:27.974253 truefoundry-0.2.0rc4/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       39 2024-04-12 09:17:27.978253 truefoundry-0.2.0rc4/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      151 2024-04-12 09:17:27.978253 truefoundry-0.2.0rc4/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc4/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/README.md
+-rw-r--r--   0        0        0     1147 2024-04-15 10:42:34.319432 truefoundry-0.2.0rc5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4428 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2348 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    11713 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0      435 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5890 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5076 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc5/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc4/README.md` & `truefoundry-0.2.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/pyproject.toml` & `truefoundry-0.2.0rc5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc4"
+version = "0.2.0rc5"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.6"
```

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,17 +205,30 @@
     console = Console()
     openai_client = _get_openai_client()
     docker_client = _get_docker(console)
     project_root_path = os.path.abspath(project_root_path)
     console.print(
         "[bold magenta]TFY-Agent[/]: A tool for building and deploying [magenta]Jobs/Services[/] to the Truefoundry platform."
     )
-    console.print(
-        "[bold reverse red]DISCLAIMER:[/] The contents of the project will be sent to OpenAI."
-    )
+    if AUTODEPLOY_OPENAI_BASE_URL is not None and AUTODEPLOY_OPENAI_API_KEY is not None:
+        console.print(
+            "[bold green]OpenAI credentials found in environment variables.[/]"
+        )
+        console.print(
+            "[bold reverse red]DISCLAIMER:[/] The contents of your project will be sent to OpenAI.",
+            "This operation will use tokens from your provided OpenAI account and may incur costs.",
+        )
+    else:
+        console.print(
+            "[bold reverse red]DISCLAIMER:[/] The contents of the project will be sent to OpenAI."
+        )
+        console.print(
+            "[dim]To use your own LLM, set the environment variables [dim italic green]AUTODEPLOY_OPENAI_BASE_URL[/],[/]",
+            "[dim][dim italic green]AUTODEPLOY_OPENAI_API_KEY[/], and [dim italic green]AUTODEPLOY_MODEL_NAME[/] for URL, API key, and LLM model name respectively.[/]",
+        )
     console.print(
         "[bold cyan]Note:[/] All changes will be committed to a new branch. Please ensure you have a repository."
     )
     _check_repo(project_root_path=project_root_path, console=console)
 
     component_type = ComponentType[
         Prompt.ask(
```

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/truefoundry/cli/__main__.py` & `truefoundry-0.2.0rc5/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc4/PKG-INFO` & `truefoundry-0.2.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc4
+Version: 0.2.0rc5
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

