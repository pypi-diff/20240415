# Comparing `tmp/spanking-0.0.3.tar.gz` & `tmp/spanking-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanking-0.0.3.tar", last modified: Sun Apr 14 22:03:58 2024, max compression
+gzip compressed data, was "spanking-0.0.4.tar", last modified: Sun Apr 14 22:38:26 2024, max compression
```

## Comparing `spanking-0.0.3.tar` & `spanking-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:03:42.000000 spanking-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 22:03:58.265798 spanking-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-14 22:03:42.000000 spanking-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:03:58.265798 spanking-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-14 22:03:42.000000 spanking-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/spanking/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/spanking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:38:16.000000 spanking-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:38:26.214398 spanking-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-14 22:38:16.000000 spanking-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:38:26.214398 spanking-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-14 22:38:16.000000 spanking-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/spanking/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/spanking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/top_level.txt
```

### Comparing `spanking-0.0.3/LICENSE` & `spanking-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spanking-0.0.3/PKG-INFO` & `spanking-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.3
+Version: 0.0.4
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,30 +51,42 @@
 ```python
 index = 0
 new_text = "i enjoy eating pizza"
 vector_db.update_text(index, new_text)
 ```
 This will update the text and its corresponding embedding at the specified index with the new text.
 
-6. Iterate over the stored texts:
+6. Save the database to a file:
+```python
+vector_db.save('vector_db.pkl')
+```
+This will save the current state of the `VectorDB` instance to a file named 'vector_db.pkl'.
+
+7. Load the database from a file:
+```python
+vector_db = VectorDB.load('vector_db.pkl')
+```
+This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
+
+8. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-7. Access individual texts by index:
+9. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-8. Get the number of texts in the database:
+10. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -96,14 +108,20 @@
 
 # Update a text
 vector_db.update_text(1, "i enjoy playing chess")
 
 # Delete a text
 vector_db.delete_text(2)
 
-# Iterate over the stored texts
-print("\nStored texts:")
-for text in vector_db:
+# Save the database
+vector_db.save('vector_db.pkl')
+
+# Load the database
+loaded_vector_db = VectorDB.load('vector_db.pkl')
+
+# Iterate over the stored texts in the loaded database
+print("\nStored texts in the loaded database:")
+for text in loaded_vector_db:
     print(text)
 ```
 
 This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

### Comparing `spanking-0.0.3/README.md` & `spanking-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,30 +35,42 @@
 ```python
 index = 0
 new_text = "i enjoy eating pizza"
 vector_db.update_text(index, new_text)
 ```
 This will update the text and its corresponding embedding at the specified index with the new text.
 
-6. Iterate over the stored texts:
+6. Save the database to a file:
+```python
+vector_db.save('vector_db.pkl')
+```
+This will save the current state of the `VectorDB` instance to a file named 'vector_db.pkl'.
+
+7. Load the database from a file:
+```python
+vector_db = VectorDB.load('vector_db.pkl')
+```
+This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
+
+8. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-7. Access individual texts by index:
+9. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-8. Get the number of texts in the database:
+10. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -80,14 +92,20 @@
 
 # Update a text
 vector_db.update_text(1, "i enjoy playing chess")
 
 # Delete a text
 vector_db.delete_text(2)
 
-# Iterate over the stored texts
-print("\nStored texts:")
-for text in vector_db:
+# Save the database
+vector_db.save('vector_db.pkl')
+
+# Load the database
+loaded_vector_db = VectorDB.load('vector_db.pkl')
+
+# Iterate over the stored texts in the loaded database
+print("\nStored texts in the loaded database:")
+for text in loaded_vector_db:
     print(text)
 ```
 
 This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

### Comparing `spanking-0.0.3/setup.py` & `spanking-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `spanking-0.0.3/spanking/main.py` & `spanking-0.0.4/spanking/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 from sentence_transformers import SentenceTransformer
 
 class VectorDB:
     def __init__(self, model_name='BAAI/bge-base-en-v1.5'):
         self.model = SentenceTransformer(model_name)
         self.texts = []
         self.embeddings = None
-    
+
     def add_texts(self, texts):
-        new_embeddings = self.model.encode(texts, normalize_embeddings=True)
+        new_embeddings = jnp.array(self.model.encode(texts, normalize_embeddings=True))
         if self.embeddings is None:
             self.embeddings = new_embeddings
         else:
             self.embeddings = jnp.concatenate((self.embeddings, new_embeddings), axis=0)
         self.texts.extend(texts)
-    
+
     def delete_text(self, index):
         if 0 <= index < len(self.texts):
             self.texts.pop(index)
-            self.embeddings = jnp.delete(self.embeddings, index, axis=0)
+            self.embeddings = self.embeddings.at[index].delete()
         else:
             raise IndexError("Invalid index")
-    
+
     def update_text(self, index, new_text):
         if 0 <= index < len(self.texts):
             self.texts[index] = new_text
-            new_embedding = self.model.encode([new_text], normalize_embeddings=True).squeeze()
-            self.embeddings = (self.embeddings).at[index].set(new_embedding)
+            new_embedding = jnp.array(self.model.encode([new_text], normalize_embeddings=True)).squeeze()
+            self.embeddings = self.embeddings.at[index].set(new_embedding)
         else:
             raise IndexError("Invalid index")
-    
+
     def search(self, query, top_k=5):
-        query_embedding = self.model.encode([query], normalize_embeddings=True)
+        query_embedding = jnp.array(self.model.encode([query], normalize_embeddings=True))
         similarities = jnp.dot(self.embeddings, query_embedding.T).squeeze()
         top_indices = jnp.argsort(similarities)[-top_k:][::-1]
         return [(self.texts[i], similarities[i]) for i in top_indices]
-    
+
     def save(self, file_path):
         with open(file_path, 'wb') as file:
             pickle.dump(self, file)
 
     @staticmethod
     def load(file_path):
         with open(file_path, 'rb') as file:
             return pickle.load(file)
-    
+
     def __len__(self):
         return len(self.texts)
-    
+
     def __getitem__(self, index):
         return self.texts[index]
-    
+
     def __iter__(self):
         return iter(self.texts)
 
 def main():
     print("🍑👋")
```

### Comparing `spanking-0.0.3/spanking.egg-info/PKG-INFO` & `spanking-0.0.4/spanking.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.3
+Version: 0.0.4
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,30 +51,42 @@
 ```python
 index = 0
 new_text = "i enjoy eating pizza"
 vector_db.update_text(index, new_text)
 ```
 This will update the text and its corresponding embedding at the specified index with the new text.
 
-6. Iterate over the stored texts:
+6. Save the database to a file:
+```python
+vector_db.save('vector_db.pkl')
+```
+This will save the current state of the `VectorDB` instance to a file named 'vector_db.pkl'.
+
+7. Load the database from a file:
+```python
+vector_db = VectorDB.load('vector_db.pkl')
+```
+This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
+
+8. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-7. Access individual texts by index:
+9. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-8. Get the number of texts in the database:
+10. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -96,14 +108,20 @@
 
 # Update a text
 vector_db.update_text(1, "i enjoy playing chess")
 
 # Delete a text
 vector_db.delete_text(2)
 
-# Iterate over the stored texts
-print("\nStored texts:")
-for text in vector_db:
+# Save the database
+vector_db.save('vector_db.pkl')
+
+# Load the database
+loaded_vector_db = VectorDB.load('vector_db.pkl')
+
+# Iterate over the stored texts in the loaded database
+print("\nStored texts in the loaded database:")
+for text in loaded_vector_db:
     print(text)
 ```
 
 This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

