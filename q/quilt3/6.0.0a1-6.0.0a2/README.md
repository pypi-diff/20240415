# Comparing `tmp/quilt3-6.0.0a1.tar.gz` & `tmp/quilt3-6.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-2b7oklrf/quilt3-6.0.0a1.tar", last modified: Mon Feb 26 19:43:03 2024, max compression
+gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-nunz_r4w/quilt3-6.0.0a2.tar", last modified: Mon Apr 15 15:46:14 2024, max compression
```

## Comparing `quilt3-6.0.0a1.tar` & `quilt3-6.0.0a2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42519 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    65391 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/search_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/quilt3/workflows/config-1.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/quilt3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 19:43:03.000000 quilt3-6.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    29428 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_s3clientprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-02-26 19:42:49.000000 quilt3-6.0.0a1/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54270 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42519 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/quilt3/workflows/config-1.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/quilt3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:14.000000 quilt3-6.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29428 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_s3clientprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-15 15:45:55.000000 quilt3-6.0.0a2/tests/test_workflows.py
```

### Comparing `quilt3-6.0.0a1/LICENSE` & `quilt3-6.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/PKG-INFO` & `quilt3-6.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 6.0.0a1
+Version: 6.0.0a2
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-6.0.0a1/quilt3/__init__.py` & `quilt3-6.0.0a2/quilt3/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/admin.py` & `quilt3-6.0.0a2/quilt3/admin.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/api.py` & `quilt3-6.0.0a2/quilt3/api.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/backends/__init__.py` & `quilt3-6.0.0a2/quilt3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/backends/base.py` & `quilt3-6.0.0a2/quilt3/backends/base.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/backends/local.py` & `quilt3-6.0.0a2/quilt3/backends/local.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/backends/s3.py` & `quilt3-6.0.0a2/quilt3/backends/s3.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/bucket.py` & `quilt3-6.0.0a2/quilt3/bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/data_transfer.py` & `quilt3-6.0.0a2/quilt3/data_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -996,15 +996,15 @@
                 bytes_remaining = length
                 with open(src.path, 'rb') as fd:
                     fd.seek(offset)
                     while bytes_remaining > 0:
                         chunk = fd.read(min(s3_transfer_config.io_chunksize, bytes_remaining))
                         if not chunk:
                             # Should not happen, but let's not get stuck in an infinite loop.
-                            break
+                            raise QuiltException("Unexpected end of file")
                         hash_obj.update(chunk)
                         progress_update(len(chunk))
                         bytes_remaining -= len(chunk)
             else:
                 end = offset + length - 1
                 params = dict(
                     Bucket=src.bucket,
```

### Comparing `quilt3-6.0.0a1/quilt3/formats.py` & `quilt3-6.0.0a2/quilt3/formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/imports.py` & `quilt3-6.0.0a2/quilt3/imports.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/main.py` & `quilt3-6.0.0a2/quilt3/main.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/packages.py` & `quilt3-6.0.0a2/quilt3/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     copy_file,
     copy_file_list,
     get_bytes,
     get_size_and_version,
     legacy_calculate_checksum,
     legacy_calculate_checksum_bytes,
     list_object_versions,
+    list_objects,
     list_url,
     put_bytes,
 )
 from .exceptions import PackageException
 from .formats import CompressionRegistry, FormatRegistry
 from .telemetry import ApiTelemetry
 from .util import CACHE_PATH, DISABLE_TQDM, PACKAGE_UPDATE_POLICY
@@ -837,15 +838,15 @@
                     obj['hash'],
                     obj['meta'],
                 )
         finally:
             gc.enable()
         return pkg
 
-    def set_dir(self, lkey, path=None, meta=None, update_policy="incoming"):
+    def set_dir(self, lkey, path=None, meta=None, update_policy="incoming", unversioned: bool = False):
         """
         Adds all files from `path` to the package.
 
         Recursively enumerates every file in `path`, and adds them to
             the package according to their relative location to `path`.
 
         Args:
@@ -854,14 +855,15 @@
             path(string): path to scan for files to add to package.
                 If None, lkey will be substituted in as the path.
             meta(dict): user level metadata dict to attach to lkey directory entry.
             update_policy(str): can be either 'incoming' (default) or 'existing'.
                 If 'incoming', whenever logical keys match, always take the new entry from set_dir.
                 If 'existing', whenever logical keys match, retain existing entries
                 and ignore new entries from set_dir.
+            unversioned(bool): when True, do not retrieve VersionId for S3 physical keys.
 
         Returns:
             self
 
         Raises:
             PackageException: When `path` doesn't exist.
             ValueError: When `update_policy` is invalid.
@@ -906,18 +908,21 @@
                 root._set(logical_key, entry)
         else:
             if src.version_id is not None:
                 raise PackageException("Directories cannot have versions")
             src_path = src.path
             if src.basename() != '':
                 src_path += '/'
-            objects, _ = list_object_versions(src.bucket, src_path)
+            if not unversioned:
+                objects, _ = list_object_versions(src.bucket, src_path)
+                objects = filter(lambda obj: obj["IsLatest"], objects)
+            else:
+                objects = list_objects(src.bucket, src_path, recursive=True)
+
             for obj in objects:
-                if not obj['IsLatest']:
-                    continue
                 # Skip S3 pseduo directory files and Keys that end in /
                 if obj['Key'].endswith('/'):
                     if obj['Size'] != 0:
                         warnings.warn(f'Logical keys cannot end in "/", skipping: {obj["Key"]}')
                     continue
                 obj_pk = PhysicalKey(src.bucket, obj['Key'], obj.get('VersionId'))
                 logical_key = obj['Key'][len(src_path):]
@@ -1130,15 +1135,23 @@
         """
         yield self._meta
         for dir_key, meta in self._walk_dir_meta():
             yield {'logical_key': dir_key, 'meta': meta}
         for logical_key, entry in self.walk():
             yield {'logical_key': logical_key, **entry.as_dict()}
 
-    def set(self, logical_key, entry=None, meta=None, serialization_location=None, serialization_format_opts=None):
+    def set(
+        self,
+        logical_key,
+        entry=None,
+        meta=None,
+        serialization_location=None,
+        serialization_format_opts=None,
+        unversioned: bool = False,
+    ):
         """
         Returns self with the object at logical_key set to entry.
 
         Args:
             logical_key(string): logical key to update
             entry(PackageEntry OR string OR object): new entry to place at logical_key in the package.
                 If entry is a string, it is treated as a URL, and an entry is created based on it.
@@ -1150,25 +1163,35 @@
             serialization_format_opts(dict): Optional. If passed in, only used if entry is an object. Options to help
                 Quilt understand how the object should be serialized. Useful for underspecified file formats like csv
                 when content contains confusing characters. Will be passed as kwargs to the FormatHandler.serialize()
                 function. See docstrings for individual FormatHandlers for full list of options -
                 https://github.com/quiltdata/quilt/blob/master/api/python/quilt3/formats.py
             serialization_location(string): Optional. If passed in, only used if entry is an object. Where the
                 serialized object should be written, e.g. "./mydataframe.parquet"
+            unversioned(bool): when True, do not retrieve VersionId for S3 physical keys.
 
         Returns:
             self
         """
         return self._set(logical_key=logical_key,
                          entry=entry,
                          meta=meta,
                          serialization_location=serialization_location,
-                         serialization_format_opts=serialization_format_opts)
+                         serialization_format_opts=serialization_format_opts,
+                         unversioned=unversioned)
 
-    def _set(self, logical_key, entry=None, meta=None, serialization_location=None, serialization_format_opts=None):
+    def _set(
+        self,
+        logical_key,
+        entry=None,
+        meta=None,
+        serialization_location=None,
+        serialization_format_opts=None,
+        unversioned: bool = False,
+    ):
         if not logical_key or logical_key.endswith('/'):
             raise QuiltException(
                 f"Invalid logical key {logical_key!r}. "
                 f"A package entry logical key cannot be a directory."
             )
 
         validate_key(logical_key)
@@ -1177,15 +1200,15 @@
             entry = pathlib.Path(logical_key).resolve().as_uri()
 
         if isinstance(entry, (str, os.PathLike)):
             src = PhysicalKey.from_url(fix_url(str(entry)))
             size, version_id = get_size_and_version(src)
 
             # Determine if a new version needs to be appended.
-            if not src.is_local() and src.version_id is None and version_id is not None:
+            if not src.is_local() and src.version_id is None and version_id is not None and not unversioned:
                 src.version_id = version_id
             entry = PackageEntry(src, size, None, None)
         elif isinstance(entry, PackageEntry):
             assert meta is None
 
         elif FormatRegistry.object_is_serializable(entry):
             # Use file extension from serialization_location, fall back to file extension from logical_key
```

### Comparing `quilt3-6.0.0a1/quilt3/search_util.py` & `quilt3-6.0.0a2/quilt3/search_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/session.py` & `quilt3-6.0.0a2/quilt3/session.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/telemetry.py` & `quilt3-6.0.0a2/quilt3/telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/util.py` & `quilt3-6.0.0a2/quilt3/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,16 @@
     """
     path = pathlib.Path(yaml_path)
     now = datetime.datetime.now(datetime.timezone.utc).strftime("%Y%m%dT%H%M%S.%fZ")  # ISO 8601 'basic format'
     backup_path = path.with_name(path.name + '.backup.' + now)
 
     try:
         if path.exists():
-            path.rename(backup_path)
+            # TODO: use something from tempfile to make sure backup_path doesn't exist.
+            path.replace(backup_path)
         path.parent.mkdir(parents=True, exist_ok=True)
         with path.open('w') as config_file:
             yaml.dump(data, config_file)
     except Exception:     # intentionally wide catch -- reraised immediately.
         if backup_path.exists():
             backup_path.replace(path)
         raise
```

### Comparing `quilt3-6.0.0a1/quilt3/workflows/__init__.py` & `quilt3-6.0.0a2/quilt3/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3/workflows/config-1.schema.json` & `quilt3-6.0.0a2/quilt3/workflows/config-1.schema.json`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/quilt3.egg-info/PKG-INFO` & `quilt3-6.0.0a2/quilt3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 6.0.0a1
+Version: 6.0.0a2
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-6.0.0a1/quilt3.egg-info/SOURCES.txt` & `quilt3-6.0.0a2/quilt3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/setup.py` & `quilt3-6.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_api.py` & `quilt3-6.0.0a2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_bucket.py` & `quilt3-6.0.0a2/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_cli.py` & `quilt3-6.0.0a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_data_transfer.py` & `quilt3-6.0.0a2/tests/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_formats.py` & `quilt3-6.0.0a2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_s3clientprovider.py` & `quilt3-6.0.0a2/tests/test_s3clientprovider.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_search.py` & `quilt3-6.0.0a2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_session.py` & `quilt3-6.0.0a2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_telemetry.py` & `quilt3-6.0.0a2/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_util.py` & `quilt3-6.0.0a2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-6.0.0a1/tests/test_workflows.py` & `quilt3-6.0.0a2/tests/test_workflows.py`

 * *Files identical despite different names*

