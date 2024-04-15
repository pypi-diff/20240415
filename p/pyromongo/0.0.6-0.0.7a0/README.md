# Comparing `tmp/pyromongo-0.0.6.tar.gz` & `tmp/pyromongo-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyromongo-0.0.6.tar", last modified: Sun Apr 14 06:04:37 2024, max compression
+gzip compressed data, was "pyromongo-0.0.7a0.tar", last modified: Mon Apr 15 08:15:10 2024, max compression
```

## Comparing `pyromongo-0.0.6.tar` & `pyromongo-0.0.7a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/
--rw-r--r--   0 user      (1000) user      (1000)     1070 2024-04-14 05:14:58.000000 pyromongo-0.0.6/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2303 2024-04-14 06:04:37.120772 pyromongo-0.0.6/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1271 2024-04-14 05:14:58.000000 pyromongo-0.0.6/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/pyromongo/
--rw-r--r--   0 user      (1000) user      (1000)     4950 2024-04-14 05:14:58.000000 pyromongo-0.0.6/pyromongo/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/pyromongo.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2303 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      212 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      179 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-14 06:04:37.120772 pyromongo-0.0.6/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1476 2024-04-14 06:04:07.000000 pyromongo-0.0.6/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:15:10.332278 pyromongo-0.0.7a0/
+-rw-r--r--   0 user      (1000) user      (1000)     1070 2024-04-14 05:14:58.000000 pyromongo-0.0.7a0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2305 2024-04-15 08:15:10.332278 pyromongo-0.0.7a0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1271 2024-04-14 05:14:58.000000 pyromongo-0.0.7a0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:15:10.332278 pyromongo-0.0.7a0/pyromongo/
+-rw-r--r--   0 user      (1000) user      (1000)     4955 2024-04-15 08:12:11.000000 pyromongo-0.0.7a0/pyromongo/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:15:10.332278 pyromongo-0.0.7a0/pyromongo.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2305 2024-04-15 08:15:10.000000 pyromongo-0.0.7a0/pyromongo.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      212 2024-04-15 08:15:10.000000 pyromongo-0.0.7a0/pyromongo.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-15 08:15:10.000000 pyromongo-0.0.7a0/pyromongo.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      179 2024-04-15 08:15:10.000000 pyromongo-0.0.7a0/pyromongo.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2024-04-15 08:15:10.000000 pyromongo-0.0.7a0/pyromongo.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-15 08:15:10.332278 pyromongo-0.0.7a0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1477 2024-04-15 08:14:59.000000 pyromongo-0.0.7a0/setup.py
```

### Comparing `pyromongo-0.0.6/LICENSE` & `pyromongo-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyromongo-0.0.6/PKG-INFO` & `pyromongo-0.0.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyromongo
-Version: 0.0.6
+Version: 0.0.7a0
 Summary: Mongo Session Storage for pyrogram
 Home-page: https://github.com/animeshxd/pyromongo
 Author: Animesh Murmu
 Author-email: am2646374@gmail.com
 License: MIT
 Keywords: async mongo session storage pyrogram
 Classifier: Intended Audience :: Developers
```

### Comparing `pyromongo-0.0.6/README.md` & `pyromongo-0.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `pyromongo-0.0.6/pyromongo/__init__.py` & `pyromongo-0.0.7a0/pyromongo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     async def close(self):
         pass
 
     async def delete(self):
         try:
             await self._session.delete_one({'_id': 0})
             if self._remove_peers:
-                await self._peer.remove({})
+                await self._peer.delete_many({})
         except Exception as _:
             return
 
     async def update_peers(self, peers: List[Tuple[int, int, str, str, str]]):
         """(id, access_hash, type, username, phone_number)"""
         s = int(time.time())
         bulk = [
```

### Comparing `pyromongo-0.0.6/pyromongo.egg-info/PKG-INFO` & `pyromongo-0.0.7a0/pyromongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyromongo
-Version: 0.0.6
+Version: 0.0.7a0
 Summary: Mongo Session Storage for pyrogram
 Home-page: https://github.com/animeshxd/pyromongo
 Author: Animesh Murmu
 Author-email: am2646374@gmail.com
 License: MIT
 Keywords: async mongo session storage pyrogram
 Classifier: Intended Audience :: Developers
```

### Comparing `pyromongo-0.0.6/setup.py` & `pyromongo-0.0.7a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 with open("requirements.txt", encoding="utf-8") as r:
     requires = [i.strip() for i in r]
 
 setup(
     name="pyromongo",
-    version="0.0.6",
+    version="0.0.7a",
     description="Mongo Session Storage for pyrogram",
     long_description=readme,
     long_description_content_type="text/markdown",
 
     packages=["pyromongo"],
 
     url="https://github.com/animeshxd/pyromongo",
```

