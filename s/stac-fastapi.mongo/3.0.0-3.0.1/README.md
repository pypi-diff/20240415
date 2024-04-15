# Comparing `tmp/stac-fastapi.mongo-3.0.0.tar.gz` & `tmp/stac_fastapi_mongo-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.mongo-3.0.0.tar", last modified: Sun Mar 10 16:17:38 2024, max compression
+gzip compressed data, was "stac_fastapi_mongo-3.0.1.tar", last modified: Mon Apr 15 06:55:54 2024, max compression
```

## Comparing `stac-fastapi.mongo-3.0.0.tar` & `stac_fastapi_mongo-3.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-10 16:17:38.605581 stac-fastapi.mongo-3.0.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/LICENSE
--rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 15:53:44.000000 stac-fastapi.mongo-3.0.0/MANIFEST.in
--rw-r--r--   0 primeradiant   (501) staff       (20)     2834 2024-03-10 16:17:38.599279 stac-fastapi.mongo-3.0.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)     1483 2024-03-10 15:59:02.000000 stac-fastapi.mongo-3.0.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-03-10 16:17:38.605818 stac-fastapi.mongo-3.0.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1495 2024-03-10 16:07:23.000000 stac-fastapi.mongo-3.0.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-10 16:17:38.538654 stac-fastapi.mongo-3.0.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-10 16:17:38.582426 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/
--rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2979 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2499 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    39725 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1072 2024-03-03 16:18:26.000000 stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/utilities.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-10 16:17:38.587502 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     2834 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      488 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      219 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-03-10 16:17:38.000000 stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.546510 stac_fastapi_mongo-3.0.1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac_fastapi_mongo-3.0.1/LICENSE
+-rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.0.1/MANIFEST.in
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3194 2024-04-15 06:55:54.545365 stac_fastapi_mongo-3.0.1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1843 2024-04-15 06:40:35.000000 stac_fastapi_mongo-3.0.1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-04-15 06:55:54.546884 stac_fastapi_mongo-3.0.1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1495 2024-04-15 06:46:05.000000 stac_fastapi_mongo-3.0.1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.464399 stac_fastapi_mongo-3.0.1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.527717 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       25 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2995 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2477 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    39873 2024-04-15 06:40:35.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1072 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/utilities.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.529154 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3194 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      488 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      219 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/top_level.txt
```

### Comparing `stac-fastapi.mongo-3.0.0/LICENSE` & `stac_fastapi_mongo-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-fastapi.mongo-3.0.0/PKG-INFO` & `stac_fastapi_mongo-3.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.mongo
-Version: 3.0.0
+Version: 3.0.1
 Summary: Mongodb stac-fastapi backend.
 Home-page: https://github.com/Healy-Hyperspatial/stac-fastapi-mongo
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -35,15 +35,16 @@
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
 # stac-fastapi-mongo
 
 ## Mongo backend for the stac-fastapi project built on top of the [sfeos](https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch) core api library. 
 
-   
+[![PyPI version](https://badge.fury.io/py/stac-fastapi.mongo.svg)](https://badge.fury.io/py/stac-fastapi.mongo)
+[![Join the chat at https://gitter.im/stac-fastapi-mongo/community](https://badges.gitter.im/stac-fastapi-mongo/community.svg)](https://gitter.im/stac-fastapi-mongo/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 To install from PyPI:
 
 ```shell
 pip install stac_fastapi.mongo
 ```
 
@@ -65,15 +66,15 @@
 
 Prior to commit, run:
 
 ```shell
 pre-commit run --all-files
 ```
 
-## Build Elasticsearh API backend
+## Build stac-fastapi.mongo backend
 
 ```shell
 docker-compose up mongo
 docker-compose build app-mongo
 ```
   
 ## Running Mongo API on localhost:8084
```

### Comparing `stac-fastapi.mongo-3.0.0/README.md` & `stac_fastapi_mongo-3.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stac-fastapi-mongo
 
 ## Mongo backend for the stac-fastapi project built on top of the [sfeos](https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch) core api library. 
 
-   
+[![PyPI version](https://badge.fury.io/py/stac-fastapi.mongo.svg)](https://badge.fury.io/py/stac-fastapi.mongo)
+[![Join the chat at https://gitter.im/stac-fastapi-mongo/community](https://badges.gitter.im/stac-fastapi-mongo/community.svg)](https://gitter.im/stac-fastapi-mongo/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 To install from PyPI:
 
 ```shell
 pip install stac_fastapi.mongo
 ```
 
@@ -28,15 +29,15 @@
 
 Prior to commit, run:
 
 ```shell
 pre-commit run --all-files
 ```
 
-## Build Elasticsearh API backend
+## Build stac-fastapi.mongo backend
 
 ```shell
 docker-compose up mongo
 docker-compose build app-mongo
 ```
   
 ## Running Mongo API on localhost:8084
```

### Comparing `stac-fastapi.mongo-3.0.0/setup.py` & `stac_fastapi_mongo-3.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
     "server": ["uvicorn[standard]==0.19.0"],
 }
 
 setup(
     name="stac-fastapi.mongo",
-    version="3.0.0",
+    version="3.0.1",
     description="Mongodb stac-fastapi backend.",
     long_description=desc,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

### Comparing `stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/app.py` & `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """FastAPI application."""
 
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_get_request_model, create_post_request_model
-from stac_fastapi.core.core import (
-    BulkTransactionsClient,
+from stac_fastapi.core.core import (  # BulkTransactionsClient,
     CoreClient,
     EsAsyncBaseFiltersClient,
     TransactionsClient,
 )
 from stac_fastapi.core.extensions import QueryExtension
 from stac_fastapi.core.session import Session
 from stac_fastapi.extensions.core import (
     ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
-from stac_fastapi.extensions.third_party import BulkTransactionExtension
+
+# from stac_fastapi.extensions.third_party import BulkTransactionExtension
 from stac_fastapi.mongo.config import AsyncMongoDBSettings
 from stac_fastapi.mongo.database_logic import (
     DatabaseLogic,
     create_collection_index,
     create_item_index,
 )
 
@@ -39,21 +39,21 @@
 extensions = [
     TransactionExtension(
         client=TransactionsClient(
             database=database_logic, session=session, settings=settings
         ),
         settings=settings,
     ),
-    BulkTransactionExtension(
-        client=BulkTransactionsClient(
-            database=database_logic,
-            session=session,
-            settings=settings,
-        )
-    ),
+    # BulkTransactionExtension(
+    #     client=BulkTransactionsClient(
+    #         database=database_logic,
+    #         session=session,
+    #         settings=settings,
+    #     )
+    # ),
     FieldsExtension(),
     QueryExtension(),
     SortExtension(),
     TokenPaginationExtension(),
     ContextExtension(),
     filter_extension,
 ]
```

### Comparing `stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/config.py` & `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,9 +68,8 @@
     forbidden_fields: Set[str] = _forbidden_fields
     indexed_fields: Set[str] = {"datetime"}
 
     @property
     def create_client(self) -> AsyncIOMotorClient:
         """Create an asynchronous MongoDB client."""
         config = _mongodb_config()
-        print(config)
         return AsyncIOMotorClient(config["uri"])
```

### Comparing `stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/database_logic.py` & `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/database_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,31 +550,39 @@
         """
         db = self.client[DATABASE]
         collection = db[ITEMS_INDEX]
 
         query = {"$and": search.filters} if search and search.filters else {}
 
         print("Query: ", query)
+
         if collection_ids:
             query["collection"] = {"$in": collection_ids}
 
         sort_criteria = sort if sort else [("id", 1)]  # Default sort
+
         try:
             if token:
                 last_id = decode_token(token)
-                query["id"] = {"$gt": last_id}
-
-            cursor = collection.find(query).sort(sort_criteria).limit(limit + 1)
+                skip_count = int(last_id)
+            else:
+                skip_count = 0
+
+            cursor = (
+                collection.find(query)
+                .sort(sort_criteria)
+                .skip(skip_count)
+                .limit(limit + 1)
+            )
             items = await cursor.to_list(length=limit + 1)
 
             next_token = None
             if len(items) > limit:
-                next_token = base64.urlsafe_b64encode(
-                    str(items[-1]["_id"]).encode()
-                ).decode()
+                next_skip = skip_count + limit
+                next_token = base64.urlsafe_b64encode(str(next_skip).encode()).decode()
                 items = items[:-1]
 
             maybe_count = None
             if not token:
                 maybe_count = await collection.count_documents(query)
 
             return items, maybe_count, next_token
@@ -611,15 +619,15 @@
         Asynchronously inserts a STAC item into MongoDB, ensuring the item does not already exist.
 
         Args:
             item (Item): The STAC item to be created.
             refresh (bool, optional): Not used for MongoDB, kept for compatibility with Elasticsearch interface.
 
         Raises:
-            ConflictError: If the item with the same ID already exists within the collection.
+            ConflictError: If the item with the same ID already exists within the collection
             NotFoundError: If the specified collection does not exist in MongoDB.
         """
         db = self.client[DATABASE]
         items_collection = db[ITEMS_INDEX]
         collections_collection = db[COLLECTIONS_INDEX]
 
         collection_exists = await collections_collection.count_documents(
@@ -632,14 +640,15 @@
         new_item["_id"] = item.get("_id", ObjectId())
 
         existing_item = await items_collection.find_one({"_id": new_item["_id"]})
         if existing_item:
             raise ConflictError(f"Item with _id {item['_id']} already exists")
 
         await items_collection.insert_one(new_item)
+
         item = serialize_doc(item)
 
     async def prep_create_item(
         self, item: Item, base_url: str, exist_ok: bool = False
     ) -> Item:
         """
         Preps an item for insertion into the MongoDB database.
```

### Comparing `stac-fastapi.mongo-3.0.0/stac_fastapi/mongo/utilities.py` & `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/utilities.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.mongo-3.0.0/stac_fastapi.mongo.egg-info/PKG-INFO` & `stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.mongo
-Version: 3.0.0
+Version: 3.0.1
 Summary: Mongodb stac-fastapi backend.
 Home-page: https://github.com/Healy-Hyperspatial/stac-fastapi-mongo
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -35,15 +35,16 @@
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
 # stac-fastapi-mongo
 
 ## Mongo backend for the stac-fastapi project built on top of the [sfeos](https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch) core api library. 
 
-   
+[![PyPI version](https://badge.fury.io/py/stac-fastapi.mongo.svg)](https://badge.fury.io/py/stac-fastapi.mongo)
+[![Join the chat at https://gitter.im/stac-fastapi-mongo/community](https://badges.gitter.im/stac-fastapi-mongo/community.svg)](https://gitter.im/stac-fastapi-mongo/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 To install from PyPI:
 
 ```shell
 pip install stac_fastapi.mongo
 ```
 
@@ -65,15 +66,15 @@
 
 Prior to commit, run:
 
 ```shell
 pre-commit run --all-files
 ```
 
-## Build Elasticsearh API backend
+## Build stac-fastapi.mongo backend
 
 ```shell
 docker-compose up mongo
 docker-compose build app-mongo
 ```
   
 ## Running Mongo API on localhost:8084
```

