# Comparing `tmp/MinVectorDB-0.2.4.tar.gz` & `tmp/minvectordb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinVectorDB-0.2.4.tar", last modified: Tue Apr  2 10:44:44 2024, max compression
+gzip compressed data, was "minvectordb-0.2.5.tar", last modified: Mon Apr 15 05:22:21 2024, max compression
```

## Comparing `MinVectorDB-0.2.4.tar` & `minvectordb-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.925522 MinVectorDB-0.2.4/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 MinVectorDB-0.2.4/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924993 MinVectorDB-0.2.4/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    18634 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)      950 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      145 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    18634 2024-04-02 10:44:44.925266 MinVectorDB-0.2.4/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    17426 2024-04-02 10:37:16.000000 MinVectorDB-0.2.4/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920038 MinVectorDB-0.2.4/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)       81 2024-04-02 09:07:59.000000 MinVectorDB-0.2.4/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920376 MinVectorDB-0.2.4/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 MinVectorDB-0.2.4/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10441 2024-04-02 10:16:24.000000 MinVectorDB-0.2.4/min_vec/api/api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920725 MinVectorDB-0.2.4/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 MinVectorDB-0.2.4/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2245 2024-04-02 08:22:33.000000 MinVectorDB-0.2.4/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.921071 MinVectorDB-0.2.4/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 MinVectorDB-0.2.4/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2184 2024-04-02 10:16:24.000000 MinVectorDB-0.2.4/min_vec/configs/config.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.922296 MinVectorDB-0.2.4/min_vec/data_structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 MinVectorDB-0.2.4/min_vec/data_structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-03-07 02:06:51.000000 MinVectorDB-0.2.4/min_vec/data_structures/fields_mapper.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 MinVectorDB-0.2.4/min_vec/data_structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1578 2024-03-28 05:59:46.000000 MinVectorDB-0.2.4/min_vec/data_structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)      687 2024-04-02 10:06:58.000000 MinVectorDB-0.2.4/min_vec/data_structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-02 09:57:20.000000 MinVectorDB-0.2.4/min_vec/data_structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.923297 MinVectorDB-0.2.4/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 MinVectorDB-0.2.4/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    29345 2024-04-02 09:51:33.000000 MinVectorDB-0.2.4/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9163 2024-04-02 08:40:53.000000 MinVectorDB-0.2.4/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 MinVectorDB-0.2.4/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.923640 MinVectorDB-0.2.4/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 MinVectorDB-0.2.4/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    21534 2024-04-02 10:06:58.000000 MinVectorDB-0.2.4/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924132 MinVectorDB-0.2.4/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 MinVectorDB-0.2.4/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4533 2024-04-01 09:19:24.000000 MinVectorDB-0.2.4/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-02 10:44:44.925562 MinVectorDB-0.2.4/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1422 2024-04-02 09:07:59.000000 MinVectorDB-0.2.4/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924637 MinVectorDB-0.2.4/test/
--rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 MinVectorDB-0.2.4/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    12645 2024-03-07 02:27:36.000000 MinVectorDB-0.2.4/test/test_model.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645943 minvectordb-0.2.5/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.5/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645464 minvectordb-0.2.5/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    17717 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.5/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    17717 2024-04-15 05:22:21.645708 minvectordb-0.2.5/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    16402 2024-04-15 04:50:27.000000 minvectordb-0.2.5/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.639970 minvectordb-0.2.5/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-08 06:55:08.000000 minvectordb-0.2.5/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.640289 minvectordb-0.2.5/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.5/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11729 2024-04-15 03:57:26.000000 minvectordb-0.2.5/min_vec/api/api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.640646 minvectordb-0.2.5/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.5/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      931 2024-04-13 16:15:59.000000 minvectordb-0.2.5/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.641230 minvectordb-0.2.5/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.5/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2896 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-15 03:56:30.000000 minvectordb-0.2.5/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.642668 minvectordb-0.2.5/min_vec/data_structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.5/min_vec/data_structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.5/min_vec/data_structures/fields_mapper.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.5/min_vec/data_structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/data_structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.5/min_vec/data_structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2587 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/data_structures/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.5/min_vec/data_structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.643803 minvectordb-0.2.5/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.5/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2541 2024-04-13 15:41:43.000000 minvectordb-0.2.5/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    19860 2024-04-15 02:51:07.000000 minvectordb-0.2.5/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9989 2024-04-13 15:53:22.000000 minvectordb-0.2.5/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.5/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.644117 minvectordb-0.2.5/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.5/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    16973 2024-04-13 15:51:50.000000 minvectordb-0.2.5/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.644518 minvectordb-0.2.5/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.5/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.5/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-15 05:22:21.645982 minvectordb-0.2.5/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1470 2024-04-12 09:51:44.000000 minvectordb-0.2.5/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645152 minvectordb-0.2.5/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.5/test/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.5/test/test_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.5/test/test_save_and_query.py
```

### Comparing `MinVectorDB-0.2.4/LICENSE` & `minvectordb-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.4/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,42 @@
-Metadata-Version: 2.1
-Name: MinVectorDB
-Version: 0.2.4
-Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
-Home-page: https://github.com/BirchKwok/MinVectorDB
-Author: Birch Kwok
-Author-email: birchkwok@gmail.com
-Keywords: vector database
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: spinesUtils>=0.3.13
-Requires-Dist: torch>=2.0.0
-Requires-Dist: msgpack>=1.0.2
-Requires-Dist: h5py>=3.4.0
-Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: cloudpickle>=2.0.0
-Requires-Dist: numexpr>=2.7.3
-Requires-Dist: pyroaring>=0.4.5
-
 <div align="center">
-  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
-  <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
+  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-<div align="center">
-  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
-</div>
+⚡ **Serverless, simple parameters, simple API.**
+
+⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
+
+⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
+
+⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
+
+⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
+
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
-
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
 ```shell
@@ -95,39 +70,34 @@
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
 os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
-# computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.3
+    MinVectorDB version is:  0.2.5
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
-     - MVDB_COMPUTE_DEVICE: cpu
-     - MVDB_USER_MESSAGE_PATH: None
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -141,33 +111,33 @@
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
-                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
         if id == 0:
-            query = t / np.linalg.norm(t)
+            query = t
             query_id = 0
             query_field = None
-        # Vectors need to be normalized before writing to the database.
-        db.add_item(t, index=id, normalize=True, save_immediately=False)
+        # Vectors will be normalized after writing to the database.
+        db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
@@ -175,34 +145,33 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=100000,
+    //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=False, 
-    //    reindex_if_conflict=False, scaler_bits=8
+    //    dtypes='float32', use_cache=True, 
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
+    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (1000000, 1024)
-    | - Query time: 0.34045 s
+    | - Query time: 0.52161 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
-    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
-     0.78069043 0.7806051  0.78056455 0.78041667]
+    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+     0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
@@ -221,60 +190,57 @@
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t 
+            query_id = id
+            query_field = None
         vectors.append((t, id))
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
-    db.bulk_add_items(vectors, normalize=True, save_immediately=False)
-
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.03720 s
+    | - Query time: 0.10599 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+     0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
@@ -286,66 +252,66 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
+    db.bulk_add_items(vectors)
 
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
+
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01311 s
+    | - Query time: 0.08010 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
-     0.7637025  0.7637025  0.7620634  0.7620634 ]
+    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+     0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
 
@@ -364,23 +330,23 @@
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
+
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
@@ -390,33 +356,32 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01752 s
+    | - Query time: 0.05818 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
-     0.7559968  0.7528333  0.74891967 0.7427169 ]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
@@ -427,32 +392,31 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     last_field = None
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
 res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
@@ -464,29 +428,28 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
-    //    distance='L2', index_mode='IVF-FLAT', 
+    //    n_clusters=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.02081 s
+    | - Query time: 0.00418 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
-    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
-     0.69857436 0.7030885  0.70863307 0.70987064]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `MinVectorDB-0.2.4/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.2.5/MinVectorDB.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 min_vec/__init__.py
 min_vec/api/__init__.py
 min_vec/api/api.py
 min_vec/computational_layer/__init__.py
 min_vec/computational_layer/engines.py
 min_vec/configs/__init__.py
 min_vec/configs/config.py
+min_vec/configs/parameters_validator.py
 min_vec/data_structures/__init__.py
 min_vec/data_structures/fields_mapper.py
 min_vec/data_structures/filter.py
 min_vec/data_structures/kmeans.py
 min_vec/data_structures/limited_dict.py
+min_vec/data_structures/limited_sort.py
 min_vec/data_structures/scaler.py
 min_vec/execution_layer/__init__.py
+min_vec/execution_layer/cluster_worker.py
 min_vec/execution_layer/matrix_serializer.py
 min_vec/execution_layer/query.py
 min_vec/execution_layer/session.py
 min_vec/storage_layer/__init__.py
 min_vec/storage_layer/storage.py
 min_vec/utils/__init__.py
 min_vec/utils/utils.py
 test/__init__.py
-test/test_model.py
+test/test_initial.py
+test/test_save_and_query.py
```

### Comparing `MinVectorDB-0.2.4/PKG-INFO` & `minvectordb-0.2.5/MinVectorDB.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.4
+Version: 0.2.5
 Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: spinesUtils>=0.3.13
-Requires-Dist: torch>=2.0.0
 Requires-Dist: msgpack>=1.0.2
 Requires-Dist: h5py>=3.4.0
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: numexpr>=2.7.3
 Requires-Dist: pyroaring>=0.4.5
+Requires-Dist: jax>=0.4.25
+Requires-Dist: numba>=0.54.0
+Requires-Dist: jaxlib>=0.4.25
 
 <div align="center">
-  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
-  <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
+  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-<div align="center">
-  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
-</div>
+⚡ **Serverless, simple parameters, simple API.**
+
+⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
+
+⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
+
+⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
+
+⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
+
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
-
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
 ```shell
@@ -95,39 +103,34 @@
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
 os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
-# computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.3
+    MinVectorDB version is:  0.2.5
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
-     - MVDB_COMPUTE_DEVICE: cpu
-     - MVDB_USER_MESSAGE_PATH: None
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -141,33 +144,33 @@
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
-                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
         if id == 0:
-            query = t / np.linalg.norm(t)
+            query = t
             query_id = 0
             query_field = None
-        # Vectors need to be normalized before writing to the database.
-        db.add_item(t, index=id, normalize=True, save_immediately=False)
+        # Vectors will be normalized after writing to the database.
+        db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
@@ -175,34 +178,33 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=100000,
+    //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=False, 
-    //    reindex_if_conflict=False, scaler_bits=8
+    //    dtypes='float32', use_cache=True, 
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
+    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (1000000, 1024)
-    | - Query time: 0.34045 s
+    | - Query time: 0.52161 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
-    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
-     0.78069043 0.7806051  0.78056455 0.78041667]
+    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+     0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
@@ -221,60 +223,57 @@
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t 
+            query_id = id
+            query_field = None
         vectors.append((t, id))
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
-    db.bulk_add_items(vectors, normalize=True, save_immediately=False)
-
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.03720 s
+    | - Query time: 0.10599 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+     0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
@@ -286,66 +285,66 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
+    db.bulk_add_items(vectors)
 
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
+
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01311 s
+    | - Query time: 0.08010 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
-     0.7637025  0.7637025  0.7620634  0.7620634 ]
+    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+     0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
 
@@ -364,23 +363,23 @@
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
+
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
@@ -390,33 +389,32 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01752 s
+    | - Query time: 0.05818 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
-     0.7559968  0.7528333  0.74891967 0.7427169 ]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
@@ -427,32 +425,31 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     last_field = None
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
 res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
@@ -464,29 +461,28 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
-    //    distance='L2', index_mode='IVF-FLAT', 
+    //    n_clusters=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.02081 s
+    | - Query time: 0.00418 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
-    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
-     0.69857436 0.7030885  0.70863307 0.70987064]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `MinVectorDB-0.2.4/README.md` & `minvectordb-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,75 @@
+Metadata-Version: 2.1
+Name: MinVectorDB
+Version: 0.2.5
+Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
+Home-page: https://github.com/BirchKwok/MinVectorDB
+Author: Birch Kwok
+Author-email: birchkwok@gmail.com
+Keywords: vector database
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: spinesUtils>=0.3.13
+Requires-Dist: msgpack>=1.0.2
+Requires-Dist: h5py>=3.4.0
+Requires-Dist: scikit-learn>=1.0.0
+Requires-Dist: cloudpickle>=2.0.0
+Requires-Dist: numexpr>=2.7.3
+Requires-Dist: pyroaring>=0.4.5
+Requires-Dist: jax>=0.4.25
+Requires-Dist: numba>=0.54.0
+Requires-Dist: jaxlib>=0.4.25
+
 <div align="center">
-  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
-  <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
+  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-<div align="center">
-  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
-</div>
+⚡ **Serverless, simple parameters, simple API.**
+
+⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
+
+⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
+
+⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
+
+⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
+
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
-
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
 ```shell
@@ -65,39 +103,34 @@
 
 # query cache size
 os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
 os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
-# computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
-
 # specify the number of chunks in the memory cache
 os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.3
+    MinVectorDB version is:  0.2.5
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
      - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
-     - MVDB_COMPUTE_DEVICE: cpu
-     - MVDB_USER_MESSAGE_PATH: None
      - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
 ### Sequentially add vectors.
 
 
 ```python
@@ -111,33 +144,33 @@
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
 # distance can be 'L2' or 'cosine'
 # index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
-                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', index_mode='FLAT',
+                 chunk_size=100000, use_cache=False, scaler_bits=8, n_threads=10, distance='cosine')
 
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
     for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
         if id == 0:
-            query = t / np.linalg.norm(t)
+            query = t
             query_id = 0
             query_field = None
-        # Vectors need to be normalized before writing to the database.
-        db.add_item(t, index=id, normalize=True, save_immediately=False)
+        # Vectors will be normalized after writing to the database.
+        db.add_item(t, index=id)
 
         id += 1
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
@@ -145,34 +178,33 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=100000,
+    //    n_clusters=16, chunk_size=100000,
     //    distance='cosine', index_mode='FLAT', 
-    //    dtypes='float32', use_cache=False, 
-    //    reindex_if_conflict=False, scaler_bits=8
+    //    dtypes='float32', use_cache=True, 
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
-    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
+    100%|██████████| 1000000/1000000 [00:12<00:00, 81258.92vector/s]
 
 
       - Query sample id:  0
       - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (1000000, 1024)
-    | - Query time: 0.34045 s
+    | - Query time: 0.52161 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
-    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
-     0.78069043 0.7806051  0.78056455 0.78041667]
+    | - Top 10 results index: [     0 126163 934623 376250 136782 927723  67927 454821 909201 226748]
+    | - Top 10 results similarity: [0.996918 0.783403 0.779208 0.778662 0.778039 0.777809 0.777673 0.777481
+     0.777456 0.777079]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
@@ -191,60 +223,57 @@
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t 
+            query_id = id
+            query_field = None
         vectors.append((t, id))
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
-    db.bulk_add_items(vectors, normalize=True, save_immediately=False)
-
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
-res = db.query(query, k=10)
+res = db.query(query, k=10, return_similarity=True)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.03720 s
+    | - Query time: 0.10599 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [    0 67927 53447 47665 13859  5788 41949 64134 38082 18507]
+    | - Top 10 results similarity: [0.997411 0.778021 0.774815 0.774266 0.77306  0.77304  0.772899 0.772897
+     0.772079 0.771447]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
@@ -256,66 +285,66 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
+    db.bulk_add_items(vectors)
 
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
+
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01311 s
+    | - Query time: 0.08010 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
-     0.7637025  0.7637025  0.7620634  0.7620634 ]
+    | - Top 10 results index: [ 0 60 76 63 52 14 27 61 83 79]
+    | - Top 10 results similarity: [0.997411 0.75152  0.748989 0.748342 0.746665 0.745256 0.743775 0.739018
+     0.730766 0.728236]
     * - END OF REPORT -
     
 
 
 ### Use subset_indices to narrow down the search range
 
 
@@ -334,23 +363,23 @@
 db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
+
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
@@ -360,33 +389,32 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
+    //    n_clusters=16, chunk_size=10000,
     //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.01752 s
+    | - Query time: 0.05818 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
-    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
-     0.7559968  0.7528333  0.74891967 0.7427169 ]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
     
 
 
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
@@ -397,32 +425,31 @@
 
 # Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
 
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     last_field = None
     for t in get_test_vectors((100000, 1024)):
-        # Vectors need to be normalized before writing to the database.
+        if id == 0:
+            query = t
+            query_id = id
+            query_field = 'test_'+str(id // 100)
         vectors.append((t, id, 'test_'+str(id // 100)))
         id += 1
         
-    db.bulk_add_items(vectors, normalize=True)
-
-query = db.head(10)[0]
-query_id = db.head(10, returns='indices')[0]
-query_field = db.head(10, returns='fields')[0]
+    db.bulk_add_items(vectors)
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
 res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
@@ -434,29 +461,28 @@
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=16, chunk_size=10000,
-    //    distance='L2', index_mode='IVF-FLAT', 
+    //    n_clusters=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
     //    dtypes='float32', use_cache=True, 
-    //    reindex_if_conflict=False, scaler_bits=None
+    //    scaler_bits=8
     
     MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-      - Query sample id:  11
+      - Query sample id:  0
       - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.02081 s
+    | - Query time: 0.00418 s
     | - Query K: 10
-    | - Query normalize: False
-    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
-    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
-     0.69857436 0.7030885  0.70863307 0.70987064]
+    | - Top 10 results index: [ 0  9 14  7  3  1 19 18  8 17]
+    | - Top 10 results similarity: [0.997411   0.75857097 0.745256   0.742031   0.741346   0.737684
+     0.737088   0.734952   0.733552   0.730605  ]
     * - END OF REPORT -
```

### Comparing `MinVectorDB-0.2.4/min_vec/api/api.py` & `minvectordb-0.2.5/min_vec/api/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,248 @@
 """api.py - The MinVectorDB API."""
-import gc
+import os
+from typing import Union, List, Tuple
 
-from min_vec.configs.config import *
+import numpy as np
+from spinesUtils.asserts import raise_if, ParameterTypeAssert
+from spinesUtils.logging import Logger
+from spinesUtils.timer import Timer
+
+from min_vec.configs.config import config
+from min_vec.configs.parameters_validator import ParametersValidator
+from min_vec.execution_layer.query import Query
+from min_vec.execution_layer.matrix_serializer import MatrixSerializer
+from min_vec.utils.utils import unavailable_if_deleted
+
+logger = Logger(
+    fp=config.MVDB_LOG_PATH,
+    name='MinVectorDB',
+    truncate_file=config.MVDB_TRUNCATE_LOG,
+    with_time=config.MVDB_LOG_WITH_TIME,
+    level=config.MVDB_LOG_LEVEL
+)
 
 
 class MinVectorDB:
     """
     A class for managing a vector database stored in .mvdb files and computing vectors similarity.
     """
 
-    from spinesUtils.asserts import ParameterValuesAssert, ParameterTypeAssert
-
+    @ParametersValidator(
+        update_configs=['dim', 'database_path', 'n_clusters', 'chunk_size', 'index_mode', 'dtypes', 'scaler_bits',
+                        'distance'],
+        logger=logger
+    )
     @ParameterTypeAssert({
-        'use_cache': bool, 'reindex_if_conflict': bool
+        'dim': int,
+        'database_path': str,
+        'n_clusters': int,
+        'chunk_size': int,
+        'distance': str,
+        'index_mode': str,
+        'dtypes': str,
+        'use_cache': bool,
+        'scaler_bits': (None, int),
+        'n_threads': (None, int)
     }, func_name='MinVectorDB')
     def __init__(
-            self, dim, database_path, n_cluster=16, chunk_size=100_000, distance='cosine',
-            index_mode='IVF-FLAT', dtypes='float32',
-            use_cache=True, reindex_if_conflict=False, scaler_bits=None, n_threads=None
+            self, dim: int, database_path: str, n_clusters: int = 16, chunk_size: int = 100_000,
+            distance: str = 'cosine', index_mode: str = 'IVF-FLAT', dtypes: str = 'float32',
+            use_cache: bool = True, scaler_bits: int = 8, n_threads: int = None
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
-            n_cluster (int): The number of clusters for the IVF-FLAT index. Default is 8.
+            n_clusters (int): The number of clusters for the IVF-FLAT index. Default is 8.
             chunk_size (int): The size of each data chunk. Default is 100_000.
             distance (str): Method for calculating vector distance.
                 Options are 'cosine' or 'L2' for Euclidean distance. Default is 'cosine'.
             index_mode (str): The storage mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             use_cache (bool): Whether to use cache for query. Default is True.
-            reindex_if_conflict (bool): Whether to reindex if there is a conflict. Default is False.
             scaler_bits (int): The number of bits for scalar quantization.
                 Options are 8, 16, or 32. The default is None, which means no scalar quantization.
                 The 8 for 8-bit, 16 for 16-bit, and 32 for 32-bit.
-            n_threads (int): The number of threads to use for parallel processing. Default is None,
-                which means the number of CPUs.
+            n_threads (int): The number of threads to use for parallel processing. Default is None, which means using
+                twice the number of CPU cores.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
-        from spinesUtils.logging import Logger
-        from spinesUtils.timer import Timer
-
-        from min_vec.execution_layer.query import DatabaseQuery
-        from min_vec.execution_layer.matrix_serializer import MatrixSerializer
+        raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
+        raise_if(ValueError, chunk_size <= 1, 'chunk_size must greater than 1')
+        raise_if(ValueError, distance not in ('cosine', 'L2'), 'distance must be "cosine" or "L2"')
+        raise_if(ValueError, index_mode not in ('FLAT', 'IVF-FLAT'), 'index_mode must be "FLAT" or "IVF-FLAT"')
+        raise_if(ValueError, dtypes not in ('float16', 'float32', 'float64'),
+                 'dtypes must be "float16", "float32" or "float64')
+        raise_if(ValueError, not isinstance(n_clusters, int) or n_clusters <= 0,
+                 'n_clusters must be int and greater than 0')
+        raise_if(ValueError, scaler_bits not in (8, 16, 32, None), 'sq_bits must be 8, 16, 32 or None')
 
-        logger = Logger(
-            fp=MVDB_LOG_PATH,
-            name='MinVectorDB',
-            truncate_file=MVDB_TRUNCATE_LOG,
-            with_time=MVDB_LOG_WITH_TIME,
-            level=MVDB_LOG_LEVEL
-        )
         logger.info("Initializing MinVectorDB with: \n "
                     f"\r//    dim={dim}, database_path='{database_path}', \n"
-                    f"\r//    n_cluster={n_cluster}, chunk_size={chunk_size},\n"
+                    f"\r//    n_clusters={n_clusters}, chunk_size={chunk_size},\n"
                     f"\r//    distance='{distance}', index_mode='{index_mode}', \n"
                     f"\r//    dtypes='{dtypes}', use_cache={use_cache}, \n"
-                    f"\r//    reindex_if_conflict={reindex_if_conflict}, scaler_bits={scaler_bits}\n"
+                    f"\r//    scaler_bits={scaler_bits}\n"
                     )
 
         if chunk_size <= 1:
             raise ValueError('chunk_size must be greater than 1')
 
         self._matrix_serializer = MatrixSerializer(
             dim=dim,
             database_path=database_path,
-            n_clusters=n_cluster,
+            n_clusters=n_clusters,
             chunk_size=chunk_size,
             distance=distance,
             index_mode=index_mode,
             logger=logger,
             dtypes=dtypes,
-            reindex_if_conflict=reindex_if_conflict,
-            scaler_bits=scaler_bits,
-            n_threads=n_threads
+            scaler_bits=scaler_bits
         )
-        # matrix_serializer functions
-        self.add_item = self._matrix_serializer.add_item
-        self.bulk_add_items = self._matrix_serializer.bulk_add_items
         self._data_loader = self._matrix_serializer.iterable_dataloader
-        self.check_commit = self._matrix_serializer.check_commit
         self._id_filter = self._matrix_serializer.id_filter
-        self.commit = self._matrix_serializer.commit
 
         self._timer = Timer()
-        self.use_cache = use_cache
-        self.distance = distance
+        self._use_cache = use_cache
+        self._distance = distance
+
+        raise_if(TypeError, n_threads is not None and not isinstance(n_threads, int), "n_threads must be an integer.")
+        raise_if(ValueError, n_threads is not None and n_threads <= 0, "n_threads must be greater than 0.")
 
-        self._matrix_query = DatabaseQuery(
-            matrix_serializer=self._matrix_serializer
+        self._query = Query(
+            matrix_serializer=self._matrix_serializer,
+            n_threads=n_threads if n_threads else 2 * os.cpu_count()
         )
 
-        self._matrix_query.query.clear_cache()
+        self._query.query.clear_cache()
 
         self._most_recent_query_report = {}
 
-    def query(self, vector, k: int | str = 12, *, fields: list = None, normalize: bool = False, subset_indices=None):
+    @unavailable_if_deleted
+    def add_item(self, vector: np.ndarray, *, index: int = None, field: str = None) -> int:
+        """
+        Add a single vector to the database.
+
+        Parameters:
+            vector (np.ndarray): The vector to be added.
+            index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
+            field (str, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
+                set to an empty string.
+
+        Returns:
+            int: The ID of the added vector.
+
+        Raises:
+            ValueError: If the vector dimensions don't match or the ID already exists.
+        """
+        return self._matrix_serializer.add_item(vector, index=index, field=field)
+
+    @unavailable_if_deleted
+    def bulk_add_items(
+            self, vectors: Union[List[Tuple[np.ndarray, int, str]], List[Tuple[np.ndarray, int]], List[np.ndarray]]
+    ):
+        """
+        Bulk add vectors to the database in batches.
+
+        Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
+            vector, id, field).
+
+        Returns:
+            list: A list of indices where the vectors are stored.
+        """
+        return self._matrix_serializer.bulk_add_items(vectors)
+
+    @unavailable_if_deleted
+    def commit(self):
+        """
+        Save the database, ensuring that all data is written to disk.
+        This method is required to be called after saving vectors to query them.
+        """
+        self._matrix_serializer.commit()
+
+    @unavailable_if_deleted
+    def query(self, vector: np.ndarray, k: Union[int, str] = 12, *, fields: List = None, subset_indices: List = None,
+              return_similarity: bool = True):
+        """
+        Query the database for the vectors most similar to the given vector in batches.
+
+        Parameters:
+            vector (np.ndarray): The query vector.
+            k (int or str): The number of nearest vectors to return. if be 'all', return all vectors.
+            fields (list, optional): The target of the vector.
+            subset_indices (list, optional): The subset of indices to query.
+            return_similarity (bool): Whether to return the similarity scores.Default is True.
+
+        Returns:
+            Tuple: The indices and similarity scores of the top k nearest vectors.
+
+        Raises:
+            ValueError: If the database is empty.
+        """
         import datetime
 
         self._most_recent_query_report = {}
 
         self._timer.start()
-        if self.use_cache:
-            res = self._matrix_query.query(vector=vector, k=k, fields=fields, normalize=normalize,
-                                           subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
-                                           distance=self.distance)
+        if self._use_cache:
+            res = self._query.query(vector=vector, k=k, fields=fields,
+                                    subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
+                                    distance=self._distance, return_similarity=return_similarity)
         else:
-            res = self._matrix_query.query(vector=vector, k=k, fields=fields, normalize=normalize,
-                                           subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
-                                           now_time=datetime.datetime.now().timestamp(), distance=self.distance)
+            res = self._query.query(vector=vector, k=k, fields=fields,
+                                    subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
+                                    now_time=datetime.datetime.now().timestamp(), distance=self._distance,
+                                    return_similarity=return_similarity)
 
         time_cost = self._timer.last_timestamp_diff()
         self._most_recent_query_report['Database shape'] = self.shape
         self._most_recent_query_report['Query time'] = f"{time_cost :>.5f} s"
         self._most_recent_query_report['Query K'] = k
-        self._most_recent_query_report['Query normalize'] = normalize
         self._most_recent_query_report[f'Top {k} results index'] = res[0]
-        self._most_recent_query_report[f'Top {k} results similarity'] = res[1]
+        if return_similarity:
+            self._most_recent_query_report[f'Top {k} results similarity'] = np.array([round(i, 6) for i in res[1]])
 
         return res
 
     @property
     def shape(self):
         """
         Return the shape of the entire database.
 
         Returns:
             tuple: The number of vectors and the dimension of each vector in the database.
         """
         return self._matrix_serializer.shape
 
-    def _get_n_elements(self, returns, n, from_tail=False):
-        """get the first/last n vectors/indices/fields in the database."""
-        import numpy as np
-
-        _database = None
-        _indices = []
-        _fields = []
-        for database, indices, fields in self._data_loader(read_chunk_only=False, from_tail=from_tail,
-                                                           order_read=True):
-            if _database is None:
-                _database = database
-            else:
-                _database = np.vstack((_database, database))
-
-            _indices.extend(indices)
-            _fields.extend(fields)
-
-            if _database.shape[0] >= n:
-                break
-
-        if _database is None:
-            return None
-
-        if returns == 'database':
-            return _database[:n, :]
-        elif returns == 'indices':
-            return [int(i) for i in _indices[:n]]
-        else:
-            return _fields[:n]
-
-    @ParameterTypeAssert({'n': int, 'returns': str})
-    @ParameterValuesAssert({'returns': ('database', 'indices', 'fields')})
-    def head(self, n=10, returns='database'):
-        """Return the first n vectors/indices/fields in the database.
-
-        Parameters:
-            n (int): The number of vectors to return.
-            returns (str): The type of data to return. Options are 'database', 'indices', or 'fields'.
-
-        Returns:
-            The first n vectors in the database.
-        """
-        self.check_commit()
-
-        if self._matrix_serializer.shape[0] == 0:
-            return None
-
-        return self._get_n_elements(returns, n, from_tail=False)
-
-    @ParameterTypeAssert({'n': int, 'returns': str})
-    @ParameterValuesAssert({'returns': ('database', 'indices', 'fields')})
-    def tail(self, n=10, returns='database'):
-        """Return the last n vectors/indices/fields in the database.
-
-        Parameters:
-            n (int): The number of vectors to return.
-            returns (str): The type of data to return. Options are 'database', 'indices', or 'fields'.
-
-        Returns:
-            The last n vectors/indices/fields in the database.
-        """
-        self.check_commit()
-
-        if self._matrix_serializer.shape[0] == 0:
-            return None
-
-        return self._get_n_elements(returns, n, from_tail=True)
-
+    @unavailable_if_deleted
     def insert_session(self):
         """
         Create a session to insert data, which will automatically commit the data when the session ends.
         """
         from min_vec.execution_layer.session import DatabaseSession
 
         return DatabaseSession(self)
 
+    @unavailable_if_deleted
     def delete(self):
         """
         Delete the database.
         """
+        import gc
+
         self._matrix_serializer.delete()
-        self._matrix_query.query.clear_cache()
+        self._query.query.clear_cache()
+        self._query.delete()
 
         gc.collect()
 
     @property
     def query_report_(self):
         """
         Return the most recent query report.
@@ -237,22 +258,21 @@
         return report
 
     @property
     def status_report_(self):
         """
         Return the database report.
         """
-        db_report = {'DATABASE STATUS REPORT':{
+        db_report = {'DATABASE STATUS REPORT': {
             'Database shape': (0, self._matrix_serializer.dim) if self._matrix_serializer.IS_DELETED else self.shape,
             'Database last_commit_time': self._matrix_serializer.last_commit_time,
             'Database commit status': self._matrix_serializer.COMMIT_FLAG,
             'Database index_mode': self._matrix_serializer.index_mode,
-            'Database distance': self.distance,
-            'Database use_cache': self.use_cache,
-            'Database reindex_if_conflict': self._matrix_serializer.reindex_if_conflict,
+            'Database distance': self._distance,
+            'Database use_cache': self._use_cache,
             'Database status': 'DELETED' if self._matrix_serializer.IS_DELETED else 'ACTIVE'
         }}
 
         return db_report
 
     def __repr__(self):
         title = "Deleted MinVectorDB object with status: \n"
@@ -265,8 +285,9 @@
     def __str__(self):
         return self.__repr__()
 
     def __len__(self):
         return self.shape[0]
 
     def is_deleted(self):
+        """To check if the database is deleted."""
         return self._matrix_serializer.IS_DELETED
```

### Comparing `MinVectorDB-0.2.4/min_vec/data_structures/fields_mapper.py` & `minvectordb-0.2.5/min_vec/data_structures/fields_mapper.py`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.4/min_vec/data_structures/filter.py` & `minvectordb-0.2.5/min_vec/data_structures/filter.py`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.4/min_vec/data_structures/kmeans.py` & `minvectordb-0.2.5/min_vec/data_structures/kmeans.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from sklearn.cluster import MiniBatchKMeans
 
 
 class BatchKMeans:
-    def __init__(self, n_clusters, random_state=42, epochs=100, batch_size=1024, distance='euclidean'):
+    def __init__(self, n_clusters, random_state=42, epochs=100, batch_size=1024):
         self.model = MiniBatchKMeans(n_clusters=n_clusters, random_state=random_state, max_iter=epochs,
-                                     batch_size=batch_size, n_init='auto')
+                                     batch_size=batch_size, n_init='auto', reassignment_ratio=0)
 
         self.n_clusters = n_clusters
-        self.distance = distance
         self.epochs = epochs
         self.batch_size = batch_size
 
         self.fitted = False
 
     def fit(self, X):
         self.model.fit(X)
```

### Comparing `MinVectorDB-0.2.4/min_vec/data_structures/scaler.py` & `minvectordb-0.2.5/min_vec/data_structures/scaler.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,31 +54,36 @@
 
         epsilon = 1e-9
         n_levels_minus_1 = self.n_levels - 1
         min_vals = self.min_vals
         max_vals = self.max_vals
 
         quantized = ne.evaluate(
-            "((vectors - min_vals) / (max_vals - min_vals + epsilon)) * n_levels_minus_1", optimization='moderate'
-        ).astype(self.bits)
+            "((vectors - min_vals) / (max_vals - min_vals + epsilon)) * n_levels_minus_1", optimization='moderate',
+            local_dict={'vectors': vectors, 'min_vals': min_vals, 'max_vals': max_vals,
+                        'n_levels_minus_1': n_levels_minus_1, 'epsilon': epsilon}
+        )
+        quantized = np.clip(quantized, 0, n_levels_minus_1).astype(self.bits)
 
         return quantized
 
     def fit_transform(self, vectors):
         self.partial_fit(vectors)
         return self.encode(vectors)
 
     def decode(self, quantized_vectors):
         raise_if(ValueError, not self.fitted, 'The model must be fitted before decoding.')
         n_levels_minus_1 = self.n_levels - 1
         range_vals = self.range_vals
         min_vals = self.min_vals
 
         decoded = ne.evaluate(
-            "(quantized_vectors / n_levels_minus_1) * range_vals + min_vals", optimization='moderate'
+            "(quantized_vectors / n_levels_minus_1) * range_vals + min_vals", optimization='moderate',
+            local_dict={'quantized_vectors': quantized_vectors, 'range_vals': range_vals,
+                        'min_vals': min_vals, 'n_levels_minus_1': n_levels_minus_1}
         )
 
         if decoded.dtype != self.decode_dtype:
             decoded = decoded.astype(self.decode_dtype)
 
         return decoded
```

### Comparing `MinVectorDB-0.2.4/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.2.5/min_vec/execution_layer/matrix_serializer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from datetime import datetime
 from pathlib import Path
 import shutil
 
 import numpy as np
 from spinesUtils.asserts import raise_if
+from spinesUtils.logging import Logger
 
-from min_vec.computational_layer.engines import to_normalize
 from min_vec.data_structures.filter import IDFilter
 from min_vec.utils.utils import io_checker
-from min_vec.configs.config import *
+from min_vec.configs.config import config
 from min_vec.data_structures.kmeans import BatchKMeans
 from min_vec.data_structures.scaler import ScalarQuantization
 from min_vec.data_structures.fields_mapper import FieldsMapper
 from min_vec.storage_layer.storage import StorageWorker
+from min_vec.execution_layer.cluster_worker import ClusterWorker
 
 
 class MatrixSerializer:
+    """
+    The MatrixSerializer class is used to serialize and deserialize the matrix data.
+    """
     def __init__(
-            self, dim, database_path, distance, logger, n_clusters=16, chunk_size=1_000_000,
-            index_mode='IVF-FLAT', dtypes='float32',
-            reindex_if_conflict=False, scaler_bits=None, n_threads=10
+            self,
+            dim: int,
+            database_path: str,
+            distance: str,
+            logger: Logger,
+            n_clusters: int = 16,
+            chunk_size: int = 1_000_000,
+            index_mode: str = 'IVF-FLAT',
+            dtypes: str = 'float32',
+            scaler_bits=None
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
@@ -32,39 +43,22 @@
             logger (Logger): The logger object.
             n_clusters (int): The number of clusters for the IVF-FLAT index. Default is 16.
             chunk_size (int): The size of each data chunk. Default is 1_000_000.
             index_mode (str): The index mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
-            reindex_if_conflict (bool): Whether to reindex the database if there is an index mode conflict.
-                Default is False.
             scaler_bits (int): The number of bits for scalar quantization. Default is None.
                 Options are 8, 16, 32. If None, scalar quantization will not be used.
                 The 8 bits for uint8, 16 bits for uint16, 32 bits for uint32.
-            n_threads (int): The number of threads to use for reading and writing the database. Default is 10.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
-        raise_if(ValueError, not isinstance(dim, int), 'dim must be int')
-        raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
-        raise_if(ValueError, not isinstance(chunk_size, int) or chunk_size <= 1,
-                 'chunk_size must be int and greater than 1')
-        raise_if(ValueError, distance not in ('cosine', 'L2'), 'distance must be "cosine" or "L2"')
-        raise_if(ValueError, index_mode not in ('FLAT', 'IVF-FLAT'), 'index_mode must be "FLAT" or "IVF-FLAT"')
-        raise_if(ValueError, dtypes not in ('float16', 'float32', 'float64'),
-                 'dtypes must be "float16", "float32" or "float64')
-        raise_if(ValueError, not isinstance(n_clusters, int) or n_clusters <= 0,
-                 'n_clusters must be int and greater than 0')
-        raise_if(ValueError, not isinstance(reindex_if_conflict, bool), 'reindex_if_conflict must be bool')
-        raise_if(ValueError, scaler_bits not in (8, 16, 32, None), 'sq_bits must be 8, 16, 32 or None')
-
         self.last_commit_time = None
-        self.reindex_if_conflict = reindex_if_conflict
         # set commit flag, if the flag is True, the database will not be saved
         self.COMMIT_FLAG = True
         # set flag for scalar quantization, if the flag is True, the database will be rescanned for scalar quantization
         self.RESCAN_FOR_SQ_FLAG = False
 
         self.IS_DELETED = False
 
@@ -85,45 +79,50 @@
         self.n_clusters = n_clusters
         # set dim
         self.dim = dim
         # set chunk size
         self.chunk_size = chunk_size
         # set filter path
         self._filter_path = self.database_path_parent / 'id_filter.mvdb'
-        # set device
-        self.device = torch.device(MVDB_COMPUTE_DEVICE)
-        # set scalar quantization bits
-        self.scaler_bits = scaler_bits if scaler_bits is not None else None
 
         # set database path
         self.database_path = self.database_path_parent / Path(database_path).name.split('.mvdb')[0]
 
+        # set scalar quantization bits
+        self.scaler_bits = scaler_bits if scaler_bits is not None else None
+        self.scaler = None
+        if self.scaler_bits is not None:
+            self._initialize_scalar_quantization()
+
         # initialize the storage worker
-        self.storage_worker = StorageWorker(self.database_path_parent, self.dim, self.chunk_size, n_threads=n_threads)
+        self.storage_worker = StorageWorker(self.database_path_parent, self.dim,
+                                            self.chunk_size,
+                                            quantizer=None if self.scaler_bits is None else self.scaler)
 
         self.logger.info(f"Initializing database folder path: '{'.mvdb'.join(database_path.split('.mvdb')[:-1])}/'")
-        if MVDB_COMPUTE_DEVICE != 'cpu':
-            self.logger.info(f"Using device: {MVDB_COMPUTE_DEVICE}")
 
         # ============== Loading or create one empty database ==============
         # first of all, initialize a database
         self.database = []
         self.indices = []
         self.fields = []
 
-        # check initialize params
-        self._check_initialize_params(dtypes, reindex_if_conflict)
-
-        if self.scaler_bits is not None:
-            self._initialize_scalar_quantization()
-
         self._initialize_fields_mapper()
         self._initialize_ann_model()
         self._initialize_id_filter()
 
+        self.cluster_worker = ClusterWorker(
+            logger=self.logger,
+            iterable_dataloader=self.iterable_dataloader,
+            ann_model=self.ann_model,
+            storage_worker=self.storage_worker,
+            save_data=self.save_data,
+            n_clusters=self.n_clusters
+        )
+
         # save initial parameters
         self._write_params(dtypes=dtypes)
 
         if self._get_cluster_dataset_num() > 0 and self.index_mode == 'FLAT':
             # cause the index mode is FLAT, but the cluster dataset is not empty,
             # so the clustered datasets will also be traversed during querying.
             self.logger.warning('The index mode is FLAT, but the cluster dataset is not empty, '
@@ -138,119 +137,41 @@
         }
 
         if self.scaler_bits is not None:
             attrs['sq_bits'] = self.scaler_bits
 
         self.storage_worker.write_file_attributes(attrs)
 
-    def _check_initialize_params(self, dtypes, reindex_if_conflict):
-        """check initialize params"""
-        write_params_flag = False
-        if self.database_path.exists():
-            self.logger.info('Database file exists, reading parameters...')
-
-            attrs = self.storage_worker.read_file_attributes()
-            dim = attrs.get('dim', self.dim)
-            chunk_size = attrs.get('chunk_size', self.chunk_size)
-            distance = attrs.get('distance', self.distance)
-            file_dtypes = attrs.get('dtypes', dtypes)
-            old_index_mode = attrs.get('index_mode', None)
-            old_sq_bits = attrs.get('sq_bits', self.scaler_bits)
-
-            if dim != self.dim:
-                self.logger.warning(
-                    f'* dim={dim} in the file is not equal to the dim={self.dim} in the parameters, '
-                    f'the parameter dim will be covered by the dim in the file.')
-                self.dim = dim
-                write_params_flag = True
-
-            if chunk_size != self.chunk_size:
-                self.logger.warning(
-                    f'* chunk_size={chunk_size} in the file is not '
-                    f'equal to the chunk_size={self.chunk_size}'
-                    f'in the parameters, the parameter chunk_size will be covered by the chunk_size '
-                    f'in the file.'
-                )
-                self.chunk_size = chunk_size
-                write_params_flag = True
-
-            if distance != self.distance:
-                self.logger.warning(f'* distance=\'{distance}\' in the file is not '
-                                    f'equal to the distance=\'{self.distance}\' '
-                                    f'in the parameters, the parameter distance will be covered by the distance '
-                                    f'in the file.')
-                self.distance = distance
-                write_params_flag = True
-
-            if file_dtypes != dtypes:
-                self.logger.warning(
-                    f'* dtypes=\'{file_dtypes}\' in the file is not equal to the dtypes=\'{dtypes}\' '
-                    f'in the parameters, the parameter dtypes will be covered by the dtypes '
-                    f'in the file.')
-                self.dtypes = self._dtypes_map[attrs.get('dtypes', dtypes)]
-                write_params_flag = True
-
-            if old_index_mode != self.index_mode and self.index_mode == 'IVF-FLAT':
-                if reindex_if_conflict:
-                    self.logger.warning(
-                        f'* index_mode=\'{old_index_mode}\' in the file is not equal to the index_mode='
-                        f'\'{self.index_mode}\' in the parameters, if you really want to change the '
-                        f'index_mode to \'IVF-FLAT\', you need to run `commit()` function after initializing '
-                        f'the database.')
-
-                    self.COMMIT_FLAG = False
-                else:
-                    self.logger.warning(
-                        f'* index_mode=\'{old_index_mode}\' in the file is not equal to the index_mode='
-                        f'\'{self.index_mode}\' in the parameters, if you really want to change the '
-                        f'index_mode to \'IVF-FLAT\', you need to set `reindex_if_conflict=True` first '
-                        f'and run `commit()` function after initializing the database.')
-
-            if self.scaler_bits is not None and old_sq_bits != self.scaler_bits:
-                self.logger.warning(f'* sq_bits={old_sq_bits} in the file is not equal to the sq_bits='
-                                    f'{self.scaler_bits} in the parameters, '
-                                    f'the sq_bits in the file will be covered by the sq_bits in the parameters.')
-                self.RESCAN_FOR_SQ_FLAG = True
-
-            self.logger.info('Reading parameters done.')
-
-        if write_params_flag or not self.database_path.exists():
-            self._write_params(dtypes)
-
     def _initialize_parent_path(self, database_path):
         """make directory if not exist"""
         self.database_path_parent = Path(database_path).parent.absolute() / Path(
             '.mvdb'.join(Path(database_path).absolute().name.split('.mvdb')[:-1]))
 
-        if not self.database_path_parent.exists():
-            self.database_path_parent.mkdir(parents=True)
+        self.database_path_parent.mkdir(parents=True, exist_ok=True)
 
     def _initialize_scalar_quantization(self):
         if Path(self.database_path_parent / 'sq_model.mvdb').exists():
             self.scaler = ScalarQuantization.load(self.database_path_parent / 'sq_model.mvdb')
         else:
             self.scaler = ScalarQuantization(bits=self.scaler_bits, decode_dtype=self.dtypes)
-            # if the database file exists, the model will be fitted
-            if self.database_path.exists() and self.RESCAN_FOR_SQ_FLAG:
-                for i in self.iterable_dataloader(read_chunk_only=False):
-                    self.scaler.partial_fit(i[0])
 
     def _initialize_ann_model(self):
         """initialize ann model"""
         if self.index_mode == 'IVF-FLAT':
+            MVDB_KMEANS_EPOCHS = config.MVDB_KMEANS_EPOCHS
             self.ann_model = BatchKMeans(n_clusters=self.n_clusters, random_state=0,
-                                         batch_size=10240, epochs=MVDB_KMEANS_EPOCHS, distance=self.distance)
+                                         batch_size=10240, epochs=MVDB_KMEANS_EPOCHS)
 
             if Path(self.database_path_parent / 'ann_model.mvdb').exists() and self.index_mode == 'IVF-FLAT':
                 self.ann_model = self.ann_model.load(self.database_path_parent / 'ann_model.mvdb')
-                if (self.ann_model.n_clusters != self.n_clusters or self.ann_model.distance != self.distance or
+                if (self.ann_model.n_clusters != self.n_clusters or
                         self.ann_model.epochs != MVDB_KMEANS_EPOCHS or
                         self.ann_model.batch_size != 10240):
                     self.ann_model = BatchKMeans(n_clusters=self.n_clusters, random_state=0,
-                                                 batch_size=10240, epochs=MVDB_KMEANS_EPOCHS, distance=self.distance)
+                                                 batch_size=10240, epochs=MVDB_KMEANS_EPOCHS)
         else:
             self.ann_model = None
 
     def _initialize_fields_mapper(self):
         """initialize fields mapper"""
         if Path(self.database_path_parent / 'fields_mapper.mvdb').exists():
             self.fields_mapper = FieldsMapper().load(self.database_path_parent / 'fields_mapper.mvdb')
@@ -277,15 +198,15 @@
     def reset_database(self):
         """Reset the database to its initial state with zeros."""
         self.database = []
         self.indices = []
         self.fields = []
 
     @io_checker
-    def iterable_dataloader(self, read_chunk_only=False, from_tail=False, mode='eager', order_read=False):
+    def iterable_dataloader(self, read_chunk_only=False, from_tail=False, mode='eager'):
         """
         Generator for loading the database and index.
 
         Parameters:
             read_chunk_only (bool): Whether to read only the chunk.
             from_tail (bool): Whether to read from the end of the file.
             mode (str): The mode of the generator. Options are 'eager' or 'lazy'. Default is 'eager'.
@@ -295,24 +216,17 @@
 
         Raises:
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
-        if self.scaler_bits is not None:
-            # decoder = self.scaler.decode
-            self.storage_worker.update_scaler(self.scaler)
-        # else:
-        #     decoder = lambda x: x
-
         read_type = 'all' if not read_chunk_only else 'chunk'
 
-        for data, indices, fields in self.storage_worker.read(read_type=read_type, reverse=from_tail,
-                                                              order_read=order_read):
+        for data, indices, fields in self.storage_worker.read(read_type=read_type, reverse=from_tail):
             if data is None:
                 continue
 
             if mode == 'lazy':
                 yield data, indices, fields
             else:
                 yield data, indices, self.fields_mapper.decode(fields)
@@ -330,21 +244,14 @@
 
         Raises:
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
-        if self.scaler_bits is not None:
-            raise_if(ValueError, not self.scaler.fitted, 'The model must be fitted before decoding.')
-            # decoder = self.scaler.decode
-            self.storage_worker.update_scaler(self.scaler)
-        # else:
-        #     decoder = lambda x: x
-
         for data, indices, fields in self.storage_worker.read(read_type='cluster', cluster_id=str(cluster_id)):
             if mode == 'lazy':
                 yield data, indices, fields
             else:
                 yield data, indices, self.fields_mapper.decode(fields)
 
     def _is_database_reset(self):
@@ -363,36 +270,29 @@
         Raises:
             ValueError: If the lengths of the database, indices, and fields are not the same.
         """
         if not self._is_database_reset() and not self.COMMIT_FLAG:
             if not (len(self.database) == len(self.indices) == len(self.fields)):
                 raise ValueError('The database, index length and field length not the same.')
 
-    def reset_chunk_partition(self):
-        """
-        Reset the chunk partition.
-        """
-        self.storage_worker.delete_chunk()
-
-    def save_data(self, data, indices, fields, to_chunk=True, cluster_id=None):
+    def save_data(self, data, indices, fields, write_chunk=True, cluster_id=None, normalize=False):
         """Optimized method to save data to chunk or cluster group with reusable logic."""
-        if self.scaler_bits is not None:
-            self.storage_worker.update_scaler(self.scaler)
 
         if isinstance(fields, str) or all(isinstance(i, str) for i in fields):
             fields_indices = self.fields_mapper.encode(fields)
         else:
             fields_indices = fields
 
         self.storage_worker.write(data, indices, fields_indices,
-                                  write_type='chunk' if to_chunk else 'cluster',
-                                  cluster_id=str(cluster_id) if cluster_id is not None else cluster_id)
+                                  write_type='chunk' if write_chunk else 'cluster',
+                                  cluster_id=str(cluster_id) if cluster_id is not None else cluster_id,
+                                  normalize=normalize)
 
     @io_checker
-    def save_chunk_immediately(self):
+    def save_chunk_immediately(self, normalize=True):
         """
         Save the current state of the database to a .mvdb file.
 
         Returns:
             Path: The path of the saved database file.
         """
         self._length_checker()
@@ -400,24 +300,25 @@
         if self._is_database_reset():
             return []
 
         self.save_data(
             self.database,
             self.indices,
             self.fields,
-            to_chunk=True,
-            cluster_id=None
+            write_chunk=True,
+            cluster_id=None,
+            normalize=normalize
         )
 
         self.reset_database()  # reset database, indices and fields
 
-    def auto_save_chunk(self):
+    def auto_save_chunk(self, normalize=True):
         self._length_checker()
         if len(self.database) >= self.chunk_size:
-            self.save_chunk_immediately()
+            self.save_chunk_immediately(normalize=normalize)
 
         return
 
     def _get_cluster_dataset_num(self):
         if not self.database_path.exists():
             return 0
 
@@ -426,25 +327,20 @@
     def commit(self):
         """
         Save the database, ensuring that all data is written to disk.
         This method is required to be called after saving vectors to query them.
         """
         if not self.COMMIT_FLAG:
             self.logger.debug('Saving chunk immediately...')
-            self.save_chunk_immediately()
+            self.save_chunk_immediately(normalize=True)
 
             self.logger.debug('Saving id filter...')
             # save filter
             self.id_filter.to_file(self._filter_path)
 
-            # save scalar quantization model
-            if self.scaler_bits is not None:
-                self.logger.debug('Saving scalar quantization model...')
-                self.scaler.save(self.database_path_parent / 'sq_model.mvdb')
-
             # save fields mapper
             self.logger.debug('Saving fields mapper...')
             self.fields_mapper.save(self.database_path_parent / 'fields_mapper.mvdb')
 
             chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
             if chunk_partition_size >= 100000 and self.index_mode != 'FLAT':
                 self.logger.debug('Building index...')
@@ -471,50 +367,41 @@
         while True:
             self.last_id += 1
             if self.last_id not in self.id_filter:
                 break
 
         return self.last_id
 
-    def _process_vector_item(self, vector, index, field, normalize):
+    def _process_vector_item(self, vector, index, field):
         if index in self.id_filter:
             raise ValueError(f'id {index} already exists')
 
         if len(vector) != self.dim:
             raise ValueError(f'vector dim error, expect {self.dim}, got {len(vector)}')
 
         if vector.dtype != self.dtypes:
             vector = vector.astype(self.dtypes)
 
         if vector.ndim == 1:
             vector = vector.reshape(1, -1)
 
-        if normalize:
-            vector = to_normalize(vector)
-
         return vector, index, field if field is not None else ''
 
-    def bulk_add_items(self, vectors, *, normalize: bool = False, save_immediately=False):
+    def bulk_add_items(self, vectors):
         """
         Bulk add vectors to the database in batches.
 
         Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
             vector, id, field).
-        normalize (bool, optional, keyword-only): Whether to normalize the input vectors. Default is False.
-        save_immediately (bool, optional, keyword-only): Whether to save the database immediately. Default is False.
 
         Returns:
             list: A list of indices where the vectors are stored.
         """
         raise_if(ValueError, not isinstance(vectors, (tuple, list)),
                  f'vectors must be tuple or list, got {type(vectors)}')
-        raise_if(ValueError, not isinstance(normalize, bool),
-                 f'normalize must be bool, got {type(normalize)}')
-        raise_if(ValueError, not isinstance(save_immediately, bool),
-                 f'save_immediately must be bool, got {type(save_immediately)}')
         raise_if(ValueError, not all(isinstance(i, tuple) for i in vectors),
                  f'vectors must be tuple of (vector, id[optional], field[optional]).')
 
         new_ids = []
 
         for i in range(0, len(vectors), self.chunk_size):
             batch = vectors[i:i + self.chunk_size]
@@ -533,42 +420,39 @@
                     vector, index, field = sample
 
                 index = self._generate_new_id() if index is None else index
 
                 raise_if(ValueError, index < 0, f'id must be greater than 0, got {index}')
 
                 field = '' if field is None else field
-                vector, index, field = self._process_vector_item(vector, index, field, normalize)
+                vector, index, field = self._process_vector_item(vector, index, field)
 
                 self.database.append(vector)
                 internal_id = index if index is not None else self._generate_new_id()
                 self.indices.append(internal_id)
                 new_ids.append(internal_id)
                 self.fields.append(field)
                 self.id_filter.add(index)
 
-            self.save_chunk_immediately() if save_immediately else self.auto_save_chunk()
+            self.auto_save_chunk(normalize=True)
 
         if self.COMMIT_FLAG:
             self.COMMIT_FLAG = False
 
         return new_ids
 
-    def add_item(self, vector, *, index: int = None, field: str = None, normalize: bool = False,
-                 save_immediately=False) -> int:
+    def add_item(self, vector, *, index: int = None, field: str = None) -> int:
         """
         Add a single vector to the database.
 
         Parameters:
             vector (np.ndarray): The vector to be added.
             index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
             field (str, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
                 set to an empty string.
-            normalize (bool, optional, keyword-only): Whether to normalize the input vector. Default is False.
-            save_immediately (bool, optional, keyword-only): Whether to save the database immediately. Default is False.
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
         raise_if(ValueError, len(vector) != self.dim,
@@ -576,33 +460,29 @@
         raise_if(ValueError, vector.ndim != 1, f'vector dim error, expect 1, got {vector.ndim}')
         raise_if(ValueError, field is not None and not isinstance(field, str),
                  f'field must be str, got {type(field)}')
         raise_if(ValueError, index is not None and not isinstance(index, int), f'id must be int, got {type(index)}')
         raise_if(ValueError, index is not None and index < 0, f'id must be greater than 0, got {index}')
         raise_if(ValueError, field is not None and not isinstance(field, str),
                  f'field must be str, got {type(field)}')
-        raise_if(ValueError, not isinstance(normalize, bool),
-                 f'normalize must be bool, got {type(normalize)}')
-        raise_if(ValueError, not isinstance(save_immediately, bool),
-                 f'save_immediately must be bool, got {type(save_immediately)}')
 
         index = self._generate_new_id() if index is None else index
 
         raise_if(ValueError, index in self.id_filter, f'id {index} already exists')
 
-        vector, index, field = self._process_vector_item(vector, index, field, normalize)
+        vector, index, field = self._process_vector_item(vector, index, field)
 
         # Add the id to then filter.
         self.id_filter.add(index)
 
         self.database.append(vector)
         self.indices.append(index)
         self.fields.append(field)
 
-        self.save_chunk_immediately() if save_immediately else self.auto_save_chunk()
+        self.auto_save_chunk(normalize=True)
 
         if self.COMMIT_FLAG:
             self.COMMIT_FLAG = False
 
         return index
 
     def delete(self):
@@ -625,72 +505,17 @@
         self._initialize_fields_mapper()
         self._initialize_ann_model()
         self._initialize_id_filter()
 
         # clear cache
         self.storage_worker.clear_cache()
 
-
-    def _kmeans_clustering(self, data):
-        """kmeans clustering"""
-        self.ann_model = self.ann_model.partial_fit(data)
-
-        return self.ann_model.cluster_centers_, self.ann_model.labels_
-
-    def _clustering_for_ivf(self, data, indices, fields):
-        # Perform K-means clustering.
-        self.cluster_centers, labels = self._kmeans_clustering(data)
-
-        # Current batch's IVF index.
-        ivf_index = {i: [] for i in range(self.n_clusters)}
-        # Allocate data to various cluster centers.
-        for idx, label in enumerate(labels):
-            try:
-                ivf_index[label].append([idx, indices[idx], fields[idx]])
-            except Exception as e:
-                self.logger.error(f"Error in adding to cluster: {e}")
-                raise e
-
-        return ivf_index
-
-    def _build_index(self):
-        for database, indices, fields in self.iterable_dataloader(read_chunk_only=True, mode='lazy'):
-            # Create an IVF index.
-            ivf_index = self._clustering_for_ivf(database, indices, fields)
-            # reorganize files
-            self.save_cluster_partitions(database, ivf_index)
-
     def build_index(self):
         """
         Build the IVF index.
         """
-        self._build_index()
-
-        self.reset_chunk_partition()
-
-    def save_cluster_partitions(self, database, ivf_index):
-        """
-        Rearrange files according to the IVF index.
-        """
-        for cluster_id in range(self.n_clusters):
-            all_vectors, all_indices, all_fields = [], [], []
-
-            for cid, _ in ivf_index.items():
-                if len(_) == 0:
-                    continue
-                vec_idx, index, field = zip(*_)
-                if cid == cluster_id:
-                    # Extract all vectors, indices, and fields from the current cluster center.
-                    all_vectors.extend([database[i] for i in vec_idx])
-                    all_indices.extend(index)
-                    all_fields.extend(field)
-
-            if len(all_vectors) == 0:
-                continue
-
-            self.save_data(all_vectors, all_indices, all_fields, to_chunk=False,
-                           cluster_id=cluster_id)
+        self.cluster_worker.build_index(self.scaler, self.distance)
 
     @property
     def shape(self):
         self.check_commit()
         return tuple(self.storage_worker.get_shape(read_type='all'))
```

### Comparing `MinVectorDB-0.2.4/min_vec/storage_layer/storage.py` & `minvectordb-0.2.5/min_vec/storage_layer/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,150 @@
-import os
 from pathlib import Path
 import json
-from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import numpy as np
 from spinesUtils.asserts import raise_if
 
-from min_vec.configs.config import MVDB_DATALOADER_BUFFER_SIZE
+from min_vec.computational_layer.engines import to_normalize
+from min_vec.configs.config import config
 from min_vec.data_structures.limited_dict import LimitedDict
 
+
 class StorageWorker:
-    """A class to read and write data to a file, with optimized file handle management."""
+    """The worker class for reading and writing data to the files."""
 
-    def __init__(self, database_path, dimension, chunk_size, n_threads=None):
+    def __init__(self, database_path, dimension, chunk_size, quantizer=None):
         self.database_path = Path(database_path)
         self.database_chunk_path = self.database_path / 'chunk_data'
         self.database_chunk_indices_path = self.database_path / 'chunk_indices_data'
         self.database_chunk_fields_path = self.database_path / 'chunk_fields_data'
 
-        if not self.database_chunk_path.exists():
-            self.database_chunk_path.mkdir(parents=True)
-
-        if not self.database_chunk_indices_path.exists():
-            self.database_chunk_indices_path.mkdir(parents=True)
-
-        if not self.database_chunk_fields_path.exists():
-            self.database_chunk_fields_path.mkdir(parents=True)
-
         self.database_cluster_path = self.database_path / 'cluster_data'
         self.database_cluster_indices_path = self.database_path / 'cluster_indices_data'
         self.database_cluster_fields_path = self.database_path / 'cluster_fields_data'
 
-        if not self.database_cluster_path.exists():
-            self.database_cluster_path.mkdir(parents=True)
-
-        if not self.database_cluster_indices_path.exists():
-            self.database_cluster_indices_path.mkdir(parents=True)
-
-        if not self.database_cluster_fields_path.exists():
-            self.database_cluster_fields_path.mkdir(parents=True)
+        for path in [self.database_chunk_path, self.database_chunk_indices_path,
+                     self.database_chunk_fields_path, self.database_cluster_path,
+                     self.database_cluster_indices_path, self.database_cluster_fields_path]:
+            path.mkdir(parents=True, exist_ok=True)
 
         self.dimension = dimension
         self.chunk_size = chunk_size
 
         self.cluster_last_file_shape = {}
 
-        raise_if(ValueError, (n_threads is not None) and not (isinstance(n_threads, int) and n_threads > 0),
-                 'n_jobs must be a positive integer or None.')
-        self.n_threads = n_threads if n_threads is not None else os.cpu_count()
-
-        self.cache = LimitedDict(max_size=MVDB_DATALOADER_BUFFER_SIZE)
+        self.cache = LimitedDict(max_size=config.MVDB_DATALOADER_BUFFER_SIZE)
 
-        self.scaler = None
-
-    def update_scaler(self, scaler):
-        self.scaler = scaler
+        self.quantizer = quantizer
 
     def file_exists(self):
-        return not ((self.database_chunk_path / 'chunk_0.npy').exists()
-                    or (self.database_cluster_path / 'cluster_0_0.npy').exists())
+        return ((self.database_chunk_path / 'chunk_0').exists()
+                or (self.database_cluster_path / 'cluster_0_0').exists())
 
     def _return_if_in_memory(self, filename, reverse=False):
-        if len(self.cache) == 0:
+        res = self.cache.get(filename, None)
+
+        if res is None:
             return None
 
-        res = self.cache.get(filename)
         if reverse:
             return res[0][::-1], res[1][::-1], res[2][::-1]
         return res
 
     def _write_to_memory(self, filename, data, indices, fields):
         self.cache[filename] = (data, indices, fields)
 
-    def _load_data(self, filename, data_path, indices_path, fields_path, reverse):
+    def _load_data(self, filename, data_path, indices_path, fields_path, reverse, update_memory=True):
         # 文件读取逻辑
         data = np.load(data_path / filename)
         indices = np.load(indices_path / filename)
         fields = np.load(fields_path / filename)
 
-        if self.scaler is not None:
-            data = self.scaler.decode(data)
-
-        self._write_to_memory(filename, data, indices, fields)
+        if update_memory:
+            self._write_to_memory(filename, data, indices, fields)
 
         if reverse:
             return data[::-1], indices[::-1], fields[::-1]
         else:
             return data, indices, fields
 
-    def _batch_load_data(self, executor, filenames, data_path, indices_path, fields_path, reverse):
-        batch_futures = [executor.submit(self._load_data, filename.name, data_path,
-                                         indices_path, fields_path, reverse)
-                         for filename in filenames]
-
-        for future in as_completed(batch_futures):
-            yield future.result()
-
-    def _read(self, reverse=False, read_type='chunk', cluster_id=None, order_read=False):
+    def _read(self, reverse=False, read_type='chunk', cluster_id=None):
         if not self.file_exists():
             return
 
         reverse_sign = -1 if reverse else 1
 
-        if order_read:
-            if read_type == 'chunk':
-                filenames = sorted(self.database_chunk_path.glob('chunk_*'),
-                                   key=lambda x: reverse_sign * int(x.stem.split('_')[-1]))
-                for filename in filenames:
-                    data, indices, fields = self._load_data(filename.name, self.database_chunk_path,
-                                                            self.database_chunk_indices_path,
-                                                            self.database_chunk_fields_path, reverse)
-                    yield data, indices, fields
-
-            elif read_type == 'cluster':
-                if cluster_id is None:
-                    cluster_ids = [int(path.stem.split('_')[-2]) for path in
-                                   self.database_cluster_path.glob('cluster_*')]
-                else:
-                    cluster_ids = [cluster_id]
+        if read_type == 'chunk':
+            filenames = sorted([x.stem for x in self.database_chunk_path.glob('chunk_*')],
+                               key=lambda x: reverse_sign * int(x.split('_')[-1]))
 
-                for cluster_id in cluster_ids:
-                    filenames = sorted(self.database_cluster_path.glob(f'cluster_{cluster_id}_*'),
-                                       key=lambda x: reverse_sign * int(x.stem.split('_')[-1]))
-                    for filename in filenames:
-                        data, indices, fields = self._load_data(filename.name, self.database_cluster_path,
-                                                                self.database_cluster_indices_path,
-                                                                self.database_cluster_fields_path, reverse)
-                        yield data, indices, fields
-            else:
-                raise ValueError('read_type must be "chunk" or "cluster"')
-        else:
-            # 创建线程池实例
-            if read_type == 'chunk':
-                filenames = sorted(self.database_chunk_path.glob('chunk_*'),
-                                   key=lambda x: reverse_sign * int(x.stem.split('_')[-1]))
-                # check the memory cache first
-                in_memo = [filename for filename in filenames if filename.name in self.cache]
-                if len(in_memo) != 0:
-                    for filename in in_memo:
-                        yield self._return_if_in_memory(filename.name, reverse=reverse)
-
-                if len(in_memo) < len(filenames):
-                    filenames = [filename for filename in filenames if filename.name not in self.cache]
-                    with ThreadPoolExecutor(max_workers=self.n_threads) as executor:
-                        for i in range(0, len(filenames), self.n_threads):
-                            yield from self._batch_load_data(executor, filenames[i:i + self.n_threads],
-                                                             self.database_chunk_path,
-                                                             self.database_chunk_indices_path,
-                                                             self.database_chunk_fields_path,
-                                                             reverse)
-
-            elif read_type == 'cluster':
-                if cluster_id is None:
-                    cluster_ids = [int(path.stem.split('_')[-2]) for path in
-                                   self.database_cluster_path.glob('cluster_*')]
+            for filename in filenames:
+                if filename in self.cache:
+                    yield self._return_if_in_memory(filename, reverse=reverse)
                 else:
-                    cluster_ids = [cluster_id]
 
-                for cluster_id in cluster_ids:
-                    filenames = sorted(self.database_cluster_path.glob(f'cluster_{cluster_id}_*'),
-                                       key=lambda x: reverse_sign * int(x.stem.split('_')[-1]))
-
-                    # check the memory cache first
-                    in_memo = [filename for filename in filenames if filename.name in self.cache]
-                    if len(in_memo) != 0:
-                        for filename in in_memo:
-                            yield self._return_if_in_memory(filename.name, reverse=reverse)
-
-                    if len(in_memo) < len(filenames):
-                        filenames = [filename for filename in filenames if filename.name not in self.cache]
-
-                    with ThreadPoolExecutor(max_workers=self.n_threads) as executor:
-                        for i in range(0, len(filenames), self.n_threads):
-                            yield from self._batch_load_data(executor, filenames[i:i + self.n_threads],
-                                                             self.database_cluster_path,
-                                                             self.database_cluster_indices_path,
-                                                             self.database_cluster_fields_path, reverse)
+                    yield self._load_data(filename, self.database_chunk_path,
+                                          self.database_chunk_indices_path,
+                                          self.database_chunk_fields_path, reverse)
+        elif read_type == 'cluster':
+            if cluster_id is None:
+                cluster_ids = [int(path.stem.split('_')[-2]) for path in
+                               self.database_cluster_path.glob('cluster_*')]
             else:
-                raise ValueError('read_type must be "chunk" or "cluster"')
+                cluster_ids = [cluster_id]
+
+            for cluster_id in cluster_ids:
+                filenames = sorted([x.stem for x in self.database_cluster_path.glob(f'cluster_{cluster_id}_*')],
+                                   key=lambda x: reverse_sign * int(x.split('_')[-1]))
+                for filename in filenames:
+                    if filename in self.cache:
+                        yield self._return_if_in_memory(filename, reverse=reverse)
+                    else:
+                        yield self._load_data(filename, self.database_cluster_path,
+                                              self.database_cluster_indices_path,
+                                              self.database_cluster_fields_path, reverse)
+        else:
+            raise ValueError('read_type must be "chunk" or "cluster"')
 
-    def chunk_read(self, reverse=False, order_read=False):
+    def chunk_read(self, reverse=False):
         """Read the data from the file."""
-        yield from self._read(reverse=reverse, read_type='chunk', order_read=order_read)
+        yield from self._read(reverse=reverse, read_type='chunk')
 
-    def cluster_read(self, cluster_id, reverse=False, order_read=False):
+    def cluster_read(self, cluster_id, reverse=False):
         """Read the data from the file."""
-        yield from self._read(reverse=reverse, read_type='cluster', cluster_id=cluster_id, order_read=order_read)
+        yield from self._read(reverse=reverse, read_type='cluster', cluster_id=cluster_id)
 
     def get_last_id(self, contains='chunk', cluster_id=None):
         if contains == 'chunk':
             ids = [int(str(i).split('.mvdb')[0].split('_')[-1])
                    for i in self.database_chunk_path.glob('chunk_*')]
         else:
             ids = [int(str(i).split('.mvdb')[0].split('_')[-1])
                    for i in self.database_cluster_path.glob(f'cluster_{cluster_id}_*')]
 
         if len(ids) > 0:
             return max(ids)
 
         return -1
 
-    def _write(self, data, indices, fields, write_type='chunk', cluster_id=None):
+    @staticmethod
+    def _write_to_disk(data, indices, fields, data_path, indices_path, fields_path, filename):
+        with open(data_path / filename, 'wb') as f:
+            np.save(f, data)
+
+        with open(indices_path / filename, 'wb') as f:
+            np.save(f, indices)
+
+        with open(fields_path / filename, 'wb') as f:
+            np.save(f, fields)
+
+    def _write(self, data, indices, fields, write_type='chunk', cluster_id=None, normalize=False):
+        if normalize:
+            data = to_normalize(np.vstack(data))
+
         if write_type == 'chunk':
             database_subfile_path = self.database_chunk_path
             database_indices_path = self.database_chunk_indices_path
             database_fields_path = self.database_chunk_fields_path
             file_prefix = 'chunk'
         else:
             database_subfile_path = self.database_cluster_path
@@ -220,14 +160,20 @@
             if not (self.database_path / 'info.json').exists():
                 total_shape = [0, self.dimension]
                 with open(self.database_path / 'info.json', 'w') as f:
                     json.dump({"total_shape": total_shape}, f)
             else:
                 with open(self.database_path / 'info.json', 'r') as f:
                     total_shape = json.load(f)['total_shape']
+
+            # in this class, we only use the quantizer in chunk_write, after quantization,
+            # the disk data and memory data will be changed to quantized data
+            if self.quantizer is not None:
+                data = self.quantizer.fit_transform(data)
+
         else:
             if self.cluster_last_file_shape.get(cluster_id) is None:
                 if last_file_id == -1:
                     total_shape = [0, self.dimension]
                 else:
                     total_shape = [len(np.load(database_subfile_path / f'{file_prefix}_{last_file_id}.npy')),
                                    self.dimension]
@@ -236,35 +182,28 @@
 
         data_shape = len(data)
         # 新文件
         if total_shape[0] % self.chunk_size == 0 or last_file_id == -1:
             while len(data) != 0:
                 last_file_id = self.get_last_id(contains=write_type, cluster_id=cluster_id)
 
-                temp_data = np.vstack(data[:self.chunk_size])
+                temp_data = data[:self.chunk_size]
                 temp_indices = np.array(indices[:self.chunk_size])
                 temp_fields = np.array(fields[:self.chunk_size])
 
                 data = data[self.chunk_size:]
                 indices = indices[self.chunk_size:]
                 fields = fields[self.chunk_size:]
 
+                filename = f'{file_prefix}_{last_file_id + 1}'
                 # save data
-                with open(database_subfile_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                    np.save(f, temp_data) if self.scaler is None else np.save(f, self.scaler.fit_transform(temp_data))
-
-                # save indices
-                with open(database_indices_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                    np.save(f, temp_indices)
-
-                # save fields
-                with open(database_fields_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                    np.save(f, temp_fields)
+                self._write_to_disk(temp_data, temp_indices, temp_fields, database_subfile_path, database_indices_path,
+                                    database_fields_path, filename)
 
-                self._write_to_memory(f'{file_prefix}_{last_file_id + 1}', temp_data, temp_indices, temp_fields)
+                self._write_to_memory(filename, temp_data, temp_indices, temp_fields)
         # 存在未满chunk_size的新文件
         else:
             data_shape = len(data)
             already_stack = False
             while len(data) != 0:
                 last_file_id = self.get_last_id(contains=write_type, cluster_id=cluster_id)
                 # run once
@@ -277,89 +216,79 @@
                     data = data[temp_index:]
                     indices = indices[temp_index:]
                     fields = fields[temp_index:]
                     already_stack = True
 
                     # save data
                     old_data = np.load(database_subfile_path / f'{file_prefix}_{last_file_id}')
-                    temp_data = np.vstack((old_data, np.vstack(temp_data)))
-                    with open(database_subfile_path / f'{file_prefix}_{last_file_id}', 'wb') as f:
-                        np.save(f, temp_data) if self.scaler is None else np.save(f, self.scaler.fit_transform(temp_data))
-
+                    temp_data = np.vstack((old_data, temp_data))
                     # save indices
                     old_indices = np.load(database_indices_path / f'{file_prefix}_{last_file_id}')
                     temp_indices = np.concatenate((old_indices, temp_indices))
-                    with open(database_indices_path / f'{file_prefix}_{last_file_id}', 'wb') as f:
-                        np.save(f, temp_indices)
-
                     # save fields
                     old_fields = np.load(database_fields_path / f'{file_prefix}_{last_file_id}')
                     temp_fields = np.concatenate((old_fields, temp_fields))
-                    with open(database_fields_path / f'{file_prefix}_{last_file_id}', 'wb') as f:
-                        np.save(f, temp_fields)
 
-                    self._write_to_memory(f'{file_prefix}_{last_file_id}', temp_data, temp_indices, temp_fields)
+                    filename = f'{file_prefix}_{last_file_id}'
+                    self._write_to_disk(temp_data, temp_indices, temp_fields, database_subfile_path,
+                                        database_indices_path, database_fields_path, filename)
+
+                    self._write_to_memory(filename, temp_data, temp_indices, temp_fields)
                 else:
                     temp_index = min(self.chunk_size, len(data))
-                    temp_data = np.vstack(data[:temp_index])
+                    temp_data = data[:temp_index]
                     temp_indices = np.array(indices[:temp_index])
                     temp_fields = np.array(fields[:temp_index])
 
                     data = data[temp_index:]
                     indices = indices[temp_index:]
                     fields = fields[temp_index:]
-                    # save data
-                    with open(database_subfile_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                        np.save(f, temp_data) if self.scaler is None else np.save(f, self.scaler.fit_transform(temp_data))
-
-                    # save indices
-                    with open(database_indices_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                        np.save(f, temp_indices)
 
-                    # save fields
-                    with open(database_fields_path / f'{file_prefix}_{last_file_id + 1}', 'wb') as f:
-                        np.save(f, temp_fields)
+                    filename = f'{file_prefix}_{last_file_id + 1}'
+                    self._write_to_disk(temp_data, temp_indices, temp_fields, database_subfile_path,
+                                        database_indices_path,
+                                        database_fields_path, filename)
 
-                    self._write_to_memory(f'{file_prefix}_{last_file_id + 1}', temp_data, temp_indices, temp_fields)
+                    self._write_to_memory(filename, temp_data, temp_indices, temp_fields)
 
         if write_type == 'chunk':
             with open(self.database_path / 'info.json', 'w') as f:
                 total_shape[0] += data_shape
                 json.dump({"total_shape": total_shape}, f)
         else:
             self.cluster_last_file_shape[cluster_id] = [data_shape + total_shape[0], self.dimension]
 
-    def cluster_write(self, cluster_id, data, indices, fields):
+    def cluster_write(self, cluster_id, data, indices, fields, normalize=False):
         """Write the data to the file."""
-        self._write(data, indices, fields, write_type='cluster', cluster_id=cluster_id)
+        self._write(data, indices, fields, write_type='cluster', cluster_id=cluster_id, normalize=normalize)
 
-    def chunk_write(self, data, indices, fields):
+    def chunk_write(self, data, indices, fields, normalize=False):
         """Write the data to the file."""
-        self._write(data, indices, fields, write_type='chunk')
+        self._write(data, indices, fields, write_type='chunk', normalize=normalize)
 
-    def read(self, read_type='chunk', cluster_id=None, reverse=False, order_read=False):
+    def read(self, read_type='chunk', cluster_id=None, reverse=False):
         """Read the data from the file."""
         if read_type == 'chunk':
-            yield from self.chunk_read(reverse=reverse, order_read=order_read)
+            yield from self.chunk_read(reverse=reverse)
         elif read_type == 'cluster':
-            yield from self.cluster_read(cluster_id, reverse=reverse, order_read=order_read)
+            yield from self.cluster_read(cluster_id, reverse=reverse)
         elif read_type == 'all':
-            yield from self.chunk_read(reverse=reverse, order_read=order_read)
-            yield from self.cluster_read(cluster_id, reverse=reverse, order_read=order_read)
+            yield from self.chunk_read(reverse=reverse)
+            yield from self.cluster_read(cluster_id, reverse=reverse)
         else:
             raise ValueError('read_type must be "chunk" or "cluster"')
 
-    def write(self, data, indices, fields, write_type='chunk', cluster_id=None):
+    def write(self, data, indices, fields, write_type='chunk', cluster_id=None, normalize=False):
         """Write the data to the file."""
         if write_type == 'chunk':
-            self.chunk_write(data, indices, fields)
+            self.chunk_write(data, indices, fields, normalize=normalize)
         elif write_type == 'cluster':
             raise_if(ValueError, not isinstance(cluster_id, str) and not cluster_id.isdigit(),
                      "cluster_id must be string-type integer.")
-            self.cluster_write(cluster_id, data, indices, fields)
+            self.cluster_write(cluster_id, data, indices, fields, normalize=normalize)
         else:
             raise ValueError('write_type must be "chunk" or "cluster"')
 
     def get_shape(self, read_type='all'):
         """Get the shape of the data.
         parameters:
             read_type (str): The type of data to read. Must be 'chunk' or 'cluster' or 'all'.
@@ -434,15 +363,15 @@
 
         for path in paths:
             _data, indices, fields = self._load_data(
                 path,
                 self.database_chunk_path if read_type == 'chunk' else self.database_cluster_path,
                 self.database_chunk_indices_path if read_type == 'chunk' else self.database_cluster_indices_path,
                 self.database_chunk_fields_path if read_type == 'chunk' else self.database_cluster_fields_path,
-                reverse=False
+                reverse=False, update_memory=False
             )
 
             if by_indices not in indices:
                 continue
 
             index = np.where(indices == by_indices)[0][0]
             _data[index] = data
```

### Comparing `MinVectorDB-0.2.4/min_vec/utils/utils.py` & `minvectordb-0.2.5/min_vec/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """utils.py: this file contains some useful functions and decorators."""
 
 from functools import wraps
 
-from min_vec.configs.config import MVDB_COSINE_SIMILARITY_THRESHOLD
-
 
 class UnKnownError(Exception):
     pass
 
 
 def io_checker(func):
-    from functools import wraps
     from pathlib import Path
     from spinesUtils.asserts import raise_if
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             res = func(*args, **kwargs)
@@ -38,36 +35,24 @@
 class QueryVectorCache:
     """A decorator that caches the results of a function call with the same arguments.
         Only use for DatabaseQuery.query function.
     """
 
     def __init__(self, max_size=1000):
         from collections import OrderedDict
-        from min_vec.computational_layer.engines import cosine_distance
 
         self.cache = OrderedDict()
         self.max_size = max_size
-        self._cosine_similarity = cosine_distance
 
     def clear_cache(self):
         self.cache.clear()
 
     def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            import numpy as np
-
-            if len(args) < 2:
-                query_vec = kwargs['vector']
-            else:
-                query_vec = args[1]  # this argument is the query vector
-
-            best_similarity = 0.0
-            best_result = None
-
             # 生成基于参数的唯一键，确保所有部分都是可哈希的
             key_parts = []
             for arg in args[1:]:  # ignore the self parameter
                 if hasattr(arg, 'tobytes'):
                     key_parts.append(('vector', arg.tobytes()))
                 elif hasattr(arg, '__dict__'):
                     key_parts.append(arg.__dict__)
@@ -87,36 +72,30 @@
                     key_parts.append((k, v))
 
             # 将参数列表转换为元组，作为键
             key = tuple(key_parts)
 
             # 检查是否在缓存中找到对应的向量并计算相似度
             if key in self.cache:
-                return self.cache[key]
+                best_result = self.cache[key]
             else:
-                if MVDB_COSINE_SIMILARITY_THRESHOLD is not None:
-                    # 遍历缓存中的向量，找到最相似的向量
-                    for cached_key, cached_vec in self.cache.items():
-                        for cv in cached_vec:
-                            if cv[0] == 'vector':
-                                cached_vec = np.frombuffer(cv, dtype=np.float32)
-
-                                similarity = self._cosine_similarity(query_vec, cached_vec)
-                                if similarity > MVDB_COSINE_SIMILARITY_THRESHOLD:
-                                    if similarity > best_similarity:
-                                        best_similarity = similarity
-                                        best_result = self.cache[key]
-                                        break
-
-            # 如果没有找到足够相似的结果，则执行原函数获取新的结果并更新缓存
-            if best_result is None:
-                if len(self.cache) >= self.max_size:
-                    self.cache.popitem(last=False)
-
-                result = func(*args, **kwargs)
-                best_result = result
-                self.cache[key] = result
+                best_result = func(*args, **kwargs)
+                self.cache[key] = best_result
 
             return best_result
 
         wrapper.clear_cache = self.clear_cache
         return wrapper
+
+
+def unavailable_if_deleted(func):
+    """A decorator that detects if the function is called after the object is deleted."""
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        # self is the first parameter
+        if args[0]._matrix_serializer.IS_DELETED:
+            print("The database has been deleted, and the operation is invalid.")
+            return None
+        return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `MinVectorDB-0.2.4/setup.py` & `minvectordb-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,33 +11,34 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.2.4",
+    version="0.2.5",
     description='MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed database' \
                 'that offers clear and concise Python APIs, aimed at lowering the barrier to ' \
                 'the use of vector databases.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    python_requires=">=3.10",
+    python_requires=">=3.9",
     url='https://github.com/BirchKwok/MinVectorDB',
     author='Birch Kwok',
     author_email='birchkwok@gmail.com',
     install_requires=reqs,
     zip_safe=False,
 )
```

### Comparing `MinVectorDB-0.2.4/test/test_model.py` & `minvectordb-0.2.5/test/test_save_and_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,128 +24,93 @@
         database.bulk_add_items(items)
 
     return database
 
 
 def test_add_single_item_without_id_and_field():
     database = get_database()
-    id = database.add_item(np.ones(100), save_immediately=True)
+    id = database.add_item(np.ones(100))
+
+    database.commit()
 
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
-
     assert database.shape == (1, 100)
 
     database.delete()
 
 
 def test_add_single_item_with_id_and_field():
     database = get_database()
-    id = database.add_item(np.ones(100), index=1, field="test", save_immediately=True)
+    id = database.add_item(np.ones(100), index=1, field="test")
+
+    database.commit()
 
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
-
     assert database.shape == (1, 100)
 
     database.delete()
 
 
 def test_bulk_add_item_without_id_and_field():
     database = get_database()
     items = []
     for i in range(101):
         items.append((np.ones(100), ))
 
-    database.bulk_add_items(items, save_immediately=True)
-
-    assert database._matrix_serializer.database == []
-    assert database._matrix_serializer.fields == []
-    assert database._matrix_serializer.indices == []
+    database.bulk_add_items(items)
 
     database.commit()
-
-    assert database.shape == (101, 100)
-
-    database.delete()
-
-
-def test_add_single_item_with_vector_normalize():
-    database = get_database()
-    id = database.add_item(np.ones(100), index=1, field="test", save_immediately=True, normalize=True)
-
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
-
-    assert database.shape == (1, 100)
+    assert database.shape == (101, 100)
 
     database.delete()
 
 
-def test_add_bulk_item_with_id_and_field():
+def test_bulk_add_item_with_id_and_field():
     database = get_database()
     items = []
     for i in range(101):
         items.append((np.ones(100), i, "test_" + str(i // 10)))
 
-    database.bulk_add_items(items, save_immediately=True)
-
-    assert database._matrix_serializer.database == []
-    assert database._matrix_serializer.fields == []
-    assert database._matrix_serializer.indices == []
+    database.bulk_add_items(items)
 
     database.commit()
 
-    assert database.shape == (101, 100)
-
-    database.delete()
-
-
-def test_add_bulk_item_with_normalize():
-    database = get_database()
-    items = []
-    for i in range(101):
-        items.append((np.ones(100), i, "test_" + str(i // 10)))
-
-    database.bulk_add_items(items, save_immediately=True, normalize=True)
-
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
-
     assert database.shape == (101, 100)
 
     database.delete()
 
 
 def test_add_bulk_item_with_id_and_chinese_field():
     database = get_database()
     items = []
     for i in range(101):
         items.append((np.ones(100), i, "测试_" + str(i // 10)))
 
-    database.bulk_add_items(items, save_immediately=True)
+    database.bulk_add_items(items)
+
+    database.commit()
 
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
-
     assert database.shape == (101, 100)
 
     database.delete()
 
 
 def test_query_without_field():
     database = get_database_for_query(with_field=False)
@@ -175,15 +140,15 @@
     database.delete()
 
 
 def test_query_with_normalize():
     database = get_database_for_query(with_field=True)
 
     vec = np.random.random(100)
-    n, d = database.query(vec, k=6, fields=['test_1'], normalize=True)
+    n, d = database.query(vec, k=6, fields=['test_1'])
 
     assert len(n) == len(d) == 6
     assert list(d) == sorted(d, key=lambda s: -s)
     assert all(i in database._id_filter for i in n)
     assert all(10 <= i < 20 for i in n)
 
     database.delete()
@@ -227,73 +192,86 @@
     assert list(d) == sorted(d, key=lambda s: -s)
     assert all(i in database._id_filter for i in n)
     assert all((10 <= i < 20) or (70 <= i < 80) for i in n)
 
     database.delete()
 
 
-def test_query_stability_of_mvdb_files():
-    """Test whether the modification time of the mvdb file changes when querying multiple times."""
+def test_query_with_subset_indices():
     database = get_database_for_query(with_field=True)
+
     vec = np.random.random(100)
-    last_n, last_d = database.query(vec, k=6, fields=['test_1'])
-    assert len(last_n) == len(last_d) == 6
-    for i in range(20):
-        n, d = database.query(vec, k=6, fields=['test_1'])
-        assert last_d.tolist() == d.tolist()
-        assert last_n.tolist() == n.tolist()
-        assert len(n) == len(d) == 6
-        assert list(d) == sorted(d, key=lambda s: -s)
-        assert all(i in database._id_filter for i in n)
-        assert all(10 <= i < 20 for i in n)
+    n, d = database.query(vec, k=6, subset_indices=list(range(10)))
+
+    assert len(n) == len(d) == 6
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(i < 10 for i in n)
 
     database.delete()
 
 
-def test_lazy_bulk_add_items():
-    database = get_database()
-    items = []
-    for i in range(101):
-        items.append((np.ones(100), ))
+def test_query_with_subset_indices_and_field():
+    database = get_database_for_query(with_field=True, field_prefix='test_')
 
-    with database.insert_session():
-        database.bulk_add_items(items, save_immediately=False)
+    vec = np.random.random(100)
+    n, d = database.query(vec, k=6, fields=['test_0'], subset_indices=list(range(10)))
+
+    assert len(n) == len(d) == 6
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(i < 10 for i in n)
 
-    assert database.shape == (101, 100)
-    assert int(database.head(101).sum()) == 101 * 100
     database.delete()
 
 
-def test_lazy_add_item():
-    database = get_database()
-    id = database.add_item(np.ones(100), save_immediately=False)
+def test_query_with_subset_indices_and_list_field():
+    database = get_database_for_query(with_field=True)
+
+    vec = np.random.random(100)
+    n, d = database.query(vec, k=12, fields=['test_1', 'test_7'], subset_indices=list(range(10, 20)) + list(range(70, 80)))
+
+    assert len(n) == len(d) == 12
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all((10 <= i < 20) or (70 <= i < 80) for i in n)
 
-    database.commit()
-    assert database.shape == (1, 100)
-    assert int(database.head(1).sum()) == 100
     database.delete()
 
 
-def test_lazy_add_item_and_lazy_bulk_add_items():
-    database = get_database()
-    items = []
-    for i in range(101):
-        items.append((np.ones(100), ))
+def test_query_with_subset_indices_and_chinese_field():
+    database = get_database_for_query(with_field=True, field_prefix='测试_')
 
-    with database.insert_session():
-        database.bulk_add_items(items, save_immediately=False)
-        database.add_item(np.ones(100), save_immediately=False)
+    vec = np.random.random(100)
+    n, d = database.query(vec, k=6, fields=['测试_0'], subset_indices=list(range(10)))
+
+    assert len(n) == len(d) == 6
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(i < 10 for i in n)
+
+    database.delete()
+
+
+def test_query_with_subset_indices_and_chinese_list_field():
+    database = get_database_for_query(with_field=True, field_prefix='测试_')
+
+    vec = np.random.random(100)
+    n, d = database.query(vec, k=12, fields=['测试_1', '测试_7'],
+                          subset_indices=list(range(10, 20)) + list(range(70, 80)))
+
+    assert len(n) == len(d) == 12
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all((10 <= i < 20) or (70 <= i < 80) for i in n)
 
-    assert database.shape == (102, 100)
-    assert int(database.head(102).sum()) == 102 * 100
     database.delete()
 
 
-def test_query_stability_of_query_function():
-    """Test whether the modification time of the mvdb file changes when querying multiple times."""
+def test_query_stability_of_mvdb_files():
     database = get_database_for_query(with_field=True)
     vec = np.random.random(100)
     last_n, last_d = database.query(vec, k=6, fields=['test_1'])
     assert len(last_n) == len(last_d) == 6
     for i in range(20):
         n, d = database.query(vec, k=6, fields=['test_1'])
         assert last_d.tolist() == d.tolist()
@@ -309,105 +287,109 @@
 # Test whether calling bulk_add_items multiple times can insert data normally
 def test_multiple_bulk_add_items():
     database = get_database()
     items = []
     for i in range(101):
         items.append((np.ones(100), ))
 
-    database.bulk_add_items(items, save_immediately=False)
+    database.bulk_add_items(items)
     assert len(database._matrix_serializer.fields) == 101
     assert database._matrix_serializer.indices == list(range(101))
 
     database.commit()
     assert database.shape == (101, 100)
 
-    database.bulk_add_items(items, save_immediately=True)
+    database.bulk_add_items(items)
+    database.commit()
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
     assert database.shape == (202, 100)
 
     database.delete()
 
+
 def test_multiple_bulk_add_items_with_insert_session():
     database = get_database()
     items = []
     for i in range(101):
         items.append((np.ones(100), ))
 
-    database.bulk_add_items(items, save_immediately=False)
-    assert len(database._matrix_serializer.fields) == 101
-    assert database._matrix_serializer.indices == list(range(101))
+    with database.insert_session():
+        database.bulk_add_items(items)
+        assert len(database._matrix_serializer.fields) == 101
+        assert database._matrix_serializer.indices == list(range(101))
 
-    database.commit()
     assert database.shape == (101, 100)
 
-    database.bulk_add_items(items, save_immediately=True)
+    with database.insert_session():
+        database.bulk_add_items(items)
+
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
-    database.commit()
     assert database.shape == (202, 100)
 
     database.delete()
 
 
 # Test if secondary initialization can properly initialize and query
 def test_multiple_initialization(dim=100, database_path='test_min_vec.mvdb', chunk_size=1000, dtypes='float32'):
     database = MinVectorDB(dim=dim, database_path=database_path, chunk_size=chunk_size, dtypes=dtypes)
     items = []
     for i in range(101):
         items.append((np.ones(100), i, "test_" + str(i // 10)))
 
     with database.insert_session():
-        database.bulk_add_items(items, save_immediately=False)
+        database.bulk_add_items(items)
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
     assert database.shape == (101, 100)
     del database
 
     database = MinVectorDB(dim=dim, database_path=database_path, chunk_size=chunk_size, dtypes=dtypes)
 
     items = []
     for i in range(101):
         items.append((np.ones(100), None, "test_" + str(i // 10)))
     # insert
     with database.insert_session():
-        database.bulk_add_items(items, save_immediately=True)
+        database.bulk_add_items(items)
 
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
     assert database.shape == (202, 100)
     database.delete()
 
 
-# Test if secondary initialization can properly initialize and insert
-def test_multiple_initialization_with_insert_session(dim=100, database_path='test_min_vec.mvdb', chunk_size=1000, dtypes='float32'):
-    database = MinVectorDB(dim=dim, database_path=database_path, chunk_size=chunk_size, dtypes=dtypes)
-    items = []
-    for i in range(101):
-        items.append((np.ones(100), i, "test_" + str(i // 10)))
+def test_result_order():
+    def get_test_vectors(shape):
+        for i in range(shape[0]):
+            yield np.random.random(shape[1])
+
+    for index_mode in ['FLAT', 'IVF-FLAT']:
+        # for distance in ['cosine', 'L2']:
+        db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb',
+                         chunk_size=10000, index_mode=index_mode)
+
+        # You can perform this operation multiple times, and the data will be appended to the database.
+        with db.insert_session():
+            # Define the initial ID.
+            id = 0
+            vectors = []
+            for t in get_test_vectors((100000, 1024)):
+                if id == 0:
+                    query = t
+                vectors.append((t, id))
+                id += 1
+
+            # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
+            db.bulk_add_items(vectors)
 
-    with database.insert_session():
-        database.bulk_add_items(items, save_immediately=False)
-    assert database._matrix_serializer.fields == []
-    assert database._matrix_serializer.indices == []
+        index, score = db.query(query, k=10, return_similarity=True)
 
-    assert database.shape == (101, 100)
-    del database
+        assert len(index) == len(score) == 10
+        assert index[0] == 0
 
-    database = MinVectorDB(dim=dim, database_path=database_path, chunk_size=chunk_size, dtypes=dtypes)
-
-    items = []
-    for i in range(101):
-        items.append((np.ones(100), None, "test_" + str(i // 10)))
-    # insert
-    with database.insert_session():
-        database.bulk_add_items(items, save_immediately=True)
-    assert database._matrix_serializer.fields == []
-    assert database._matrix_serializer.indices == []
-
-    assert database.shape == (202, 100)
-    database.delete()
+        db.delete()
```

