# Comparing `tmp/dawnai-0.0.8.tar.gz` & `tmp/dawnai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawnai-0.0.8.tar", last modified: Fri Apr 12 21:35:50 2024, max compression
+gzip compressed data, was "dawnai-0.0.9.tar", last modified: Mon Apr 15 20:42:09 2024, max compression
```

## Comparing `dawnai-0.0.8.tar` & `dawnai-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:35:50.646462 dawnai-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-12 21:35:50.646462 dawnai-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 21:35:38.000000 dawnai-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:35:50.646462 dawnai-0.0.8/dawnai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:35:38.000000 dawnai-0.0.8/dawnai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-12 21:35:38.000000 dawnai-0.0.8/dawnai/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:35:50.646462 dawnai-0.0.8/dawnai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-12 21:35:50.000000 dawnai-0.0.8/dawnai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 21:35:50.000000 dawnai-0.0.8/dawnai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:35:50.000000 dawnai-0.0.8/dawnai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 21:35:50.000000 dawnai-0.0.8/dawnai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 21:35:50.000000 dawnai-0.0.8/dawnai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:35:50.646462 dawnai-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-12 21:35:38.000000 dawnai-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:35:50.646462 dawnai-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 21:35:38.000000 dawnai-0.0.8/tests/test_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:42:09.646986 dawnai-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 20:42:09.646986 dawnai-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 20:42:00.000000 dawnai-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:42:09.646986 dawnai-0.0.9/dawnai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:42:00.000000 dawnai-0.0.9/dawnai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-15 20:42:00.000000 dawnai-0.0.9/dawnai/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:42:09.646986 dawnai-0.0.9/dawnai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 20:42:09.000000 dawnai-0.0.9/dawnai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-15 20:42:09.000000 dawnai-0.0.9/dawnai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:42:09.000000 dawnai-0.0.9/dawnai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:42:09.000000 dawnai-0.0.9/dawnai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 20:42:09.000000 dawnai-0.0.9/dawnai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:42:09.646986 dawnai-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-15 20:42:00.000000 dawnai-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:42:09.646986 dawnai-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 20:42:00.000000 dawnai-0.0.9/tests/test_analytics.py
```

### Comparing `dawnai-0.0.8/PKG-INFO` & `dawnai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.8/dawnai/analytics.py` & `dawnai-0.0.9/dawnai/analytics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import time
 from typing import Union, List, Dict, Optional
 import aiohttp
+from datetime import datetime, timezone
 
 write_key = None
 api_url = "https://api.dawnai.com/"
 buffer_size = 50
 buffer_timeout = 5
 buffer = []
 flush_task = None
@@ -17,32 +18,45 @@
     asyncio.run(save_to_buffer({"type": "identify", "data": data}))
 
 
 def track(
     user_id: str,
     event: str,
     properties: Optional[Dict[str, Union[str, int, bool, float]]] = None,
+    timestamp: Optional[str] = None,
 ) -> None:
-    data = {"user_id": user_id, "event": event, "properties": properties}
+    if timestamp is None:
+        timestamp = datetime.now(timezone.utc).isoformat()
+    data = {
+        "user_id": user_id,
+        "event": event,
+        "properties": properties,
+        "timestamp": timestamp,
+    }
     asyncio.run(save_to_buffer({"type": "track", "data": data}))
 
 
 def track_ai(
     user_id: str,
     event: str,
     model: Optional[str] = None,
     user_input: Optional[str] = None,
     output: Optional[str] = None,
     convo_id: Optional[str] = None,
     properties: Optional[Dict[str, Union[str, int, bool, float]]] = None,
+    timestamp: Optional[str] = None,
 ) -> None:
+    if timestamp is None:
+        timestamp = datetime.now(timezone.utc).isoformat()
+
     data = {
         "user_id": user_id,
         "event": event,
         "properties": properties or {},
+        "timestamp": timestamp,
         "ai_data": {
             "model": model,
             "input": user_input,
             "output": output,
             "convo_id": convo_id,
         },
     }
```

### Comparing `dawnai-0.0.8/dawnai.egg-info/PKG-INFO` & `dawnai-0.0.9/dawnai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.8/setup.py` & `dawnai-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dawnai",
-    version="0.0.8",
+    version="0.0.9",
     description="Dawn (Python SDK)",
     author="Dawn",
     author_email="sdk@dawnai.com",
     long_description="For questions, email us at sdk@dawnai.com",
     long_description_content_type="text/markdown",
     url="https://dawnai.com",
     packages=find_packages(include=["dawnai", "README.md"]),
```

### Comparing `dawnai-0.0.8/tests/test_analytics.py` & `dawnai-0.0.9/tests/test_analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest.mock import patch
 import dawnai.analytics as analytics
 
 
 class TestAnalytics(unittest.TestCase):
     def setUp(self):
         # Set up any necessary test data or configurations
-        analytics.write_key = "XXXX"
+        analytics.write_key = "0000"
         analytics.debug_logs = True
 
     #  analytics.api_url = "http://localhost:3000/"
 
     def tearDown(self):
         # Clean up any resources or reset any state after each test
         pass
```

