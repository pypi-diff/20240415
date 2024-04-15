# Comparing `tmp/pongo-python-2.0.3.tar.gz` & `tmp/pongo-python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pongo-python-2.0.3.tar", last modified: Mon Mar 25 14:44:30 2024, max compression
+gzip compressed data, was "pongo-python-3.0.0.tar", last modified: Mon Apr 15 08:14:29 2024, max compression
```

## Comparing `pongo-python-2.0.3.tar` & `pongo-python-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-03-25 14:44:30.553212 pongo-python-2.0.3/
--rw-r--r--   0 caleb      (501) staff       (20)    11356 2023-11-15 21:54:34.000000 pongo-python-2.0.3/LICENSE
--rw-r--r--   0 caleb      (501) staff       (20)      551 2024-03-25 14:44:30.553012 pongo-python-2.0.3/PKG-INFO
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-03-25 14:44:30.551598 pongo-python-2.0.3/pongo/
--rw-r--r--   0 caleb      (501) staff       (20)       32 2024-03-22 01:18:56.000000 pongo-python-2.0.3/pongo/__init__.py
--rw-r--r--   0 caleb      (501) staff       (20)     2731 2024-03-25 14:44:06.000000 pongo-python-2.0.3/pongo/client.py
--rw-r--r--   0 caleb      (501) staff       (20)      885 2024-03-25 14:43:51.000000 pongo-python-2.0.3/pongo/rerank.py
--rw-r--r--   0 caleb      (501) staff       (20)       39 2024-03-23 17:13:30.000000 pongo-python-2.0.3/pongo/utils.py
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-03-25 14:44:30.552794 pongo-python-2.0.3/pongo_python.egg-info/
--rw-r--r--   0 caleb      (501) staff       (20)      551 2024-03-25 14:44:30.000000 pongo-python-2.0.3/pongo_python.egg-info/PKG-INFO
--rw-r--r--   0 caleb      (501) staff       (20)      300 2024-03-25 14:44:30.000000 pongo-python-2.0.3/pongo_python.egg-info/SOURCES.txt
--rw-r--r--   0 caleb      (501) staff       (20)        1 2024-03-25 14:44:30.000000 pongo-python-2.0.3/pongo_python.egg-info/dependency_links.txt
--rw-r--r--   0 caleb      (501) staff       (20)        9 2024-03-25 14:44:30.000000 pongo-python-2.0.3/pongo_python.egg-info/requires.txt
--rw-r--r--   0 caleb      (501) staff       (20)        6 2024-03-25 14:44:30.000000 pongo-python-2.0.3/pongo_python.egg-info/top_level.txt
--rw-r--r--   0 caleb      (501) staff       (20)       38 2024-03-25 14:44:30.553252 pongo-python-2.0.3/setup.cfg
--rw-r--r--   0 caleb      (501) staff       (20)      693 2024-03-25 14:44:20.000000 pongo-python-2.0.3/setup.py
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-03-25 14:44:30.552553 pongo-python-2.0.3/tests/
--rw-r--r--   0 caleb      (501) staff       (20)      453 2024-02-06 16:55:51.000000 pongo-python-2.0.3/tests/test_auth.py
--rw-r--r--   0 caleb      (501) staff       (20)      985 2024-03-22 01:18:56.000000 pongo-python-2.0.3/tests/test_rerank.py
+drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-04-15 08:14:29.147497 pongo-python-3.0.0/
+-rw-r--r--   0 caleb      (501) staff       (20)    11356 2023-11-15 21:54:34.000000 pongo-python-3.0.0/LICENSE
+-rw-r--r--   0 caleb      (501) staff       (20)      551 2024-04-15 08:14:29.147297 pongo-python-3.0.0/PKG-INFO
+drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-04-15 08:14:29.145786 pongo-python-3.0.0/pongo/
+-rw-r--r--   0 caleb      (501) staff       (20)       32 2024-03-22 01:18:56.000000 pongo-python-3.0.0/pongo/__init__.py
+-rw-r--r--   0 caleb      (501) staff       (20)     4428 2024-04-15 07:42:22.000000 pongo-python-3.0.0/pongo/client.py
+-rw-r--r--   0 caleb      (501) staff       (20)     1178 2024-04-15 07:43:58.000000 pongo-python-3.0.0/pongo/filter.py
+-rw-r--r--   0 caleb      (501) staff       (20)     1178 2024-04-15 07:47:03.000000 pongo-python-3.0.0/pongo/rerank.py
+-rw-r--r--   0 caleb      (501) staff       (20)       39 2024-04-15 07:52:52.000000 pongo-python-3.0.0/pongo/utils.py
+drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-04-15 08:14:29.147083 pongo-python-3.0.0/pongo_python.egg-info/
+-rw-r--r--   0 caleb      (501) staff       (20)      551 2024-04-15 08:14:29.000000 pongo-python-3.0.0/pongo_python.egg-info/PKG-INFO
+-rw-r--r--   0 caleb      (501) staff       (20)      316 2024-04-15 08:14:29.000000 pongo-python-3.0.0/pongo_python.egg-info/SOURCES.txt
+-rw-r--r--   0 caleb      (501) staff       (20)        1 2024-04-15 08:14:29.000000 pongo-python-3.0.0/pongo_python.egg-info/dependency_links.txt
+-rw-r--r--   0 caleb      (501) staff       (20)        9 2024-04-15 08:14:29.000000 pongo-python-3.0.0/pongo_python.egg-info/requires.txt
+-rw-r--r--   0 caleb      (501) staff       (20)        6 2024-04-15 08:14:29.000000 pongo-python-3.0.0/pongo_python.egg-info/top_level.txt
+-rw-r--r--   0 caleb      (501) staff       (20)       38 2024-04-15 08:14:29.147535 pongo-python-3.0.0/setup.cfg
+-rw-r--r--   0 caleb      (501) staff       (20)      693 2024-04-15 07:47:39.000000 pongo-python-3.0.0/setup.py
+drwxr-xr-x   0 caleb      (501) staff       (20)        0 2024-04-15 08:14:29.146821 pongo-python-3.0.0/tests/
+-rw-r--r--   0 caleb      (501) staff       (20)      453 2024-02-06 16:55:51.000000 pongo-python-3.0.0/tests/test_auth.py
+-rw-r--r--   0 caleb      (501) staff       (20)     1010 2024-04-15 08:13:59.000000 pongo-python-3.0.0/tests/test_filter.py
```

### Comparing `pongo-python-2.0.3/LICENSE` & `pongo-python-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pongo-python-2.0.3/PKG-INFO` & `pongo-python-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pongo-python
-Version: 2.0.3
+Version: 3.0.0
 Summary: A Python package for interacting with the Pongo API
 Home-page: https://github.com/PongoAI/pongo-python
 Author: Caleb John
 Author-email: caleb.john@joinpongo.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pongo-python-2.0.3/pongo/rerank.py` & `pongo-python-3.0.0/pongo/rerank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import requests
 from .utils import BASE_URL
+import json
+import gzip
 
 
 def rerank(
     secret_key,
     query,
     docs,
     num_results=10,
@@ -13,16 +15,18 @@
     plaintext_sample_size=5,
     text_field="text",
     expand=False,
     version="v1",
 ):
     headers = {
         "secret": secret_key,
+        'Content-Encoding': 'gzip',
+        'Content-Type': 'application/json',
     }
-    url = f"{BASE_URL}/api/{version}/rerank"
+    url = f"{BASE_URL}/api/{version}/filter"
 
     payload = {
         "query": query,
         "text_field": text_field,
         "public_metadata_field": public_metadata_field,
         "plaintext_sample_size": plaintext_sample_size,
         "num_results": num_results,
@@ -30,9 +34,15 @@
         "key_field": key_field,
         "docs": docs,
         "expand": expand,
     }
 
     body = {k: v for k, v in payload.items() if v is not None}
 
-    response = requests.post(url, json=body, headers=headers)
+    # Serialize the data to JSON format
+    json_data = json.dumps(body).encode('utf-8')
+
+    # Compress the JSON data using gzip
+    compressed_data = gzip.compress(json_data)
+
+    response = requests.post(url, data=compressed_data, headers=headers)
     return response
```

### Comparing `pongo-python-2.0.3/pongo_python.egg-info/PKG-INFO` & `pongo-python-3.0.0/pongo_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pongo-python
-Version: 2.0.3
+Version: 3.0.0
 Summary: A Python package for interacting with the Pongo API
 Home-page: https://github.com/PongoAI/pongo-python
 Author: Caleb John
 Author-email: caleb.john@joinpongo.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pongo-python-2.0.3/setup.py` & `pongo-python-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pongo-python",
-    version="2.0.3",
+    version="3.0.0",
     packages=find_packages(),
     description="A Python package for interacting with the Pongo API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Caleb John",
     author_email="caleb.john@joinpongo.com",
     url="https://github.com/PongoAI/pongo-python",
```

### Comparing `pongo-python-2.0.3/tests/test_rerank.py` & `pongo-python-3.0.0/tests/test_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 
 pongo_client = pongo.PongoClient(PONGO_SECRET)
 
 
 class TestSearch(unittest.TestCase):
     def test_search(self):
         # Ensure that the client is initialized properly and connected to server
-        res = pongo_client.rerank(
+        res = pongo_client.filter(
             docs=[
                 {"ig": 1, "text": "Roses are red", "betadata": {}},
                 {"ig": 2, "text": "Violets are blue", "betadata": {}},
                 {"ig": 3, "text": "Roses are red2", "betadata": {}},
                 {"ig": 4, "text": "Roses are red3", "betadata": {}},
             ],
             num_results=3,
             query="what color are roses?",
             public_metadata_field="betadata",
+            expand=True,
             key_field="ig",
         )
 
         print(res.json())
 
         assert len(res.json()) == 3
```

