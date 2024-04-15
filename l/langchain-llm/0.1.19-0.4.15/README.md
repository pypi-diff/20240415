# Comparing `tmp/langchain_llm-0.1.19.tar.gz` & `tmp/langchain_llm-0.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_llm-0.1.19.tar", max compression
+gzip compressed data, was "langchain_llm-0.4.15.tar", max compression
```

## Comparing `langchain_llm-0.1.19.tar` & `langchain_llm-0.4.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      335 2024-01-13 01:32:31.099787 langchain_llm-0.1.19/langchain_llm/__init__.py
--rw-r--r--   0        0        0     1027 2024-01-11 01:32:36.131502 langchain_llm-0.1.19/langchain_llm/_compat.py
--rw-r--r--   0        0        0    30597 2024-01-14 11:01:57.842074 langchain_llm-0.1.19/langchain_llm/_huggingface.py
--rw-r--r--   0        0        0      168 2024-01-11 01:23:24.186770 langchain_llm-0.1.19/langchain_llm/_types.py
--rw-r--r--   0        0        0    12222 2024-01-13 03:40:18.738474 langchain_llm-0.1.19/langchain_llm/_vllm.py
--rw-r--r--   0        0        0       87 2024-01-14 11:01:57.847074 langchain_llm-0.1.19/langchain_llm/adapters/__init__.py
--rw-r--r--   0        0        0     1750 2024-01-13 01:21:21.508952 langchain_llm-0.1.19/langchain_llm/adapters/model.py
--rw-r--r--   0        0        0     5918 2024-01-13 01:21:21.513184 langchain_llm-0.1.19/langchain_llm/adapters/patcher.py
--rw-r--r--   0        0        0    47769 2024-01-19 03:53:39.386745 langchain_llm-0.1.19/langchain_llm/adapters/template.py
--rw-r--r--   0        0        0      420 2024-01-11 01:26:38.378999 langchain_llm-0.1.19/langchain_llm/generation/__init__.py
--rw-r--r--   0        0        0     2348 2024-01-11 01:29:50.914452 langchain_llm-0.1.19/langchain_llm/generation/baichuan.py
--rw-r--r--   0        0        0    10012 2024-01-11 01:29:54.374906 langchain_llm-0.1.19/langchain_llm/generation/chatglm.py
--rw-r--r--   0        0        0    10203 2024-01-19 01:34:15.968572 langchain_llm-0.1.19/langchain_llm/generation/qwen.py
--rw-r--r--   0        0        0    13011 2024-01-11 01:30:12.834599 langchain_llm-0.1.19/langchain_llm/generation/stream.py
--rw-r--r--   0        0        0     4613 2024-01-11 01:30:23.332905 langchain_llm-0.1.19/langchain_llm/generation/utils.py
--rw-r--r--   0        0        0     2674 2024-01-11 01:30:28.965701 langchain_llm-0.1.19/langchain_llm/generation/xverse.py
--rw-r--r--   0        0        0     1241 2024-01-14 11:01:57.852138 langchain_llm-0.1.19/langchain_llm/utils.py
--rw-r--r--   0        0        0      582 2024-01-19 03:54:08.739283 langchain_llm-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     3398 2024-01-19 03:54:18.965821 langchain_llm-0.1.19/README.md
--rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 langchain_llm-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0      335 2024-01-13 01:32:31.099787 langchain_llm-0.4.15/langchain_llm/__init__.py
+-rw-r--r--   0        0        0     1027 2024-01-11 01:32:36.131502 langchain_llm-0.4.15/langchain_llm/_compat.py
+-rw-r--r--   0        0        0    31032 2024-04-15 01:24:19.362102 langchain_llm-0.4.15/langchain_llm/_huggingface.py
+-rw-r--r--   0        0        0      168 2024-01-11 01:23:24.186770 langchain_llm-0.4.15/langchain_llm/_types.py
+-rw-r--r--   0        0        0    12676 2024-04-15 01:24:04.772528 langchain_llm-0.4.15/langchain_llm/_vllm.py
+-rw-r--r--   0        0        0       87 2024-01-14 11:01:57.847074 langchain_llm-0.4.15/langchain_llm/adapters/__init__.py
+-rw-r--r--   0        0        0     1750 2024-01-13 01:21:21.508952 langchain_llm-0.4.15/langchain_llm/adapters/model.py
+-rw-r--r--   0        0        0     5918 2024-01-13 01:21:21.513184 langchain_llm-0.4.15/langchain_llm/adapters/patcher.py
+-rw-r--r--   0        0        0    49053 2024-04-15 01:15:38.631786 langchain_llm-0.4.15/langchain_llm/adapters/template.py
+-rw-r--r--   0        0        0      420 2024-01-11 01:26:38.378999 langchain_llm-0.4.15/langchain_llm/generation/__init__.py
+-rw-r--r--   0        0        0     2348 2024-01-11 01:29:50.914452 langchain_llm-0.4.15/langchain_llm/generation/baichuan.py
+-rw-r--r--   0        0        0    10012 2024-01-11 01:29:54.374906 langchain_llm-0.4.15/langchain_llm/generation/chatglm.py
+-rw-r--r--   0        0        0    10203 2024-01-19 01:34:15.968572 langchain_llm-0.4.15/langchain_llm/generation/qwen.py
+-rw-r--r--   0        0        0    13011 2024-01-11 01:30:12.834599 langchain_llm-0.4.15/langchain_llm/generation/stream.py
+-rw-r--r--   0        0        0     4613 2024-01-11 01:30:23.332905 langchain_llm-0.4.15/langchain_llm/generation/utils.py
+-rw-r--r--   0        0        0     2674 2024-01-11 01:30:28.965701 langchain_llm-0.4.15/langchain_llm/generation/xverse.py
+-rw-r--r--   0        0        0     1241 2024-01-14 11:01:57.852138 langchain_llm-0.4.15/langchain_llm/utils.py
+-rw-r--r--   0        0        0      582 2024-04-15 01:24:38.239840 langchain_llm-0.4.15/pyproject.toml
+-rw-r--r--   0        0        0     3398 2024-01-19 03:54:18.965821 langchain_llm-0.4.15/README.md
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 langchain_llm-0.4.15/PKG-INFO
```

### Comparing `langchain_llm-0.1.19/langchain_llm/_compat.py` & `langchain_llm-0.4.15/langchain_llm/_compat.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/_huggingface.py` & `langchain_llm-0.4.15/langchain_llm/_huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,15 +484,18 @@
         """Validate that python package exists in environment."""
 
         # Check whether to need to construct prompts or inputs. """
         model_name = values["llm"].model_name
 
         values["chat_template"] = values["chat_template"].lower() if values["chat_template"] is not None else None
         if not values["prompt_adapter"]:
-            values["prompt_adapter"] = get_prompt_adapter(model_name, values["chat_template"])
+            try:
+                values["prompt_adapter"] = get_prompt_adapter(model_name, values["chat_template"])
+            except KeyError:
+                values["chat_template"] = None
 
         values["construct_prompt"] = values["chat_template"] is not None
 
         if "chatglm3" in model_name:
             logger.info("Using ChatGLM3 Model for Chat!")
         elif check_is_baichuan(values["llm"].model):
             logger.info("Using Baichuan Model for Chat!")
@@ -627,15 +630,23 @@
             messages = self.prompt_adapter.postprocess_messages(
                 messages, functions, tools=tools,
             )
             if functions or tools:
                 logger.debug(f"==== Messages with tools ====\n{messages}")
 
         if self.construct_prompt:
-            prompt = self.prompt_adapter.apply_chat_template(messages)
+            if getattr(self.llm.tokenizer, "chat_template", None) and not self.chat_template:
+                prompt = self.llm.tokenizer.apply_chat_template(
+                    conversation=messages,
+                    tokenize=False,
+                    add_generation_prompt=True,
+                )
+            else:
+                prompt = self.prompt_adapter.apply_chat_template(messages)
+
             if check_is_qwen(self.llm.model):
                 inputs = self.llm.tokenizer(prompt, allowed_special="all", disallowed_special=()).input_ids
             elif check_is_chatglm(self.llm.model):
                 inputs = self.llm.tokenizer([prompt], return_tensors="pt")
             else:
                 inputs = self.llm.tokenizer(prompt).input_ids
```

### Comparing `langchain_llm-0.1.19/langchain_llm/_vllm.py` & `langchain_llm-0.4.15/langchain_llm/_vllm.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,18 @@
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that python package exists in environment."""
 
         # Check whether to need to construct prompts or inputs. """
         model_name = values["llm"].model_name
         values["chat_template"] = values["chat_template"].lower() if values["chat_template"] is not None else None
         if not values["prompt_adapter"]:
-            values["prompt_adapter"] = get_prompt_adapter(model_name, values["chat_template"])
+            try:
+                values["prompt_adapter"] = get_prompt_adapter(model_name, values["chat_template"])
+            except KeyError:
+                values["chat_template"] = None
 
         values["tokenizer"] = values["llm"].client.get_tokenizer()
 
         return values
 
     def _get_parameters(
         self,
@@ -245,15 +248,23 @@
                 self.tokenizer,
                 messages,
                 self.max_window_size,
                 functions,
                 tools,
             )
         else:
-            return self.prompt_adapter.apply_chat_template(messages)
+            if getattr(self.tokenizer, "chat_template", None) and not self.chat_template:
+                prompt = self.tokenizer.apply_chat_template(
+                    conversation=messages,
+                    tokenize=False,
+                    add_generation_prompt=True,
+                )
+            else:
+                prompt = self.prompt_adapter.apply_chat_template(messages)
+            return prompt
 
     def _to_chatml_format(self, message: BaseMessage) -> dict:
         """Convert LangChain message to ChatML format."""
 
         if isinstance(message, SystemMessage):
             role = "system"
         elif isinstance(message, AIMessage):
```

### Comparing `langchain_llm-0.1.19/langchain_llm/adapters/model.py` & `langchain_llm-0.4.15/langchain_llm/adapters/model.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/adapters/patcher.py` & `langchain_llm-0.4.15/langchain_llm/adapters/patcher.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/adapters/template.py` & `langchain_llm-0.4.15/langchain_llm/adapters/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Dict,
     Any,
     Tuple,
 )
 
 from openai.types.chat import ChatCompletionMessageParam
 
-from .._types import Role
+from api.utils.protocol import Role
 
 
 @lru_cache
 def _compile_jinja_template(chat_template: str):
     """
     Compile a Jinja template from a string.
 
@@ -30,20 +30,22 @@
         >>> template_string = "Hello, {{ name }}!"
         >>> template = _compile_jinja_template(template_string)
     """
     try:
         from jinja2.exceptions import TemplateError
         from jinja2.sandbox import ImmutableSandboxedEnvironment
     except ImportError:
-        raise ImportError("apply_chat_template requires jinja2 to be installed.")
+        raise ImportError(
+            "apply_chat_template requires jinja2 to be installed.")
 
     def raise_exception(message):
         raise TemplateError(message)
 
-    jinja_env = ImmutableSandboxedEnvironment(trim_blocks=True, lstrip_blocks=True)
+    jinja_env = ImmutableSandboxedEnvironment(
+        trim_blocks=True, lstrip_blocks=True)
     jinja_env.globals["raise_exception"] = raise_exception
     return jinja_env.from_string(chat_template)
 
 
 class BaseTemplate(ABC):
 
     name: str = "chatml"
@@ -143,15 +145,16 @@
 
 class QwenTemplate(BaseTemplate):
 
     name = "qwen"
     system_prompt = "<|im_start|>system\nYou are a helpful assistant.<|im_end|>\n"
     allow_models = ["qwen"]
     stop = {
-        "token_ids": [151643, 151644, 151645],  # "<|endoftext|>", "<|im_start|>", "<|im_end|>"
+        # "<|endoftext|>", "<|im_start|>", "<|im_end|>"
+        "token_ids": [151643, 151644, 151645],
         "strings": ["<|endoftext|>", "<|im_end|>"],
     }
     function_call_available = True
 
     @property
     def template(self) -> str:
         """ This template formats inputs in the standard ChatML format. See
@@ -206,14 +209,42 @@
 
         z = output.rfind("\nFinal Answer: ")
         if z >= 0:
             output = output[z + len("\nFinal Answer: "):]
         return output, None
 
 
+class Qwen2Template(BaseTemplate):
+
+    name = "qwen2"
+    allow_models = ["qwen2"]
+    stop = {
+        "strings": ["<|endoftext|>", "<|im_end|>"],
+    }
+
+    @property
+    def template(self) -> str:
+        """ This template formats inputs in the standard ChatML format. See
+        https://github.com/openai/openai-python/blob/main/chatml.md
+        """
+        return (
+            "{% for message in messages %}"
+            "{% if loop.first and messages[0]['role'] != 'system' %}"
+            "{{ '<|im_start|>system\nYou are a helpful assistant<|im_end|>\n' }}"
+            "{% endif %}"
+            "{{'<|im_start|>' + message['role'] + '\n' + message['content']}}"
+            "{% if (loop.last and add_generation_prompt) or not loop.last %}"
+            "{{ '<|im_end|>' + '\n'}}"
+            "{% endif %}"
+            "{% endfor %}"
+            "{% if add_generation_prompt and messages[-1]['role'] != 'assistant' %}"
+            "{{ '<|im_start|>assistant\n' }}{% endif %}"
+        )
+
+
 class Llama2Template(BaseTemplate):
 
     name = "llama2"
     system_prompt = "You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe." \
                     "Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content." \
                     "Please ensure that your responses are socially unbiased and positive in nature.\n\n" \
                     "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not" \
@@ -240,43 +271,49 @@
 
         The reference for this chat template is [this code
         snippet](https://github.com/facebookresearch/llama/blob/556949fdfb72da27c2f4a40b7f0e4cf0b8153a28/llama/generation.py#L320-L362)
         in the original repository.
         """
         template = (
             "{% if messages[0]['role'] == 'system' %}"
-            "{% set loop_messages = messages[1:] %}"  # Extract system message if it's present
+            # Extract system message if it's present
+            "{% set loop_messages = messages[1:] %}"
             "{% set system_message = messages[0]['content'] %}"
             "{% elif USE_DEFAULT_PROMPT == true and not '<<SYS>>' in messages[0]['content'] %}"
-            "{% set loop_messages = messages %}"  # Or use the default system message if the flag is set
+            # Or use the default system message if the flag is set
+            "{% set loop_messages = messages %}"
             "{% set system_message = 'DEFAULT_SYSTEM_MESSAGE' %}"
             "{% else %}"
             "{% set loop_messages = messages %}"
             "{% set system_message = false %}"
             "{% endif %}"
-            "{% for message in loop_messages %}"  # Loop over all non-system messages
+            # Loop over all non-system messages
+            "{% for message in loop_messages %}"
             "{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}"
             "{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}"
             "{% endif %}"
-            "{% if loop.index0 == 0 and system_message != false %}"  # Embed system message in first message
+            # Embed system message in first message
+            "{% if loop.index0 == 0 and system_message != false %}"
             "{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}"
             "{% else %}"
             "{% set content = message['content'] %}"
             "{% endif %}"
-            "{% if message['role'] == 'user' %}"  # After all of that, handle messages/roles in a fairly normal way
+            # After all of that, handle messages/roles in a fairly normal way
+            "{% if message['role'] == 'user' %}"
             "{{ '<s>' + '[INST] ' + content.strip() + ' [/INST]' }}"
             "{% elif message['role'] == 'system' %}"
             "{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}"
             "{% elif message['role'] == 'assistant' %}"
             "{{ ' '  + content.strip() + ' ' + '</s>' }}"
             "{% endif %}"
             "{% endfor %}"
         )
         template = template.replace("USE_DEFAULT_PROMPT", "true")
-        default_message = self.system_prompt.replace("\n", "\\n").replace("'", "\\'")
+        default_message = self.system_prompt.replace(
+            "\n", "\\n").replace("'", "\\'")
         return template.replace("DEFAULT_SYSTEM_MESSAGE", default_message)
 
 
 class ChineseAlpaca2Template(Llama2Template):
 
     name = "chinese-llama-alpaca2"
     allow_models = ["chinese-llama-alpaca-2"]
@@ -417,15 +454,16 @@
                         "content": content,
                     }
                 )
             elif role == Role.ASSISTANT:
                 if content is not None:
                     for response in content.split("<|assistant|>"):
                         if "\n" in response:
-                            metadata, sub_content = response.split("\n", maxsplit=1)
+                            metadata, sub_content = response.split(
+                                "\n", maxsplit=1)
                         else:
                             metadata, sub_content = "", response
                         messages.append(
                             {
                                 "role": role,
                                 "metadata": metadata,
                                 "content": sub_content.strip()
@@ -717,19 +755,21 @@
             "{% endfor %}"
         )
 
 
 class InternLMTemplate(BaseTemplate):
 
     name = "internlm"
-    allow_models = ["internlm"]
     stop = {
         "strings": ["</s>", "<eoa>"],
     }
 
+    def match(self, name) -> bool:
+        return name.startswith("internlm") and not name.startswith("internlm2")
+
     @property
     def template(self) -> str:
         """ The output should look something like:
 
         <s><|User|>:{Prompt}<eoh>
         <|Bot|>:{Answer}<eoa>
         <s><|User|>:{Prompt}<eoh>
@@ -745,39 +785,41 @@
             "{% endfor %}"
         )
 
 
 class InternLM2Template(BaseTemplate):
 
     name = "internlm2"
-    allow_models = ["internlm2"]
     system_prompt = (
         "You are an AI assistant whose name is InternLM (书生·浦语).\n"
         "- InternLM (书生·浦语) is a conversational language model that is developed by Shanghai AI Laboratory (上海人工智能实验室). It is designed to be helpful, honest, and harmless.\n"
         "- InternLM (书生·浦语) can understand and communicate fluently in the language chosen by the user such as English and 中文."
     )
     stop = {
-        "strings": ["</s>", "[UNUSED_TOKEN_145]"],
+        "strings": ["</s>", "<|im_end|>"],
     }
 
+    def match(self, name) -> bool:
+        return name.startswith("internlm2")
+
     @property
     def template(self) -> str:
         return (
             "{% if messages[0]['role'] == 'system' %}"
-            "{{ '<s>[UNUSED_TOKEN_146]' + 'system\\n' + messages[0]['content'] + '[UNUSED_TOKEN_145]' + '\\n' }}"
+            "{{ '<s><|im_start|>' + 'system\\n' + messages[0]['content'] + '<|im_end|>' + '\\n' }}"
             "{% else %}"
-            "{{ '<s>[UNUSED_TOKEN_146]' + 'system\\n' + system_prompt + '[UNUSED_TOKEN_145]' + '\\n' }}"
+            "{{ '<s><|im_start|>' + 'system\\n' + system_prompt + '<|im_end|>' + '\\n' }}"
             "{% endif %}"
             "{% for message in messages %}"
             "{% if messages[0]['role'] != 'system' %}"
-            "{{ '[UNUSED_TOKEN_146]' + message['role'] + '\\n' + message['content'] + '[UNUSED_TOKEN_145]' + '\\n' }}"
+            "{{ '<|im_start|>' + message['role'] + '\\n' + message['content'] + '<|im_end|>' + '\\n' }}"
             "{% endif %}"
             "{% endfor %}"
             "{% if add_generation_prompt %}"
-            "{{ '[UNUSED_TOKEN_146]assistant\\n' }}"
+            "{{ '<|im_start|>assistant\\n' }}"
             "{% endif %}"
         )
 
 
 class BaiChuanTemplate(BaseTemplate):
 
     name = "baichuan"
@@ -1193,44 +1235,45 @@
             "{{ message['content'] + '</s>' }}"
             "{% endif %}"
             "{% endfor %}"
         )
 
 
 class OrionStarTemplate(BaseTemplate):
-    """ https://huggingface.co/OrionStarAI/OrionStar-Yi-34B-Chat/blob/fc0420da8cd5ea5b8f36760c1b14e0a718447e1f/generation_utils.py#L5 """
+    """ https://huggingface.co/OrionStarAI/Orion-14B-Chat/blob/4de9f928abf60f8f3a3f4d7f972f4807aa57c573/generation_utils.py#L12 """
 
     name = "orionstar"
-    allow_models = ["orionstar"]
+    allow_models = ["orion"]
     stop = {
-        "strings": ["<|endoftext|>"],
+        "strings": ["</s>"],
     }
 
     @property
     def template(self) -> str:
         return (
-            "{{ '<|startoftext|>' }}"
+            "{{ '<s>' }}"
             "{% for message in messages %}"
             "{% if message['role'] == 'user' %}"
-            "{{ 'Human: ' + message['content'] + '\\n\\nAssistant: <|endoftext|>' }}"
+            "{{ 'Human: ' + message['content'] + '\\n\\nAssistant: </s>' }}"
             "{% elif message['role'] == 'assistant' %}"
-            "{{ message['content'] + '<|endoftext|>' }}"
+            "{{ message['content'] + '</s>>' }}"
             "{% endif %}"
             "{% endfor %}"
         )
 
 
 class YiAITemplate(BaseTemplate):
     """ https://huggingface.co/01-ai/Yi-34B-Chat/blob/main/tokenizer_config.json """
 
     name = "yi"
     allow_models = ["yi"]
     stop = {
         "strings": ["<|endoftext|>", "<|im_end|>"],
-        "token_ids": [2, 6, 7, 8],  # "<|endoftext|>", "<|im_start|>", "<|im_end|>", "<|im_sep|>"
+        # "<|endoftext|>", "<|im_start|>", "<|im_end|>", "<|im_sep|>"
+        "token_ids": [2, 6, 7, 8],
     }
 
     @property
     def template(self) -> str:
         return (
             "{% for message in messages %}"
             "{{ '<|im_start|>' + message['role'] + '\\n' + message['content'] + '<|im_end|>' + '\\n' }}"
@@ -1265,27 +1308,27 @@
             "{% elif message['role'] == 'assistant' %}"
             "{{ message['content'] }}"
             "{% endif %}"
             "{% endfor %}"
         )
 
 
-class MixtralTemplate(BaseTemplate):
+class MistralTemplate(BaseTemplate):
     """ https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2/blob/main/tokenizer_config.json """
 
-    name = "mixtral"
-    allow_models = ["mixtral"]
+    name = "mistral"
+    allow_models = ["mistral"]
     stop = {
         "strings": ["[INST]", "[/INST]"],
     }
 
     @property
     def template(self) -> str:
         return (
-            "{{ bos_token }}"
+            "{{ '<s>' }}"
             "{% for message in messages %}"
             "{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}"
             "{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}"
             "{% endif %}"
             "{% if message['role'] == 'user' %}"
             "{{ '[INST] ' + message['content'] + ' [/INST]' }}"
             "{% elif message['role'] == 'assistant' %}"
@@ -1295,50 +1338,68 @@
             "{% endif %}"
             "{% endfor %}"
         )
 
 
 register_prompt_adapter(AlpacaTemplate)
 register_prompt_adapter(AquilaChatTemplate)
+
 register_prompt_adapter(BaiChuanTemplate)
 register_prompt_adapter(BaiChuan2Template)
 register_prompt_adapter(BelleTemplate)
 register_prompt_adapter(BlueLMTemplate)
+
 register_prompt_adapter(ChatglmTemplate)
 register_prompt_adapter(Chatglm2Template)
 register_prompt_adapter(Chatglm3Template)
 register_prompt_adapter(ChineseAlpaca2Template)
+
 register_prompt_adapter(DeepseekTemplate)
 register_prompt_adapter(DeepseekCoderTemplate)
+
 register_prompt_adapter(FireflyTemplate)
 register_prompt_adapter(FireflyForQwenTemplate)
+
 register_prompt_adapter(HuatuoTemplate)
+
 register_prompt_adapter(InternLMTemplate)
 register_prompt_adapter(InternLM2Template)
+
 register_prompt_adapter(Llama2Template)
-register_prompt_adapter(MixtralTemplate)
+
+register_prompt_adapter(MistralTemplate)
 register_prompt_adapter(MossTemplate)
+
 register_prompt_adapter(OctopackTemplate)
 register_prompt_adapter(OpenBuddyTemplate)
 register_prompt_adapter(OrionStarTemplate)
+
 register_prompt_adapter(PhindTemplate)
 register_prompt_adapter(PhoenixTemplate)
+
 register_prompt_adapter(QwenTemplate)
+register_prompt_adapter(Qwen2Template)
+
 register_prompt_adapter(StarChatTemplate)
 register_prompt_adapter(SusChatTemplate)
+
 register_prompt_adapter(VicunaTemplate)
+
 register_prompt_adapter(XuanYuanTemplate)
 register_prompt_adapter(XverseTemplate)
+
 register_prompt_adapter(YiAITemplate)
+
 register_prompt_adapter(ZephyrTemplate)
+
 register_prompt_adapter(BaseTemplate)
 
 
 if __name__ == '__main__':
     chat = [
         {"role": "user", "content": "Hello, how are you?"},
         {"role": "assistant", "content": "I'm doing great. How can I help you today?"},
         {"role": "user", "content": "I'd like to show off how chat templating works!"},
     ]
-    template = get_prompt_adapter(prompt_name="internlm2")
+    template = get_prompt_adapter(prompt_name="mistral")
     messages = template.postprocess_messages(chat)
     print(template.apply_chat_template(messages))
```

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/baichuan.py` & `langchain_llm-0.4.15/langchain_llm/generation/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/chatglm.py` & `langchain_llm-0.4.15/langchain_llm/generation/chatglm.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/qwen.py` & `langchain_llm-0.4.15/langchain_llm/generation/qwen.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/stream.py` & `langchain_llm-0.4.15/langchain_llm/generation/stream.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/utils.py` & `langchain_llm-0.4.15/langchain_llm/generation/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/generation/xverse.py` & `langchain_llm-0.4.15/langchain_llm/generation/xverse.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/langchain_llm/utils.py` & `langchain_llm-0.4.15/langchain_llm/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/pyproject.toml` & `langchain_llm-0.4.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-llm"
-version = "0.1.19"
+version = "0.4.15"
 description = "langchain llm wrapper"
 authors = ["xusenlin <xusenlin@dnect.cn>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 openai = ">=1.6.1"
```

### Comparing `langchain_llm-0.1.19/README.md` & `langchain_llm-0.4.15/README.md`

 * *Files identical despite different names*

### Comparing `langchain_llm-0.1.19/PKG-INFO` & `langchain_llm-0.4.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-llm
-Version: 0.1.19
+Version: 0.4.15
 Summary: langchain llm wrapper
 Author: xusenlin
 Author-email: xusenlin@dnect.cn
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

