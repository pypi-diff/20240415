# Comparing `tmp/arion_library-1.1rc58.dev58.tar.gz` & `tmp/arion_library-1.1rc59.dev59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc58.dev58.tar", last modified: Mon Apr 15 11:54:17 2024, max compression
+gzip compressed data, was "arion_library-1.1rc59.dev59.tar", last modified: Mon Apr 15 11:59:45 2024, max compression
```

## Comparing `arion_library-1.1rc58.dev58.tar` & `arion_library-1.1rc59.dev59.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.020036 arion_library-1.1rc58.dev58/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:54:16.000000 arion_library-1.1rc58.dev58/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 11:54:16.000000 arion_library-1.1rc58.dev58/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:54:16.000000 arion_library-1.1rc58.dev58/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 11:54:16.000000 arion_library-1.1rc58.dev58/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:54:16.000000 arion_library-1.1rc58.dev58/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.020036 arion_library-1.1rc58.dev58/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.020036 arion_library-1.1rc58.dev58/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3074 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 11:53:48.000000 arion_library-1.1rc58.dev58/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:54:17.024036 arion_library-1.1rc58.dev58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-15 11:54:15.000000 arion_library-1.1rc58.dev58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.066065 arion_library-1.1rc59.dev59/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:59:45.066065 arion_library-1.1rc59.dev59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:59:45.000000 arion_library-1.1rc59.dev59/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 11:59:45.000000 arion_library-1.1rc59.dev59/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:59:45.000000 arion_library-1.1rc59.dev59/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 11:59:45.000000 arion_library-1.1rc59.dev59/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:59:45.000000 arion_library-1.1rc59.dev59/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3090 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:45.062065 arion_library-1.1rc59.dev59/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 11:59:17.000000 arion_library-1.1rc59.dev59/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:59:45.066065 arion_library-1.1rc59.dev59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-15 11:59:43.000000 arion_library-1.1rc59.dev59/setup.py
```

### Comparing `arion_library-1.1rc58.dev58/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc59.dev59/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc59.dev59/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc59.dev59/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc59.dev59/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc59.dev59/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from io import BytesIO
 from datetime import datetime
 import logging
 
 class AzureBlobProcessor:
     """
-    A class for processing files in Azure Blob Storage.
+    A class for processing files in Azure Blob Storage. . . . . . . . .
     
     :param account_name: The Azure Storage account name.
     :param account_key: The Azure Storage account key.
     :param container_name: The name of the container in Azure Blob Storage.
     :param flow_name: The name of the flow for organizing files.
     """
```

### Comparing `arion_library-1.1rc58.dev58/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc59.dev59/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc59.dev59/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc59.dev59/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc59.dev59/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc58.dev58/setup.py` & `arion_library-1.1rc59.dev59/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc58.dev58',  # Replace with your package version
+    version='1.1rc59.dev59',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pysftp==0.2.9', 'azure-data-tables==12.5.0', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==1.4.0', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', '', 'pytest', 'pyodbc'],
 )
```
