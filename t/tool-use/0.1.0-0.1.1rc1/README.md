# Comparing `tmp/tool_use-0.1.0.tar.gz` & `tmp/tool_use-0.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.1.0.tar", last modified: Sun Apr 14 06:26:36 2024, max compression
+gzip compressed data, was "tool_use-0.1.1rc1.tar", last modified: Mon Apr 15 09:29:37 2024, max compression
```

## Comparing `tool_use-0.1.0.tar` & `tool_use-0.1.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122943 tool_use-0.1.0/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.0/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-14 06:26:36.122681 tool_use-0.1.0/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      265 2024-04-14 06:25:21.000000 tool_use-0.1.0/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.0/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-14 06:26:36.123015 tool_use-0.1.0/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      527 2024-04-14 05:56:49.000000 tool_use-0.1.0/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.119863 tool_use-0.1.0/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.0/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     2812 2024-04-14 06:22:21.000000 tool_use-0.1.0/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.0/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.0/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.120037 tool_use-0.1.0/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.0/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.121754 tool_use-0.1.0/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.0/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    16672 2024-04-14 06:22:21.000000 tool_use-0.1.0/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.0/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.0/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122131 tool_use-0.1.0/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      918 2024-04-14 05:35:46.000000 tool_use-0.1.0/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.0/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122377 tool_use-0.1.0/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.133193 tool_use-0.1.1rc1/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc1/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 09:29:37.132911 tool_use-0.1.1rc1/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc1/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc1/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 09:29:37.133260 tool_use-0.1.1rc1/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 09:29:19.000000 tool_use-0.1.1rc1/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.130319 tool_use-0.1.1rc1/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc1/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     2818 2024-04-15 09:28:27.000000 tool_use-0.1.1rc1/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc1/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc1/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.130468 tool_use-0.1.1rc1/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc1/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.131986 tool_use-0.1.1rc1/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc1/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    16678 2024-04-15 09:28:21.000000 tool_use-0.1.1rc1/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc1/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc1/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.132323 tool_use-0.1.1rc1/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      918 2024-04-14 05:35:46.000000 tool_use-0.1.1rc1/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc1/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 09:29:37.132584 tool_use-0.1.1rc1/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 09:29:37.000000 tool_use-0.1.1rc1/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 09:29:37.000000 tool_use-0.1.1rc1/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 09:29:37.000000 tool_use-0.1.1rc1/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 09:29:37.000000 tool_use-0.1.1rc1/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 09:29:37.000000 tool_use-0.1.1rc1/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.1.0/pyproject.toml` & `tool_use-0.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/setup.py` & `tool_use-0.1.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.1.0",
+    version="0.1.1rc1",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.1.0/tests/test_anthropic_tool_use.py` & `tool_use-0.1.1rc1/tests/test_anthropic_tool_use.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import unittest
 from ast import literal_eval
 from typing import Tuple
 
 import pytest
 import pytest_asyncio
 
-from tool_use.connections.anthropic import AnthropicConnection
 from tool_use.tools.anthropic_tool_use import anthropic_tool_use
+from tool_use.tools.connections.anthropic import AnthropicConnection
 
 # Run the unit tests
 if __name__ == "__main__":
     from dotenv import load_dotenv
 
     load_dotenv()
     unittest.main()
```

### Comparing `tool_use-0.1.0/tests/test_exception.py` & `tool_use-0.1.1rc1/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tests/test_openai_tool_use.py` & `tool_use-0.1.1rc1/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.1.1rc1/tool_use/tools/anthropic_tool_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ChatAPIInvalidFunctions,
     ExceedMaxRetryTimes,
     FunctionCallNotSupportedInStreamMode,
     LLMError,
     WrappedOpenAIError,
 )
 
-from tool_use.connections.anthropic import AnthropicConnection
+from tool_use.tools.connections.anthropic import AnthropicConnection
 
 try:
     from anthropic import AsyncAnthropic as AnthropicClient
     from anthropic import AsyncAnthropicBedrock as AnthropicBedrockClient
     from anthropic import AsyncAnthropicVertex as AnthropicVertexClient
 except Exception:
     raise Exception(
```

### Comparing `tool_use-0.1.0/tool_use/tools/openai_tool_use.py` & `tool_use-0.1.1rc1/tool_use/tools/openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tool_use/tools/utils.py` & `tool_use-0.1.1rc1/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.1.1rc1/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.1.1rc1/tool_use/yamls/openai_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.0/tool_use.egg-info/SOURCES.txt` & `tool_use-0.1.1rc1/tool_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

