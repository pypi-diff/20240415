# Comparing `tmp/datagouv_python-0.0.18.tar.gz` & `tmp/datagouv_python-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagouv_python-0.0.18.tar", max compression
+gzip compressed data, was "datagouv_python-0.0.19.tar", max compression
```

## Comparing `datagouv_python-0.0.18.tar` & `datagouv_python-0.0.19.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.0.18/LICENSE
--rw-r--r--   0        0        0     1937 2024-04-15 18:41:15.142307 datagouv_python-0.0.18/README.md
--rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.0.18/datagouv/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.0.18/datagouv/api_client/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-14 15:16:06.984989 datagouv_python-0.0.18/datagouv/api_client/_data_requestor.py
--rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.0.18/datagouv/api_client/_datagouv_client.py
--rw-r--r--   0        0        0     1456 2024-04-15 18:25:21.049046 datagouv_python-0.0.18/datagouv/api_client/_datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.0.18/datagouv/downloader/__init__.py
--rw-r--r--   0        0        0      886 2024-04-15 18:41:44.380886 datagouv_python-0.0.18/datagouv/downloader/_resources_downloader.py
--rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.0.18/datagouv/downloader/_utils.py
--rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.0.18/datagouv/main.py
--rw-r--r--   0        0        0      468 2024-04-15 18:43:03.585360 datagouv_python-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 datagouv_python-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.0.19/LICENSE
+-rw-r--r--   0        0        0     1937 2024-04-15 18:41:15.142307 datagouv_python-0.0.19/README.md
+-rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.0.19/datagouv/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.0.19/datagouv/api_client/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-14 15:16:06.984989 datagouv_python-0.0.19/datagouv/api_client/_data_requestor.py
+-rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.0.19/datagouv/api_client/_datagouv_client.py
+-rw-r--r--   0        0        0     1456 2024-04-15 18:25:21.049046 datagouv_python-0.0.19/datagouv/api_client/_datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.0.19/datagouv/downloader/__init__.py
+-rw-r--r--   0        0        0      912 2024-04-15 18:45:33.019203 datagouv_python-0.0.19/datagouv/downloader/_resources_downloader.py
+-rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.0.19/datagouv/downloader/_utils.py
+-rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.0.19/datagouv/main.py
+-rw-r--r--   0        0        0      468 2024-04-15 18:45:42.707826 datagouv_python-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 datagouv_python-0.0.19/PKG-INFO
```

### Comparing `datagouv_python-0.0.18/LICENSE` & `datagouv_python-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.18/README.md` & `datagouv_python-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.18/datagouv/api_client/_data_requestor.py` & `datagouv_python-0.0.19/datagouv/api_client/_data_requestor.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.18/datagouv/api_client/_datasets_service.py` & `datagouv_python-0.0.19/datagouv/api_client/_datasets_service.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.18/datagouv/downloader/_resources_downloader.py` & `datagouv_python-0.0.19/datagouv/downloader/_resources_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 
     def download(self, directory_path: str = None):
         """
         Download resources into `directory_path`
         """
         for url in self.urls:
             _utils.download(url, directory_path)
-
-        return
+        
+        return self.urls
+
```

### Comparing `datagouv_python-0.0.18/datagouv/downloader/_utils.py` & `datagouv_python-0.0.19/datagouv/downloader/_utils.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.0.18/PKG-INFO` & `datagouv_python-0.0.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagouv-python
-Version: 0.0.18
+Version: 0.0.19
 Summary: 
 License: GPL-3.0-or-later
 Author: Maxime Pawlak
 Author-email: maxime.pawlak@amatek.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```
