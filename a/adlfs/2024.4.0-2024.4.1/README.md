# Comparing `tmp/adlfs-2024.4.0.tar.gz` & `tmp/adlfs-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adlfs-2024.4.0.tar", last modified: Sat Apr 13 13:04:56 2024, max compression
+gzip compressed data, was "adlfs-2024.4.1.tar", last modified: Mon Apr 15 21:37:45 2024, max compression
```

## Comparing `adlfs-2024.4.0.tar` & `adlfs-2024.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.515181 adlfs-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-13 13:04:43.000000 adlfs-2024.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-13 13:04:43.000000 adlfs-2024.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 13:04:43.000000 adlfs-2024.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-13 13:04:43.000000 adlfs-2024.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 13:04:43.000000 adlfs-2024.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-13 13:04:56.515181 adlfs-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-13 13:04:43.000000 adlfs-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/adlfs/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/gen1.py
--rw-r--r--   0 runner    (1001) docker     (127)    78702 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/adlfs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_fetch_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    61876 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_uri_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/adlfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-13 13:04:43.000000 adlfs-2024.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/earliest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/latest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-13 13:04:56.515181 adlfs-2024.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.666049 adlfs-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.658049 adlfs-2024.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 21:37:41.000000 adlfs-2024.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-15 21:37:41.000000 adlfs-2024.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 21:37:41.000000 adlfs-2024.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 21:37:41.000000 adlfs-2024.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-15 21:37:41.000000 adlfs-2024.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 21:37:41.000000 adlfs-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-15 21:37:45.666049 adlfs-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-15 21:37:41.000000 adlfs-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/adlfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/gen1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78786 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/adlfs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/test_fetch_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61876 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/tests/test_uri_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-15 21:37:41.000000 adlfs-2024.4.1/adlfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/adlfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 21:37:45.000000 adlfs-2024.4.1/adlfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 21:37:41.000000 adlfs-2024.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 21:37:41.000000 adlfs-2024.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:37:45.662049 adlfs-2024.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 21:37:41.000000 adlfs-2024.4.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 21:37:41.000000 adlfs-2024.4.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:37:41.000000 adlfs-2024.4.1/requirements/earliest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 21:37:41.000000 adlfs-2024.4.1/requirements/latest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 21:37:45.666049 adlfs-2024.4.1/setup.cfg
```

### Comparing `adlfs-2024.4.0/.github/workflows/docs.yml` & `adlfs-2024.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/.github/workflows/release.yml` & `adlfs-2024.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/.github/workflows/tests.yml` & `adlfs-2024.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/.gitignore` & `adlfs-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/CHANGELOG.md` & `adlfs-2024.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/CONTRIBUTING.md` & `adlfs-2024.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/LICENSE.txt` & `adlfs-2024.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/PKG-INFO` & `adlfs-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Maintainer-email: Greg Hayes <hayesgb@gmail.com>
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `adlfs-2024.4.0/README.md` & `adlfs-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/gen1.py` & `adlfs-2024.4.1/adlfs/gen1.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/spec.py` & `adlfs-2024.4.1/adlfs/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,19 +273,22 @@
         self.connection_string = connection_string or os.getenv(
             "AZURE_STORAGE_CONNECTION_STRING"
         )
         self.sas_token = sas_token or os.getenv("AZURE_STORAGE_SAS_TOKEN")
         self.client_id = client_id or os.getenv("AZURE_STORAGE_CLIENT_ID")
         self.client_secret = client_secret or os.getenv("AZURE_STORAGE_CLIENT_SECRET")
         self.tenant_id = tenant_id or os.getenv("AZURE_STORAGE_TENANT_ID")
-        self.anon = anon or os.getenv("AZURE_STORAGE_ANON", "true").lower() not in [
-            "false",
-            "0",
-            "f",
-        ]
+        if anon is not None:
+            self.anon = anon
+        else:
+            self.anon = os.getenv("AZURE_STORAGE_ANON", "true").lower() not in [
+                "false",
+                "0",
+                "f",
+            ]
         self.location_mode = location_mode
         self.credential = credential
         self.request_session = request_session
         self.assume_container_exists = assume_container_exists
         if socket_timeout is not _SOCKET_TIMEOUT_DEFAULT:
             warnings.warn(
                 "socket_timeout is deprecated and has no effect.", FutureWarning
```

### Comparing `adlfs-2024.4.0/adlfs/tests/conftest.py` & `adlfs-2024.4.1/adlfs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/tests/test_fetch_range.py` & `adlfs-2024.4.1/adlfs/tests/test_fetch_range.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/tests/test_loop.py` & `adlfs-2024.4.1/adlfs/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/tests/test_spec.py` & `adlfs-2024.4.1/adlfs/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/tests/test_uri_format.py` & `adlfs-2024.4.1/adlfs/tests/test_uri_format.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs/utils.py` & `adlfs-2024.4.1/adlfs/utils.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/adlfs.egg-info/PKG-INFO` & `adlfs-2024.4.1/adlfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Maintainer-email: Greg Hayes <hayesgb@gmail.com>
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `adlfs-2024.4.0/adlfs.egg-info/SOURCES.txt` & `adlfs-2024.4.1/adlfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/docs/Makefile` & `adlfs-2024.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/docs/conf.py` & `adlfs-2024.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/docs/index.md` & `adlfs-2024.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/docs/make.bat` & `adlfs-2024.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `adlfs-2024.4.0/pyproject.toml` & `adlfs-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

