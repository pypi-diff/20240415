# Comparing `tmp/datagouv_python-0.0.17.tar.gz` & `tmp/datagouv_python-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagouv_python-0.0.17.tar", max compression
+gzip compressed data, was "datagouv_python-0.0.18.tar", max compression
```

## Comparing `datagouv_python-0.0.17.tar` & `datagouv_python-0.0.18.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.0.17/LICENSE
--rw-r--r--   0        0        0     6188 2024-04-15 18:36:11.742768 datagouv_python-0.0.17/README.md
--rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.0.17/datagouv/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.0.17/datagouv/api_client/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-14 15:16:06.984989 datagouv_python-0.0.17/datagouv/api_client/_data_requestor.py
--rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.0.17/datagouv/api_client/_datagouv_client.py
--rw-r--r--   0        0        0     1456 2024-04-15 18:25:21.049046 datagouv_python-0.0.17/datagouv/api_client/_datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.0.17/datagouv/downloader/__init__.py
--rw-r--r--   0        0        0      862 2024-04-15 18:20:37.915207 datagouv_python-0.0.17/datagouv/downloader/_resources_downloader.py
--rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.0.17/datagouv/downloader/_utils.py
--rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.0.17/datagouv/main.py
--rw-r--r--   0        0        0      468 2024-04-15 18:26:51.514899 datagouv_python-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 datagouv_python-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.0.18/LICENSE
+-rw-r--r--   0        0        0     1937 2024-04-15 18:41:15.142307 datagouv_python-0.0.18/README.md
+-rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.0.18/datagouv/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.0.18/datagouv/api_client/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-14 15:16:06.984989 datagouv_python-0.0.18/datagouv/api_client/_data_requestor.py
+-rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.0.18/datagouv/api_client/_datagouv_client.py
+-rw-r--r--   0        0        0     1456 2024-04-15 18:25:21.049046 datagouv_python-0.0.18/datagouv/api_client/_datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.0.18/datagouv/downloader/__init__.py
+-rw-r--r--   0        0        0      886 2024-04-15 18:41:44.380886 datagouv_python-0.0.18/datagouv/downloader/_resources_downloader.py
+-rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.0.18/datagouv/downloader/_utils.py
+-rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.0.18/datagouv/main.py
+-rw-r--r--   0        0        0      468 2024-04-15 18:43:03.585360 datagouv_python-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 datagouv_python-0.0.18/PKG-INFO
```

### Comparing `datagouv_python-0.0.17/LICENSE` & `datagouv_python-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.17/datagouv/api_client/_data_requestor.py` & `datagouv_python-0.0.18/datagouv/api_client/_data_requestor.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.17/datagouv/api_client/_datasets_service.py` & `datagouv_python-0.0.18/datagouv/api_client/_datasets_service.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.17/datagouv/downloader/_resources_downloader.py` & `datagouv_python-0.0.18/datagouv/downloader/_resources_downloader.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
         self.dataset = None
         self.resources = []
         self.urls = []
 
         self.client = DatagouvClient()
 
+        self.prepare()
+
     def prepare(self):
         """
         Fetch dataset, set resources and urls.
         """
         self.dataset = self.client.datasets.get(self.dataset_id)
         self.resources = self.dataset.get("resources")
         self.urls = [resource.get("url") for resource in self.resources]
```

### Comparing `datagouv_python-0.0.17/datagouv/downloader/_utils.py` & `datagouv_python-0.0.18/datagouv/downloader/_utils.py`

 * *Files identical despite different names*

