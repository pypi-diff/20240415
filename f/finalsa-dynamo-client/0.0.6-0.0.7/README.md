# Comparing `tmp/finalsa-dynamo-client-0.0.6.tar.gz` & `tmp/finalsa_dynamo_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-dynamo-client-0.0.6.tar", last modified: Sat Mar 30 05:51:04 2024, max compression
+gzip compressed data, was "finalsa_dynamo_client-0.0.7.tar", last modified: Mon Apr 15 03:57:43 2024, max compression
```

## Comparing `finalsa-dynamo-client-0.0.6.tar` & `finalsa_dynamo_client-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.524350 finalsa-dynamo-client-0.0.6/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.524350 finalsa-dynamo-client-0.0.6/finalsa/dynamo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.524350 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.524350 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 05:51:04.000000 finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:51:04.528349 finalsa-dynamo-client-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-30 05:51:00.000000 finalsa-dynamo-client-0.0.6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.592161 finalsa_dynamo_client-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 03:57:43.592161 finalsa_dynamo_client-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.584161 finalsa_dynamo_client-0.0.7/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.584161 finalsa_dynamo_client-0.0.7/finalsa/dynamo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.588161 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.588161 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.588161 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.588161 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.592161 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:57:43.000000 finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 03:57:43.592161 finalsa_dynamo_client-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:57:43.592161 finalsa_dynamo_client-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-15 03:57:32.000000 finalsa_dynamo_client-0.0.7/tests/test_client.py
```

### Comparing `finalsa-dynamo-client-0.0.6/LICENSE.md` & `finalsa_dynamo_client-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/PKG-INFO` & `finalsa_dynamo_client-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/__init__.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     AsyncDynamoClient as AsyncDynamoClientImpl
 )
 from finalsa.dynamo.client.tests import (SyncDynamoClientTestImpl, AsyncDynamoClientTestImpl)
 from finalsa.dynamo.client.tests import seed
 
 
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 __all__ = [
     "SyncDynamoClient",
     "SyncDynamoClientImpl",
     "SyncDynamoClientTestImpl",
 
     "AsyncDynamoClient",
```

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/async_client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/async_client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/client/implementation.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/client/implementation.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/async_client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/async_client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/interface/client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/interface/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/async_client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/async_client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/client.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/finalsa/dynamo/client/tests/implementation.py` & `finalsa_dynamo_client-0.0.7/finalsa/dynamo/client/tests/implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 def is_equal(item: Dict, key: Dict):
     for k, v in key.items():
         if item.get(k) != v:
             return False
     return True
 
 
+def eval_expressions(item, filters, actions):
+    for filter in filters:
+        if filter[0] in actions and filter[1]['key'] in item:
+            action_eval = actions[filter[0]](
+                item[filter[1]['key']], filter[1]['value'])
+            if not action_eval:
+                return False
+    return True
+
+
 class DynamoClientTestImpl(Interface):
 
     def __init__(self):
         self.tables = {}
 
     def get_table(self, TableName: str):
         if TableName not in self.tables:
@@ -103,14 +113,18 @@
             lambda x: not is_equal(x, key), self.tables[TableName]))
 
     def scan(self, TableName: str, **kwargs):
         if TableName not in self.tables:
             return {'Items': []}
 
         def begins_with(x: str, y):
+            if isinstance(y, dict):
+                return x.startswith(y['S'])
+            if isinstance(x, dict):
+                return begins_with(x['S'], y)
             return x.startswith(y)
         actions = {
             "begins_with": begins_with
         }
         if not kwargs or len(kwargs) == 0:
             return {'Items': self.tables[TableName]}
         filters = []
@@ -129,20 +143,16 @@
                     filters.append(('begins_with', {
                         "key": key,
                         "value": values[value]
                     }))
 
         items = []
         for item in self.tables[TableName]:
-            for filter in filters:
-                if filter[0] in actions:
-                    action_eval = actions[filter[0]](
-                        item[filter[1]['key']], filter[1]['value'])
-                    if action_eval:
-                        items.append(item)
+            if eval_expressions(item, filters, actions):
+                items.append(item)
         return {'Items': items}
 
     def update(self, TableName: str, key: Dict, item: Dict):
         self.get_table(TableName)
         for i in self.tables[TableName]:
             if is_equal(i, key):
                 for k, v in item.items():
```

### Comparing `finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/PKG-INFO` & `finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-dynamo-client-0.0.6/finalsa_dynamo_client.egg-info/SOURCES.txt` & `finalsa_dynamo_client-0.0.7/finalsa_dynamo_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/setup.py` & `finalsa_dynamo_client-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-client-0.0.6/tests/test_client.py` & `finalsa_dynamo_client-0.0.7/tests/test_client.py`

 * *Files identical despite different names*

