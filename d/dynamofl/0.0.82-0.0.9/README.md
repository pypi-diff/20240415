# Comparing `tmp/dynamofl-0.0.82.tar.gz` & `tmp/dynamofl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamofl-0.0.82.tar", last modified: Mon Apr 15 15:59:50 2024, max compression
+gzip compressed data, was "dynamofl-0.0.9.tar", last modified: Tue Apr 12 20:51:49 2022, max compression
```

## Comparing `dynamofl-0.0.82.tar` & `dynamofl-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,13 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.325841 dynamofl-0.0.82/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2024-04-15 15:59:50.325841 dynamofl-0.0.82/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2052 2024-03-13 06:23:25.000000 dynamofl-0.0.82/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.309841 dynamofl-0.0.82/dynamofl/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1146 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/Datasource.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3767 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/Helpers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5084 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/MessageHandler.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4505 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/Project.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/Request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19066 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/State.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.309841 dynamofl-0.0.82/dynamofl/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/api/DatasourceAPI.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7689 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/api/ProjectAPI.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/api/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.313841 dynamofl-0.0.82/dynamofl/attacks/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/attacks/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      510 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/attacks/attack.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      379 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/attacks/pii_extraction.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.313841 dynamofl-0.0.82/dynamofl/datasets/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/datasets/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      984 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/datasets/base_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3147 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/datasets/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      817 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/datasets/hf_dataset.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.313841 dynamofl-0.0.82/dynamofl/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      953 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/entities/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/entities/model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/entities/test.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.317841 dynamofl-0.0.82/dynamofl/file_transfer/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/download.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1732 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/metadata.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/multipart_file_uploader_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      494 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/sha.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      651 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/thread_executor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5384 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/file_transfer/upload_v2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      889 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/logging.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.321841 dynamofl-0.0.82/dynamofl/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7872 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/models/local_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/models/model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3321 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/models/remote_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37180 2024-04-15 15:58:19.000000 dynamofl-0.0.82/dynamofl/src.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.325841 dynamofl-0.0.82/dynamofl/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/tests/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1182 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/tests/gpu_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3510 2024-04-15 15:04:15.000000 dynamofl-0.0.82/dynamofl/tests/test.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2015 2024-03-13 06:23:25.000000 dynamofl-0.0.82/dynamofl/vector_db.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 15:59:50.309841 dynamofl-0.0.82/dynamofl.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2024-04-15 15:59:50.000000 dynamofl-0.0.82/dynamofl.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1335 2024-04-15 15:59:50.000000 dynamofl-0.0.82/dynamofl.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 15:59:50.000000 dynamofl-0.0.82/dynamofl.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 15:59:49.000000 dynamofl-0.0.82/dynamofl.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-15 15:59:50.000000 dynamofl-0.0.82/dynamofl.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-15 15:59:50.000000 dynamofl-0.0.82/dynamofl.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-13 06:23:25.000000 dynamofl-0.0.82/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 15:59:50.325841 dynamofl-0.0.82/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      545 2024-04-15 15:59:45.000000 dynamofl-0.0.82/setup.py
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.534735 dynamofl-0.0.9/
+-rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-04-12 20:51:49.534924 dynamofl-0.0.9/PKG-INFO
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.526846 dynamofl-0.0.9/dynamofl/
+-rw-r--r--   0 emileindik   (501) staff       (20)       25 2022-04-12 20:48:47.000000 dynamofl-0.0.9/dynamofl/__init__.py
+-rw-r--r--   0 emileindik   (501) staff       (20)     8988 2022-04-12 20:48:38.000000 dynamofl-0.0.9/dynamofl/src.py
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.534355 dynamofl-0.0.9/dynamofl.egg-info/
+-rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-04-12 20:51:48.000000 dynamofl-0.0.9/dynamofl.egg-info/PKG-INFO
+-rw-r--r--   0 emileindik   (501) staff       (20)      220 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/SOURCES.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)        1 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/dependency_links.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)       41 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/requires.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)        9 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/top_level.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)      104 2021-10-23 03:06:00.000000 dynamofl-0.0.9/pyproject.toml
+-rw-r--r--   0 emileindik   (501) staff       (20)      247 2022-04-12 20:51:49.535678 dynamofl-0.0.9/setup.cfg
```

