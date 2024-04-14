# Comparing `tmp/safe_store-0.4.0.tar.gz` & `tmp/safe_store-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_store-0.4.0.tar", last modified: Thu Dec 14 23:21:29 2023, max compression
+gzip compressed data, was "safe_store-0.6.0.tar", last modified: Sun Apr 14 22:05:50 2024, max compression
```

## Comparing `safe_store-0.4.0.tar` & `safe_store-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-14 23:21:29.812456 safe_store-0.4.0/
--rw-rw-rw-   0        0        0    11558 2023-10-20 09:04:04.000000 safe_store-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     7400 2023-12-14 23:21:29.811948 safe_store-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     6330 2023-12-12 17:13:19.000000 safe_store-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-14 23:21:29.786550 safe_store-0.4.0/safe_store/
--rw-rw-rw-   0        0        0     3941 2023-10-20 09:04:04.000000 safe_store-0.4.0/safe_store/BM25Vectorizer.py
--rw-rw-rw-   0        0        0      203 2023-10-20 09:04:04.000000 safe_store-0.4.0/safe_store/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-11-13 15:10:52.000000 safe_store-0.4.0/safe_store/document_decomposer.py
--rw-rw-rw-   0        0        0    10081 2023-11-29 19:26:41.000000 safe_store-0.4.0/safe_store/generic_data_loader.py
--rw-rw-rw-   0        0        0        0 2023-10-31 11:16:20.000000 safe_store-0.4.0/safe_store/knowledge_base.py
--rw-rw-rw-   0        0        0    29842 2023-12-03 23:59:01.000000 safe_store-0.4.0/safe_store/text_vectorizer.py
--rw-rw-rw-   0        0        0      899 2023-10-20 09:04:04.000000 safe_store-0.4.0/safe_store/tfidf_loader.py
--rw-rw-rw-   0        0        0      502 2023-10-20 09:04:04.000000 safe_store-0.4.0/safe_store/utils.py
--rw-rw-rw-   0        0        0        0 2023-11-12 16:07:53.000000 safe_store-0.4.0/safe_store/word2vec.py
-drwxrwxrwx   0        0        0        0 2023-12-14 23:21:29.810947 safe_store-0.4.0/safe_store.egg-info/
--rw-rw-rw-   0        0        0     7400 2023-12-14 23:21:29.000000 safe_store-0.4.0/safe_store.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-12-14 23:21:29.000000 safe_store-0.4.0/safe_store.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-14 23:21:29.000000 safe_store-0.4.0/safe_store.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-12-14 23:21:29.000000 safe_store-0.4.0/safe_store.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-12-14 23:21:29.000000 safe_store-0.4.0/safe_store.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-14 23:21:29.813464 safe_store-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-12-14 23:20:33.000000 safe_store-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 22:05:50.657869 safe_store-0.6.0/
+-rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     7438 2024-04-14 22:05:50.656869 safe_store-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 22:05:50.632826 safe_store-0.6.0/safe_store/
+-rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/BM25Vectorizer.py
+-rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/__init__.py
+-rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/document_decomposer.py
+-rw-rw-rw-   0        0        0    10902 2024-04-10 19:55:07.000000 safe_store-0.6.0/safe_store/generic_data_loader.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/knowledge_base.py
+-rw-rw-rw-   0        0        0    32084 2024-04-14 22:01:11.000000 safe_store-0.6.0/safe_store/text_vectorizer.py
+-rw-rw-rw-   0        0        0      899 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/tfidf_loader.py
+-rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/utils.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.0/safe_store/word2vec.py
+drwxrwxrwx   0        0        0        0 2024-04-14 22:05:50.655870 safe_store-0.6.0/safe_store.egg-info/
+-rw-rw-rw-   0        0        0     7438 2024-04-14 22:05:50.000000 safe_store-0.6.0/safe_store.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-14 22:05:50.000000 safe_store-0.6.0/safe_store.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 22:05:50.000000 safe_store-0.6.0/safe_store.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-04-14 22:05:50.000000 safe_store-0.6.0/safe_store.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-14 22:05:50.000000 safe_store-0.6.0/safe_store.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 22:05:50.657869 safe_store-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2024-04-14 21:48:09.000000 safe_store-0.6.0/setup.py
```

### Comparing `safe_store-0.4.0/LICENSE` & `safe_store-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_store-0.4.0/PKG-INFO` & `safe_store-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.4.0
+Version: 0.6.0
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,16 @@
 Requires-Dist: python-docx
 Requires-Dist: python-pptx
 Requires-Dist: pandas
 Requires-Dist: beautifulsoup4
 Requires-Dist: mplcursors
 Requires-Dist: PyPDF2
 Requires-Dist: dpkt
-Requires-Dist: transformers
+Requires-Dist: pipmaster
+Requires-Dist: sentence-transformers
 
 <img src="assets/logo.png" width="200px">
 
 # safe_store
 ![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-brightgreen.svg)
 ![PyPI Version](https://img.shields.io/pypi/v/safe-store.svg)
 ![License](https://img.shields.io/github/license/ParisNeo/safe_store.svg)
@@ -138,15 +139,15 @@
 ```
 
 #### Embedding a Query and Retrieving Similar Documents
 
 ```python
 # Embed a query and retrieve similar documents
 query_text = "what is space"
-similar_texts, _ = vectorizer.recover_text(query_text, top_k=3)
+similar_texts, _, _ = vectorizer.recover_text(query_text, top_k=3)
 
 # Show the interactive document visualization
 vectorizer.show_document(show_interactive_form=True)
 
 print("Similar Documents:")
 for i, text in enumerate(similar_texts):
     print(f"{i + 1}: {text}")
```

### Comparing `safe_store-0.4.0/README.md` & `safe_store-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 ```
 
 #### Embedding a Query and Retrieving Similar Documents
 
 ```python
 # Embed a query and retrieve similar documents
 query_text = "what is space"
-similar_texts, _ = vectorizer.recover_text(query_text, top_k=3)
+similar_texts, _, _ = vectorizer.recover_text(query_text, top_k=3)
 
 # Show the interactive document visualization
 vectorizer.show_document(show_interactive_form=True)
 
 print("Similar Documents:")
 for i, text in enumerate(similar_texts):
     print(f"{i + 1}: {text}")
```

### Comparing `safe_store-0.4.0/safe_store/BM25Vectorizer.py` & `safe_store-0.6.0/safe_store/BM25Vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.4.0/safe_store/document_decomposer.py` & `safe_store-0.6.0/safe_store/document_decomposer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.4.0/safe_store/generic_data_loader.py` & `safe_store-0.6.0/safe_store/generic_data_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,36 +26,38 @@
         """
         file_path = Path(file_path)
         
         if file_path.suffix.lower() ==".pdf":
             return GenericDataLoader.read_pdf_file(file_path)
         elif file_path.suffix.lower() == ".docx":
             return GenericDataLoader.read_docx_file(file_path)
+        elif file_path.suffix.lower() == ".xlsx":
+            return GenericDataLoader.read_xlsx_file(file_path)
         elif file_path.suffix.lower() == ".json":
             return GenericDataLoader.read_json_file(file_path)
         elif file_path.suffix.lower() == ".html":
             return GenericDataLoader.read_html_file(file_path)
         elif file_path.suffix.lower() == ".pptx":
             return GenericDataLoader.read_pptx_file(file_path)
         if file_path.suffix.lower() in [".pcap"]:
             return GenericDataLoader.read_pcap_file(file_path)
-        if file_path.suffix.lower() in [".txt", ".rtf", ".md", ".log", ".csv", ".cpp", ".java", ".js", ".py", ".rb", ".sh", ".sql", ".css", ".html", ".php", ".json", ".xml", ".yaml", ".yml", ".h", ".hh", ".hpp", ".inc", ".snippet", ".snippets", ".asm", ".s", ".se", ".sym", ".ini", ".inf", ".map", ".bat"]:
+        if file_path.suffix.lower() in ['.sh', '.json', '.sym', '.log', '.snippet', '.se', '.yml', '.snippets', '.lua', '.pdf', '.md', '.docx', '.yaml', '.inc', '.txt', '.ini', '.pas', '.pptx', '.map', '.php', '.xlsx', '.rtf', '.hpp', '.h', '.asm', '.xml', '.hh', '.sql', '.java', '.c', '.html', '.inf', '.rb', '.py', '.cs', '.js', '.bat', '.css', '.s', '.cpp', '.csv']:
             return GenericDataLoader.read_text_file(file_path)
         else:
             raise ValueError("Unknown file type")
         
     @staticmethod
     def get_supported_file_types() -> List[str]:
         """
         Get the list of supported file types.
 
         Returns:
             List[str]: The list of supported file types.
         """
-        return ["pdf", "txt", "docx", "json", "css", "css", "html", "pptx",".txt", ".md", ".log", ".cpp", ".java", ".js", ".py", ".rb", ".sh", ".sql", ".css", ".html", ".php", ".json", ".xml", ".yaml", ".yml", ".h", ".hh", ".hpp", ".inc", ".snippet", ".snippets", ".asm", ".s", ".se", ".sym", ".ini", ".inf", ".map", ".bat", ".rtf"]    
+        return ['.sh', '.json', '.sym', '.log', '.snippet', '.se', '.yml', '.snippets', '.lua', '.pdf', '.md', '.docx', '.yaml', '.inc', '.txt', '.ini', '.pas', '.pptx', '.map', '.php', '.xlsx', '.rtf', '.hpp', '.h', '.asm', '.xml', '.hh', '.sql', '.java', '.c', '.html', '.inf', '.rb', '.py', '.cs', '.js', '.bat', '.css', '.s', '.cpp', '.csv']    
     
     @staticmethod
     def read_pcap_file(file_path):
         import dpkt
         result = ""  # Create an empty string to store the packet details
         with open(file_path, 'rb') as f:
             pcap = dpkt.pcap.Reader(f)
@@ -144,14 +146,15 @@
         text = extract_text_from_pdf(file_path)
 
         # Convert to Markdown (You may need to implement custom logic based on your specific use case)
         markdown_text = text.replace('\n', '  \n')  # Adding double spaces at the end of each line for Markdown line breaks
         
         return markdown_text
 
+    
     @staticmethod
     def read_docx_file(file_path: Path) -> str:
         """
         Read a DOCX file and return its content as a string.
 
         Args:
             file_path (Path): The path to the DOCX file.
@@ -167,14 +170,36 @@
         doc = Document(file_path)
         text = ""
         for paragraph in doc.paragraphs:
             text += paragraph.text + "\n"
         return text
 
     @staticmethod
+    def read_xlsx_file(file_path: Path) -> str:
+        """
+        Read a DOCX file and return its content as a string.
+
+        Args:
+            file_path (Path): The path to the DOCX file.
+
+        Returns:
+            str: The content of the DOCX file.
+        """
+        try:
+            import pandas as pd
+            import openpyxl
+        except ImportError:
+            PackageManager.install_package("openpyxl")
+            PackageManager.install_package("pandas")
+            import pandas as pd
+        xls = pd.read_excel(file_path)
+
+        return xls.to_string()
+
+    @staticmethod
     def read_json_file(file_path: Path) -> str:
         """
         Read a JSON file and return its content as a string.
 
         Args:
             file_path (Path): The path to the JSON file.
```

### Comparing `safe_store-0.4.0/safe_store/text_vectorizer.py` & `safe_store-0.6.0/safe_store/text_vectorizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+from pipmaster import PackageManager
+pm = PackageManager()
 from sklearn.feature_extraction.text import TfidfVectorizer
+from ascii_colors import ASCIIColors, trace_exception
 from sklearn.metrics.pairwise import cosine_similarity
 from safe_store.BM25Vectorizer import BM25Vectorizer, split_string  # Import BM25Vectorizer
 import numpy as np
 from pathlib import Path
 import json
-from ascii_colors import ASCIIColors, trace_exception
 from safe_store.document_decomposer import DocumentDecomposer
 from safe_store.tfidf_loader import TFIDFLoader
 from safe_store.utils import NumpyEncoderDecoder
 from typing import Union, Tuple, List, Dict, Any
 from enum import Enum
 
 class VectorizationMethod(Enum):
     MODEL_EMBEDDING = "model_embedding"
     TFIDF_VECTORIZER = "tfidf_vectorizer"
     BM25_VECTORIZER = "bm25_vectorizer"
-    BERT = "bert"
+    SENTENCE_TRANSFORMER_EMBEDDING = "sentense_transformer"
 class VisualizationMethod(Enum):
     PCA = "PCA"
     TSNE = "TSNE"
 
 class TextVectorizer:
     def __init__(
                     self, 
                     vectorization_method:VectorizationMethod|str, # supported "model_embedding" or "tfidf_vectorizer"
                     model=None, #needed in case of using model_embedding
                     database_path=None,
                     save_db=False,
                     data_visualization_method:VisualizationMethod|str=VisualizationMethod.PCA,
-                    database_dict=None
+                    database_dict=None,
+                    embedding_model = "all-MiniLM-L6-v2"
                     ):
+        # Only useful when using  VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING
+        self.embedding_model = embedding_model
         if isinstance(vectorization_method, str):
             try:
                 vectorization_method = VectorizationMethod(vectorization_method)
             except ValueError:
                 raise ValueError("Invalid vectorization_method string. Please use valid enum values or strings.")
         elif not isinstance(vectorization_method, VectorizationMethod):
             raise ValueError("Invalid vectorization_method. Please use VectorizationMethod enum values or strings.")
@@ -42,16 +47,22 @@
             try:
                 data_visualization_method = VisualizationMethod(vectorization_method)
             except ValueError:
                 raise ValueError("Invalid vectorization_method string. Please use valid enum values or strings.")
         elif not isinstance(data_visualization_method, VisualizationMethod):
             raise ValueError("Invalid vectorization_method. Please use VisualizationMethod enum values or strings.")
         
-        
-        
+        if vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
+            try:
+                if not pm.is_installed("sentence_transformers"):
+                    pm.install("sentence_transformers")
+                from sentence_transformers import SentenceTransformer
+                self.embedding_model = SentenceTransformer(self.embedding_model)
+            except Exception as ex:
+                ASCIIColors.warning("Couldn't load sentence_transformers. reverting to tf-idf format")        
         self.vectorization_method = vectorization_method
         self.save_db = save_db
         self.model = model
         self.database_file = database_path
         
         self.data_visualization_method = data_visualization_method
         
@@ -82,31 +93,19 @@
                     self.infos={
                         "vectorization_method":VectorizationMethod.TFIDF_VECTORIZER.value
                     }
             elif vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                 self.infos = {
                     "vectorization_method": VectorizationMethod.BM25_VECTORIZER.value
                 }
-            elif vectorization_method==VectorizationMethod.BERT:
-                from transformers import BertTokenizer, BertModel
-                import torch
-                tokenizer = BertTokenizer.from_pretrained('bert-base-multilingual-cased')
-                model = BertModel.from_pretrained("bert-base-multilingual-cased")
-                def embed(text):
-                    with torch.no_grad():
-                        encoded_input = tokenizer(text, return_tensors='pt')
-                        out =  model(**encoded_input)
-                        # Extract components from the model output
-                        return out.last_hidden_state.numpy()
-                
-                self.embed = embed
+            elif vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
+                self.embed = self.embedding_model.encode
                 self.infos = {
-                    "vectorization_method": VectorizationMethod.BERT.value
+                    "vectorization_method": VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING.value
                 }
-
             else:
                 self.infos={
                     "vectorization_method":VectorizationMethod.TFIDF_VECTORIZER.value
                 }
 
         # Load previous state from the JSON file
         if self.save_db:
@@ -217,24 +216,24 @@
             colors = sns.color_palette("Set1", n_colors=num_colors)
 
             # Now you can use the 'colors' list for your document paths
             document_path_colors = colors
             unique_document_paths = list(set(document_paths))
             legend_labels= []
             embeddings_by_document={doc:[] for doc in unique_document_paths}
-            for i,document_name in enumerate(document_paths):
-                legend_labels.append(Path(document_name).stem if "/" in document_name or "\\" in document_name else document_name)
-                embeddings_by_document[document_name].append(embeddings_2d[i,:][None,:])
+            for i,document_id in enumerate(document_paths):
+                legend_labels.append(Path(document_id).stem if type(document_id) in [Path, str] and "/" in document_id or "\\" in document_id else str(document_id))
+                embeddings_by_document[document_id].append(embeddings_2d[i,:][None,:])
 
             labels=[]
-            for i, (document_name, emb) in enumerate(embeddings_by_document.items()):
-                label = Path(document_name).stem if "/" in document_name or "\\" in document_name else document_name
+            for i, (document_id, emb) in enumerate(embeddings_by_document.items()):
+                label = Path(document_id).stem if type(document_id) in [Path, str] and "/" in document_id or "\\" in document_id else str(document_id)
                 labels.append(label)
                 embeddings_2d = np.vstack(emb)
-                plt.scatter(embeddings_2d[:,0], embeddings_2d[:,1],  color=document_path_colors[i], label=label, marker='o' if document_name!="Query" else "x")
+                plt.scatter(embeddings_2d[:,0], embeddings_2d[:,1],  color=document_path_colors[i], label=label, marker='o' if document_id!="Query" else "x")
                 # Add labels to the scatter plot
                 for j, (x, y) in enumerate(embeddings_2d[:]):
                     if label!="Query":
                         plt.text(x, y, f"{i}_{j}", fontsize=8)
                     else:
                         plt.text(x, y, f"query", fontsize=8)
             # Create the legend
@@ -316,89 +315,100 @@
                 except Exception as ex:
                     trace_exception(ex)
 
             if show_interactive_form:
                 plt.show()
 
     
-    def file_exists(self, document_name: str) -> bool:
+    def document_exists(self, document_id: str) -> bool:
         """
         Check if a document exists in the vector store.
         Args:
-            document_name (str): The name of the document to check.
+            document_id (str): The name of the document to check.
         Returns:
             bool: True if the document exists, False otherwise.
         """
 
         # Loop through the list of dictionaries
         for dictionary in self.chunks:
-            if 'document_name' in dictionary and dictionary['document_name'] == document_name:
-                # If the document_name is found in the current dictionary, set the flag to True and break the loop
-                document_name_found = True
+            if 'document_id' in dictionary and dictionary['document_id'] == document_id:
+                # If the document_id is found in the current dictionary, set the flag to True and break the loop
+                document_id_found = True
                 return True
         return False
     
-    def remove_document(self, document_name: str):
+    def remove_document(self, document_id: str):
         """
         Remove a document from the vector store.
         Args:
-            document_name (str): The name of the document to be removed.
+            document_id (str): The name of the document to be removed.
         Returns:
             bool: True if the document was successfully removed, False otherwise.
         """
         for dictionary in self.chunks:
-            if 'document_name' in dictionary and dictionary['document_name'] == document_name:
-                # If the document_name is found in the current dictionary, set the flag to True and break the loop
+            if 'document_id' in dictionary and dictionary['document_id'] == document_id:
+                # If the document_id is found in the current dictionary, set the flag to True and break the loop
                 self.chunks.remove(dictionary)
                 return True
         return False
 
-    def add_document(self, document_name: Path, text: str, chunk_size: int=512, overlap_size: int=0, force_vectorize: bool = False, add_as_a_bloc: bool = False, add_to_index=False):
+    def add_document(self, document_id: Any, text: str, chunk_size: int=512, overlap_size: int=0, force_vectorize: bool = False, add_as_a_bloc: bool = False, add_to_index=False, add_first_line_to_all_chunks=False):
         """
         Add a document to the vector store.
 
         Args:
-            document_name (Path): The name of the document.
+            document_id (Any): The identifier of the document.
             text (str): The text content of the document.
             chunk_size (int): The size of each chunk in tokens.
             overlap_size (int): The number of overlapping tokens between chunks.
             force_vectorize (bool, optional): Whether to force vectorization even if the document already exists. Defaults to False.
             add_as_a_bloc (bool, optional): Whether to add the entire document as a single chunk. Defaults to False.
         """
 
-        if self.file_exists(document_name) and not force_vectorize:
-            print(f"Document {document_name} already exists. Skipping vectorization.")
+        if self.document_exists(document_id) and not force_vectorize:
+            print(f"Document {document_id} already exists. Skipping vectorization.")
             return
         if add_as_a_bloc:
             chunks_text = [self.model.tokenize(text)]
             for i, chunk in enumerate(chunks_text):
-                chunk_id = f"{document_name}_chunk_{i + 1}"
+                chunk_id = f"{document_id}_chunk_{i + 1}"
+                document_id_type = type(document_id)
                 chunk_dict = {
-                    "document_name": str(document_name),
+                    "document_id":  document_id if document_id_type == dict or document_id_type ==  list else str(document_id),
                     "chunk_index": i+1,
                     "chunk_text":self.model.detokenize(chunk),
                     "embeddings":[]
                 }
                 self.chunks[chunk_id] = chunk_dict
         else:
+            if add_first_line_to_all_chunks:
+                try:
+                    add_to_chunks = text[:text.index("\n")]
+                except:
+                    add_to_chunks = ""
+            else:
+                add_to_chunks = None            
             if self.model:
                 chunks_text = DocumentDecomposer.decompose_document(text, chunk_size, overlap_size, self.model.tokenize, self.model.detokenize)
             else:
                 chunks_text = DocumentDecomposer.decompose_document(text, chunk_size, overlap_size)
 
             for i, chunk in enumerate(chunks_text):
-                chunk_id = f"{document_name}_chunk_{i + 1}"
+                if add_to_chunks:
+                    chunk = self.model.tokenize(add_to_chunks + "\n") + chunk
+                chunk_id = f"{document_id}_chunk_{i + 1}"
+                document_id_type = type(document_id)
                 chunk_dict = {
-                    "document_name": str(document_name),
+                    "document_id": document_id if document_id_type == dict or document_id_type ==  list else str(document_id),
                     "chunk_index": i+1,
                     "chunk_text":self.model.detokenize(chunk) if (self.model and self.model.detokenize) else ''.join(chunk),
                     "embeddings":[]
                 }
                 if add_to_index:
-                    if self.vectorization_method==VectorizationMethod.BERT:
+                    if self.vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
                         chunk_dict["embeddings"] = self.embed(chunk_dict["chunk_text"])
                     elif self.vectorization_method==VectorizationMethod.MODEL_EMBEDDING:
                         chunk_dict["embeddings"] = self.model.embed(chunk_dict["chunk_text"])
                     elif self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
                         try:
                             chunk["embeddings"] = self.vectorizer.transform([chunk_dict["chunk_text"]]).toarray()
                         except:
@@ -440,15 +450,15 @@
         for chunk_id, chunk in self.chunks.items():
             # Store chunk ID, embeddings, and original text
             try:
                 if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
                     chunk["embeddings"] = self.vectorizer.transform([chunk["chunk_text"]]).toarray()
                 elif self.vectorization_method==VectorizationMethod.BM25_VECTORIZER:
                     chunk["BM25_data"] = (self.vectorizer.doc_term_freqs, self.vectorizer.doc_lengths) 
-                elif self.vectorization_method==VectorizationMethod.BERT:
+                elif self.vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
                     chunk["embeddings"] = self.embed(chunk["chunk_text"])
                 else:
                     chunk["embeddings"] = self.model.embed(chunk["chunk_text"])
             except Exception as ex:
                 print("oups")
 
         if self.save_db:
@@ -467,15 +477,15 @@
             query_text (str): The query text to be embedded.
         Returns:
             Union[np.ndarray, None]: The embedded query text as a numpy array, or None if embedding is not supported.
         """
         # Generate query embeddings
         if self.vectorization_method == VectorizationMethod.TFIDF_VECTORIZER:
             query_embedding = self.vectorizer.transform([query_text]).toarray()
-        elif self.vectorization_method == VectorizationMethod.BERT:
+        elif self.vectorization_method == VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
             query_embedding = self.embed(query_text)
         elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
             raise Exception("BM25 doesn't use embedding")
         else:
             query_embedding = self.model.embed(query_text)
             if query_embedding is None:
                 ASCIIColors.warning("The model doesn't implement embeddings extraction")
@@ -499,60 +509,79 @@
             index (int): The index of the chunk.
         Returns:
             str: The text of the chunk.
         """
         chunk_id = [ch for ch in self.chunks.keys()][index]
         return self.chunks[chunk_id]["chunk_text"]
 
-    def recover_chunk_by_document_name(self, document_name: str) -> List[Dict[str, Any]]:
+    def recover_chunk_by_document_id(self, document_id: str) -> List[Dict[str, Any]]:
         """
         Recovers the chunks by their document name.
         Args:
-            document_name (str): The name of the document.
+            document_id (str): The name of the document.
         Returns:
             List[Dict[str, Any]]: A list of chunks with matching document names.
         """
-        chunks = [ch for ch in self.chunks.values() if ch["document_name"]==document_name]
+        chunks = [ch for ch in self.chunks.values() if ch["document_id"]==document_id]
         return chunks
 
     def recover_text(self, query: str, top_k: int = 3) -> Tuple[List[str], np.ndarray]:
         """
         Retrieves the most similar texts to a given query.
         Args:
             query (str): The query text.
             top_k (int, optional): The number of most similar texts to retrieve. Default is 3.
         Returns:
             Tuple[List[str], np.ndarray]: A tuple containing a list of the most similar texts and an array of the corresponding similarity scores.
         """
-        if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER or self.vectorization_method==VectorizationMethod.MODEL_EMBEDDING or self.vectorization_method==VectorizationMethod.BERT:
+        if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER or self.vectorization_method==VectorizationMethod.MODEL_EMBEDDING:
             similarities = {}
             query_embedding = self.embed_query(query)
             for chunk_id, chunk in self.chunks.items():
                 if type(chunk["embeddings"])==np.ndarray:
                     similarity = cosine_similarity(query_embedding, chunk["embeddings"])
                     similarities[chunk_id] = similarity
                 else:
                     similarities[chunk_id] = 1e10
             # Sort the similarities and retrieve the top-k most similar embeddings
             sorted_similarities = sorted(similarities.items(), key=lambda x: x[1], reverse=True)[:top_k]
 
             # Retrieve the original text associated with the most similar embeddings
             texts = [self.chunks[chunk_id]["chunk_text"] for chunk_id, _ in sorted_similarities]
+            document_ids = [self.chunks[chunk_id]["document_id"] for chunk_id, _ in sorted_similarities]
+        elif self.vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
+            from sentence_transformers.util import cos_sim
+            similarities = {}
+            query_embedding = self.embed_query(query)
+            for chunk_id, chunk in self.chunks.items():
+                if type(chunk["embeddings"])==np.ndarray:
+                    similarity = cos_sim(query_embedding, chunk["embeddings"])
+                    similarities[chunk_id] = similarity[0][0]
+                else:
+                    similarities[chunk_id] = 1e10
+            # Sort the similarities and retrieve the top-k most similar embeddings
+            sorted_similarities = sorted(similarities.items(), key=lambda x: x[1], reverse=True)[:top_k]
+
+            # Retrieve the original text associated with the most similar embeddings
+            texts = [self.chunks[chunk_id]["chunk_text"] for chunk_id, _ in sorted_similarities]
+            document_ids = [self.chunks[chunk_id]["document_id"] for chunk_id, _ in sorted_similarities]
+
         elif self.vectorization_method==VectorizationMethod.BM25_VECTORIZER:
             # Use the BM25Vectorizer to compute BM25 scores for the query
             bm25_scores = self.vectorizer.transform(query)
 
             # Find the top-k documents with the highest BM25 scores
             top_k_indices = np.argsort(bm25_scores)[::-1][:top_k]
 
             # Retrieve the original text associated with the top-k documents
             chunk_keys = [key for key,_ in self.chunks.items()]
             texts = [self.chunks[chunk_keys[chunk_id]]["chunk_text"] for chunk_id in top_k_indices]   
+            document_ids = [self.chunks[chunk_keys[chunk_id]]["document_id"] for chunk_id in top_k_indices]
             sorted_similarities = np.sort(bm25_scores)
-        return texts, sorted_similarities
+        return texts, sorted_similarities, document_ids
 
     def toJson(self) -> Dict[str, Any]:
         """
         Converts the vector store object to a JSON-compatible dictionary.
         Returns:
             Dict[str, Any]: The JSON-compatible dictionary representing the vector store object.
         """
```

### Comparing `safe_store-0.4.0/safe_store/tfidf_loader.py` & `safe_store-0.6.0/safe_store/tfidf_loader.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.4.0/safe_store.egg-info/PKG-INFO` & `safe_store-0.6.0/safe_store.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: safe-store
-Version: 0.4.0
+Name: safe_store
+Version: 0.6.0
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,16 @@
 Requires-Dist: python-docx
 Requires-Dist: python-pptx
 Requires-Dist: pandas
 Requires-Dist: beautifulsoup4
 Requires-Dist: mplcursors
 Requires-Dist: PyPDF2
 Requires-Dist: dpkt
-Requires-Dist: transformers
+Requires-Dist: pipmaster
+Requires-Dist: sentence-transformers
 
 <img src="assets/logo.png" width="200px">
 
 # safe_store
 ![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-brightgreen.svg)
 ![PyPI Version](https://img.shields.io/pypi/v/safe-store.svg)
 ![License](https://img.shields.io/github/license/ParisNeo/safe_store.svg)
@@ -138,15 +139,15 @@
 ```
 
 #### Embedding a Query and Retrieving Similar Documents
 
 ```python
 # Embed a query and retrieve similar documents
 query_text = "what is space"
-similar_texts, _ = vectorizer.recover_text(query_text, top_k=3)
+similar_texts, _, _ = vectorizer.recover_text(query_text, top_k=3)
 
 # Show the interactive document visualization
 vectorizer.show_document(show_interactive_form=True)
 
 print("Similar Documents:")
 for i, text in enumerate(similar_texts):
     print(f"{i + 1}: {text}")
```

### Comparing `safe_store-0.4.0/setup.py` & `safe_store-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Package metadata
 NAME = 'safe_store'
 DESCRIPTION = 'A library for safe document storage and vectorization.'
 URL = 'https://github.com/ParisNeo/safe_store'
 AUTHOR = 'ALOUI Saifeddine (ParisNeo)'
 AUTHOR_EMAIL = 'aloui.seifeddine@email.com'
 LICENSE = 'Apache 2.0'
-VERSION = '0.4.0'
+VERSION = '0.6.0'
 
 # Read dependencies from requirements.txt
 with open('requirements.txt', 'r') as req_file:
     INSTALL_REQUIRES = req_file.read().splitlines()
 
 # Packages to include (find_packages() automatically discovers and includes sub-packages)
 PACKAGES = find_packages()
```

