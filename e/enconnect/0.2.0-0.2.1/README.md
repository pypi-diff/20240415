# Comparing `tmp/enconnect-0.2.0.tar.gz` & `tmp/enconnect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enconnect-0.2.0.tar", last modified: Sun Apr 14 14:02:55 2024, max compression
+gzip compressed data, was "enconnect-0.2.1.tar", last modified: Mon Apr 15 09:04:20 2024, max compression
```

## Comparing `enconnect-0.2.0.tar` & `enconnect-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.678237 enconnect-0.2.0/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.2.0/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.2.0/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-14 14:02:55.678237 enconnect-0.2.0/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2363 2024-04-14 13:59:58.000000 enconnect-0.2.0/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.676237 enconnect-0.2.0/enconnect/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.2.0/enconnect/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.676237 enconnect-0.2.0/enconnect/instagram/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.2.0/enconnect/instagram/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3795 2024-04-14 10:58:49.000000 enconnect-0.2.0/enconnect/instagram/instagram.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      982 2024-04-12 05:18:12.000000 enconnect-0.2.0/enconnect/instagram/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/instagram/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.2.0/enconnect/instagram/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1829 2024-04-14 12:42:07.000000 enconnect-0.2.0/enconnect/instagram/test/test_instagram.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.2.0/enconnect/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.2.0/enconnect/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.2.0/enconnect/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.2.0/enconnect/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1706 2024-04-14 12:33:25.000000 enconnect-0.2.0/enconnect/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.2.0/enconnect/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/reddit/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.2.0/enconnect/reddit/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      954 2024-04-13 10:48:48.000000 enconnect-0.2.0/enconnect/reddit/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4027 2024-04-14 10:58:51.000000 enconnect-0.2.0/enconnect/reddit/reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/reddit/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.2.0/enconnect/reddit/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1614 2024-04-14 12:33:27.000000 enconnect-0.2.0/enconnect/reddit/test/test_reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.2.0/enconnect/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.2.0/enconnect/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4190 2024-04-14 11:28:40.000000 enconnect-0.2.0/enconnect/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.2.0/enconnect/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2132 2024-04-14 12:19:57.000000 enconnect-0.2.0/enconnect/ubiquiti/test/test_router.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-14 13:59:38.000000 enconnect-0.2.0/enconnect/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/youtube/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.2.0/enconnect/youtube/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      979 2024-04-12 06:47:27.000000 enconnect-0.2.0/enconnect/youtube/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect/youtube/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.2.0/enconnect/youtube/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1860 2024-04-14 12:51:08.000000 enconnect-0.2.0/enconnect/youtube/test/test_youtube.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4866 2024-04-14 10:58:45.000000 enconnect-0.2.0/enconnect/youtube/youtube.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 14:02:55.677237 enconnect-0.2.0/enconnect.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-14 14:02:55.000000 enconnect-0.2.0/enconnect.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1126 2024-04-14 14:02:55.000000 enconnect-0.2.0/enconnect.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-14 14:02:55.000000 enconnect-0.2.0/enconnect.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-14 14:02:55.000000 enconnect-0.2.0/enconnect.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-04-14 14:02:55.000000 enconnect-0.2.0/enconnect.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.2.0/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-08 22:20:24.000000 enconnect-0.2.0/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      305 2024-04-14 14:02:55.678237 enconnect-0.2.0/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.743415 enconnect-0.2.1/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.2.1/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.2.1/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-15 09:04:20.743415 enconnect-0.2.1/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2363 2024-04-14 13:59:58.000000 enconnect-0.2.1/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.741416 enconnect-0.2.1/enconnect/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.2.1/enconnect/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/instagram/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.2.1/enconnect/instagram/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3795 2024-04-14 10:58:49.000000 enconnect-0.2.1/enconnect/instagram/instagram.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      982 2024-04-12 05:18:12.000000 enconnect-0.2.1/enconnect/instagram/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/instagram/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.2.1/enconnect/instagram/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1896 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/instagram/test/test_instagram.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.2.1/enconnect/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.2.1/enconnect/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.2.1/enconnect/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.2.1/enconnect/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.2.1/enconnect/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/reddit/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.2.1/enconnect/reddit/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      954 2024-04-13 10:48:48.000000 enconnect-0.2.1/enconnect/reddit/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4027 2024-04-14 10:58:51.000000 enconnect-0.2.1/enconnect/reddit/reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/reddit/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.2.1/enconnect/reddit/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1681 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/reddit/test/test_reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.2.1/enconnect/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.2.1/enconnect/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4256 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.2.1/enconnect/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/ubiquiti/test/test_router.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-15 09:02:02.000000 enconnect-0.2.1/enconnect/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/youtube/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.2.1/enconnect/youtube/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      979 2024-04-12 06:47:27.000000 enconnect-0.2.1/enconnect/youtube/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect/youtube/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.2.1/enconnect/youtube/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1927 2024-04-15 09:01:50.000000 enconnect-0.2.1/enconnect/youtube/test/test_youtube.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4866 2024-04-14 10:58:45.000000 enconnect-0.2.1/enconnect/youtube/youtube.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 09:04:20.742416 enconnect-0.2.1/enconnect.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-15 09:04:20.000000 enconnect-0.2.1/enconnect.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1126 2024-04-15 09:04:20.000000 enconnect-0.2.1/enconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-15 09:04:20.000000 enconnect-0.2.1/enconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-15 09:04:20.000000 enconnect-0.2.1/enconnect.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-04-15 09:04:20.000000 enconnect-0.2.1/enconnect.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.2.1/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-08 22:20:24.000000 enconnect-0.2.1/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      305 2024-04-15 09:04:20.743415 enconnect-0.2.1/setup.cfg
```

### Comparing `enconnect-0.2.0/LICENSE` & `enconnect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/PKG-INFO` & `enconnect-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enconnect-0.2.0/README.md` & `enconnect-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/__init__.py` & `enconnect-0.2.1/enconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/instagram/instagram.py` & `enconnect-0.2.1/enconnect/instagram/instagram.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/instagram/params.py` & `enconnect-0.2.1/enconnect/instagram/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/instagram/test/test_instagram.py` & `enconnect-0.2.1/enconnect/instagram/test/test_instagram.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from encommon import ENPYRWS
+from encommon.types import inrepr
+from encommon.types import instr
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
@@ -34,21 +36,23 @@
 
     attrs = list(social.__dict__)
 
     assert attrs == [
         '_Instagram__params']
 
 
-    assert 1 <= repr(social).find(
-        'instagram.Instagram object')
+    assert inrepr(
+        'instagram.Instagram object',
+        social)
 
     assert hash(social) > 0
 
-    assert 1 <= str(social).find(
-        'instagram.Instagram object')
+    assert instr(
+        'instagram.Instagram object',
+        social)
 
 
     assert social.params is params
 
 
     def _mocker_media() -> None:
```

### Comparing `enconnect-0.2.0/enconnect/philipshue/bridge.py` & `enconnect-0.2.1/enconnect/philipshue/bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/philipshue/params.py` & `enconnect-0.2.1/enconnect/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/philipshue/test/test_bridge.py` & `enconnect-0.2.1/enconnect/philipshue/test/test_bridge.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from encommon import ENPYRWS
+from encommon.types import inrepr
+from encommon.types import instr
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
@@ -34,21 +36,23 @@
 
     attrs = list(bridge.__dict__)
 
     assert attrs == [
         '_Bridge__params']
 
 
-    assert 1 <= repr(bridge).find(
-        'bridge.Bridge object')
+    assert inrepr(
+        'bridge.Bridge object',
+        bridge)
 
     assert hash(bridge) > 0
 
-    assert 1 <= str(bridge).find(
-        'bridge.Bridge object')
+    assert instr(
+        'bridge.Bridge object',
+        bridge)
 
 
     assert bridge.params is params
 
 
     def _mocker_resource() -> None:
```

### Comparing `enconnect-0.2.0/enconnect/reddit/params.py` & `enconnect-0.2.1/enconnect/reddit/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/reddit/reddit.py` & `enconnect-0.2.1/enconnect/reddit/reddit.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/reddit/test/test_reddit.py` & `enconnect-0.2.1/enconnect/reddit/test/test_reddit.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from encommon import ENPYRWS
+from encommon.types import inrepr
+from encommon.types import instr
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
@@ -32,21 +34,23 @@
 
     attrs = list(social.__dict__)
 
     assert attrs == [
         '_Reddit__params']
 
 
-    assert 1 <= repr(social).find(
-        'reddit.Reddit object')
+    assert inrepr(
+        'reddit.Reddit object',
+        social)
 
     assert hash(social) > 0
 
-    assert 1 <= str(social).find(
-        'reddit.Reddit object')
+    assert instr(
+        'reddit.Reddit object',
+        social)
 
 
     assert social.params is params
 
 
     def _mocker_new() -> None:
```

### Comparing `enconnect-0.2.0/enconnect/ubiquiti/params.py` & `enconnect-0.2.1/enconnect/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/ubiquiti/router.py` & `enconnect-0.2.1/enconnect/ubiquiti/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,19 +77,23 @@
 
         params = self.params
 
         payload = {
             'username': params.username,
             'password': params.password}
 
-        return self.request(
+        response = self.request(
             method='post',
             path='api/auth/login',
             json=payload)
 
+        response.raise_for_status()
+
+        return response
+
 
     def request(
         self,
         method: str,
         path: str,
         params: Optional[dict[str, Any]] = None,
         json: Optional[dict[str, Any]] = None,
```

### Comparing `enconnect-0.2.0/enconnect/ubiquiti/test/test_router.py` & `enconnect-0.2.1/enconnect/ubiquiti/test/test_router.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from encommon import ENPYRWS
+from encommon.types import inrepr
+from encommon.types import instr
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
@@ -36,21 +38,23 @@
     attrs = list(router.__dict__)
 
     assert attrs == [
         '_Router__params',
         '_Router__session']
 
 
-    assert 1 <= repr(router).find(
-        'router.Router object')
+    assert inrepr(
+        'router.Router object',
+        router)
 
     assert hash(router) > 0
 
-    assert 1 <= str(router).find(
-        'router.Router object')
+    assert instr(
+        'router.Router object',
+        router)
 
 
     assert router.params is params
 
     assert router.session is not None
```

### Comparing `enconnect-0.2.0/enconnect/youtube/params.py` & `enconnect-0.2.1/enconnect/youtube/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect/youtube/test/test_youtube.py` & `enconnect-0.2.1/enconnect/youtube/test/test_youtube.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from encommon import ENPYRWS
+from encommon.types import inrepr
+from encommon.types import instr
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
@@ -33,21 +35,23 @@
 
     attrs = list(social.__dict__)
 
     assert attrs == [
         '_YouTube__params']
 
 
-    assert 1 <= repr(social).find(
-        'youtube.YouTube object')
+    assert inrepr(
+        'youtube.YouTube object',
+        social)
 
     assert hash(social) > 0
 
-    assert 1 <= str(social).find(
-        'youtube.YouTube object')
+    assert instr(
+        'youtube.YouTube object',
+        social)
 
 
     assert social.params is params
 
 
     def _mocker_search() -> None:
```

### Comparing `enconnect-0.2.0/enconnect/youtube/youtube.py` & `enconnect-0.2.1/enconnect/youtube/youtube.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/enconnect.egg-info/PKG-INFO` & `enconnect-0.2.1/enconnect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enconnect-0.2.0/enconnect.egg-info/SOURCES.txt` & `enconnect-0.2.1/enconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.0/pyproject.toml` & `enconnect-0.2.1/pyproject.toml`

 * *Files identical despite different names*

