# Comparing `tmp/upstash_vector-0.2.1.tar.gz` & `tmp/upstash_vector-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_vector-0.2.1.tar", max compression
+gzip compressed data, was "upstash_vector-0.3.0.tar", max compression
```

## Comparing `upstash_vector-0.2.1.tar` & `upstash_vector-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/LICENSE
--rw-r--r--   0        0        0     4442 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/README.md
--rw-r--r--   0        0        0     1669 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      160 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/__init__.py
--rw-r--r--   0        0        0     3403 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/client.py
--rw-r--r--   0        0        0    13809 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/core/index_operations.py
--rw-r--r--   0        0        0       81 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/errors.py
--rw-r--r--   0        0        0     2187 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/http.py
--rw-r--r--   0        0        0        0 2024-03-14 09:32:12.312411 upstash_vector-0.2.1/upstash_vector/py.typed
--rw-r--r--   0        0        0     1963 2024-03-14 09:32:12.316411 upstash_vector-0.2.1/upstash_vector/types.py
--rw-r--r--   0        0        0     1735 2024-03-14 09:32:12.316411 upstash_vector-0.2.1/upstash_vector/utils.py
--rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 upstash_vector-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-15 16:37:02.003429 upstash_vector-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4667 2024-04-15 16:37:02.003429 upstash_vector-0.3.0/README.md
+-rw-r--r--   0        0        0     1669 2024-04-15 16:37:02.003429 upstash_vector-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/__init__.py
+-rw-r--r--   0        0        0     3403 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/client.py
+-rw-r--r--   0        0        0    16201 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/core/index_operations.py
+-rw-r--r--   0        0        0       81 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/errors.py
+-rw-r--r--   0        0        0     2187 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/http.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/py.typed
+-rw-r--r--   0        0        0     2074 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/types.py
+-rw-r--r--   0        0        0     3145 2024-04-15 16:37:02.007429 upstash_vector-0.3.0/upstash_vector/utils.py
+-rw-r--r--   0        0        0     5938 1970-01-01 00:00:00.000000 upstash_vector-0.3.0/PKG-INFO
```

### Comparing `upstash_vector-0.2.1/LICENSE` & `upstash_vector-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.2.1/README.md` & `upstash_vector-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -150,13 +150,25 @@
 
 ## Code Formatting
 ```bash 
 poetry run ruff format .
 ```
 
 ## Running tests
+
 To run all the tests, make sure the poetry virtual environment activated with all 
-the necessary dependencies. Set the necessary environment variables and run:
+the necessary dependencies.
+
+Create two Vector Stores on upstash. First one should have 2 dimensions. Second one should use an embedding model. Set the necessary environment variables:
+
+```
+URL=****
+TOKEN=****
+EMBEDDING_URL=****
+EMBEDDING_TOKEN=****
+```
+
+Then, run the following command to run tests:
 
 ```bash
 poetry run pytest
 ```
```

### Comparing `upstash_vector-0.2.1/pyproject.toml` & `upstash_vector-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upstash-vector"
-version = "0.2.1"
+version = "0.3.0"
 description = "Serverless Vector SDK from Upstash"
 license = "MIT"
 authors = ["Upstash <support@upstash.com>"]
 maintainers = ["Upstash <support@upstash.com>"]
 readme = "README.md"
 repository = "https://github.com/upstash/vector-py"
 keywords = ["Upstash Vector", "Serverless Vector"]
```

### Comparing `upstash_vector-0.2.1/upstash_vector/client.py` & `upstash_vector-0.3.0/upstash_vector/client.py`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.2.1/upstash_vector/core/index_operations.py` & `upstash_vector-0.3.0/upstash_vector/core/index_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # Define vector operations here:
 # Upsert and query functions and signatures
 
 from typing import Sequence, Union, List, Dict, Optional
 from upstash_vector.errors import ClientError
 from upstash_vector.types import (
+    Data,
     DeleteResult,
     RangeResult,
     InfoResult,
     SupportsToList,
-    Vector,
     FetchResult,
     QueryResult,
+    Vector,
 )
 
-from upstash_vector.utils import convert_to_list, convert_to_vectors
+from upstash_vector.utils import convert_to_list, convert_to_vectors, convert_to_payload
 
 UPSERT_PATH = "/upsert"
+UPSERT_DATA_PATH = "/upsert-data"
 QUERY_PATH = "/query"
+QUERY_DATA_PATH = "/query-data"
 DELETE_PATH = "/delete"
 RESET_PATH = "/reset"
 RANGE_PATH = "/range"
 FETCH_PATH = "/fetch"
 INFO_PATH = "/info"
 
 
 class IndexOperations:
     def _execute_request(self, payload, path):
         raise NotImplementedError("execute_request")
 
     def upsert(
         self,
-        vectors: Sequence[Union[Dict, tuple, Vector]],
+        vectors: Sequence[Union[Dict, tuple, Vector, Data]],
     ) -> str:
         """
         Upserts(update or insert) vectors. There are 3 ways to upsert vectors.
 
         Example usages:
 
         ```python
@@ -60,61 +63,97 @@
         res = index.upsert(
             vectors=[
                 Vector(id="id5", vector=[1, 2], metadata={"metadata_f": "metadata_v"}),
                 Vector(id="id6", vector=[6, 7]),
             ]
         )
         ```
+
+        #OR
+
+        ```python
+        from upstash_vector import Data
+        res = index.upsert(
+            vectors=[
+                Data(id="id5", data="Goodbye-World", metadata={"metadata_f": "metadata_v"}),
+                Data(id="id6", data="Hello-World"),
+            ]
+        )
+        ```
         """
+
         vectors = convert_to_vectors(vectors)
-        payload = [
-            {"id": vector.id, "vector": vector.vector, "metadata": vector.metadata}
-            for vector in vectors
-        ]
+        payload, is_vector = convert_to_payload(vectors)
+        path = UPSERT_PATH if is_vector else UPSERT_DATA_PATH
 
-        return self._execute_request(payload=payload, path=UPSERT_PATH)
+        return self._execute_request(payload=payload, path=path)
 
     def query(
         self,
-        vector: Union[List[float], SupportsToList],
+        vector: Optional[Union[List[float], SupportsToList]] = None,
         top_k: int = 10,
         include_vectors: bool = False,
         include_metadata: bool = False,
         filter: str = "",
+        data: Optional[str] = None,
     ) -> List[QueryResult]:
         """
-        Query `top_k` many similar vectors.
+        Query `top_k` many similar vectors. Requires either `data` or `vector` fields. Raises exception if `data` and `vector` fields are both used.
 
         :param vector: list of floats for the values of vector.
         :param top_k: number that indicates how many vectors will be returned as the query result.
         :param include_vectors: bool value that indicates whether the resulting top_k vectors will have their vector values shown.
         :param include_metadata: bool value that indicates whether the resulting top_k vectors will have their metadata shown.
         :param filter: filter expression to narrow down the query results.
+        :param data: string (to be embedded) to query for
 
         Example usage:
 
         ```python
         query_res = index.query(
             vector=[0.6, 0.9],
             top_k=3,
             include_vectors=True,
             include_metadata=True,
         )
         ```
+
+        ```python
+        query_res = index.query(
+            data="hello"
+            top_k=3,
+            include_vectors=True,
+            include_metadata=True,
+        )
+        ```
         """
         payload = {
-            "vector": convert_to_list(vector),
             "topK": top_k,
             "includeVectors": include_vectors,
             "includeMetadata": include_metadata,
             "filter": filter,
         }
+
+        if data is None and vector is None:
+            raise ClientError("either `data` or `vector` values must be given")
+        if data is not None and vector is not None:
+            raise ClientError(
+                "`data` and `vector` values cannot be given at the same time"
+            )
+
+        if data is not None:
+            payload["data"] = data
+            path = QUERY_DATA_PATH
+        else:
+            payload["vector"] = convert_to_list(vector)
+            path = QUERY_PATH
+
         return [
             QueryResult._from_json(obj)
-            for obj in self._execute_request(payload=payload, path=QUERY_PATH)
+            for obj in self._execute_request(payload=payload, path=path)
         ]
 
     def delete(self, ids: Union[str, List[str]]) -> DeleteResult:
         """
         Deletes the given vector(s) with given ids.
 
         Response contains deleted vector count.
@@ -233,15 +272,15 @@
 
 class AsyncIndexOperations:
     async def _execute_request_async(self, payload, path):
         raise NotImplementedError("execute_request")
 
     async def upsert(
         self,
-        vectors: Sequence[Union[Dict, tuple, Vector]],
+        vectors: Sequence[Union[Dict, tuple, Vector, Data]],
     ) -> str:
         """
         Upserts(update or insert) vectors asynchronously. There are 3 ways to upsert vectors.
 
         Example usages:
 
         ```python
@@ -268,62 +307,96 @@
         res = await index.upsert(
             vectors=[
                 Vector(id="id5", vector=[1, 2], metadata={"metadata_f": "metadata_v"}),
                 Vector(id="id6", vector=[6, 7]),
             ]
         )
         ```
+
+        # OR
+
+        ```python
+        from upstash_vector import Data
+        res = await index.upsert(
+            vectors=[
+                Data(id="id5", data="Goodbye-World", metadata={"metadata_f": "metadata_v"}),
+                Data(id="id6", data="Hello-World"),
+            ]
+        )
+        ```
         """
         vectors = convert_to_vectors(vectors)
-        payload = [
-            {"id": vector.id, "vector": vector.vector, "metadata": vector.metadata}
-            for vector in vectors
-        ]
+        payload, is_vector = convert_to_payload(vectors)
+        path = UPSERT_PATH if is_vector else UPSERT_DATA_PATH
 
-        return await self._execute_request_async(payload=payload, path=UPSERT_PATH)
+        return await self._execute_request_async(payload=payload, path=path)
 
     async def query(
         self,
-        vector: Union[List[float], SupportsToList],
+        vector: Optional[Union[List[float], SupportsToList]] = None,
         top_k: int = 10,
         include_vectors: bool = False,
         include_metadata: bool = False,
         filter: str = "",
+        data: Optional[str] = None,
     ) -> List[QueryResult]:
         """
-        Query `top_k` many similar vectors asynchronously.
+        Query `top_k` many similar vectors. Requires either `data` or `vector` fields. Raises exception if `data` and `vector` fields are both used.
 
         :param vector: list of floats for the values of vector.
         :param top_k: number that indicates how many vectors will be returned as the query result.
         :param include_vectors: bool value that indicates whether the resulting top_k vectors will have their vector values shown.
         :param include_metadata: bool value that indicates whether the resulting top_k vectors will have their metadata shown.
+        :param filter: filter expression to narrow down the query results.
+        :param data: string (to be embedded) to query for
 
         Example usage:
 
         ```python
         query_res = await index.query(
             vector=[0.6, 0.9],
             top_k=3,
             include_vectors=True,
             include_metadata=True,
         )
         ```
+
+        ```python
+        query_res = await index.query(
+            data="hello"
+            top_k=3,
+            include_vectors=True,
+            include_metadata=True,
+        )
+        ```
         """
         payload = {
-            "vector": convert_to_list(vector),
             "topK": top_k,
             "includeVectors": include_vectors,
             "includeMetadata": include_metadata,
             "filter": filter,
         }
+
+        if data is None and vector is None:
+            raise ClientError("either `data` or `vector` values must be given")
+        if data is not None and vector is not None:
+            raise ClientError(
+                "`data` and `vector` values cannot be given at the same time"
+            )
+
+        if data is not None:
+            payload["data"] = data
+            path = QUERY_DATA_PATH
+        else:
+            payload["vector"] = convert_to_list(vector)
+            path = QUERY_PATH
+
         return [
             QueryResult._from_json(obj)
-            for obj in await self._execute_request_async(
-                payload=payload, path=QUERY_PATH
-            )
+            for obj in await self._execute_request_async(payload=payload, path=path)
         ]
 
     async def delete(self, ids: Union[str, List[str]]) -> DeleteResult:
         """
         Deletes the given vector(s) with given ids asynchronously.
 
         Response contains deleted vector count.
```

### Comparing `upstash_vector-0.2.1/upstash_vector/http.py` & `upstash_vector-0.3.0/upstash_vector/http.py`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.2.1/upstash_vector/types.py` & `upstash_vector-0.3.0/upstash_vector/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 class SupportsToList(Protocol):
     def tolist(self) -> List[float]:
         ...
 
 
 @dataclass
 class Vector:
-    id: str
+    id: Union[int, str]
     vector: Union[List[float], SupportsToList]
     metadata: Optional[Dict] = None
 
 
 @dataclass
+class Data:
+    id: Union[int, str]
+    data: str
+    metadata: Optional[Dict] = None
+
+
+@dataclass
 class FetchResult:
     id: str
     vector: Optional[List[float]] = None
     metadata: Optional[Dict] = None
 
     @classmethod
     def _from_json(cls, obj: dict) -> "FetchResult":
```

### Comparing `upstash_vector-0.2.1/PKG-INFO` & `upstash_vector-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-vector
-Version: 0.2.1
+Version: 0.3.0
 Summary: Serverless Vector SDK from Upstash
 Home-page: https://github.com/upstash/vector-py
 License: MIT
 Keywords: Upstash Vector,Serverless Vector
 Author: Upstash
 Author-email: support@upstash.com
 Maintainer: Upstash
@@ -182,14 +182,26 @@
 
 ## Code Formatting
 ```bash 
 poetry run ruff format .
 ```
 
 ## Running tests
+
 To run all the tests, make sure the poetry virtual environment activated with all 
-the necessary dependencies. Set the necessary environment variables and run:
+the necessary dependencies.
+
+Create two Vector Stores on upstash. First one should have 2 dimensions. Second one should use an embedding model. Set the necessary environment variables:
+
+```
+URL=****
+TOKEN=****
+EMBEDDING_URL=****
+EMBEDDING_TOKEN=****
+```
+
+Then, run the following command to run tests:
 
 ```bash
 poetry run pytest
 ```
```

