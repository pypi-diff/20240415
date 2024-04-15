# Comparing `tmp/codeqai-0.0.8.tar.gz` & `tmp/codeqai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeqai-0.0.8.tar", max compression
+gzip compressed data, was "codeqai-0.0.9.tar", max compression
```

## Comparing `codeqai-0.0.8.tar` & `codeqai-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-01-13 16:01:55.306171 codeqai-0.0.8/LICENSE
--rw-r--r--   0        0        0     5444 2024-01-13 16:01:55.306171 codeqai-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/__init__.py
--rw-r--r--   0        0        0       92 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/__main__.py
--rw-r--r--   0        0        0     7318 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/app.py
--rw-r--r--   0        0        0     1905 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/cache.py
--rw-r--r--   0        0        0     2307 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/codeparser.py
--rw-r--r--   0        0        0     6024 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/config.py
--rw-r--r--   0        0        0      816 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/constants.py
--rw-r--r--   0        0        0     3745 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/embeddings.py
--rw-r--r--   0        0        0     5467 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/llm.py
--rw-r--r--   0        0        0     2188 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/repo.py
--rw-r--r--   0        0        0      742 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/__init__.py
--rw-r--r--   0        0        0     2587 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter.py
--rw-r--r--   0        0        0     1021 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_c.py
--rw-r--r--   0        0        0     1029 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_cpp.py
--rw-r--r--   0        0        0     2580 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_cs.py
--rw-r--r--   0        0        0      427 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_go.py
--rw-r--r--   0        0        0      461 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_java.py
--rw-r--r--   0        0        0      481 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_js.py
--rw-r--r--   0        0        0      472 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_kt.py
--rw-r--r--   0        0        0     1930 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_py.py
--rw-r--r--   0        0        0      457 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_registry.py
--rw-r--r--   0        0        0     1957 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_rs.py
--rw-r--r--   0        0        0      481 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/treesitter/treesitter_ts.py
--rw-r--r--   0        0        0     2802 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/utils.py
--rw-r--r--   0        0        0     7880 2024-01-13 16:01:55.306171 codeqai-0.0.8/codeqai/vector_store.py
--rw-r--r--   0        0        0      624 2024-01-13 16:01:55.310171 codeqai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 codeqai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-14 17:09:20.317137 codeqai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5444 2024-01-14 17:09:20.317137 codeqai-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/__init__.py
+-rw-r--r--   0        0        0       92 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/__main__.py
+-rw-r--r--   0        0        0     7323 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/app.py
+-rw-r--r--   0        0        0     1905 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/cache.py
+-rw-r--r--   0        0        0     2307 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/codeparser.py
+-rw-r--r--   0        0        0     6024 2024-01-14 17:09:20.317137 codeqai-0.0.9/codeqai/config.py
+-rw-r--r--   0        0        0      816 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/constants.py
+-rw-r--r--   0        0        0     3745 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/embeddings.py
+-rw-r--r--   0        0        0     5467 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/llm.py
+-rw-r--r--   0        0        0     2188 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/repo.py
+-rw-r--r--   0        0        0      742 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/__init__.py
+-rw-r--r--   0        0        0     2587 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter.py
+-rw-r--r--   0        0        0     1021 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_c.py
+-rw-r--r--   0        0        0     1029 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_cpp.py
+-rw-r--r--   0        0        0     2580 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_cs.py
+-rw-r--r--   0        0        0      427 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_go.py
+-rw-r--r--   0        0        0      461 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_java.py
+-rw-r--r--   0        0        0      481 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_js.py
+-rw-r--r--   0        0        0      472 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_kt.py
+-rw-r--r--   0        0        0     1930 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_py.py
+-rw-r--r--   0        0        0      457 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_registry.py
+-rw-r--r--   0        0        0     1957 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_rs.py
+-rw-r--r--   0        0        0      481 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/treesitter/treesitter_ts.py
+-rw-r--r--   0        0        0     2802 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/utils.py
+-rw-r--r--   0        0        0     8241 2024-01-14 17:09:20.321137 codeqai-0.0.9/codeqai/vector_store.py
+-rw-r--r--   0        0        0      624 2024-01-14 17:09:20.321137 codeqai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 codeqai-0.0.9/PKG-INFO
```

### Comparing `codeqai-0.0.8/LICENSE` & `codeqai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/README.md` & `codeqai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/app.py` & `codeqai-0.0.9/codeqai/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         model=EmbeddingsModel[config["embeddings"].upper().replace("-", "_")],
         deployment=config["embeddings-deployment"]
         if "embeddings-deployment" in config
         else None,
     )
 
     # check if faiss.index exists
-    if not os.path.exists(os.path.join(get_cache_path(), f"{repo_name}.faiss")):
+    if not os.path.exists(os.path.join(get_cache_path(), f"{repo_name}.faiss.bytes")):
         spinner = yaspin(text="🔧 Parsing codebase...", color="green")
         files = repo.load_files()
         documents = codeparser.parse_code_files(files)
         vector_store = VectorStore(
             repo_name,
             embeddings=embeddings_model.embeddings,
         )
@@ -136,15 +136,15 @@
     if args.action == "sync":
         spinner = yaspin(text="🔧 Parsing codebase...", color="green")
         files = repo.load_files()
         documents = codeparser.parse_code_files(files)
         vector_store.sync_documents(documents)
         save_vector_cache(vector_store.vector_cache, f"{repo_name}.json")
         spinner.stop()
-        print("⚙️  Vector store synced with current git checkout.")
+        print("⚙️ Vector store synced with current git checkout.")
 
     llm = LLM(
         llm_host=LlmHost[config["llm-host"].upper().replace("-", "_")],
         chat_model=config["chat-model"],
         deployment=config["model-deployment"] if "model-deployment" in config else None,
     )
     memory = ConversationSummaryMemory(
```

### Comparing `codeqai-0.0.8/codeqai/cache.py` & `codeqai-0.0.9/codeqai/cache.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/codeparser.py` & `codeqai-0.0.9/codeqai/codeparser.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/config.py` & `codeqai-0.0.9/codeqai/config.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/constants.py` & `codeqai-0.0.9/codeqai/constants.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/embeddings.py` & `codeqai-0.0.9/codeqai/embeddings.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/llm.py` & `codeqai-0.0.9/codeqai/llm.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/repo.py` & `codeqai-0.0.9/codeqai/repo.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/__init__.py` & `codeqai-0.0.9/codeqai/treesitter/__init__.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter_c.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter_c.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter_cpp.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter_cpp.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter_cs.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter_cs.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter_py.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter_py.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/treesitter/treesitter_rs.py` & `codeqai-0.0.9/codeqai/treesitter/treesitter_rs.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/utils.py` & `codeqai-0.0.9/codeqai/utils.py`

 * *Files identical despite different names*

### Comparing `codeqai-0.0.8/codeqai/vector_store.py` & `codeqai-0.0.9/codeqai/vector_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import inquirer
 from langchain.embeddings.base import Embeddings
 from langchain.schema import Document
 from langchain.vectorstores import FAISS
 from yaspin import yaspin
 
 from codeqai import utils
@@ -13,30 +15,36 @@
         self.name = name
         self.embeddings = embeddings
         self.install_faiss()
 
     def load_documents(self):
         spinner = yaspin(text="💾 Loading vector store...", color="green")
         spinner.start()
-        self.db = FAISS.load_local(
-            index_name=self.name,
-            folder_path=get_cache_path(),
-            embeddings=self.embeddings,
+        with open(
+            os.path.join(get_cache_path(), f"{self.name}.faiss.bytes"), "rb"
+        ) as file:
+            index = file.read()
+
+        self.db = FAISS.deserialize_from_bytes(
+            embeddings=self.embeddings, serialized=index
         )
         self.vector_cache = load_vector_cache(f"{self.name}.json")
         spinner.stop()
         self.retriever = self.db.as_retriever(search_type="mmr", search_kwargs={"k": 8})
 
     def index_documents(self, documents: list[Document]):
         self.vector_cache = {}
         spinner = yaspin(text="💾 Indexing vector store...", color="green")
         spinner.start()
         self.db = FAISS.from_documents(documents, self.embeddings)
-        self.db.save_local(index_name=self.name, folder_path=get_cache_path())
-
+        index = self.db.serialize_to_bytes()
+        with open(
+            os.path.join(get_cache_path(), f"{self.name}.faiss.bytes"), "wb"
+        ) as binary_file:
+            binary_file.write(index)
         # Create vector cache
         index_to_docstore_id = self.db.index_to_docstore_id
         for i in range(len(documents)):
             document = self.db.docstore.search(index_to_docstore_id[i])
             if document:
                 # Check if the document is already present in the vector cache
                 # if yes, then add the vector id to the vector cache entry
@@ -123,15 +131,19 @@
                 self.db.delete(cache_item.vector_ids)
                 old_filenames.append(cache_item.filename)
 
         # Remove old filenames from the vector cache
         for old_filename in old_filenames:
             self.vector_cache.pop(old_filename)
 
-        self.db.save_local(index_name=self.name, folder_path=get_cache_path())
+        index = self.db.serialize_to_bytes()
+        with open(
+            os.path.join(get_cache_path(), f"{self.name}.faiss.bytes"), "wb"
+        ) as binary_file:
+            binary_file.write(index)
         spinner.stop()
 
     def similarity_search(self, query: str):
         return self.db.similarity_search(query, k=4)
 
     def install_faiss(self):
         try:
```

### Comparing `codeqai-0.0.8/pyproject.toml` & `codeqai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeqai"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["fynnfluegge <fynnfluegge@gmx.de>"]
 readme = "README.md"
 packages = [{ include = "codeqai" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `codeqai-0.0.8/PKG-INFO` & `codeqai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeqai
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: fynnfluegge
 Author-email: fynnfluegge@gmx.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

