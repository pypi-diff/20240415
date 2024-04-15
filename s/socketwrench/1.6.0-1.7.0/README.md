# Comparing `tmp/socketwrench-1.6.0.tar.gz` & `tmp/socketwrench-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.6.0.tar", last modified: Mon Apr 15 17:16:45 2024, max compression
+gzip compressed data, was "socketwrench-1.7.0.tar", last modified: Mon Apr 15 17:50:38 2024, max compression
```

## Comparing `socketwrench-1.6.0.tar` & `socketwrench-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:45.538158 socketwrench-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 17:16:41.000000 socketwrench-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:16:45.538158 socketwrench-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-15 17:16:41.000000 socketwrench-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 17:16:41.000000 socketwrench-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:16:45.538158 socketwrench-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:45.534158 socketwrench-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:45.538158 socketwrench-1.6.0/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:45.538158 socketwrench-1.6.0/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    20017 2024-04-15 17:16:41.000000 socketwrench-1.6.0/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:16:45.538158 socketwrench-1.6.0/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:16:45.000000 socketwrench-1.6.0/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-15 17:16:45.000000 socketwrench-1.6.0/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:16:45.000000 socketwrench-1.6.0/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 17:16:45.000000 socketwrench-1.6.0/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.192571 socketwrench-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 17:50:33.000000 socketwrench-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:50:38.192571 socketwrench-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-15 17:50:33.000000 socketwrench-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 17:50:33.000000 socketwrench-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:50:38.192571 socketwrench-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20017 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.6.0/LICENSE` & `socketwrench-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/PKG-INFO` & `socketwrench-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.6.0
+Version: 1.7.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.6.0/README.md` & `socketwrench-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/pyproject.toml` & `socketwrench-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.6.0"
+version = "1.7.0"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.6.0/src/socketwrench/__init__.py` & `socketwrench-1.7.0/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/__main__.py` & `socketwrench-1.7.0/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/connection.py` & `socketwrench-1.7.0/src/socketwrench/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,15 @@
             body = b''
 
         r = Request.from_components(pre_body_bytes, body, self.client_addr)
         logger.info(f"{r}")
         return r
 
     def send_response(self, connection_socket: socket.socket, response: Response):
-        # connection_socket.send(response.pre_body_bytes)
-        # connection_socket.send(response.body)
-        logger.info(f"{response}\n")
-        connection_socket.send(response)
+        connection_socket.send(bytes(response))
         connection_socket.close()
 
     def check_cleanup(self):
         if self.cleanup_event and self.cleanup_event.is_set():
             self.close()
             return True
         return False
```

### Comparing `socketwrench-1.6.0/src/socketwrench/handlers.py` & `socketwrench-1.7.0/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/openapi.py` & `socketwrench-1.7.0/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/samples/file_sample.py` & `socketwrench-1.7.0/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/samples/sample.py` & `socketwrench-1.7.0/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/server.py` & `socketwrench-1.7.0/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/tags.py` & `socketwrench-1.7.0/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench/types.py` & `socketwrench-1.7.0/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.6.0/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.7.0/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.6.0
+Version: 1.7.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.6.0/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.7.0/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*
