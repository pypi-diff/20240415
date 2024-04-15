# Comparing `tmp/langchain_postgres-0.0.1.tar.gz` & `tmp/langchain_postgres-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_postgres-0.0.1.tar", max compression
+gzip compressed data, was "langchain_postgres-0.0.2.tar", max compression
```

## Comparing `langchain_postgres-0.0.1.tar` & `langchain_postgres-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/LICENSE
--rw-r--r--   0        0        0     4238 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/README.md
--rw-r--r--   0        0        0      621 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/__init__.py
--rw-r--r--   0        0        0     2914 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/_utils.py
--rw-r--r--   0        0        0    14033 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/chat_message_histories.py
--rw-r--r--   0        0        0    23519 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/checkpoint.py
--rw-r--r--   0        0        0        0 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/py.typed
--rw-r--r--   0        0        0    49908 2024-04-09 18:01:49.141412 langchain_postgres-0.0.1/langchain_postgres/vectorstores.py
--rw-r--r--   0        0        0     2127 2024-04-09 18:01:49.145412 langchain_postgres-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5186 1970-01-01 00:00:00.000000 langchain_postgres-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4238 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/README.md
+-rw-r--r--   0        0        0      621 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/__init__.py
+-rw-r--r--   0        0        0     2914 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/_utils.py
+-rw-r--r--   0        0        0    14033 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/chat_message_histories.py
+-rw-r--r--   0        0        0    23519 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/checkpoint.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/py.typed
+-rw-r--r--   0        0        0    49908 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/vectorstores.py
+-rw-r--r--   0        0        0     2127 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5186 1970-01-01 00:00:00.000000 langchain_postgres-0.0.2/PKG-INFO
```

### Comparing `langchain_postgres-0.0.1/LICENSE` & `langchain_postgres-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/README.md` & `langchain_postgres-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/langchain_postgres/__init__.py` & `langchain_postgres-0.0.2/langchain_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/langchain_postgres/_utils.py` & `langchain_postgres-0.0.2/langchain_postgres/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/langchain_postgres/chat_message_histories.py` & `langchain_postgres-0.0.2/langchain_postgres/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/langchain_postgres/checkpoint.py` & `langchain_postgres-0.0.2/langchain_postgres/checkpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.1/langchain_postgres/vectorstores.py` & `langchain_postgres-0.0.2/langchain_postgres/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
         connection: Optional[str] = None,
         pre_delete_collection: bool = False,
         *,
         use_jsonb: bool = True,
         **kwargs: Any,
     ) -> PGVector:
         if ids is None:
-            ids = [str(uuid.uuid1()) for _ in texts]
+            ids = [str(uuid.uuid4()) for _ in texts]
 
         if not metadatas:
             metadatas = [{} for _ in texts]
 
         store = cls(
             connection=connection,
             collection_name=collection_name,
@@ -464,15 +464,15 @@
         Args:
             texts: Iterable of strings to add to the vectorstore.
             embeddings: List of list of embedding vectors.
             metadatas: List of metadatas associated with the texts.
             kwargs: vectorstore specific parameters
         """
         if ids is None:
-            ids = [str(uuid.uuid1()) for _ in texts]
+            ids = [str(uuid.uuid4()) for _ in texts]
 
         if not metadatas:
             metadatas = [{} for _ in texts]
 
         with self._session_maker() as session:  # type: ignore[arg-type]
             collection = self.get_collection(session)
             if not collection:
```

### Comparing `langchain_postgres-0.0.1/pyproject.toml` & `langchain_postgres-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-postgres"
-version = "0.0.1"
+version = "0.0.2"
 description = "An integration package connecting Postgres and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-postgres"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `langchain_postgres-0.0.1/PKG-INFO` & `langchain_postgres-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-postgres
-Version: 0.0.1
+Version: 0.0.2
 Summary: An integration package connecting Postgres and LangChain
 Home-page: https://github.com/langchain-ai/langchain-postgres
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

