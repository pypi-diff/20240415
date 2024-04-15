# Comparing `tmp/llama_index_readers_smart_pdf_loader-0.1.3.tar.gz` & `tmp/llama_index_readers_smart_pdf_loader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_smart_pdf_loader-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_smart_pdf_loader-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_smart_pdf_loader-0.1.3.tar` & `llama_index_readers_smart_pdf_loader-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1906 2024-02-13 13:53:01.873811 llama_index_readers_smart_pdf_loader-0.1.3/README.md
--rw-r--r--   0        0        0       99 2024-02-13 13:53:01.874003 llama_index_readers_smart_pdf_loader-0.1.3/llama_index/readers/smart_pdf_loader/__init__.py
--rw-r--r--   0        0        0     1371 2024-02-13 13:53:01.874061 llama_index_readers_smart_pdf_loader-0.1.3/llama_index/readers/smart_pdf_loader/base.py
--rw-r--r--   0        0        0     1557 2024-02-21 20:52:13.885216 llama_index_readers_smart_pdf_loader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 llama_index_readers_smart_pdf_loader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1983 2024-04-15 18:30:10.938201 llama_index_readers_smart_pdf_loader-0.1.4/README.md
+-rw-r--r--   0        0        0       99 2024-04-15 18:30:10.942201 llama_index_readers_smart_pdf_loader-0.1.4/llama_index/readers/smart_pdf_loader/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-15 18:30:10.942201 llama_index_readers_smart_pdf_loader-0.1.4/llama_index/readers/smart_pdf_loader/base.py
+-rw-r--r--   0        0        0     1557 2024-04-15 18:30:10.942201 llama_index_readers_smart_pdf_loader-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 llama_index_readers_smart_pdf_loader-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_smart_pdf_loader-0.1.3/README.md` & `llama_index_readers_smart_pdf_loader-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Smart PDF Loader
 
+```bash
+pip install llama-index-readers-smart-pdf-loader
+```
+
 SmartPDFLoader is a super fast PDF reader that understands the layout structure of PDFs such as nested sections, nested lists, paragraphs and tables.
 It uses layout information to smartly chunk PDFs into optimal short contexts for LLMs.
 
 ## Requirements
 
 Install the llmsherpa library if it is not already present:
 
@@ -12,26 +16,26 @@
 ```
 
 ## Usage
 
 Here's an example usage of the SmartPDFLoader:
 
 ```python
-from llama_hub.smart_pdf_loader import SmartPDFLoader
+from llama_index.readers.smart_pdf_loader import SmartPDFLoader
 
 llmsherpa_api_url = "https://readers.llmsherpa.com/api/document/developer/parseDocument?renderFormat=all"
 pdf_url = "https://arxiv.org/pdf/1910.13461.pdf"  # also allowed is a file path e.g. /home/downloads/xyz.pdf
 pdf_loader = SmartPDFLoader(llmsherpa_api_url=llmsherpa_api_url)
 documents = pdf_loader.load_data(pdf_url)
 ```
 
 Now you can use the documents with other LlamaIndex components. For example, for retrieval augmented generation, try this:
 
 ```python
-from llama_index import VectorStoreIndex
+from llama_index.core import VectorStoreIndex
 
 index = VectorStoreIndex.from_documents(documents)
 query_engine = index.as_query_engine()
 
 response = query_engine.query("list all the tasks that work with bart")
 print(response)
```

### Comparing `llama_index_readers_smart_pdf_loader-0.1.3/llama_index/readers/smart_pdf_loader/base.py` & `llama_index_readers_smart_pdf_loader-0.1.4/llama_index/readers/smart_pdf_loader/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,11 +31,14 @@
         Returns:
             List[Document]: List of documents.
         """
         results = []
         doc = self.pdf_reader.read_pdf(pdf_path_or_url)
         for chunk in doc.chunks():
             document = Document(
-                text=chunk.to_context_text(), extra_info={"chunk_type": chunk.tag}
+                text=chunk.to_context_text(),
+                extra_info={**extra_info, "chunk_type": chunk.tag}
+                if extra_info
+                else {"chunk_type": chunk.tag},
             )
             results.append(document)
         return results
```

### Comparing `llama_index_readers_smart_pdf_loader-0.1.3/pyproject.toml` & `llama_index_readers_smart_pdf_loader-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers smart_pdf_loader integration"
 exclude = ["**/BUILD"]
 keywords = ["pdf layout", "pdf table", "pdf"]
 license = "MIT"
 maintainers = ["ansukla"]
 name = "llama-index-readers-smart-pdf-loader"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llmsherpa = "^0.1.4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_smart_pdf_loader-0.1.3/PKG-INFO` & `llama_index_readers_smart_pdf_loader-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-smart-pdf-loader
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers smart_pdf_loader integration
 License: MIT
 Keywords: pdf layout,pdf table,pdf
 Author: Your Name
 Author-email: you@example.com
 Maintainer: ansukla
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llmsherpa (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Smart PDF Loader
 
+```bash
+pip install llama-index-readers-smart-pdf-loader
+```
+
 SmartPDFLoader is a super fast PDF reader that understands the layout structure of PDFs such as nested sections, nested lists, paragraphs and tables.
 It uses layout information to smartly chunk PDFs into optimal short contexts for LLMs.
 
 ## Requirements
 
 Install the llmsherpa library if it is not already present:
 
@@ -32,26 +35,26 @@
 ```
 
 ## Usage
 
 Here's an example usage of the SmartPDFLoader:
 
 ```python
-from llama_hub.smart_pdf_loader import SmartPDFLoader
+from llama_index.readers.smart_pdf_loader import SmartPDFLoader
 
 llmsherpa_api_url = "https://readers.llmsherpa.com/api/document/developer/parseDocument?renderFormat=all"
 pdf_url = "https://arxiv.org/pdf/1910.13461.pdf"  # also allowed is a file path e.g. /home/downloads/xyz.pdf
 pdf_loader = SmartPDFLoader(llmsherpa_api_url=llmsherpa_api_url)
 documents = pdf_loader.load_data(pdf_url)
 ```
 
 Now you can use the documents with other LlamaIndex components. For example, for retrieval augmented generation, try this:
 
 ```python
-from llama_index import VectorStoreIndex
+from llama_index.core import VectorStoreIndex
 
 index = VectorStoreIndex.from_documents(documents)
 query_engine = index.as_query_engine()
 
 response = query_engine.query("list all the tasks that work with bart")
 print(response)
```

