# Comparing `tmp/injected_utils-0.1.6.tar.gz` & `tmp/injected_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "injected_utils-0.1.6.tar", max compression
+gzip compressed data, was "injected_utils-0.1.7.tar", max compression
```

## Comparing `injected_utils-0.1.6.tar` & `injected_utils-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-19 05:19:08.455997 injected_utils-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-19 02:58:41.015807 injected_utils-0.1.6/injected_utils/__init__.py
--rw-r--r--   0        0        0        2 2023-11-13 05:36:52.583543 injected_utils-0.1.6/injected_utils/async_cached_function.py
--rw-r--r--   0        0        0    17439 2023-12-27 05:31:12.462515 injected_utils-0.1.6/injected_utils/cached_function.py
--rw-r--r--   0        0        0    19384 2024-04-03 03:47:00.467836 injected_utils-0.1.6/injected_utils/injected_cache_utils.py
--rw-r--r--   0        0        0     4515 2024-02-15 11:54:53.408850 injected_utils-0.1.6/injected_utils/picklability_checker.py
--rw-r--r--   0        0        0     3950 2023-04-18 01:16:04.722640 injected_utils-0.1.6/injected_utils/shelf_util.py
--rw-r--r--   0        0        0      551 2024-04-03 03:48:01.378698 injected_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 injected_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 05:19:08.455997 injected_utils-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 02:58:41.015807 injected_utils-0.1.7/injected_utils/__init__.py
+-rw-r--r--   0        0        0        2 2023-11-13 05:36:52.583543 injected_utils-0.1.7/injected_utils/async_cached_function.py
+-rw-r--r--   0        0        0    17391 2024-04-15 03:13:29.237981 injected_utils-0.1.7/injected_utils/cached_function.py
+-rw-r--r--   0        0        0    19384 2024-04-03 03:47:00.467836 injected_utils-0.1.7/injected_utils/injected_cache_utils.py
+-rw-r--r--   0        0        0     4515 2024-02-15 11:54:53.408850 injected_utils-0.1.7/injected_utils/picklability_checker.py
+-rw-r--r--   0        0        0     3950 2023-04-18 01:16:04.722640 injected_utils-0.1.7/injected_utils/shelf_util.py
+-rw-r--r--   0        0        0      551 2024-04-15 03:13:40.093046 injected_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 injected_utils-0.1.7/PKG-INFO
```

### Comparing `injected_utils-0.1.6/injected_utils/cached_function.py` & `injected_utils-0.1.7/injected_utils/cached_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from returns.maybe import Nothing, Maybe, Some
 
 from injected_utils.picklability_checker import assert_picklable
 from injected_utils.shelf_util import MyShelf
 from pinjected import Injected
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.di.util import check_picklable
-from ray_proxy import RemoteInterpreterFactory, Var
 from loguru import logger
 
 
 class IStringKeyProtocol(ABC):
     @abstractmethod
     def get_cache_key(self, *args, **kwargs):
         raise NotImplementedError
@@ -215,15 +214,15 @@
         logger.info(f"current working dir is {os.getcwd()}")
         shelf = SqliteDict(path, encode=encode, decode=decode, autocommit=True)
         cache_serializer = Some(lambda sd: sd.filename)
         cache_deserializer = Some(lambda filename: SqliteDict(filename, encode=encode, decode=decode, autocommit=True))
         return CachedFunction(shelf, func, cache_serializer, cache_deserializer)
 
     @staticmethod
-    def create_with_proxy(rif: RemoteInterpreterFactory, gen_cache: Callable[[], Dict], func):
+    def create_with_proxy(rif: "RemoteInterpreterFactory", gen_cache: Callable[[], Dict], func):
         env = rif.create(num_cpus=0)
         r_cache = env.put(gen_cache)()
         return CachedFunction(RemoteDict(r_cache), func)
 
 
 @dataclass
 class TimeCachedFunction:
@@ -433,15 +432,15 @@
         if self.key_deserializer is None:
             raise RuntimeError("key_deserializer is None. so key retrieval is not possible.")
         return self.key_deserializer(key)
 
 
 @dataclass
 class RemoteDict:
-    src: Var#[Dict]
+    src: "Var"#[Dict]
 
     def __getitem__(self, item):
         return self.src[item].fetch()
 
     def __setitem__(self, key, value):
         self.src[key] = value
```

### Comparing `injected_utils-0.1.6/injected_utils/injected_cache_utils.py` & `injected_utils-0.1.7/injected_utils/injected_cache_utils.py`

 * *Files identical despite different names*

### Comparing `injected_utils-0.1.6/injected_utils/picklability_checker.py` & `injected_utils-0.1.7/injected_utils/picklability_checker.py`

 * *Files identical despite different names*

### Comparing `injected_utils-0.1.6/injected_utils/shelf_util.py` & `injected_utils-0.1.7/injected_utils/shelf_util.py`

 * *Files identical despite different names*

### Comparing `injected_utils-0.1.6/pyproject.toml` & `injected_utils-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "injected-utils"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Kento Masui <nameissoap@gmail.com>"]
 readme = "README.md"
 packages = [{include = "injected_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `injected_utils-0.1.6/PKG-INFO` & `injected_utils-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: injected-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Kento Masui
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

