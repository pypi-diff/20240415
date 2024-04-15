# Comparing `tmp/motion_lake_client-0.0.6.tar.gz` & `tmp/motion_lake_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_lake_client-0.0.6.tar", last modified: Fri Apr 12 17:48:59 2024, max compression
+gzip compressed data, was "motion_lake_client-0.0.7.tar", last modified: Mon Apr 15 15:27:05 2024, max compression
```

## Comparing `motion_lake_client-0.0.6.tar` & `motion_lake_client-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.6/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion_lake_client-0.0.6/README.md
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-12 17:48:54.000000 motion_lake_client-0.0.6/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.6/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.6/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    10390 2024-04-12 17:48:37.000000 motion_lake_client-0.0.6/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:48:59.385078 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-12 17:48:59.000000 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-12 17:48:59.000000 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-12 17:48:59.000000 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-12 17:48:59.000000 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-12 17:48:59.000000 motion_lake_client-0.0.6/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.7/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion_lake_client-0.0.7/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-15 15:26:21.000000 motion_lake_client-0.0.7/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.7/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.7/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    11076 2024-04-15 15:25:57.000000 motion_lake_client-0.0.7/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion_lake_client-0.0.6/LICENSE` & `motion_lake_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `motion_lake_client-0.0.6/PKG-INFO` & `motion_lake_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

### Comparing `motion_lake_client-0.0.6/README.md` & `motion_lake_client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `motion_lake_client-0.0.6/pyproject.toml` & `motion_lake_client-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.6"
+version = "0.0.7"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion_lake_client-0.0.6/src/motion_lake_client/client.py` & `motion_lake_client-0.0.7/src/motion_lake_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,40 +57,49 @@
     A network client to make requests to the storage server.
     """
 
     def get(self, url: str, query_params: Dict[str, Any] = None) -> dict: ...
 
     def post(self, url: str, body: dict) -> dict: ...
 
+    def delete(self, url: str, body: dict = None) -> dict: ...
 
 class RequestsClient(NetworkClient):
     """
     A network client using the requests library.
     """
 
     def __init__(self, base_url: str, **kwargs):
         super().__init__(**kwargs)
         self.base_url = base_url
 
     def get(self, url: str, query_params: Dict[str, Any] = None) -> dict:
         try:
             return requests.get(self.base_url + url, params=query_params).json()
-        except requests.exceptions.RequestException as e:
+        except requests.exceptions.RequestException:
             return {"error": "A request error occurred."}
-        except requests.exceptions.JSONDecodeError as e:
+        except requests.exceptions.JSONDecodeError:
             return {"error": "The response could not be decoded."}
 
     def post(self, url: str, body: dict) -> dict:
         try:
             return requests.post(self.base_url + url, json=body).json()
         except requests.exceptions.RequestException as e:
             return {"error": "A request error occurred."}
         except requests.exceptions.JSONDecodeError as e:
             return {"error": "The response could not be decoded."}
 
+    def delete(self, url: str, body: dict = None) -> dict:
+        try:
+            return requests.delete(self.base_url + url, json=body).json()
+        except requests.exceptions.RequestException:
+            return {"error": "A request error occurred."}
+        except requests.exceptions.JSONDecodeError:
+            return {"error": "The response could not be decoded."}
+
 
 class InnerClient:
     def __init__(self, network_client: NetworkClient):
         self.network_client = network_client
 
     def flush_buffer(self, collection_name: str) -> dict:
         """
@@ -206,14 +215,17 @@
             {
                 "query": query,
                 "min_timestamp": int(min_timestamp.timestamp() ),
                 "max_timestamp": int(max_timestamp.timestamp() ),
             },
         )
 
+    def delete_collection(self, collection_name: str):
+        return self.network_client.delete(f"/delete/{collection_name}/", {})
+
 
 class BaseClient:
     def __init__(self, lake_url: str = "http://localhost:8000"):
         """
         Initialize the client with the base URL of the storage server.
         :param lake_url: The base URL of the storage server
         """
@@ -324,7 +336,10 @@
     ):
         assert (
             "[table]" in query
         ), """Query must contain [table] placeholder (it will be replaced with a view on a table)"""
         return self.inner_client.advanced_query(
             collection_name, query, min_timestamp, max_timestamp
         )
+
+    def delete_collection(self, collection_name: str):
+        return self.inner_client.delete_collection(collection_name)
```

### Comparing `motion_lake_client-0.0.6/src/motion_lake_client.egg-info/PKG-INFO` & `motion_lake_client-0.0.7/src/motion_lake_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

