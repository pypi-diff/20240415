# Comparing `tmp/tool_use-0.1.1rc2.tar.gz` & `tmp/tool_use-0.1.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.1.1rc2.tar", last modified: Mon Apr 15 13:13:03 2024, max compression
+gzip compressed data, was "tool_use-0.1.1rc3.tar", last modified: Mon Apr 15 14:08:58 2024, max compression
```

## Comparing `tool_use-0.1.1rc2.tar` & `tool_use-0.1.1rc3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.373362 tool_use-0.1.1rc2/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc2/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 13:13:03.373107 tool_use-0.1.1rc2/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc2/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc2/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 13:13:03.373411 tool_use-0.1.1rc2/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 13:13:00.000000 tool_use-0.1.1rc2/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.370132 tool_use-0.1.1rc2/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc2/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     2770 2024-04-15 12:53:45.000000 tool_use-0.1.1rc2/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc2/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc2/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.370263 tool_use-0.1.1rc2/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc2/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.372245 tool_use-0.1.1rc2/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc2/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    17217 2024-04-15 12:53:45.000000 tool_use-0.1.1rc2/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc2/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc2/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.372655 tool_use-0.1.1rc2/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      918 2024-04-14 05:35:46.000000 tool_use-0.1.1rc2/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc2/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 13:13:03.372857 tool_use-0.1.1rc2/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 13:13:03.000000 tool_use-0.1.1rc2/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 13:13:03.000000 tool_use-0.1.1rc2/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 13:13:03.000000 tool_use-0.1.1rc2/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 13:13:03.000000 tool_use-0.1.1rc2/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 13:13:03.000000 tool_use-0.1.1rc2/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.692390 tool_use-0.1.1rc3/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc3/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 14:08:58.692146 tool_use-0.1.1rc3/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc3/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc3/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 14:08:58.692437 tool_use-0.1.1rc3/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 14:08:40.000000 tool_use-0.1.1rc3/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.689973 tool_use-0.1.1rc3/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc3/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     2770 2024-04-15 12:53:45.000000 tool_use-0.1.1rc3/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc3/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc3/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.690114 tool_use-0.1.1rc3/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc3/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.691410 tool_use-0.1.1rc3/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc3/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    17232 2024-04-15 14:08:29.000000 tool_use-0.1.1rc3/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc3/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc3/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.691676 tool_use-0.1.1rc3/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      918 2024-04-14 05:35:46.000000 tool_use-0.1.1rc3/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc3/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:08:58.691891 tool_use-0.1.1rc3/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 14:08:58.000000 tool_use-0.1.1rc3/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 14:08:58.000000 tool_use-0.1.1rc3/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 14:08:58.000000 tool_use-0.1.1rc3/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 14:08:58.000000 tool_use-0.1.1rc3/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 14:08:58.000000 tool_use-0.1.1rc3/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.1.1rc2/pyproject.toml` & `tool_use-0.1.1rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/setup.py` & `tool_use-0.1.1rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.1.1rc2",
+    version="0.1.1rc3",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.1.1rc2/tests/test_anthropic_tool_use.py` & `tool_use-0.1.1rc3/tests/test_anthropic_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tests/test_exception.py` & `tool_use-0.1.1rc3/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tests/test_openai_tool_use.py` & `tool_use-0.1.1rc3/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.1.1rc3/tool_use/tools/anthropic_tool_use.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from anthropic.types.beta.tools import (
     ToolParam,
     ToolsBetaMessage,
     ToolsBetaMessageParam,
 )
 from anthropic.types.message_param import MessageParam
 from promptflow import tool
-from promptflow.connections import CustomStrongTypeConnection
+from promptflow.connections import CustomConnection, CustomStrongTypeConnection
 from promptflow.contracts.types import PromptTemplate, Secret
 from promptflow.exceptions import SystemErrorException, UserErrorException
 from promptflow.tools.common import (
     generate_retry_interval,
     render_jinja_template,
     to_bool,
     validate_role,
@@ -372,15 +372,15 @@
             # chat api may return message with no content.
             return completion.model_dump()["content"]
 
 
 @tool
 @handle_anthropic_error()
 async def anthropic_tool_use(
-    connection: AnthropicConnection,
+    connection: CustomConnection,
     prompt: PromptTemplate,
     model: ModelEnum,
     max_tokens: int,
     temperature: float = 1,
     top_p: float = 1,
     n: int = 1,
     stream: Optional[bool] = False,
```

### Comparing `tool_use-0.1.1rc2/tool_use/tools/openai_tool_use.py` & `tool_use-0.1.1rc3/tool_use/tools/openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tool_use/tools/utils.py` & `tool_use-0.1.1rc3/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.1.1rc3/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.1.1rc3/tool_use/yamls/openai_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc2/tool_use.egg-info/SOURCES.txt` & `tool_use-0.1.1rc3/tool_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

