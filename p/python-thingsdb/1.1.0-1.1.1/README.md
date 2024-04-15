# Comparing `tmp/python-thingsdb-1.1.0.tar.gz` & `tmp/python-thingsdb-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-thingsdb-1.1.0.tar", last modified: Wed Apr 10 11:13:21 2024, max compression
+gzip compressed data, was "python-thingsdb-1.1.1.tar", last modified: Mon Apr 15 12:07:51 2024, max compression
```

## Comparing `python-thingsdb-1.1.0.tar` & `python-thingsdb-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      679 2024-01-26 11:10:22.000000 python-thingsdb-1.1.0/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)      119 2021-09-14 09:36:12.000000 python-thingsdb-1.1.0/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)     1066 2019-12-20 12:14:05.000000 python-thingsdb-1.1.0/LICENSE
--rw-r--r--   0 joente    (1000) joente    (1000)    18778 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)    18022 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/examples/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/examples/bookstore/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3377 2022-02-23 09:48:18.000000 python-thingsdb-1.1.0/examples/bookstore/webserver.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/python_thingsdb.egg-info/
--rw-r--r--   0 joente    (1000) joente    (1000)    18778 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      741 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       20 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        9 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       59 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2023-02-10 12:47:09.000000 python-thingsdb-1.1.0/setup.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      776 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/test_thingsdb.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/
--rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.1.0/thingsdb/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/client/
--rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.1.0/thingsdb/client/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    16343 2024-01-26 11:10:22.000000 python-thingsdb-1.1.0/thingsdb/client/buildin.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    25656 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/client.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2247 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    11933 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.1.0/thingsdb/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/room/
--rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/room/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/room/event.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.1.0/thingsdb/room/room.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8704 2023-07-20 17:58:48.000000 python-thingsdb-1.1.0/thingsdb/room/roombase.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/thingsdb/util/
--rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.1.0/thingsdb/util/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/util/access.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.1.0/thingsdb/util/cleancode.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/util/cnscope.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      501 2023-07-20 17:58:21.000000 python-thingsdb-1.1.0/thingsdb/util/id.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.485545 python-thingsdb-1.1.1/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.485545 python-thingsdb-1.1.1/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      679 2024-01-26 11:10:22.000000 python-thingsdb-1.1.1/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)      119 2021-09-14 09:36:12.000000 python-thingsdb-1.1.1/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1066 2019-12-20 12:14:05.000000 python-thingsdb-1.1.1/LICENSE
+-rw-r--r--   0 joente    (1000) joente    (1000)    19059 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)    18303 2024-04-15 12:05:24.000000 python-thingsdb-1.1.1/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.485545 python-thingsdb-1.1.1/examples/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.485545 python-thingsdb-1.1.1/examples/bookstore/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3377 2022-02-23 09:48:18.000000 python-thingsdb-1.1.1/examples/bookstore/webserver.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/python_thingsdb.egg-info/
+-rw-r--r--   0 joente    (1000) joente    (1000)    19059 2024-04-15 12:07:51.000000 python-thingsdb-1.1.1/python_thingsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      741 2024-04-15 12:07:51.000000 python-thingsdb-1.1.1/python_thingsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-04-15 12:07:51.000000 python-thingsdb-1.1.1/python_thingsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       20 2024-04-15 12:07:51.000000 python-thingsdb-1.1.1/python_thingsdb.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        9 2024-04-15 12:07:51.000000 python-thingsdb-1.1.1/python_thingsdb.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       59 2024-04-10 11:12:35.000000 python-thingsdb-1.1.1/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2023-02-10 12:47:09.000000 python-thingsdb-1.1.1/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      776 2024-04-10 11:12:35.000000 python-thingsdb-1.1.1/test_thingsdb.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/thingsdb/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.1.1/thingsdb/__init__.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/thingsdb/client/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.1.1/thingsdb/client/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    16343 2024-01-26 11:10:22.000000 python-thingsdb-1.1.1/thingsdb/client/buildin.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    26023 2024-04-15 12:05:43.000000 python-thingsdb-1.1.1/thingsdb/client/client.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2247 2024-04-10 11:12:35.000000 python-thingsdb-1.1.1/thingsdb/client/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    11933 2024-04-10 11:12:35.000000 python-thingsdb-1.1.1/thingsdb/client/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.1.1/thingsdb/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/thingsdb/room/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.1.1/thingsdb/room/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.1.1/thingsdb/room/event.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.1.1/thingsdb/room/room.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8704 2023-07-20 17:58:48.000000 python-thingsdb-1.1.1/thingsdb/room/roombase.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-15 12:07:51.489545 python-thingsdb-1.1.1/thingsdb/util/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.1.1/thingsdb/util/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.1.1/thingsdb/util/access.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.1.1/thingsdb/util/cleancode.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.1.1/thingsdb/util/cnscope.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      501 2023-07-20 17:58:21.000000 python-thingsdb-1.1.1/thingsdb/util/id.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2024-04-15 12:05:51.000000 python-thingsdb-1.1.1/thingsdb/version.py
```

### Comparing `python-thingsdb-1.1.0/.github/workflows/ci.yml` & `python-thingsdb-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/LICENSE` & `python-thingsdb-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/PKG-INFO` & `python-thingsdb-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-thingsdb
-Version: 1.1.0
+Version: 1.1.1
 Summary: ThingsDB Connector
 Home-page: https://github.com/thingsdb/python-thingsdb
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: MIT
 Keywords: database connector
 Classifier: Development Status :: 4 - Beta
@@ -333,14 +333,15 @@
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
+        skip_strip_code: bool = False,
         **kwargs: Any
 ) -> asyncio.Future
 ```
 
 Query ThingsDB.
 
 Use this method to run `code` in a scope.
@@ -353,14 +354,18 @@
     Run the code in this scope. If not specified, the default scope
     will be used. See https://docs.thingsdb.net/v0/overview/scopes/
     for how to format a scope.
 - *timeout (int, optional)*:
     Raise a time-out exception if no response is received within X
     seconds. If no time-out is given, the client will wait forever.
     Defaults to `None`.
+- *skip_strip_code (bool, optional)*:
+    This can be set to `True` which can be helpful when line numbers
+    in syntax errors need to match. When `False`, the code will be
+    stripped from white-space and comments to reduce the code size.
 - *\*\*kwargs (any, optional)*:
     Can be used to inject variable into the ThingsDB code.
 
 #### Examples
 
 Although we could just as easy have wrote everything in the
 ThingsDB code itself, this example shows how to use **kwargs for
```

### Comparing `python-thingsdb-1.1.0/README.md` & `python-thingsdb-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
+        skip_strip_code: bool = False,
         **kwargs: Any
 ) -> asyncio.Future
 ```
 
 Query ThingsDB.
 
 Use this method to run `code` in a scope.
@@ -331,14 +332,18 @@
     Run the code in this scope. If not specified, the default scope
     will be used. See https://docs.thingsdb.net/v0/overview/scopes/
     for how to format a scope.
 - *timeout (int, optional)*:
     Raise a time-out exception if no response is received within X
     seconds. If no time-out is given, the client will wait forever.
     Defaults to `None`.
+- *skip_strip_code (bool, optional)*:
+    This can be set to `True` which can be helpful when line numbers
+    in syntax errors need to match. When `False`, the code will be
+    stripped from white-space and comments to reduce the code size.
 - *\*\*kwargs (any, optional)*:
     Can be used to inject variable into the ThingsDB code.
 
 #### Examples
 
 Although we could just as easy have wrote everything in the
 ThingsDB code itself, this example shows how to use **kwargs for
```

### Comparing `python-thingsdb-1.1.0/examples/bookstore/webserver.py` & `python-thingsdb-1.1.1/examples/bookstore/webserver.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/python_thingsdb.egg-info/PKG-INFO` & `python-thingsdb-1.1.1/python_thingsdb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-thingsdb
-Version: 1.1.0
+Version: 1.1.1
 Summary: ThingsDB Connector
 Home-page: https://github.com/thingsdb/python-thingsdb
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: MIT
 Keywords: database connector
 Classifier: Development Status :: 4 - Beta
@@ -333,14 +333,15 @@
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
+        skip_strip_code: bool = False,
         **kwargs: Any
 ) -> asyncio.Future
 ```
 
 Query ThingsDB.
 
 Use this method to run `code` in a scope.
@@ -353,14 +354,18 @@
     Run the code in this scope. If not specified, the default scope
     will be used. See https://docs.thingsdb.net/v0/overview/scopes/
     for how to format a scope.
 - *timeout (int, optional)*:
     Raise a time-out exception if no response is received within X
     seconds. If no time-out is given, the client will wait forever.
     Defaults to `None`.
+- *skip_strip_code (bool, optional)*:
+    This can be set to `True` which can be helpful when line numbers
+    in syntax errors need to match. When `False`, the code will be
+    stripped from white-space and comments to reduce the code size.
 - *\*\*kwargs (any, optional)*:
     Can be used to inject variable into the ThingsDB code.
 
 #### Examples
 
 Although we could just as easy have wrote everything in the
 ThingsDB code itself, this example shows how to use **kwargs for
```

### Comparing `python-thingsdb-1.1.0/python_thingsdb.egg-info/SOURCES.txt` & `python-thingsdb-1.1.1/python_thingsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/setup.py` & `python-thingsdb-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/test_thingsdb.py` & `python-thingsdb-1.1.1/test_thingsdb.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/client/buildin.py` & `python-thingsdb-1.1.1/thingsdb/client/buildin.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/client/client.py` & `python-thingsdb-1.1.1/thingsdb/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,15 @@
         await self._authenticate(timeout)
 
     def query(
             self,
             code: str,
             scope: Optional[str] = None,
             timeout: Optional[int] = None,
+            skip_strip_code: bool = False,
             **kwargs: Any
     ) -> asyncio.Future:
         """Query ThingsDB.
 
         Use this method to run `code` in a scope.
 
         Args:
@@ -307,14 +308,18 @@
                 Run the code in this scope. If not specified, the default scope
                 will be used. See https://docs.thingsdb.net/v0/overview/scopes/
                 for how to format a scope.
             timeout (int, optional):
                 Raise a time-out exception if no response is received within X
                 seconds. If no time-out is given, the client will wait forever.
                 Defaults to `None`.
+            skip_strip_code (bool, optional):
+                This can be set to True which can be helpful when line numbers
+                in syntax errors need to match. When False, the code will be
+                stripped from white-space and comments to reduce the code size.
             **kwargs (any, optional):
                 Can be used to inject variable into the ThingsDB code.
 
         Examples:
             Although we could just as easy have wrote everything in the
             ThingsDB code itself, this example shows how to use **kwargs for
             injecting variable into code. In this case the variable `book`.
@@ -333,15 +338,17 @@
             exception will be translated to a Python Exception which will be
             raised. See thingsdb.exceptions for all possible exceptions and
             https://docs.thingsdb.net/v0/errors/ for info on the error codes.
         """
         if scope is None:
             scope = self._scope
 
-        code = strip_code(code)
+        if skip_strip_code is False:
+            code = strip_code(code)
+
         data = [scope, code]
         if kwargs:
             data.append(kwargs)
 
         return self._write_pkg(Proto.REQ_QUERY, data, timeout=timeout)
 
     async def _ensure_write(
```

### Comparing `python-thingsdb-1.1.0/thingsdb/client/package.py` & `python-thingsdb-1.1.1/thingsdb/client/package.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/client/protocol.py` & `python-thingsdb-1.1.1/thingsdb/client/protocol.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/exceptions.py` & `python-thingsdb-1.1.1/thingsdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/room/room.py` & `python-thingsdb-1.1.1/thingsdb/room/room.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/room/roombase.py` & `python-thingsdb-1.1.1/thingsdb/room/roombase.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.1.0/thingsdb/util/cnscope.py` & `python-thingsdb-1.1.1/thingsdb/util/cnscope.py`

 * *Files identical despite different names*

