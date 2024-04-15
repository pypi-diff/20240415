# Comparing `tmp/async_redis_uow-0.0.8.tar.gz` & `tmp/async_redis_uow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_redis_uow-0.0.8.tar", last modified: Fri Sep 22 05:35:00 2023, max compression
+gzip compressed data, was "async_redis_uow-0.0.9.tar", last modified: Wed Sep 27 03:58:24 2023, max compression
```

## Comparing `async_redis_uow-0.0.8.tar` & `async_redis_uow-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.877265 async_redis_uow-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/async_redis_uow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/async_redis_uow/repository/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/adder.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/all_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/deleter.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/getter.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/paginated.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/paginated_all_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/status_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/repository/updateter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/async_redis_uow/session_maker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/session_maker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/session_maker/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/session_maker/session_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/async_redis_uow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/async_redis_uow/utils/creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 05:35:00.873265 async_redis_uow-0.0.8/async_redis_uow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-09-22 05:35:00.000000 async_redis_uow-0.0.8/async_redis_uow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-09-22 05:35:00.000000 async_redis_uow-0.0.8/async_redis_uow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 05:35:00.000000 async_redis_uow-0.0.8/async_redis_uow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-22 05:35:00.000000 async_redis_uow-0.0.8/async_redis_uow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-22 05:35:00.000000 async_redis_uow-0.0.8/async_redis_uow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 05:35:00.877265 async_redis_uow-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-09-22 05:34:36.000000 async_redis_uow-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.353534 async_redis_uow-0.0.9/async_redis_uow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/async_redis_uow/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/adder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/all_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/deleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/paginated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/paginated_all_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/status_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/repository/updateter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/async_redis_uow/session_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/session_maker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/session_maker/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/session_maker/session_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/async_redis_uow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/async_redis_uow/utils/creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 03:58:24.353534 async_redis_uow-0.0.9/async_redis_uow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-09-27 03:58:24.000000 async_redis_uow-0.0.9/async_redis_uow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2023-09-27 03:58:24.000000 async_redis_uow-0.0.9/async_redis_uow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 03:58:24.000000 async_redis_uow-0.0.9/async_redis_uow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-27 03:58:24.000000 async_redis_uow-0.0.9/async_redis_uow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-27 03:58:24.000000 async_redis_uow-0.0.9/async_redis_uow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 03:58:24.357534 async_redis_uow-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-09-27 03:57:56.000000 async_redis_uow-0.0.9/setup.py
```

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/all_getter.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/all_getter.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/base.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/base.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/common.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/common.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/getter.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/getter.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/paginated.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/paginated.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Generic, Optional
+from typing import Generic, Iterable, Optional
 from axsqlalchemy.repository.paginated import math
 from redis.commands.json.path import Path
 from .types import TIModel, TOModel
 from .all_getter import AllGetterRepo
 
 
 class PaginatedRepo(AllGetterRepo[TIModel, TOModel], Generic[TIModel, TOModel]):
     __abstract__ = True
 
     async def all_page_count(self, filters: str = '', count: Optional[int] = None) -> int:
         all_count = await self.all_count(filters)
         return math.ceil(all_count / count) if count else 1 
 
     async def all_count(self, filters: str = ''):
-        return (await self.session.json().objlen(
+        res = await self.session.json().objlen(
             self.hname, 
             Path(f'${filters}').strPath,
-        ).execute())[-1][-1]  # type: ignore
+        ).execute()  # type: ignore
+
+        return res[-1][-1] if res and res[-1] and isinstance(res[-1], Iterable) else 0
```

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/paginated_all_getter.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/paginated_all_getter.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/repository/status_updater.py` & `async_redis_uow-0.0.9/async_redis_uow/repository/status_updater.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/session_maker/session.py` & `async_redis_uow-0.0.9/async_redis_uow/session_maker/session.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow/utils/creation.py` & `async_redis_uow-0.0.9/async_redis_uow/utils/creation.py`

 * *Files identical despite different names*

### Comparing `async_redis_uow-0.0.8/async_redis_uow.egg-info/SOURCES.txt` & `async_redis_uow-0.0.9/async_redis_uow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

