# Comparing `tmp/spanking-0.0.2.tar.gz` & `tmp/spanking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanking-0.0.2.tar", last modified: Sun Apr 14 21:05:47 2024, max compression
+gzip compressed data, was "spanking-0.0.3.tar", last modified: Sun Apr 14 22:03:58 2024, max compression
```

## Comparing `spanking-0.0.2.tar` & `spanking-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 21:05:38.000000 spanking-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 21:05:47.525440 spanking-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-14 21:05:38.000000 spanking-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:05:47.525440 spanking-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-14 21:05:38.000000 spanking-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/spanking/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/spanking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:03:42.000000 spanking-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 22:03:58.265798 spanking-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-14 22:03:42.000000 spanking-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:03:58.265798 spanking-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-14 22:03:42.000000 spanking-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/spanking/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 22:03:42.000000 spanking-0.0.3/spanking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:03:58.265798 spanking-0.0.3/spanking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:03:58.000000 spanking-0.0.3/spanking.egg-info/top_level.txt
```

### Comparing `spanking-0.0.2/LICENSE` & `spanking-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spanking-0.0.2/PKG-INFO` & `spanking-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.2
+Version: 0.0.3
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: jax==0.4.26
+Requires-Dist: sentence-transformers==2.6.1
 
 # spanking 🍑👋
 
 To use the 🍑👋 `VectorDB` class, you can follow these steps:
 
 1. Create an instance of the 🍑👋 `VectorDB` class:
 ```python
```

### Comparing `spanking-0.0.2/README.md` & `spanking-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spanking-0.0.2/setup.py` & `spanking-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 assert os.path.isfile("spanking/version.py")
 with open("spanking/VERSION", "w", encoding="utf-8") as fh:
     fh.write("%s\n" % spanking_version)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+with open('requirements.txt') as fh:
+    requirements = fh.read().splitlines()
+
 setuptools.setup(
     name="spanking",
     version=spanking_version,
     author="Rishiraj Acharya",
     author_email="heyrishiraj@gmail.com",
     description="🍑👋",
     long_description=long_description,
@@ -41,11 +44,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     entry_points={"console_scripts": ["spanking = spanking.main:main"]},
-    install_requires=[
-        "numpy >= 1.26.4",
-    ],
+    install_requires=requirements,
 )
```

### Comparing `spanking-0.0.2/spanking/main.py` & `spanking-0.0.3/spanking/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import jax
 import jax.numpy as jnp
+import pickle
 from sentence_transformers import SentenceTransformer
 
 class VectorDB:
     def __init__(self, model_name='BAAI/bge-base-en-v1.5'):
         self.model = SentenceTransformer(model_name)
         self.texts = []
         self.embeddings = None
@@ -33,14 +34,23 @@
     
     def search(self, query, top_k=5):
         query_embedding = self.model.encode([query], normalize_embeddings=True)
         similarities = jnp.dot(self.embeddings, query_embedding.T).squeeze()
         top_indices = jnp.argsort(similarities)[-top_k:][::-1]
         return [(self.texts[i], similarities[i]) for i in top_indices]
     
+    def save(self, file_path):
+        with open(file_path, 'wb') as file:
+            pickle.dump(self, file)
+
+    @staticmethod
+    def load(file_path):
+        with open(file_path, 'rb') as file:
+            return pickle.load(file)
+    
     def __len__(self):
         return len(self.texts)
     
     def __getitem__(self, index):
         return self.texts[index]
     
     def __iter__(self):
```

### Comparing `spanking-0.0.2/spanking.egg-info/PKG-INFO` & `spanking-0.0.3/spanking.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.2
+Version: 0.0.3
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: jax==0.4.26
+Requires-Dist: sentence-transformers==2.6.1
 
 # spanking 🍑👋
 
 To use the 🍑👋 `VectorDB` class, you can follow these steps:
 
 1. Create an instance of the 🍑👋 `VectorDB` class:
 ```python
```

