# Comparing `tmp/msal-extensions-1.1.0.tar.gz` & `tmp/msal_extensions-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal-extensions-1.1.0.tar", last modified: Sat Dec  9 04:12:28 2023, max compression
+gzip compressed data, was "msal_extensions-1.2.0b1.tar", last modified: Mon Apr 15 19:04:48 2024, max compression
```

## Comparing `msal-extensions-1.1.0.tar` & `msal_extensions-1.2.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 04:12:27.996491 msal-extensions-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2023-12-09 04:12:27.996491 msal-extensions-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 04:12:27.996491 msal-extensions-1.1.0/msal_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/cache_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/libsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/osx.py
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/token_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/msal_extensions/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 04:12:27.996491 msal-extensions-1.1.0/msal_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2023-12-09 04:12:27.000000 msal-extensions-1.1.0/msal_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-12-09 04:12:27.000000 msal-extensions-1.1.0/msal_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 04:12:27.000000 msal-extensions-1.1.0/msal_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-09 04:12:27.000000 msal-extensions-1.1.0/msal_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-09 04:12:27.000000 msal-extensions-1.1.0/msal_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-09 04:12:28.000491 msal-extensions-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 04:12:27.996491 msal-extensions-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_agnostic_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_cache_lock_file_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_crossplatlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_macos_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-12-09 04:12:20.000000 msal-extensions-1.1.0/tests/test_windows_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/msal_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/cache_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/libsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/osx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/msal_extensions/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/msal_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-15 19:04:48.000000 msal_extensions-1.2.0b1/msal_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 19:04:48.000000 msal_extensions-1.2.0b1/msal_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:04:48.000000 msal_extensions-1.2.0b1/msal_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:04:48.000000 msal_extensions-1.2.0b1/msal_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 19:04:48.000000 msal_extensions-1.2.0b1/msal_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:04:48.733101 msal_extensions-1.2.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_agnostic_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_cache_lock_file_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_crossplatlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_macos_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-15 19:04:29.000000 msal_extensions-1.2.0b1/tests/test_windows_backend.py
```

### Comparing `msal-extensions-1.1.0/LICENSE` & `msal_extensions-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/PKG-INFO` & `msal_extensions-1.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-extensions
-Version: 1.1.0
+Version: 1.2.0b1
 Summary: Microsoft Authentication Library extensions (MSAL EX) provides a persistence API that can save your data on disk, encrypted on Windows, macOS and Linux. Concurrent data access will be coordinated by a file lock mechanism.
 License: MIT License
 Project-URL: Changelog, https://github.com/AzureAD/microsoft-authentication-extensions-for-python/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: msal<2.0.0,>=0.4.1
-Requires-Dist: portalocker<3,>=1.0; platform_system != "Windows"
-Requires-Dist: portalocker<3,>=1.6; platform_system == "Windows"
-Requires-Dist: packaging
+Requires-Dist: msal<1.29,>=1.27
+Requires-Dist: portalocker<3,>=1.4
 
 
 # Microsoft Authentication Extensions for Python
 
 The Microsoft Authentication Extensions for Python offers secure mechanisms for client applications to perform cross-platform token cache serialization and persistence. It gives additional support to the [Microsoft Authentication Library for Python (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-python).
 
 MSAL Python supports an in-memory cache by default and provides the [SerializableTokenCache](https://msal-python.readthedocs.io/en/latest/#msal.SerializableTokenCache) to perform cache serialization. You can read more about this in the MSAL Python [documentation](https://docs.microsoft.com/en-us/azure/active-directory/develop/msal-python-token-cache-serialization). Developers are required to implement their own cache persistance across multiple platforms and Microsoft Authentication Extensions makes this simpler.
```

### Comparing `msal-extensions-1.1.0/README.md` & `msal_extensions-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/msal_extensions/cache_lock.py` & `msal_extensions-1.2.0b1/msal_extensions/cache_lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,38 @@
 import os
 import sys
 import errno
 import time
 import logging
 
 import portalocker
-from packaging.version import Version
 
 
 logger = logging.getLogger(__name__)
 
 
 class CrossPlatLock(object):
     """Offers a mechanism for waiting until another process is finished interacting with a shared
     resource. This is specifically written to interact with a class of the same name in the .NET
     extensions library.
     """
     def __init__(self, lockfile_path):
         self._lockpath = lockfile_path
-        # Support for passing through arguments to the open syscall was added in v1.4.0
-        open_kwargs = ({'buffering': 0}
-            if Version(portalocker.__version__) >= Version("1.4.0") else {})
         self._lock = portalocker.Lock(
             lockfile_path,
             mode='wb+',
             # In posix systems, we HAVE to use LOCK_EX(exclusive lock) bitwise ORed
             # with LOCK_NB(non-blocking) to avoid blocking on lock acquisition.
             # More information here:
             # https://docs.python.org/3/library/fcntl.html#fcntl.lockf
             flags=portalocker.LOCK_EX | portalocker.LOCK_NB,
-            **open_kwargs)
+            # Support for passing through arguments to the open syscall
+            # was added in Portalocker v1.4.0 (2019-02-11).
+            buffering=0,
+        )
 
     def _try_to_create_lock_file(self):
         timeout = 5
         check_interval = 0.25
         current_time = getattr(time, "monotonic", time.time)
         timeout_end = current_time() + timeout
         pid = os.getpid()
```

### Comparing `msal-extensions-1.1.0/msal_extensions/libsecret.py` & `msal_extensions-1.2.0b1/msal_extensions/libsecret.py`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/msal_extensions/osx.py` & `msal_extensions-1.2.0b1/msal_extensions/osx.py`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/msal_extensions/persistence.py` & `msal_extensions-1.2.0b1/msal_extensions/persistence.py`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/msal_extensions/token_cache.py` & `msal_extensions-1.2.0b1/msal_extensions/token_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,24 +65,24 @@
             super(PersistedTokenCache, self).modify(
                 credential_type,
                 old_entry,
                 new_key_value_pairs=new_key_value_pairs)
             self._persistence.save(self.serialize())
             self._last_sync = time.time()
 
-    def find(self, credential_type, **kwargs):  # pylint: disable=arguments-differ
+    def _find(self, credential_type, **kwargs):  # pylint: disable=arguments-differ
         # Use optimistic locking rather than CrossPlatLock(self._lock_location)
         retry = 3
         for attempt in range(1, retry + 1):
             try:
                 self._reload_if_necessary()
             except Exception:  # pylint: disable=broad-except
                 # Presumably other processes are writing the file, causing dirty read
                 if attempt < retry:
                     logger.debug("Unable to load token cache file in No. %d attempt", attempt)
                     time.sleep(0.5)
                 else:
                     raise  # End of retry. Re-raise the exception as-is.
             else:  # If reload encountered no error, the data is considered intact
-                return super(PersistedTokenCache, self).find(credential_type, **kwargs)
+                return super(PersistedTokenCache, self)._find(credential_type, **kwargs)
         return []  # Not really reachable here. Just to keep pylint happy.
```

### Comparing `msal-extensions-1.1.0/msal_extensions/windows.py` & `msal_extensions-1.2.0b1/msal_extensions/windows.py`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/msal_extensions.egg-info/PKG-INFO` & `msal_extensions-1.2.0b1/msal_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-extensions
-Version: 1.1.0
+Version: 1.2.0b1
 Summary: Microsoft Authentication Library extensions (MSAL EX) provides a persistence API that can save your data on disk, encrypted on Windows, macOS and Linux. Concurrent data access will be coordinated by a file lock mechanism.
 License: MIT License
 Project-URL: Changelog, https://github.com/AzureAD/microsoft-authentication-extensions-for-python/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: msal<2.0.0,>=0.4.1
-Requires-Dist: portalocker<3,>=1.0; platform_system != "Windows"
-Requires-Dist: portalocker<3,>=1.6; platform_system == "Windows"
-Requires-Dist: packaging
+Requires-Dist: msal<1.29,>=1.27
+Requires-Dist: portalocker<3,>=1.4
 
 
 # Microsoft Authentication Extensions for Python
 
 The Microsoft Authentication Extensions for Python offers secure mechanisms for client applications to perform cross-platform token cache serialization and persistence. It gives additional support to the [Microsoft Authentication Library for Python (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-python).
 
 MSAL Python supports an in-memory cache by default and provides the [SerializableTokenCache](https://msal-python.readthedocs.io/en/latest/#msal.SerializableTokenCache) to perform cache serialization. You can read more about this in the MSAL Python [documentation](https://docs.microsoft.com/en-us/azure/active-directory/develop/msal-python-token-cache-serialization). Developers are required to implement their own cache persistance across multiple platforms and Microsoft Authentication Extensions makes this simpler.
```

### Comparing `msal-extensions-1.1.0/msal_extensions.egg-info/SOURCES.txt` & `msal_extensions-1.2.0b1/msal_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/setup.cfg` & `msal_extensions-1.2.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/tests/test_agnostic_backend.py` & `msal_extensions-1.2.0b1/tests/test_agnostic_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,39 +11,35 @@
 
 @pytest.fixture
 def temp_location():
     test_folder = tempfile.mkdtemp(prefix="test_token_cache_roundtrip")
     yield os.path.join(test_folder, 'token_cache.bin')
     shutil.rmtree(test_folder, ignore_errors=True)
 
-
-def _test_token_cache_roundtrip(cache):
+def _test_token_cache_roundtrip(persistence):
     client_id = os.getenv('AZURE_CLIENT_ID')
     client_secret = os.getenv('AZURE_CLIENT_SECRET')
     if not (client_id and client_secret):
         pytest.skip('no credentials present to test TokenCache round-trip with.')
 
-    app = msal.ConfidentialClientApplication(
-        client_id=client_id,
-        client_credential=client_secret,
-        token_cache=cache)
     desired_scopes = ['https://graph.microsoft.com/.default']
-    token1 = app.acquire_token_for_client(scopes=desired_scopes)
-    os.utime(  # Mock having another process update the cache
-        cache._persistence.get_location(), None)
-    token2 = app.acquire_token_silent(scopes=desired_scopes, account=None)
-    assert token1['access_token'] == token2['access_token']
-
-def test_file_token_cache_roundtrip(temp_location):
-    _test_token_cache_roundtrip(PersistedTokenCache(FilePersistence(temp_location)))
+    apps = [  # Multiple apps sharing same persistence
+        msal.ConfidentialClientApplication(
+        client_id, client_credential=client_secret,
+        token_cache=PersistedTokenCache(persistence)) for i in range(2)]
+    token1 = apps[0].acquire_token_for_client(scopes=desired_scopes)
+    assert token1["token_source"] == "identity_provider", "Initial token should come from IdP"
+    token2 = apps[1].acquire_token_for_client(scopes=desired_scopes)  # Hit token cache in MSAL 1.23+
+    assert token2["token_source"] == "cache", "App2 should hit cache written by app1"
+    assert token1['access_token'] == token2['access_token'], "Cache should hit"
 
-def test_current_platform_cache_roundtrip_with_persistence_builder(temp_location):
-    _test_token_cache_roundtrip(PersistedTokenCache(build_encrypted_persistence(temp_location)))
+def test_token_cache_roundtrip_with_persistence_biulder(temp_location):
+    _test_token_cache_roundtrip(build_encrypted_persistence(temp_location))
 
-def test_persisted_token_cache(temp_location):
-    _test_token_cache_roundtrip(PersistedTokenCache(FilePersistence(temp_location)))
+def test_token_cache_roundtrip_with_file_persistence(temp_location):
+    _test_token_cache_roundtrip(FilePersistence(temp_location))
 
 def test_file_not_found_error_is_not_raised():
     persistence = FilePersistence('non_existing_file')
     cache = PersistedTokenCache(persistence)
     # An exception raised here will fail the test case as it is supposed to be a NO-OP
     cache.find('')
```

### Comparing `msal-extensions-1.1.0/tests/test_cache_lock_file_perf.py` & `msal_extensions-1.2.0b1/tests/test_cache_lock_file_perf.py`

 * *Files identical despite different names*

### Comparing `msal-extensions-1.1.0/tests/test_macos_backend.py` & `msal_extensions-1.2.0b1/tests/test_macos_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,12 +35,13 @@
         subject = PersistedTokenCache(KeychainPersistence(cache_file))
         app = msal.ConfidentialClientApplication(
             client_id=client_id,
             client_credential=client_secret,
             token_cache=subject)
         desired_scopes = ['https://graph.microsoft.com/.default']
         token1 = app.acquire_token_for_client(scopes=desired_scopes)
+        # TODO: Modify this to same approach in test_agnostic_backend.py
         os.utime(cache_file, None)  # Mock having another process update the cache.
         token2 = app.acquire_token_silent(scopes=desired_scopes, account=None)
         assert token1['access_token'] == token2['access_token']
     finally:
         shutil.rmtree(test_folder, ignore_errors=True)
```

### Comparing `msal-extensions-1.1.0/tests/test_persistence.py` & `msal_extensions-1.2.0b1/tests/test_persistence.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     # string conditions and then raise an undefined "true" exception.
     # https://docs.pytest.org/en/latest/historical-notes.html#string-conditions
         os.getenv(env_var))
 
 
 # Note: If you use tox, remember to pass them through via tox.ini
 # https://tox.wiki/en/latest/example/basic.html#passing-down-environment-variables
-is_running_on_travis_ci = _is_env_var_defined("TRAVIS")
 is_running_on_github_ci = _is_env_var_defined("GITHUB_ACTIONS")
 
 @pytest.fixture
 def temp_location():
     test_folder = tempfile.mkdtemp(prefix="test_persistence_roundtrip")
     yield os.path.join(test_folder, 'persistence.bin')
     shutil.rmtree(test_folder, ignore_errors=True)
@@ -42,53 +41,53 @@
 def test_file_persistence(temp_location):
     _test_persistence_roundtrip(FilePersistence(temp_location))
 
 def test_nonexistent_file_persistence(temp_location):
     _test_nonexistent_persistence(FilePersistence(temp_location))
 
 @pytest.mark.skipif(
-    is_running_on_travis_ci or not sys.platform.startswith('win'),
+    not sys.platform.startswith('win'),
     reason="Requires Windows Desktop")
 def test_file_persistence_with_data_protection(temp_location):
     try:
         _test_persistence_roundtrip(FilePersistenceWithDataProtection(temp_location))
     except PersistenceDecryptionError:
-        if is_running_on_github_ci or is_running_on_travis_ci:
+        if is_running_on_github_ci:
             logging.warning("DPAPI tends to fail on Windows VM. Run this on your desktop to double check.")
         else:
             raise
 
 @pytest.mark.skipif(
-    is_running_on_travis_ci or not sys.platform.startswith('win'),
+    not sys.platform.startswith('win'),
     reason="Requires Windows Desktop")
 def test_nonexistent_file_persistence_with_data_protection(temp_location):
     _test_nonexistent_persistence(FilePersistenceWithDataProtection(temp_location))
 
 @pytest.mark.skipif(
     not sys.platform.startswith('darwin'),
-    reason="Requires OSX. Whether running on TRAVIS CI does not seem to matter.")
+    reason="Requires OSX.")
 def test_keychain_persistence(temp_location):
     _test_persistence_roundtrip(KeychainPersistence(temp_location))
 
 @pytest.mark.skipif(
     not sys.platform.startswith('darwin'),
-    reason="Requires OSX. Whether running on TRAVIS CI does not seem to matter.")
+    reason="Requires OSX.")
 def test_nonexistent_keychain_persistence(temp_location):
     random_service_name = random_account_name = str(id(temp_location))
     _test_nonexistent_persistence(
         KeychainPersistence(temp_location, random_service_name, random_account_name))
 
 @pytest.mark.skipif(
-    is_running_on_travis_ci or not sys.platform.startswith('linux'),
+    not sys.platform.startswith('linux'),
     reason="Requires Linux Desktop. Headless or SSH session won't work.")
 def test_libsecret_persistence(temp_location):
     _test_persistence_roundtrip(LibsecretPersistence(temp_location))
 
 @pytest.mark.skipif(
-    is_running_on_travis_ci or not sys.platform.startswith('linux'),
+    not sys.platform.startswith('linux'),
     reason="Requires Linux Desktop. Headless or SSH session won't work.")
 def test_nonexistent_libsecret_persistence(temp_location):
     random_schema_name = random_value = str(id(temp_location))
     _test_nonexistent_persistence(LibsecretPersistence(
         temp_location,
         random_schema_name,
         {"my_attr_1": random_value, "my_attr_2": random_value},
```

### Comparing `msal-extensions-1.1.0/tests/test_windows_backend.py` & `msal_extensions-1.2.0b1/tests/test_windows_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,32 +23,26 @@
         '',
         'lorem ipsum',
         'lorem-ipsum',
         '<Python>',
         uuid.uuid4().hex,
     ]
 
-    try:
-        for tc in test_cases:
-            ciphered = subject_with_entropy.protect(tc)
-            assert ciphered != tc
-
-            got = subject_with_entropy.unprotect(ciphered)
-            assert got == tc
-
-            ciphered = subject_without_entropy.protect(tc)
-            assert ciphered != tc
-
-            got = subject_without_entropy.unprotect(ciphered)
-            assert got == tc
-    except OSError as exp:
-        if exp.errno == errno.EIO and os.getenv('TRAVIS_REPO_SLUG'):
-            pytest.skip('DPAPI tests are known to fail in TravisCI. This effort tracked by '
-                        'https://github.com/AzureAD/microsoft-authentication-extentions-for-python'
-                        '/issues/21')
+    for tc in test_cases:
+        ciphered = subject_with_entropy.protect(tc)
+        assert ciphered != tc
+
+        got = subject_with_entropy.unprotect(ciphered)
+        assert got == tc
+
+        ciphered = subject_without_entropy.protect(tc)
+        assert ciphered != tc
+
+        got = subject_without_entropy.unprotect(ciphered)
+        assert got == tc
 
 
 def test_read_msal_cache_direct():
     """
     This loads and unprotects an MSAL cache directly, only using the DataProtectionAgent.
     """
     localappdata_location = os.getenv('LOCALAPPDATA', os.path.expanduser('~'))
@@ -95,12 +89,13 @@
         subject = PersistedTokenCache(FilePersistenceWithDataProtection(cache_file))
         app = msal.ConfidentialClientApplication(
             client_id=client_id,
             client_credential=client_secret,
             token_cache=subject)
         desired_scopes = ['https://graph.microsoft.com/.default']
         token1 = app.acquire_token_for_client(scopes=desired_scopes)
+        # TODO: Modify this to same approach in test_agnostic_backend.py
         os.utime(cache_file, None)  # Mock having another process update the cache.
         token2 = app.acquire_token_silent(scopes=desired_scopes, account=None)
         assert token1['access_token'] == token2['access_token']
     finally:
         shutil.rmtree(test_folder, ignore_errors=True)
```

