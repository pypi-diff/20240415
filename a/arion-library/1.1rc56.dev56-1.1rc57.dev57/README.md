# Comparing `tmp/arion_library-1.1rc56.dev56.tar.gz` & `tmp/arion_library-1.1rc57.dev57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc56.dev56.tar", last modified: Mon Apr 15 10:45:46 2024, max compression
+gzip compressed data, was "arion_library-1.1rc57.dev57.tar", last modified: Mon Apr 15 11:41:13 2024, max compression
```

## Comparing `arion_library-1.1rc56.dev56.tar` & `arion_library-1.1rc57.dev57.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.877946 arion_library-1.1rc56.dev56/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 10:45:46.000000 arion_library-1.1rc56.dev56/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 10:45:46.000000 arion_library-1.1rc56.dev56/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:45:46.000000 arion_library-1.1rc56.dev56/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 10:45:46.000000 arion_library-1.1rc56.dev56/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 10:45:46.000000 arion_library-1.1rc56.dev56/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.877946 arion_library-1.1rc56.dev56/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.877946 arion_library-1.1rc56.dev56/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.877946 arion_library-1.1rc56.dev56/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.877946 arion_library-1.1rc56.dev56/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 10:45:18.000000 arion_library-1.1rc56.dev56/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:45:46.881947 arion_library-1.1rc56.dev56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 10:45:45.000000 arion_library-1.1rc56.dev56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.607614 arion_library-1.1rc57.dev57/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:41:13.607614 arion_library-1.1rc57.dev57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 11:41:13.000000 arion_library-1.1rc57.dev57/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 11:41:13.000000 arion_library-1.1rc57.dev57/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:41:13.000000 arion_library-1.1rc57.dev57/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 11:41:13.000000 arion_library-1.1rc57.dev57/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:41:13.000000 arion_library-1.1rc57.dev57/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.603614 arion_library-1.1rc57.dev57/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.607614 arion_library-1.1rc57.dev57/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:41:13.607614 arion_library-1.1rc57.dev57/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 11:40:42.000000 arion_library-1.1rc57.dev57/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:41:13.607614 arion_library-1.1rc57.dev57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 11:41:12.000000 arion_library-1.1rc57.dev57/setup.py
```

### Comparing `arion_library-1.1rc56.dev56/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc57.dev57/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc57.dev57/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc57.dev57/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc57.dev57/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc57.dev57/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc57.dev57/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc57.dev57/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc57.dev57/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc57.dev57/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc56.dev56/setup.py` & `arion_library-1.1rc57.dev57/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc56.dev56',  # Replace with your package version
+    version='1.1rc57.dev57',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pysftp==0.2.9', 'azure-data-tables==12.5.0', 'azure-core', 'azure-data-tables', 'azure-storage-blob', 'python-dotenv', 'pytest', 'pandas==2.0.3', '', 'pytest', 'pyodbc'],
 )
```

