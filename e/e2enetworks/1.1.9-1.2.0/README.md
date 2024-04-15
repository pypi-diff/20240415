# Comparing `tmp/e2enetworks-1.1.9.tar.gz` & `tmp/e2enetworks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.1.9.tar", last modified: Fri Mar 29 10:55:29 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.0.tar", last modified: Mon Apr 15 09:52:08 2024, max compression
```

## Comparing `e2enetworks-1.1.9.tar` & `e2enetworks-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jagmeetsingh   (501) staff       (20)        0 2024-03-29 10:55:29.295262 e2enetworks-1.1.9/
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)    10786 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/LICENSE.txt
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1390 2024-03-29 10:55:29.294960 e2enetworks-1.1.9/PKG-INFO
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)        0 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/README.rst
-drwxr-xr-x   0 jagmeetsingh   (501) staff       (20)        0 2024-03-29 10:55:29.285485 e2enetworks-1.1.9/e2enetworks/
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)        0 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/__init__.py
-drwxr-xr-x   0 jagmeetsingh   (501) staff       (20)        0 2024-03-29 10:55:29.286401 e2enetworks-1.1.9/e2enetworks/cloud/
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)        0 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/__init__.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)      147 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/test.py
-drwxr-xr-x   0 jagmeetsingh   (501) staff       (20)        0 2024-03-29 10:55:29.293926 e2enetworks-1.1.9/e2enetworks/cloud/tir/
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2290 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     9296 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2794 2024-02-14 12:47:47.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     9405 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     7401 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     5788 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)    13823 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/endpoints.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2573 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1368 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2105 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     6455 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     6022 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     9999 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2849 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     4268 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     2391 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1159 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)       23 2024-02-13 12:57:49.000000 e2enetworks-1.1.9/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1517 2024-03-29 07:31:35.000000 e2enetworks-1.1.9/e2enetworks/constants.py
-drwxr-xr-x   0 jagmeetsingh   (501) staff       (20)        0 2024-03-29 10:55:29.294433 e2enetworks-1.1.9/e2enetworks.egg-info/
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1390 2024-03-29 10:55:29.000000 e2enetworks-1.1.9/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)      914 2024-03-29 10:55:29.000000 e2enetworks-1.1.9/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)        1 2024-03-29 10:55:29.000000 e2enetworks-1.1.9/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)      125 2024-03-29 10:55:29.000000 e2enetworks-1.1.9/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)       12 2024-03-29 10:55:29.000000 e2enetworks-1.1.9/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)       38 2024-03-29 10:55:29.295337 e2enetworks-1.1.9/setup.cfg
--rw-r--r--   0 jagmeetsingh   (501) staff       (20)     1809 2024-03-29 10:54:06.000000 e2enetworks-1.1.9/setup.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:52:08.758779 e2enetworks-1.2.0/
+-rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/LICENSE.txt
+-rw-r--r--   0 jagga      (501) staff       (20)     1207 2024-04-15 09:52:08.758662 e2enetworks-1.2.0/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/README.rst
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:52:08.754764 e2enetworks-1.2.0/e2enetworks/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/__init__.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:52:08.755532 e2enetworks-1.2.0/e2enetworks/cloud/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/test.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:52:08.758468 e2enetworks-1.2.0/e2enetworks/cloud/tir/
+-rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9296 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     7401 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/endpoints.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2573 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1517 2024-04-15 09:47:56.000000 e2enetworks-1.2.0/e2enetworks/constants.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:52:08.755324 e2enetworks-1.2.0/e2enetworks.egg-info/
+-rw-r--r--   0 jagga      (501) staff       (20)     1207 2024-04-15 09:52:08.000000 e2enetworks-1.2.0/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-15 09:52:08.000000 e2enetworks-1.2.0/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-15 09:52:08.000000 e2enetworks-1.2.0/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 jagga      (501) staff       (20)      125 2024-04-15 09:52:08.000000 e2enetworks-1.2.0/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-15 09:52:08.000000 e2enetworks-1.2.0/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-15 09:52:08.758829 e2enetworks-1.2.0/setup.cfg
+-rw-r--r--   0 jagga      (501) staff       (20)     1809 2024-04-15 09:52:03.000000 e2enetworks-1.2.0/setup.py
```

### Comparing `e2enetworks-1.1.9/LICENSE.txt` & `e2enetworks-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/api_client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/datasets.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/endpoints.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/endpoints.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/helpers.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/images.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/minio_service.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/models.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/notebook.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/notebook.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/pipelines.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/projects.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/skus.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.0/e2enetworks/cloud/tir/utils.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks/constants.py` & `e2enetworks-1.2.0/e2enetworks/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.0/e2enetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.1.9/setup.py` & `e2enetworks-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.1.9"
+version = "1.2.0"
 install_requires = [
     "requests~=2.30.0",
     "urllib3==1.26.6",
     "kfp==1.8.22",
     "kfp-pipeline-spec==0.1.16",
     "kfp-server-api==1.8.5",
     "minio==7.1.3",
```

