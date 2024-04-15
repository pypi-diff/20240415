# Comparing `tmp/llama_index_llms_azure_openai-0.1.5.tar.gz` & `tmp/llama_index_llms_azure_openai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_azure_openai-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_azure_openai-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_azure_openai-0.1.5.tar` & `llama_index_llms_azure_openai-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2024-02-28 16:59:35.767271 llama_index_llms_azure_openai-0.1.5/README.md
--rw-r--r--   0        0        0      177 2024-02-28 16:59:35.767271 llama_index_llms_azure_openai-0.1.5/llama_index/llms/azure_openai/__init__.py
--rw-r--r--   0        0        0     7018 2024-02-28 18:53:20.620827 llama_index_llms_azure_openai-0.1.5/llama_index/llms/azure_openai/base.py
--rw-r--r--   0        0        0     1245 2024-02-28 16:59:35.767271 llama_index_llms_azure_openai-0.1.5/llama_index/llms/azure_openai/utils.py
--rw-r--r--   0        0        0     1590 2024-02-28 19:01:03.937568 llama_index_llms_azure_openai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/README.md
+-rw-r--r--   0        0        0      177 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/__init__.py
+-rw-r--r--   0        0        0     8031 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/base.py
+-rw-r--r--   0        0        0     1245 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/utils.py
+-rw-r--r--   0        0        0     1590 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_azure_openai-0.1.5/llama_index/llms/azure_openai/base.py` & `llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from llama_index.llms.azure_openai.utils import (
     refresh_openai_azuread_token,
     resolve_from_aliases,
 )
 from llama_index.llms.openai import OpenAI
 from openai import AsyncAzureOpenAI
 from openai import AzureOpenAI as SyncAzureOpenAI
+from openai.lib.azure import AzureADTokenProvider
 
 
 class AzureOpenAI(OpenAI):
     """
     Azure OpenAI.
 
     To use this, you must first deploy a model on Azure OpenAI.
@@ -25,35 +26,58 @@
 
     - model: Name of the model (e.g. `text-davinci-003`)
         This in only used to decide completion vs. chat endpoint.
     - engine: This will correspond to the custom name you chose
         for your deployment when you deployed a model.
 
     You must have the following environment variables set:
-    - `OPENAI_API_VERSION`: set this to `2023-05-15`
+    - `OPENAI_API_VERSION`: set this to `2023-07-01-preview` or newer.
         This may change in the future.
     - `AZURE_OPENAI_ENDPOINT`: your endpoint should look like the following
         https://YOUR_RESOURCE_NAME.openai.azure.com/
     - `AZURE_OPENAI_API_KEY`: your API key if the api type is `azure`
 
     More information can be found here:
         https://learn.microsoft.com/en-us/azure/cognitive-services/openai/quickstart?tabs=command-line&pivots=programming-language-python
+
+    Examples:
+        `pip install llama-index-llms-azure-openai`
+
+        ```python
+        from llama_index.llms.azure_openai import AzureOpenAI
+
+        aoai_api_key = "YOUR_AZURE_OPENAI_API_KEY"
+        aoai_endpoint = "YOUR_AZURE_OPENAI_ENDPOINT"
+        aoai_api_version = "2023-07-01-preview"
+
+        llm = AzureOpenAI(
+            model="YOUR_AZURE_OPENAI_COMPLETION_MODEL_NAME",
+            deployment_name="YOUR_AZURE_OPENAI_COMPLETION_DEPLOYMENT_NAME",
+            api_key=aoai_api_key,
+            azure_endpoint=aoai_endpoint,
+            api_version=aoai_api_version,
+        )
+        ```
     """
 
     engine: str = Field(description="The name of the deployed azure engine.")
     azure_endpoint: Optional[str] = Field(
         default=None, description="The Azure endpoint to use."
     )
     azure_deployment: Optional[str] = Field(
         default=None, description="The Azure deployment to use."
     )
     use_azure_ad: bool = Field(
         description="Indicates if Microsoft Entra ID (former Azure AD) is used for token authentication"
     )
 
+    azure_ad_token_provider: AzureADTokenProvider = Field(
+        default=None, description="Callback function to provide Azure AD token."
+    )
+
     _azure_ad_token: Any = PrivateAttr(default=None)
     _client: SyncAzureOpenAI = PrivateAttr()
     _aclient: AsyncAzureOpenAI = PrivateAttr()
 
     def __init__(
         self,
         model: str = "gpt-35-turbo",
@@ -65,14 +89,15 @@
         timeout: float = 60.0,
         reuse_client: bool = True,
         api_key: Optional[str] = None,
         api_version: Optional[str] = None,
         # azure specific
         azure_endpoint: Optional[str] = None,
         azure_deployment: Optional[str] = None,
+        azure_ad_token_provider: AzureADTokenProvider = None,
         use_azure_ad: bool = False,
         callback_manager: Optional[CallbackManager] = None,
         # aliases for engine
         deployment_name: Optional[str] = None,
         deployment_id: Optional[str] = None,
         deployment: Optional[str] = None,
         # custom httpx client
@@ -104,14 +129,15 @@
             additional_kwargs=additional_kwargs,
             max_retries=max_retries,
             timeout=timeout,
             reuse_client=reuse_client,
             api_key=api_key,
             azure_endpoint=azure_endpoint,
             azure_deployment=azure_deployment,
+            azure_ad_token_provider=azure_ad_token_provider,
             use_azure_ad=use_azure_ad,
             api_version=api_version,
             callback_manager=callback_manager,
             http_client=http_client,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
@@ -163,14 +189,15 @@
 
         return {
             "api_key": self.api_key,
             "max_retries": self.max_retries,
             "timeout": self.timeout,
             "azure_endpoint": self.azure_endpoint,
             "azure_deployment": self.azure_deployment,
+            "azure_ad_token_provider": self.azure_ad_token_provider,
             "api_version": self.api_version,
             "default_headers": self.default_headers,
             "http_client": self._http_client,
             **kwargs,
         }
 
     def _get_model_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
```

### Comparing `llama_index_llms_azure_openai-0.1.5/llama_index/llms/azure_openai/utils.py` & `llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_azure_openai-0.1.5/pyproject.toml` & `llama_index_llms_azure_openai-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms azure openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-azure-openai"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-openai = "^0.1.1"
 azure-identity = "^1.15.0"
 httpx = "*"
```

### Comparing `llama_index_llms_azure_openai-0.1.5/PKG-INFO` & `llama_index_llms_azure_openai-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-azure-openai
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms azure openai integration
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
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: httpx
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Azure Openai
```

