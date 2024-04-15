# Comparing `tmp/rag_doc_search-0.1.4.tar.gz` & `tmp/rag_doc_search-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_doc_search-0.1.4.tar", max compression
+gzip compressed data, was "rag_doc_search-0.1.5.tar", max compression
```

## Comparing `rag_doc_search-0.1.4.tar` & `rag_doc_search-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3270 2024-03-13 11:04:32.283414 rag_doc_search-0.1.4/README.md
--rw-r--r--   0        0        0      675 2024-04-10 15:18:09.919501 rag_doc_search-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.4/rag_doc_search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.4/rag_doc_search/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/__init__.py
--rw-r--r--   0        0        0     2991 2024-04-10 15:17:55.474828 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/azure_chatbot_model.py
--rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
--rw-r--r--   0        0        0     4687 2024-03-07 06:31:57.301574 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/chatbot_model.py
--rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/openai_chatbot_model.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.4/rag_doc_search/src/enums/__init__.py
--rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.4/rag_doc_search/src/enums/provider.py
--rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.4/rag_doc_search/src/enums/search_type.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.4/rag_doc_search/src/models/__init__.py
--rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.4/rag_doc_search/src/models/chat_response.py
--rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.4/rag_doc_search/src/models/user_prompt.py
--rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.4/rag_doc_search/src/prompt_templates/default_prompt_templates.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.4/rag_doc_search/utils/__init__.py
--rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.4/rag_doc_search/utils/callback.py
--rw-r--r--   0        0        0    14038 2024-04-09 09:50:20.321385 rag_doc_search-0.1.4/rag_doc_search/utils/config.py
--rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.4/rag_doc_search/utils/miscellaneous.py
--rw-r--r--   0        0        0     4259 1970-01-01 00:00:00.000000 rag_doc_search-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3303 2024-04-15 11:58:43.574400 rag_doc_search-0.1.5/README.md
+-rw-r--r--   0        0        0      675 2024-04-15 11:57:41.852052 rag_doc_search-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.5/rag_doc_search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.5/rag_doc_search/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/__init__.py
+-rw-r--r--   0        0        0     2991 2024-04-15 11:57:02.681552 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/azure_chatbot_model.py
+-rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
+-rw-r--r--   0        0        0     4691 2024-04-15 11:49:29.070013 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/chatbot_model.py
+-rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/openai_chatbot_model.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.5/rag_doc_search/src/enums/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.5/rag_doc_search/src/enums/provider.py
+-rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.5/rag_doc_search/src/enums/search_type.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.5/rag_doc_search/src/models/__init__.py
+-rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.5/rag_doc_search/src/models/chat_response.py
+-rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.5/rag_doc_search/src/models/user_prompt.py
+-rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.5/rag_doc_search/src/prompt_templates/default_prompt_templates.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.5/rag_doc_search/utils/__init__.py
+-rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.5/rag_doc_search/utils/callback.py
+-rw-r--r--   0        0        0    14038 2024-04-15 11:37:44.195295 rag_doc_search-0.1.5/rag_doc_search/utils/config.py
+-rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.5/rag_doc_search/utils/miscellaneous.py
+-rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 rag_doc_search-0.1.5/PKG-INFO
```

### Comparing `rag_doc_search-0.1.4/README.md` & `rag_doc_search-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 ## Overview
 This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs). RAG enhances prediction quality by incorporating external data storage during inference, enabling the construction of more contextually rich prompts. Leveraging combinations of context, history, and up-to-date knowledge, RAG LLMs empower users to generate more accurate and relevant responses. This package streamlines the integration of RAG capabilities into applications, facilitating the creation of more intelligent and context-aware conversational agents, search engines, and text generation systems.
 
 ## Config Json
 ```
 {
-    "ai_provider": "OPENAI" | "BEDROCK",
-    "embeddings_model": "<embedding model of openai or bedrock as per ai_provider>",
+    "ai_provider": "OPENAI" | "BEDROCK" | "AZURE_OPENAI",
+    "embeddings_model": "<embedding model of openai or bedrock or azure openai as per ai_provider>",
     "llm": "<llm model of openai or bedrock as per ai_provider>",
     "llm_temperature": "<llm model of temperature>",
     "llm_max_output_tokens": "<llm model of mac output token>",
     "vector_store_provider": "FAISS" | "PGVector",
     "faiss_vector_embeddings_location": "./data", provide only if vector_store_provider is FAISS
     "faiss_index_name": "fiass-db", provide only if vector_store_provider is FAISS
     "name": "<name of your project>",
```

### Comparing `rag_doc_search-0.1.4/pyproject.toml` & `rag_doc_search-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag-doc-search"
-version = "0.1.4"
+version = "0.1.5"
 description = "This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs)."
 authors = ["Harshad Kadam <harshad.kadam@sourcefuse.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 boto3 = "^1.34.55"
```

### Comparing `rag_doc_search-0.1.4/rag_doc_search/__init__.py` & `rag_doc_search-0.1.5/rag_doc_search/__init__.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/azure_chatbot_model.py` & `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/azure_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/bedrock_chatbot_model.py` & `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/bedrock_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/chatbot_model.py` & `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/chatbot_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         )
 
         qa = RetrievalQA.from_chain_type(
             llm=cl_llm,
             chain_type="stuff",
             retriever=self.vector_store.as_retriever(
                 search_type=self.retriever_args.get("search_type"),
-                search_args=self.retriever_args.get("search_args"),
+                search_kwargs=self.retriever_args.get("search_args"),
             ),
             return_source_documents=True,
             chain_type_kwargs={"prompt": PROMPT},
         )
         return qa
 
     def create_conversational_qa_chain(
@@ -106,15 +106,15 @@
         # the condense prompt for Claude
         condense_prompt = PromptTemplate.from_template(DEFAULT_CHAT_HISTORY_PROMPT)
 
         qa = ConversationalRetrievalChain.from_llm(
             llm=cl_llm,
             retriever=self.vector_store.as_retriever(
                 search_type=self.retriever_args.get("search_type"),
-                search_args=self.retriever_args.get("search_args"),
+                search_kwargs=self.retriever_args.get("search_args"),
             ),
             # return_source_documents=True,
             memory=memory_chain,
             get_chat_history=get_chat_history,
             condense_question_prompt=condense_prompt,
             chain_type="stuff",  # 'refine',
         )
```

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/openai_chatbot_model.py` & `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/openai_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/enums/provider.py` & `rag_doc_search-0.1.5/rag_doc_search/src/enums/provider.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/enums/search_type.py` & `rag_doc_search-0.1.5/rag_doc_search/src/enums/search_type.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/models/chat_response.py` & `rag_doc_search-0.1.5/rag_doc_search/src/models/chat_response.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/src/prompt_templates/default_prompt_templates.py` & `rag_doc_search-0.1.5/rag_doc_search/src/prompt_templates/default_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/utils/callback.py` & `rag_doc_search-0.1.5/rag_doc_search/utils/callback.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/rag_doc_search/utils/config.py` & `rag_doc_search-0.1.5/rag_doc_search/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,23 +180,23 @@
 
         search_args = retriever_args.get("search_args", {})
 
         self.retriever_search_args_k = int(search_args.get("k", 4))
         self.retriever_search_args_fetch_k = int(search_args.get("fetch_k", 20))
 
         self.retriever_search_args_lambda_mult = float(
-            config_json.get("lambda_mult", 0.5)
+            search_args.get("lambda_mult", 0.5)
         )
         if not (0 <= self.retriever_search_args_lambda_mult <= 1):
             raise ValueError(
                 "Invalid lambda_mult value in config -> retriever -> search args"
             )
 
         self.retriever_search_args_score_threshold = float(
-            config_json.get("score_threshold", 0)
+            search_args.get("score_threshold", 0)
         )
 
     def _validate_and_initialize(self, config_json: dict):
         """
         Validates and initializes various configuration properties based on the provided JSON.
 
         Parameters:
@@ -286,15 +286,15 @@
         Raises:
         - `ValueError`: If the retriever configuration is invalid or missing required properties.
         """
         retriever_args = {
             "k": self.retriever_search_args_k,
             "fetch_k": self.retriever_search_args_fetch_k,
         }
-        match self.vector_store_provider:
+        match self.retriever_search_type:
             case RetrieverSearchType.mmr:
                 if self.retriever_search_args_lambda_mult <= 0:
                     retriever_args["lambda_mult"] = self.retriever_search_args_fetch_k
             case RetrieverSearchType.similarity_score_threshold:
                 retriever_args[
                     "score_threshold"
                 ] = self.retriever_search_args_score_threshold
```

### Comparing `rag_doc_search-0.1.4/rag_doc_search/utils/miscellaneous.py` & `rag_doc_search-0.1.5/rag_doc_search/utils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.4/PKG-INFO` & `rag_doc_search-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-doc-search
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs).
 Author: Harshad Kadam
 Author-email: harshad.kadam@sourcefuse.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,16 +25,16 @@
 
 ## Overview
 This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs). RAG enhances prediction quality by incorporating external data storage during inference, enabling the construction of more contextually rich prompts. Leveraging combinations of context, history, and up-to-date knowledge, RAG LLMs empower users to generate more accurate and relevant responses. This package streamlines the integration of RAG capabilities into applications, facilitating the creation of more intelligent and context-aware conversational agents, search engines, and text generation systems.
 
 ## Config Json
 ```
 {
-    "ai_provider": "OPENAI" | "BEDROCK",
-    "embeddings_model": "<embedding model of openai or bedrock as per ai_provider>",
+    "ai_provider": "OPENAI" | "BEDROCK" | "AZURE_OPENAI",
+    "embeddings_model": "<embedding model of openai or bedrock or azure openai as per ai_provider>",
     "llm": "<llm model of openai or bedrock as per ai_provider>",
     "llm_temperature": "<llm model of temperature>",
     "llm_max_output_tokens": "<llm model of mac output token>",
     "vector_store_provider": "FAISS" | "PGVector",
     "faiss_vector_embeddings_location": "./data", provide only if vector_store_provider is FAISS
     "faiss_index_name": "fiass-db", provide only if vector_store_provider is FAISS
     "name": "<name of your project>",
```

