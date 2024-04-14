# Comparing `tmp/teslemetry_stream-0.2.2.tar.gz` & `tmp/teslemetry_stream-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teslemetry_stream-0.2.2.tar", last modified: Mon Mar 25 10:49:13 2024, max compression
+gzip compressed data, was "teslemetry_stream-0.2.3.tar", last modified: Sun Apr 14 23:57:35 2024, max compression
```

## Comparing `teslemetry_stream-0.2.2.tar` & `teslemetry_stream-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:13.647354 teslemetry_stream-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 10:49:09.000000 teslemetry_stream-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-25 10:49:13.647354 teslemetry_stream-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-25 10:49:09.000000 teslemetry_stream-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 10:49:13.647354 teslemetry_stream-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-25 10:49:09.000000 teslemetry_stream-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:13.643354 teslemetry_stream-0.2.2/teslemetry_stream/
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-03-25 10:49:09.000000 teslemetry_stream-0.2.2/teslemetry_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-25 10:49:09.000000 teslemetry_stream-0.2.2/teslemetry_stream/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:13.647354 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-25 10:49:13.000000 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-25 10:49:13.000000 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:49:13.000000 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 10:49:13.000000 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 10:49:13.000000 teslemetry_stream-0.2.2/teslemetry_stream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:57:35.967723 teslemetry_stream-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 23:57:25.000000 teslemetry_stream-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-14 23:57:35.967723 teslemetry_stream-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-14 23:57:25.000000 teslemetry_stream-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:57:35.967723 teslemetry_stream-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-14 23:57:25.000000 teslemetry_stream-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:57:35.963723 teslemetry_stream-0.2.3/teslemetry_stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-14 23:57:25.000000 teslemetry_stream-0.2.3/teslemetry_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-14 23:57:25.000000 teslemetry_stream-0.2.3/teslemetry_stream/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:57:35.967723 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-14 23:57:35.000000 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 23:57:35.000000 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:57:35.000000 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 23:57:35.000000 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 23:57:35.000000 teslemetry_stream-0.2.3/teslemetry_stream.egg-info/top_level.txt
```

### Comparing `teslemetry_stream-0.2.2/LICENSE` & `teslemetry_stream-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `teslemetry_stream-0.2.2/PKG-INFO` & `teslemetry_stream-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslemetry_stream
-Version: 0.2.2
+Version: 0.2.3
 Summary: Teslemetry Streaming API library for Python
 Home-page: https://github.com/Teslemetry/teslemetry_stream
 Author: Brett Adams
 Author-email: hello@teslemetry.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `teslemetry_stream-0.2.2/README.md` & `teslemetry_stream-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `teslemetry_stream-0.2.2/setup.py` & `teslemetry_stream-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teslemetry_stream",
-    version="0.2.2",
+    version="0.2.3",
     author="Brett Adams",
     author_email="hello@teslemetry.com",
     description="Teslemetry Streaming API library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Teslemetry/teslemetry_stream",
     packages=setuptools.find_packages(),
```

### Comparing `teslemetry_stream-0.2.2/teslemetry_stream/__init__.py` & `teslemetry_stream-0.2.3/teslemetry_stream/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
     message = "This vehicle is not configured to connect to Teslemetry."
 
 
 class TeslemetryStream:
     """Teslemetry Stream Client"""
 
-    fields: dict[TelemetryFields, dict[str, int]]
-    alerts: list[TelemetryAlerts]
+    fields: dict[TelemetryFields, dict[str, int]] | None = None
+    alerts: list[TelemetryAlerts] | None = None
     _response: aiohttp.ClientResponse | None = None
     _listeners: dict[Callable, Callable] = {}
     delay = DELAY
     active = None
 
     def __init__(
         self,
```

### Comparing `teslemetry_stream-0.2.2/teslemetry_stream/const.py` & `teslemetry_stream-0.2.3/teslemetry_stream/const.py`

 * *Files identical despite different names*

### Comparing `teslemetry_stream-0.2.2/teslemetry_stream.egg-info/PKG-INFO` & `teslemetry_stream-0.2.3/teslemetry_stream.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslemetry_stream
-Version: 0.2.2
+Version: 0.2.3
 Summary: Teslemetry Streaming API library for Python
 Home-page: https://github.com/Teslemetry/teslemetry_stream
 Author: Brett Adams
 Author-email: hello@teslemetry.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

