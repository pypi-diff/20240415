# Comparing `tmp/tool_use-0.1.1rc4.tar.gz` & `tmp/tool_use-0.1.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.1.1rc4.tar", last modified: Mon Apr 15 14:14:22 2024, max compression
+gzip compressed data, was "tool_use-0.1.1rc5.tar", last modified: Mon Apr 15 15:52:45 2024, max compression
```

## Comparing `tool_use-0.1.1rc4.tar` & `tool_use-0.1.1rc5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.853567 tool_use-0.1.1rc4/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc4/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 14:14:22.853316 tool_use-0.1.1rc4/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc4/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc4/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 14:14:22.853617 tool_use-0.1.1rc4/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 14:14:08.000000 tool_use-0.1.1rc4/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.850718 tool_use-0.1.1rc4/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc4/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     2770 2024-04-15 12:53:45.000000 tool_use-0.1.1rc4/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc4/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc4/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.850858 tool_use-0.1.1rc4/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc4/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.852554 tool_use-0.1.1rc4/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc4/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    17235 2024-04-15 14:14:01.000000 tool_use-0.1.1rc4/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc4/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc4/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.852832 tool_use-0.1.1rc4/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-15 14:13:42.000000 tool_use-0.1.1rc4/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc4/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 14:14:22.853036 tool_use-0.1.1rc4/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 14:14:22.000000 tool_use-0.1.1rc4/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 14:14:22.000000 tool_use-0.1.1rc4/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 14:14:22.000000 tool_use-0.1.1rc4/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 14:14:22.000000 tool_use-0.1.1rc4/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 14:14:22.000000 tool_use-0.1.1rc4/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.943364 tool_use-0.1.1rc5/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc5/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 15:52:45.943124 tool_use-0.1.1rc5/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc5/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc5/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 15:52:45.943425 tool_use-0.1.1rc5/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 15:52:40.000000 tool_use-0.1.1rc5/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.939426 tool_use-0.1.1rc5/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     4507 2024-04-15 15:34:11.000000 tool_use-0.1.1rc5/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc5/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc5/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.939585 tool_use-0.1.1rc5/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.941891 tool_use-0.1.1rc5/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    17897 2024-04-15 15:46:00.000000 tool_use-0.1.1rc5/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc5/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc5/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.942574 tool_use-0.1.1rc5/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-15 14:13:42.000000 tool_use-0.1.1rc5/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc5/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.942800 tool_use-0.1.1rc5/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.1.1rc4/pyproject.toml` & `tool_use-0.1.1rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/setup.py` & `tool_use-0.1.1rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.1.1rc4",
+    version="0.1.1rc5",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.1.1rc4/tests/test_anthropic_tool_use.py` & `tool_use-0.1.1rc5/tests/test_anthropic_tool_use.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,26 @@
 @pytest_asyncio.fixture
 def my_connection(load_env) -> AnthropicConnection:
     return AnthropicConnection(
         secrets=dict(
             api_key=os.environ.get("ANTHROPIC_API_KEY"),
             api_type="anthropic",
             api_base="https://api.anthropic.com",
+            client_key=None,
+        ),
+    )
+
+
+@pytest_asyncio.fixture
+def my_custom_connection(load_env) -> AnthropicConnection:
+    return AnthropicConnection(
+        secrets=dict(
+            api_key=os.environ.get("ANTHROPIC_API_KEY"),
+            api_type="anthropic",
+            api_base=os.environ.get("ANTHROPIC_API_BASE"),
         ),
     )
 
 
 def load_tool_prompts() -> Tuple[str, dict]:
     prompt = ""
     with open(
@@ -87,14 +99,56 @@
             prompt=prompt,
             model="claude-3-haiku-20240307",
             max_tokens=500,
             stream=True,
             question="I want to make a recipe with chicken.",
         )
         chunk_count = 0
+        total_result = ""
+        async for chunk in result:
+            chunk_count += 1
+            total_result += chunk
+        print(chunk_count)
+        print(total_result)
+
+    async def test_anthropic_tool_use_2(self, my_custom_connection):
+        prompt, sample_tool = load_tool_prompts()
+        result = await anthropic_tool_use(
+            connection=my_custom_connection,
+            prompt=prompt,
+            model="claude-3-haiku-20240307",
+            max_tokens=500,
+            tools=[sample_tool],
+        )
+        assert result is not None
+        print(result)
+
+    async def test_anthropic_2(self, my_custom_connection):
+        prompt = load_prompt()
+        result = await anthropic_tool_use(
+            connection=my_custom_connection,
+            prompt=prompt,
+            model="claude-3-haiku-20240307",
+            max_tokens=500,
+            question="I want to make a recipe with chicken.",
+        )
+        assert result is not None
+        print(result)
+
+    async def test_anthropic_stream_2(self, my_custom_connection):
+        prompt = load_prompt()
+        result = await anthropic_tool_use(
+            connection=my_custom_connection,
+            prompt=prompt,
+            model="claude-3-haiku-20240307",
+            max_tokens=500,
+            stream=True,
+            question="I want to make a recipe with chicken.",
+        )
+        chunk_count = 0
         total_result = ""
         async for chunk in result:
             chunk_count += 1
             total_result += chunk
         print(chunk_count)
         print(total_result)
```

### Comparing `tool_use-0.1.1rc4/tests/test_exception.py` & `tool_use-0.1.1rc5/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tests/test_openai_tool_use.py` & `tool_use-0.1.1rc5/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.1.1rc5/tool_use/tools/anthropic_tool_use.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from anthropic.types.beta.tools import (
     ToolParam,
     ToolsBetaMessage,
     ToolsBetaMessageParam,
 )
 from anthropic.types.message_param import MessageParam
 from promptflow import tool
-from promptflow.connections import CustomConnection, CustomStrongTypeConnection
+from promptflow.connections import CustomStrongTypeConnection
 from promptflow.contracts.types import PromptTemplate, Secret
 from promptflow.exceptions import SystemErrorException, UserErrorException
 from promptflow.tools.common import (
     generate_retry_interval,
     render_jinja_template,
     to_bool,
     validate_role,
@@ -62,15 +62,16 @@
     :param api_base: The api base url.
     :type api_base: str
     :param api_type: The api type (available type: vertex_anthropic, bedrock_anthropic).
     :type api_type: str
     """
 
     api_key: Secret
-    api_base: Secret = "https://api.anthropic.com"
+    client_key: Secret
+    api_base: Secret
     api_type: Secret = "anthropic"
 
 
 class WrappedAnthropicError(WrappedOpenAIError):
     pass
 
 
@@ -100,18 +101,33 @@
 
 class ToolChoiceDict(TypedDict):
     type: str
     function: ToolChoiceFunctionDict
 
 
 def _normalize_connection_config(connection: AnthropicConnection):
+    extra_config = {}
+    typ = connection.api_type
+    if typ == "anthropic":
+        extra_config = {
+            "api_key": connection.api_key,
+            "base_url": connection.api_base,
+        }
+    elif typ == "bedrock_anthropic":
+        extra_config = {
+            "aws_secret_key": connection.api_key,
+            "aws_access_key": connection.client_key,
+            "aws_region": "ap-northeast-2",
+            "base_url": connection.api_base,
+        }
     return {
         "max_retries": 0,
         "timeout": None,
         "_strict_response_validation": True,
+        **extra_config,
     }
 
 
 def parse_template(
     template: str, valid_roles: list[str]
 ) -> Tuple[List[Dict[str, Any]], bool]:
     results = []
@@ -120,15 +136,21 @@
     separator = r"(?i)^\s*#?\s*(" + "|".join(valid_roles) + r")\s*:\s*\n"
     chunks = re.split(separator, template, flags=re.MULTILINE)
     is_tool_use = False
     for chunk in chunks:
         last_message = results[-1] if len(results) > 0 else None
         if last_message and "role" in last_message and "content" not in last_message:
             parsed_chunk = parse_section(chunk)
-            last_message["content"] = parsed_chunk
+            if "text" in parsed_chunk:
+                last_message["content"] = {
+                    "type": "text",
+                    "text": parsed_chunk["text"].strip(),
+                }
+            else:
+                last_message["content"] = parsed_chunk
             # figure out whether there is type called tool_use or tool_result
             is_tool_use |= any(map(lambda x: x["type"] == "tool_use", parsed_chunk))
         else:
             if chunk.strip() == "":
                 continue
             role = chunk.strip().lower()
             validate_role(role, valid_roles=valid_roles)
@@ -391,15 +413,14 @@
     is_raw_output: Optional[bool] = False,
     **kwargs,
 ) -> str | dict | Message | AsyncMessageStreamManager:  # type: ignore
     chat_str = render_jinja_template(
         prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs
     )
     system, messages, is_tool_use = _parse_chat(chat_str)
-    print(messages)
     # TODO: remove below type conversion after client can pass json rather than string.
     stream = to_bool(stream)
     params = {
         "model": model,
         "messages": messages,
         "system": system,
         "temperature": float(temperature),
```

### Comparing `tool_use-0.1.1rc4/tool_use/tools/openai_tool_use.py` & `tool_use-0.1.1rc5/tool_use/tools/openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tool_use/tools/utils.py` & `tool_use-0.1.1rc5/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.1.1rc5/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.1.1rc5/tool_use/yamls/openai_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc4/tool_use.egg-info/SOURCES.txt` & `tool_use-0.1.1rc5/tool_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

