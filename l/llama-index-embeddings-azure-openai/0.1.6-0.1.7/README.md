# Comparing `tmp/llama_index_embeddings_azure_openai-0.1.6.tar.gz` & `tmp/llama_index_embeddings_azure_openai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_azure_openai-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_embeddings_azure_openai-0.1.7.tar", max compression
```

## Comparing `llama_index_embeddings_azure_openai-0.1.6.tar` & `llama_index_embeddings_azure_openai-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2024-02-13 13:53:01.597587 llama_index_embeddings_azure_openai-0.1.6/README.md
--rw-r--r--   0        0        0      193 2024-02-13 13:53:01.597848 llama_index_embeddings_azure_openai-0.1.6/llama_index/embeddings/azure_openai/__init__.py
--rw-r--r--   0        0        0     4323 2024-02-20 22:37:41.279576 llama_index_embeddings_azure_openai-0.1.6/llama_index/embeddings/azure_openai/base.py
--rw-r--r--   0        0        0     1621 2024-02-21 16:59:38.112409 llama_index_embeddings_azure_openai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 llama_index_embeddings_azure_openai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-15 18:30:41.263504 llama_index_embeddings_azure_openai-0.1.7/README.md
+-rw-r--r--   0        0        0      193 2024-04-15 18:30:41.263504 llama_index_embeddings_azure_openai-0.1.7/llama_index/embeddings/azure_openai/__init__.py
+-rw-r--r--   0        0        0     4712 2024-04-15 18:30:41.263504 llama_index_embeddings_azure_openai-0.1.7/llama_index/embeddings/azure_openai/base.py
+-rw-r--r--   0        0        0     1560 2024-04-15 18:30:41.263504 llama_index_embeddings_azure_openai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 llama_index_embeddings_azure_openai-0.1.7/PKG-INFO
```

### Comparing `llama_index_embeddings_azure_openai-0.1.6/llama_index/embeddings/azure_openai/base.py` & `llama_index_embeddings_azure_openai-0.1.7/llama_index/embeddings/azure_openai/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from llama_index.embeddings.openai import (
     OpenAIEmbedding,
     OpenAIEmbeddingMode,
     OpenAIEmbeddingModelType,
 )
 from llama_index.llms.azure_openai.utils import resolve_from_aliases
 from openai import AsyncAzureOpenAI, AzureOpenAI
+from openai.lib.azure import AzureADTokenProvider
 
 
 class AzureOpenAIEmbedding(OpenAIEmbedding):
     azure_endpoint: Optional[str] = Field(
         default=None, description="The Azure endpoint to use."
     )
     azure_deployment: Optional[str] = Field(
@@ -23,28 +24,33 @@
     )
 
     api_base: str = Field(default="", description="The base URL for Azure deployment.")
     api_version: str = Field(
         default="", description="The version for Azure OpenAI API."
     )
 
+    azure_ad_token_provider: AzureADTokenProvider = Field(
+        default=None, description="Callback function to provide Azure AD token."
+    )
+
     _client: AzureOpenAI = PrivateAttr()
     _aclient: AsyncAzureOpenAI = PrivateAttr()
 
     def __init__(
         self,
         mode: str = OpenAIEmbeddingMode.TEXT_SEARCH_MODE,
         model: str = OpenAIEmbeddingModelType.TEXT_EMBED_ADA_002,
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         api_key: Optional[str] = None,
         api_version: Optional[str] = None,
         # azure specific
         azure_endpoint: Optional[str] = None,
         azure_deployment: Optional[str] = None,
+        azure_ad_token_provider: AzureADTokenProvider = None,
         deployment_name: Optional[str] = None,
         max_retries: int = 10,
         reuse_client: bool = True,
         callback_manager: Optional[CallbackManager] = None,
         # custom httpx client
         http_client: Optional[httpx.Client] = None,
         **kwargs: Any,
@@ -63,14 +69,15 @@
             model=model,
             embed_batch_size=embed_batch_size,
             additional_kwargs=additional_kwargs,
             api_key=api_key,
             api_version=api_version,
             azure_endpoint=azure_endpoint,
             azure_deployment=azure_deployment,
+            azure_ad_token_provider=azure_ad_token_provider,
             max_retries=max_retries,
             reuse_client=reuse_client,
             callback_manager=callback_manager,
             http_client=http_client,
             **kwargs,
         )
 
@@ -105,14 +112,15 @@
         if self._aclient is None:
             self._aclient = AsyncAzureOpenAI(**self._get_credential_kwargs())
         return self._aclient
 
     def _get_credential_kwargs(self) -> Dict[str, Any]:
         return {
             "api_key": self.api_key,
+            "azure_ad_token_provider": self.azure_ad_token_provider,
             "azure_endpoint": self.azure_endpoint,
             "azure_deployment": self.azure_deployment,
             "api_version": self.api_version,
             "default_headers": self.default_headers,
             "http_client": self._http_client,
         }
```

### Comparing `llama_index_embeddings_azure_openai-0.1.6/pyproject.toml` & `llama_index_embeddings_azure_openai-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.embeddings.azure_openai"
 
 [tool.llamahub.class_authors]
-AsyncAzureOpenAI = "llama-index"
-AzureOpenAI = "llama-index"
 AzureOpenAIEmbedding = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
@@ -25,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings azure openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-azure-openai"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-azure-openai = "^0.1.3"
 llama-index-embeddings-openai = "^0.1.3"
```

### Comparing `llama_index_embeddings_azure_openai-0.1.6/PKG-INFO` & `llama_index_embeddings_azure_openai-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-azure-openai
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index embeddings azure openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: llama-index-embeddings-openai (>=0.1.3,<0.2.0)
 Requires-Dist: llama-index-llms-azure-openai (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Azure Openai
```

