# Comparing `tmp/motion_lake_client-0.0.7.tar.gz` & `tmp/motion_lake_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_lake_client-0.0.7.tar", last modified: Mon Apr 15 15:27:05 2024, max compression
+gzip compressed data, was "motion_lake_client-0.0.8.tar", last modified: Mon Apr 15 16:17:23 2024, max compression
```

## Comparing `motion_lake_client-0.0.7.tar` & `motion_lake_client-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.7/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion_lake_client-0.0.7/README.md
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-15 15:26:21.000000 motion_lake_client-0.0.7/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.7/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.7/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    11076 2024-04-15 15:25:57.000000 motion_lake_client-0.0.7/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 15:27:05.162700 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-15 15:27:05.000000 motion_lake_client-0.0.7/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.8/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     4591 2024-04-15 15:35:18.000000 motion_lake_client-0.0.8/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-15 16:17:16.000000 motion_lake_client-0.0.8/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.8/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.8/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    11808 2024-04-15 16:17:16.000000 motion_lake_client-0.0.8/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion_lake_client-0.0.7/LICENSE` & `motion_lake_client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `motion_lake_client-0.0.7/pyproject.toml` & `motion_lake_client-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.7"
+version = "0.0.8"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion_lake_client-0.0.7/src/motion_lake_client/client.py` & `motion_lake_client-0.0.8/src/motion_lake_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 ]
 
 # Hopefully, we have better storage systems in 2250...
 MAX_DATE = datetime(2250, 12, 31, 23, 59, 59, 999999)
 MIN_DATE = datetime(1971, 1, 1, 0, 0, 0, 0)
 
 
+class ServerError(Exception):
+    pass
+
+
 @dataclasses.dataclass
 class Item:
     """
     A data item in the collection.
     """
 
     timestamp: datetime
@@ -59,42 +63,52 @@
 
     def get(self, url: str, query_params: Dict[str, Any] = None) -> dict: ...
 
     def post(self, url: str, body: dict) -> dict: ...
 
     def delete(self, url: str, body: dict = None) -> dict: ...
 
+
 class RequestsClient(NetworkClient):
     """
     A network client using the requests library.
     """
 
     def __init__(self, base_url: str, **kwargs):
         super().__init__(**kwargs)
         self.base_url = base_url
 
     def get(self, url: str, query_params: Dict[str, Any] = None) -> dict:
         try:
-            return requests.get(self.base_url + url, params=query_params).json()
+            response = requests.get(self.base_url + url, params=query_params)
+            if response.status_code > 399:
+                raise ServerError("Server error occurred, message: " + response.text)
+            return response.json()
         except requests.exceptions.RequestException:
             return {"error": "A request error occurred."}
         except requests.exceptions.JSONDecodeError:
             return {"error": "The response could not be decoded."}
 
     def post(self, url: str, body: dict) -> dict:
         try:
-            return requests.post(self.base_url + url, json=body).json()
+            response = requests.post(self.base_url + url, json=body)
+            if response.status_code > 399:
+                raise ServerError("Server error occurred, message: " + response.text)
+            return response.json()
         except requests.exceptions.RequestException as e:
             return {"error": "A request error occurred."}
         except requests.exceptions.JSONDecodeError as e:
             return {"error": "The response could not be decoded."}
 
     def delete(self, url: str, body: dict = None) -> dict:
         try:
-            return requests.delete(self.base_url + url, json=body).json()
+            response = requests.delete(self.base_url + url, json=body)
+            if response.status_code > 399:
+                raise ServerError("Server error occurred, message: " + response.text)
+            return response.json()
         except requests.exceptions.RequestException:
             return {"error": "A request error occurred."}
         except requests.exceptions.JSONDecodeError:
             return {"error": "The response could not be decoded."}
 
 
 class InnerClient:
@@ -148,33 +162,36 @@
         self,
         collection_name: str,
         min_timestamp: int,
         max_timestamp: int,
         ascending: bool,
         limit: int = None,
         offset: int = None,
+        skip_data: bool = False,
     ) -> dict:
         """
         Query the data in the collection with the given name.
         :param collection_name: The name of the collection to query
         :param min_timestamp: The minimum timestamp to filter the data
         :param max_timestamp: The maximum timestamp to filter the data
         :param ascending: Whether to sort the data in ascending order
         :param limit: The limit of the data to retrieve
         :param offset: The offset of the data to retrieve
+        :param skip_data: Whether to skip the data in the results (data will be None)
         :return: The data in the collection as a list of tuples of bytes and datetime
         """
         return self.network_client.get(
             f"/query/{collection_name}/",
             {
                 "min_timestamp": min_timestamp,
                 "max_timestamp": max_timestamp,
                 "ascending": ascending,
                 "limit": limit or 1,
                 "offset": offset or 0,
+                "skip_data": skip_data,
             },
         )
 
     def get_collections(self) -> List[Collection]:
         """
         Get a list of all collections.
         :return: A list of collections
@@ -210,16 +227,16 @@
         ), """Query must contain [table] placeholder (it will be replaced with a view on a 
         table)"""
 
         return self.network_client.post(
             f"/advanced/{collection_name}/",
             {
                 "query": query,
-                "min_timestamp": int(min_timestamp.timestamp() ),
-                "max_timestamp": int(max_timestamp.timestamp() ),
+                "min_timestamp": int(min_timestamp.timestamp()),
+                "max_timestamp": int(max_timestamp.timestamp()),
             },
         )
 
     def delete_collection(self, collection_name: str):
         return self.network_client.delete(f"/delete/{collection_name}/", {})
 
 
@@ -255,15 +272,19 @@
         collection_name: str,
         data: bytes,
         timestamp: datetime,
         content_type: ContentType = None,
         create_collection: bool = False,
     ) -> dict:
         return self.inner_client.store(
-            collection_name, data, int(timestamp.timestamp()), content_type, create_collection
+            collection_name,
+            data,
+            int(timestamp.timestamp()),
+            content_type,
+            create_collection,
         )
 
     def query(
         self,
         collection_name: str,
         min_datetime: datetime,
         max_datetime: datetime,
@@ -338,8 +359,8 @@
             "[table]" in query
         ), """Query must contain [table] placeholder (it will be replaced with a view on a table)"""
         return self.inner_client.advanced_query(
             collection_name, query, min_timestamp, max_timestamp
         )
 
     def delete_collection(self, collection_name: str):
-        return self.inner_client.delete_collection(collection_name)
+        return self.inner_client.delete_collection(collection_name)
```

