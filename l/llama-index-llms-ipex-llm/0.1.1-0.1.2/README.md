# Comparing `tmp/llama_index_llms_ipex_llm-0.1.1.tar.gz` & `tmp/llama_index_llms_ipex_llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ipex_llm-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_llms_ipex_llm-0.1.2.tar", max compression
```

## Comparing `llama_index_llms_ipex_llm-0.1.1.tar` & `llama_index_llms_ipex_llm-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      714 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/BUILD
--rw-r--r--   0        0        0       75 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/__init__.py
--rw-r--r--   0        0        0    15730 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/base.py
--rw-r--r--   0        0        0     1641 2024-04-08 18:18:42.143947 llama_index_llms_ipex_llm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      714 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/README.md
+-rw-r--r--   0        0        0       17 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/BUILD
+-rw-r--r--   0        0        0       75 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/__init__.py
+-rw-r--r--   0        0        0    20955 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/base.py
+-rw-r--r--   0        0        0     1642 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.2/PKG-INFO
```

### Comparing `llama_index_llms_ipex_llm-0.1.1/README.md` & `llama_index_llms_ipex_llm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_ipex_llm-0.1.1/llama_index/llms/ipex_llm/base.py` & `llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# This file is adapted from
+# https://github.com/run-llama/llama_index/blob/main/llama-index-integrations/
+# llms/llama-index-llms-huggingface/llama_index/llms/huggingface/base.py
+
 import logging
 from threading import Thread
 from typing import Any, Callable, List, Optional, Sequence
 
 import torch
 from llama_index.core.base.llms.types import (
     ChatMessage,
@@ -149,14 +153,15 @@
         generate_kwargs: Optional[dict] = None,
         is_chat_model: Optional[bool] = False,
         callback_manager: Optional[CallbackManager] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
         pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
         output_parser: Optional[BaseOutputParser] = None,
+        low_bit_model: Optional[bool] = False,
     ) -> None:
         """
         Construct IpexLLM.
 
         Args:
             context_window: The maximum number of tokens available for input.
             max_new_tokens: The maximum number of tokens to generate.
@@ -181,47 +186,21 @@
             pydantic_program_mode: DEFAULT.
             output_parser: BaseOutputParser.
 
         Returns:
             None.
         """
         model_kwargs = model_kwargs or {}
-        from ipex_llm.transformers import AutoModelForCausalLM
 
         if model:
             self._model = model
         else:
-            try:
-                if load_in_low_bit:
-                    self._model = AutoModelForCausalLM.from_pretrained(
-                        model_name,
-                        load_in_low_bit=load_in_low_bit,
-                        use_cache=True,
-                        trust_remote_code=True,
-                        **model_kwargs,
-                    )
-                else:
-                    self._model = AutoModelForCausalLM.from_pretrained(
-                        model_name,
-                        load_in_4bit=load_in_4bit,
-                        use_cache=True,
-                        trust_remote_code=True,
-                        **model_kwargs,
-                    )
-            except Exception:
-                from ipex_llm.transformers import AutoModel
-
-                if load_in_low_bit:
-                    self._model = AutoModel.from_pretrained(
-                        model_name, load_in_low_bit=load_in_low_bit, **model_kwargs
-                    )
-                else:
-                    self._model = AutoModel.from_pretrained(
-                        model_name, load_in_4bit=load_in_4bit, **model_kwargs
-                    )
+            self._model = self._load_model(
+                low_bit_model, load_in_4bit, load_in_low_bit, model_name, model_kwargs
+            )
 
         if "xpu" in device_map:
             self._model = self._model.to(device_map)
 
         # check context_window
         config_dict = self._model.config.to_dict()
         model_context_window = int(
@@ -238,33 +217,35 @@
         tokenizer_kwargs = tokenizer_kwargs or {}
         if "max_length" not in tokenizer_kwargs:
             tokenizer_kwargs["max_length"] = context_window
 
         if tokenizer:
             self._tokenizer = tokenizer
         else:
-            print(f"load tokenizer: {tokenizer_name}")
             try:
                 self._tokenizer = AutoTokenizer.from_pretrained(
                     tokenizer_name, **tokenizer_kwargs
                 )
             except Exception:
                 self._tokenizer = LlamaTokenizer.from_pretrained(
                     tokenizer_name, trust_remote_code=True
                 )
 
         if tokenizer_name != model_name:
             logger.warning(
                 f"The model `{model_name}` and tokenizer `{tokenizer_name}` "
-                f"are different, please ensure that they are compatible."
+                f"are from different paths, please ensure that they are compatible."
             )
 
         # setup stopping criteria
         stopping_ids_list = stopping_ids or []
 
+        if self._tokenizer.pad_token is None:
+            self._tokenizer.pad_token = self._tokenizer.eos_token
+
         class StopOnTokens(StoppingCriteria):
             def __call__(
                 self,
                 input_ids: torch.LongTensor,
                 scores: torch.FloatTensor,
                 **kwargs: Any,
             ) -> bool:
@@ -293,27 +274,174 @@
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
             pydantic_program_mode=pydantic_program_mode,
             output_parser=output_parser,
         )
 
     @classmethod
+    def from_model_id(
+        cls,
+        context_window: int = DEFAULT_CONTEXT_WINDOW,
+        max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
+        tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
+        model_name: str = DEFAULT_HUGGINGFACE_MODEL,
+        load_in_4bit: Optional[bool] = True,
+        load_in_low_bit: Optional[str] = None,
+        model: Optional[Any] = None,
+        tokenizer: Optional[Any] = None,
+        device_map: Optional[str] = "auto",
+        stopping_ids: Optional[List[int]] = None,
+        tokenizer_kwargs: Optional[dict] = None,
+        tokenizer_outputs_to_remove: Optional[list] = None,
+        model_kwargs: Optional[dict] = None,
+        generate_kwargs: Optional[dict] = None,
+        is_chat_model: Optional[bool] = False,
+        callback_manager: Optional[CallbackManager] = None,
+        messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
+        completion_to_prompt: Optional[Callable[[str], str]] = None,
+        pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
+        output_parser: Optional[BaseOutputParser] = None,
+    ):
+        return cls(
+            context_window=context_window,
+            max_new_tokens=max_new_tokens,
+            tokenizer_name=tokenizer_name,
+            model_name=model_name,
+            load_in_4bit=load_in_4bit,
+            load_in_low_bit=load_in_low_bit,
+            model=model,
+            tokenizer=tokenizer,
+            device_map=device_map,
+            stopping_ids=stopping_ids,
+            tokenizer_kwargs=tokenizer_kwargs,
+            tokenizer_outputs_to_remove=tokenizer_outputs_to_remove,
+            model_kwargs=model_kwargs,
+            generate_kwargs=generate_kwargs,
+            is_chat_model=is_chat_model,
+            callback_manager=callback_manager,
+            messages_to_prompt=messages_to_prompt,
+            completion_to_prompt=completion_to_prompt,
+            pydantic_program_mode=pydantic_program_mode,
+            output_parser=output_parser,
+            low_bit_model=False,
+        )
+
+    @classmethod
+    def from_model_id_low_bit(
+        cls,
+        context_window: int = DEFAULT_CONTEXT_WINDOW,
+        max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
+        tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
+        model_name: str = DEFAULT_HUGGINGFACE_MODEL,
+        model: Optional[Any] = None,
+        tokenizer: Optional[Any] = None,
+        device_map: Optional[str] = "auto",
+        stopping_ids: Optional[List[int]] = None,
+        tokenizer_kwargs: Optional[dict] = None,
+        tokenizer_outputs_to_remove: Optional[list] = None,
+        model_kwargs: Optional[dict] = None,
+        generate_kwargs: Optional[dict] = None,
+        is_chat_model: Optional[bool] = False,
+        callback_manager: Optional[CallbackManager] = None,
+        messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
+        completion_to_prompt: Optional[Callable[[str], str]] = None,
+        pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
+        output_parser: Optional[BaseOutputParser] = None,
+    ):
+        return cls(
+            context_window=context_window,
+            max_new_tokens=max_new_tokens,
+            tokenizer_name=tokenizer_name,
+            model_name=model_name,
+            model=model,
+            tokenizer=tokenizer,
+            device_map=device_map,
+            stopping_ids=stopping_ids,
+            tokenizer_kwargs=tokenizer_kwargs,
+            tokenizer_outputs_to_remove=tokenizer_outputs_to_remove,
+            model_kwargs=model_kwargs,
+            generate_kwargs=generate_kwargs,
+            is_chat_model=is_chat_model,
+            callback_manager=callback_manager,
+            messages_to_prompt=messages_to_prompt,
+            completion_to_prompt=completion_to_prompt,
+            pydantic_program_mode=pydantic_program_mode,
+            output_parser=output_parser,
+            low_bit_model=True,
+        )
+
+    @classmethod
     def class_name(cls) -> str:
         return "IpexLLM"
 
     @property
     def metadata(self) -> LLMMetadata:
         """LLM metadata."""
         return LLMMetadata(
             context_window=self.context_window,
             num_output=self.max_new_tokens,
             model_name=self.model_name,
             is_chat_model=self.is_chat_model,
         )
 
+    def _load_model(
+        self,
+        low_bit_model: bool,
+        load_in_4bit: bool,
+        load_in_low_bit: str,
+        model_name: str,
+        model_kwargs: Any,
+    ) -> Any:
+        """Attempts to load a model with AutoModelForCausalLM and falls back to AutoModel on failure."""
+        from ipex_llm.transformers import AutoModelForCausalLM, AutoModel
+
+        load_kwargs = {"use_cache": True, "trust_remote_code": True}
+
+        if not low_bit_model:
+            if load_in_low_bit is not None:
+                load_function_name = "from_pretrained"
+                load_kwargs["load_in_low_bit"] = load_in_low_bit
+            else:
+                load_function_name = "from_pretrained"
+                load_kwargs["load_in_4bit"] = load_in_4bit
+        else:
+            load_function_name = "load_low_bit"
+
+        try:
+            # Attempt to load with AutoModelForCausalLM
+            return self._load_model_general(
+                AutoModelForCausalLM,
+                load_function_name,
+                model_name,
+                load_kwargs,
+                model_kwargs,
+            )
+        except Exception:
+            # Fallback to AutoModel if there's an exception
+            return self._load_model_general(
+                AutoModel, load_function_name, model_name, load_kwargs, model_kwargs
+            )
+
+    def _load_model_general(
+        self,
+        model_class: Any,
+        load_function_name: str,
+        model_name: str,
+        load_kwargs,
+        model_kwargs: dict,
+    ) -> Any:
+        """General function to attempt to load a model."""
+        try:
+            load_function = getattr(model_class, load_function_name)
+            return load_function(model_name, **{**load_kwargs, **model_kwargs})
+        except Exception as e:
+            logger.error(
+                f"Failed to load model using {model_class.__name__}.{load_function_name}: {e}"
+            )
+
     def _tokenizer_messages_to_prompt(self, messages: Sequence[ChatMessage]) -> str:
         """
         Use the tokenizer to convert messages to prompt. Fallback to generic.
 
         Args:
             messages: Sequence of ChatMessage.
 
@@ -367,14 +495,15 @@
         for key in self.tokenizer_outputs_to_remove:
             if key in input_ids:
                 input_ids.pop(key, None)
         tokens = self._model.generate(
             **input_ids,
             max_new_tokens=self.max_new_tokens,
             stopping_criteria=self._stopping_criteria,
+            pad_token_id=self._tokenizer.pad_token_id,
             **self.generate_kwargs,
         )
         completion_tokens = tokens[0][input_ids["input_ids"].size(1) :]
         completion = self._tokenizer.decode(completion_tokens, skip_special_tokens=True)
 
         return CompletionResponse(text=completion, raw={"model_output": tokens})
 
@@ -409,14 +538,15 @@
             self._tokenizer, skip_prompt=True, skip_special_tokens=True
         )
         generation_kwargs = dict(
             input_ids=input_ids,
             streamer=streamer,
             max_new_tokens=self.max_new_tokens,
             stopping_criteria=self._stopping_criteria,
+            pad_token_id=self._tokenizer.pad_token_id,
             **self.generate_kwargs,
         )
         thread = Thread(target=self._model.generate, kwargs=generation_kwargs)
         thread.start()
 
         # create generator based off of streamer
         def gen() -> CompletionResponseGen:
```

### Comparing `llama_index_llms_ipex_llm-0.1.1/pyproject.toml` & `llama_index_llms_ipex_llm-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 IpexLLM = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 # Remove venv skip when integrated with pre-commit
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
-python_version = "3.9"
+python_version = "3.11"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ipex-llm integration"
 license = "MIT"
 name = "llama-index-llms-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.0"
 torch = "<2.2.0"
 ipex-llm = {allow-prereleases = true, extras = ["all"], version = "*"}
```

### Comparing `llama_index_llms_ipex_llm-0.1.1/PKG-INFO` & `llama_index_llms_ipex_llm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ipex-llm
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index llms ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

