# Comparing `tmp/arion_library-1.1rc61.dev61.tar.gz` & `tmp/arion_library-1.1rc62.dev62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc61.dev61.tar", last modified: Mon Apr 15 12:22:42 2024, max compression
+gzip compressed data, was "arion_library-1.1rc62.dev62.tar", last modified: Mon Apr 15 15:59:41 2024, max compression
```

## Comparing `arion_library-1.1rc61.dev61.tar` & `arion_library-1.1rc62.dev62.tar`

### file list

```diff
@@ -1,47 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 12:22:42.000000 arion_library-1.1rc61.dev61/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 12:22:42.000000 arion_library-1.1rc61.dev61/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:22:42.000000 arion_library-1.1rc61.dev61/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 12:22:42.000000 arion_library-1.1rc61.dev61/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 12:22:42.000000 arion_library-1.1rc61.dev61/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.944435 arion_library-1.1rc61.dev61/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3088 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 12:22:12.000000 arion_library-1.1rc61.dev61/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:22:42.948435 arion_library-1.1rc61.dev61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 12:22:41.000000 arion_library-1.1rc61.dev61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 15:59:41.000000 arion_library-1.1rc62.dev62/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 15:59:41.000000 arion_library-1.1rc62.dev62/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:59:41.000000 arion_library-1.1rc62.dev62/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 15:59:41.000000 arion_library-1.1rc62.dev62/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 15:59:41.000000 arion_library-1.1rc62.dev62/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.670319 arion_library-1.1rc62.dev62/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 15:59:05.000000 arion_library-1.1rc62.dev62/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:59:41.674319 arion_library-1.1rc62.dev62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 15:59:40.000000 arion_library-1.1rc62.dev62/setup.py
```

### Comparing `arion_library-1.1rc61.dev61/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc62.dev62/processors/SFTP/lib/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         self.username = username
         self.password = password
         self.sftp = None
     
     def connect(self):
 
         """
-        Establishes a connection to an SFTP server.
-        test issue 132 docs
+
+        Establishes a connection to an SFTP server_______
         This method attempts to connect to an SFTP server using the provided credentials.
         If successful, it initializes a connection object that can be used for file operations.
 
         :raises: Any exception raised during the connection attempt is caught and logged.
                 This ensures that errors are properly handled without crashing the program.
 
         :return: None
```

### Comparing `arion_library-1.1rc61.dev61/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc62.dev62/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc62.dev62/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc62.dev62/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import re
 from io import BytesIO
 from datetime import datetime
 import logging
 
 class AzureBlobProcessor:
     """
-    A class for processing files in Azure Blob Storage that can help.
+
+    A class for processing files in Azure Blob Storage_____
+
+
+
     
     :param account_name: The Azure Storage account name.
     :param account_key: The Azure Storage account key.
     :param container_name: The name of the container in Azure Blob Storage.
     :param flow_name: The name of the flow for organizing files.
     """
```

### Comparing `arion_library-1.1rc61.dev61/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc62.dev62/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc62.dev62/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc62.dev62/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc62.dev62/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc61.dev61/setup.py` & `arion_library-1.1rc62.dev62/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc61.dev61',  # Replace with your package version
+    version='1.1rc62.dev62',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
-    install_requires=['pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==1.4.0', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
+    install_requires=['pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

