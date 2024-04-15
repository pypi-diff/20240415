# Comparing `tmp/unifyai-0.7.2.tar.gz` & `tmp/unifyai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.7.2.tar", max compression
+gzip compressed data, was "unifyai-0.8.0.tar", max compression
```

## Comparing `unifyai-0.7.2.tar` & `unifyai-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.7.2/LICENSE
--rw-r--r--   0        0        0     6315 2024-04-09 09:40:15.184460 unifyai-0.7.2/README.md
--rw-r--r--   0        0        0     1019 2024-04-09 09:38:07.980455 unifyai-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      135 2024-04-09 09:26:47.592423 unifyai-0.7.2/unifyai/__init__.py
--rw-r--r--   0        0        0     3859 2024-04-09 09:39:05.408457 unifyai-0.7.2/unifyai/chat.py
--rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.7.2/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.7.2/unifyai/exceptions.py
--rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.7.2/unifyai/tests.py
--rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.7.2/unifyai/utils.py
--rw-r--r--   0        0        0     6998 1970-01-01 00:00:00.000000 unifyai-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6303 2024-04-15 01:04:35.167574 unifyai-0.8.0/README.md
+-rw-r--r--   0        0        0     1041 2024-04-15 01:13:45.407571 unifyai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-14 23:39:40.271607 unifyai-0.8.0/unify/__init__.py
+-rw-r--r--   0        0        0     6724 2024-04-15 00:29:51.867587 unifyai-0.8.0/unify/chat.py
+-rw-r--r--   0        0        0    15107 2024-04-15 01:03:44.055575 unifyai-0.8.0/unify/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.8.0/unify/exceptions.py
+-rw-r--r--   0        0        0     4321 2024-04-14 23:59:09.707599 unifyai-0.8.0/unify/tests.py
+-rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.8.0/unify/utils.py
+-rw-r--r--   0        0        0     6964 1970-01-01 00:00:00.000000 unifyai-0.8.0/PKG-INFO
```

### Comparing `unifyai-0.7.2/LICENSE` & `unifyai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.2/README.md` & `unifyai-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```bash
 pip install unifyai
 ```
 
 ## Basic Usage
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
 response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
@@ -84,15 +84,15 @@
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
 
  ```python
-from unifyai import AsyncUnify
+from unify import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
@@ -106,29 +106,29 @@
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
 You can enable streaming responses by setting `stream=True` in the `.generate` function.
 
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
 stream = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
-from unifyai import AsyncUnify
+from unify import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
@@ -148,15 +148,15 @@
 ```
 
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@lowest-input-cost"
 )
 response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
@@ -168,15 +168,15 @@
 
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
 
 ## ChatBot Agent
 Our `ChatBot` allows you to start an interactive chat session with any of our supported llm endpoints with only a few lines of code:
 
 ```python
-from unifyai import ChatBot
+from unify import ChatBot
 agent = ChatBot(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@lowest-input-cost"
 )
 agent.run()
 ```
```

### Comparing `unifyai-0.7.2/pyproject.toml` & `unifyai-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.7.2"
+packages = [{include = "unify"}]
+version = "0.8.0"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
-repository = "https://github.com/unifyai/unify-llm-python"
+repository = "https://github.com/unifyai/unify"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 openai = "^1.12.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `unifyai-0.7.2/unifyai/clients.py` & `unifyai-0.8.0/unify/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import AsyncGenerator, Dict, Generator, List, Optional, Union
 
 import openai
 import requests
-from unifyai.exceptions import BadRequestError, UnifyError, status_error_map
-from unifyai.utils import (  # noqa:WPS450
+from unify.exceptions import BadRequestError, UnifyError, status_error_map
+from unify.utils import (  # noqa:WPS450
     _available_dynamic_modes,
     _validate_api_key,
     _validate_endpoint,
 )
 
 
 class Unify:
@@ -201,15 +201,15 @@
             chat_completion = self.client.chat.completions.create(
                 model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=True,
             )
             for chunk in chat_completion:
                 content = chunk.choices[0].delta.content  # type: ignore[union-attr]
-                self._provider = chunk.model.split("@")[-1]  # type: ignore[union-attr]
+                self.set_provider(chunk.model.split("@")[-1])  # type: ignore[union-attr]
                 if content is not None:
                     yield content
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     def _generate_non_stream(
         self,
@@ -218,17 +218,17 @@
     ) -> str:
         try:
             chat_completion = self.client.chat.completions.create(
                 model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=False,
             )
-            self._provider = chat_completion.model.split(  # type: ignore[union-attr]
+            self.set_provider(chat_completion.model.split(  # type: ignore[union-attr]
                 "@",
-            )[-1]
+            )[-1])
 
             return chat_completion.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
 
 class AsyncUnify:
@@ -425,15 +425,15 @@
         try:
             async_stream = await self.client.chat.completions.create(
                 model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=True,
             )
             async for chunk in async_stream:  # type: ignore[union-attr]
-                self._provider = chunk.model.split("@")[-1]
+                self.set_provider(chunk.model.split("@")[-1])
                 yield chunk.choices[0].delta.content or ""
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     async def _generate_non_stream(
         self,
         messages: List[Dict[str, str]],
@@ -441,11 +441,11 @@
     ) -> str:
         try:
             async_response = await self.client.chat.completions.create(
                 model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=False,
             )
-            self._provider = async_response.model.split("@")[-1]  # type: ignore
+            self.set_provider(async_response.model.split("@")[-1])  # type: ignore
             return async_response.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
```

### Comparing `unifyai-0.7.2/unifyai/exceptions.py` & `unifyai-0.8.0/unify/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.2/unifyai/tests.py` & `unifyai-0.8.0/unify/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 from types import AsyncGeneratorType, GeneratorType
 from unittest.mock import MagicMock, patch
 
-from unifyai.clients import AsyncUnify, Unify
-from unifyai.exceptions import AuthenticationError, UnifyError
+from unify.clients import AsyncUnify, Unify
+from unify.exceptions import AuthenticationError, UnifyError
 
 
 class TestUnify(unittest.TestCase):
     def setUp(self) -> None:
         # Set up a valid API key for testing
         self.valid_api_key = os.environ.get("UNIFY_KEY")
```

### Comparing `unifyai-0.7.2/unifyai/utils.py` & `unifyai-0.8.0/unify/utils.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.2/PKG-INFO` & `unifyai-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.7.2
+Version: 0.8.0
 Summary: A Python package for interacting with the Unify API
-Home-page: https://github.com/unifyai/unify-llm-python
+Home-page: https://github.com/unifyai/unify
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Repository, https://github.com/unifyai/unify-llm-python
+Project-URL: Repository, https://github.com/unifyai/unify
 Description-Content-Type: text/markdown
 
 # Unify Python API Library
 The Unify Python Package provides access to the [Unify](https://unify.ai) REST API, allowing you to query Large Language Models (LLMs)
 from any Python 3.7.1+ application.
 It includes Synchronous and Asynchronous clients with Streaming responses support.
 
@@ -35,15 +35,15 @@
 ```bash
 pip install unifyai
 ```
 
 ## Basic Usage
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
 response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
@@ -102,15 +102,15 @@
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
 
  ```python
-from unifyai import AsyncUnify
+from unify import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
@@ -124,29 +124,29 @@
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
 You can enable streaming responses by setting `stream=True` in the `.generate` function.
 
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
 stream = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?", stream=True)
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
-from unifyai import AsyncUnify
+from unify import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@anyscale"
 )
@@ -166,15 +166,15 @@
 ```
 
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
-from unifyai import Unify
+from unify import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@lowest-input-cost"
 )
 response = unify.generate(user_prompt="Hello Llama! Who was Isaac Newton?")
 ```
@@ -186,15 +186,15 @@
 
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
 
 ## ChatBot Agent
 Our `ChatBot` allows you to start an interactive chat session with any of our supported llm endpoints with only a few lines of code:
 
 ```python
-from unifyai import ChatBot
+from unify import ChatBot
 agent = ChatBot(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY"),
     endpoint="llama-2-13b-chat@lowest-input-cost"
 )
 agent.run()
 ```
```

