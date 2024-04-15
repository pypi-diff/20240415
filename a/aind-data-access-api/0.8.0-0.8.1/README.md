# Comparing `tmp/aind-data-access-api-0.8.0.tar.gz` & `tmp/aind_data_access_api-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-data-access-api-0.8.0.tar", last modified: Wed Feb  7 01:03:19 2024, max compression
+gzip compressed data, was "aind_data_access_api-0.8.1.tar", last modified: Mon Apr 15 18:37:55 2024, max compression
```

## Comparing `aind-data-access-api-0.8.0.tar` & `aind_data_access_api-0.8.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.239055 aind-data-access-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.227055 aind-data-access-api-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-02-07 01:03:19.239055 aind-data-access-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 01:03:19.239055 aind-data-access-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.227055 aind-data-access-api-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.231055 aind-data-access-api-0.8.0/src/aind_data_access_api/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/document_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/rds_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/src/aind_data_access_api/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.235055 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-02-07 01:03:19.000000 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-07 01:03:19.000000 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 01:03:19.000000 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-07 01:03:19.000000 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-07 01:03:19.000000 aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:03:19.235055 aind-data-access-api-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21464 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_document_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_rds_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-02-07 01:03:05.000000 aind-data-access-api-0.8.0/tests/test_secrets_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.879806 aind_data_access_api-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.867806 aind_data_access_api-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-15 18:37:55.879806 aind_data_access_api-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:37:55.879806 aind_data_access_api-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.867806 aind_data_access_api-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.871806 aind_data_access_api-0.8.1/src/aind_data_access_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/document_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/src/aind_data_access_api/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.875806 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-15 18:37:55.000000 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-15 18:37:55.000000 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:37:55.000000 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 18:37:55.000000 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 18:37:55.000000 aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:37:55.875806 aind_data_access_api-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21464 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_document_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-15 18:37:46.000000 aind_data_access_api-0.8.1/tests/test_secrets_access.py
```

### Comparing `aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_data_access_api-0.8.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.github/workflows/init.yml` & `aind_data_access_api-0.8.1/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.github/workflows/tag_and_publish.yml` & `aind_data_access_api-0.8.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.github/workflows/test_and_lint.yml` & `aind_data_access_api-0.8.1/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/.gitignore` & `aind_data_access_api-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/LICENSE` & `aind_data_access_api-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/PKG-INFO` & `aind_data_access_api-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.8.0
+Version: 0.8.1
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,15 +23,15 @@
 Requires-Dist: aind-data-access-api[full]; extra == "dev"
 Provides-Extra: secrets
 Requires-Dist: boto3; extra == "secrets"
 Provides-Extra: docdb
 Requires-Dist: pymongo==4.3.3; extra == "docdb"
 Provides-Extra: rds
 Requires-Dist: psycopg2-binary==2.9.5; extra == "rds"
-Requires-Dist: pandas>=2.0.0; extra == "rds"
+Requires-Dist: pandas<2.2.0,>=2.0.0; extra == "rds"
 Requires-Dist: SQLAlchemy==1.4.49; extra == "rds"
 Provides-Extra: full
 Requires-Dist: aind-data-access-api[secrets]; extra == "full"
 Requires-Dist: aind-data-access-api[docdb]; extra == "full"
 Requires-Dist: aind-data-access-api[rds]; extra == "full"
 
 # aind-data-access-api
```

### Comparing `aind-data-access-api-0.8.0/README.md` & `aind_data_access_api-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/Makefile` & `aind_data_access_api-0.8.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/make.bat` & `aind_data_access_api-0.8.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/source/_static/dark-logo.svg` & `aind_data_access_api-0.8.1/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/source/_static/favicon.ico` & `aind_data_access_api-0.8.1/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/source/_static/light-logo.svg` & `aind_data_access_api-0.8.1/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/doc_template/source/conf.py` & `aind_data_access_api-0.8.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/pyproject.toml` & `aind_data_access_api-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "boto3",
 ]
 docdb = [
     "pymongo==4.3.3"
 ]
 rds = [
     "psycopg2-binary==2.9.5",
-    "pandas>=2.0.0",
+    "pandas>=2.0.0,<2.2.0",
     "SQLAlchemy==1.4.49"
 ]
 full = [
     "aind-data-access-api[secrets]",
     "aind-data-access-api[docdb]",
     "aind-data-access-api[rds]",
 ]
```

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/credentials.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # Will not be printed in repr string.
     aws_secrets_name: Optional[str] = Field(default=None, repr=False)
 
     username: str = Field(...)
     password: SecretStr = Field(...)
     host: str = Field(...)
     port: int = Field(...)
-    database: str = Field(...)
+    database: Optional[str] = Field(default=None)
 
     @classmethod
     def settings_customise_sources(
         cls,
         settings_cls: Type[BaseSettings],
         init_settings: InitSettingsSource,
         env_settings: EnvSettingsSource,
```

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/document_db.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/document_db.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/document_store.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/document_store.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/models.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/rds_tables.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/rds_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module to interface with the Relational Database"""
 
 from typing import Optional, Union
-
+from typing_extensions import Self
 import pandas as pd
 import sqlalchemy.engine
-from pydantic import AliasChoices, Field, SecretStr
+from pydantic import AliasChoices, Field, SecretStr, model_validator
 from pydantic_settings import SettingsConfigDict
 from sqlalchemy import create_engine, engine, text
 from sqlalchemy.engine.cursor import CursorResult
 
 from aind_data_access_api.credentials import CoreCredentials
 
 
@@ -22,15 +22,26 @@
     username: str = Field(
         ...,
         validation_alias=AliasChoices("username", "RDS_USER", "RDS_USERNAME"),
     )
     password: SecretStr = Field(...)
     host: str = Field(...)
     port: int = Field(default=5432)
-    database: str = Field(...)
+    dbname: Optional[str] = Field(default=None)
+
+    @model_validator(mode="after")
+    def validate_database_name(self) -> Self:
+        """Sets database to db_name"""
+        if self.database is None and self.dbname is None:
+            raise ValueError(
+                "At least one of dbname or database needs to be set"
+            )
+        elif self.database is None:
+            self.database = self.dbname
+        return self
 
 
 class Client:
     """Class to establish a relational database client. Includes methods to
     read/write pandas dataframes to backend."""
 
     def __init__(
@@ -57,15 +68,14 @@
     @property
     def _engine(self) -> sqlalchemy.engine.Engine:
         """Create a sqlalchemy engine:
         https://docs.sqlalchemy.org/en/20/core/engines.html
 
         Returns: sqlalchemy.engine.Engine
         """
-
         connection_url = engine.URL.create(
             drivername=self.drivername,
             username=self.credentials.username,
             password=self.credentials.password.get_secret_value(),
             host=self.credentials.host,
             database=self.credentials.database,
             port=self.credentials.port,
```

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api/secrets.py` & `aind_data_access_api-0.8.1/src/aind_data_access_api/secrets.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/PKG-INFO` & `aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.8.0
+Version: 0.8.1
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,15 +23,15 @@
 Requires-Dist: aind-data-access-api[full]; extra == "dev"
 Provides-Extra: secrets
 Requires-Dist: boto3; extra == "secrets"
 Provides-Extra: docdb
 Requires-Dist: pymongo==4.3.3; extra == "docdb"
 Provides-Extra: rds
 Requires-Dist: psycopg2-binary==2.9.5; extra == "rds"
-Requires-Dist: pandas>=2.0.0; extra == "rds"
+Requires-Dist: pandas<2.2.0,>=2.0.0; extra == "rds"
 Requires-Dist: SQLAlchemy==1.4.49; extra == "rds"
 Provides-Extra: full
 Requires-Dist: aind-data-access-api[secrets]; extra == "full"
 Requires-Dist: aind-data-access-api[docdb]; extra == "full"
 Requires-Dist: aind-data-access-api[rds]; extra == "full"
 
 # aind-data-access-api
```

### Comparing `aind-data-access-api-0.8.0/src/aind_data_access_api.egg-info/SOURCES.txt` & `aind_data_access_api-0.8.1/src/aind_data_access_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/tests/test_credentials.py` & `aind_data_access_api-0.8.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/tests/test_document_db.py` & `aind_data_access_api-0.8.1/tests/test_document_db.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/tests/test_document_store.py` & `aind_data_access_api-0.8.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/tests/test_models.py` & `aind_data_access_api-0.8.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.8.0/tests/test_rds_tables.py` & `aind_data_access_api-0.8.1/tests/test_rds_tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,47 @@
 
 import pandas as pd
 from sqlalchemy import text
 
 from aind_data_access_api.rds_tables import Client, RDSCredentials
 
 
+class TestRDSCredentials(unittest.TestCase):
+    """Tests RDSCredentials class"""
+
+    def test_validate_database_name(self):
+        """Tests that database is set from dbname as expected."""
+        creds = RDSCredentials(
+            username="user",
+            password="password",
+            host="localhost",
+            port=5432,
+            dbname="test_db",
+        )
+        self.assertEqual(creds.database, "test_db")
+
+        creds2 = RDSCredentials(
+            username="user",
+            password="password",
+            host="localhost",
+            port=5432,
+            database="test_db",
+        )
+        self.assertEqual(creds2.database, "test_db")
+        self.assertIsNone(creds2.dbname)
+
+        with self.assertRaises(ValueError):
+            RDSCredentials(
+                username="user",
+                password="password",
+                host="localhost",
+                port=5432,
+            )
+
+
 class TestClient(unittest.TestCase):
     """Tests methods in the Client class."""
 
     @patch("pandas.read_sql_query")
     @patch("sqlalchemy.engine.Engine.begin")
     def test_read_table(self, mock_engine: MagicMock, mock_pd_read: MagicMock):
         """Tests that read_table returns a pandas df."""
```

### Comparing `aind-data-access-api-0.8.0/tests/test_secrets_access.py` & `aind_data_access_api-0.8.1/tests/test_secrets_access.py`

 * *Files identical despite different names*

