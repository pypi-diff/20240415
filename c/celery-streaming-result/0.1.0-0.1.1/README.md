# Comparing `tmp/celery_streaming_result-0.1.0.tar.gz` & `tmp/celery_streaming_result-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_streaming_result-0.1.0.tar", last modified: Sat Apr 13 14:10:42 2024, max compression
+gzip compressed data, was "celery_streaming_result-0.1.1.tar", last modified: Mon Apr 15 14:28:23 2024, max compression
```

## Comparing `celery_streaming_result-0.1.0.tar` & `celery_streaming_result-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-13 14:10:42.408380 celery_streaming_result-0.1.0/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.0/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.0/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1814 2024-04-13 14:10:42.408242 celery_streaming_result-0.1.0/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1164 2024-04-13 14:10:00.000000 celery_streaming_result-0.1.0/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-13 14:10:42.407104 celery_streaming_result-0.1.0/celery_streaming_result/
--rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.0/celery_streaming_result/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     4287 2024-04-13 13:46:21.000000 celery_streaming_result-0.1.0/celery_streaming_result/core.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-13 14:10:42.408026 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1814 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      403 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       21 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       24 2024-04-13 14:10:42.000000 celery_streaming_result-0.1.0/celery_streaming_result.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       21 2024-04-13 13:34:25.000000 celery_streaming_result-0.1.0/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-04-13 14:10:42.408432 celery_streaming_result-0.1.0/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1473 2024-04-13 13:40:40.000000 celery_streaming_result-0.1.0/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.240257 celery_streaming_result-0.1.1/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.1/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.1/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3060 2024-04-15 14:28:23.240128 celery_streaming_result-0.1.1/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2410 2024-04-15 14:16:34.000000 celery_streaming_result-0.1.1/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.238978 celery_streaming_result-0.1.1/celery_streaming_result/
+-rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.1/celery_streaming_result/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     7022 2024-04-15 14:17:11.000000 celery_streaming_result-0.1.1/celery_streaming_result/core.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.239902 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3060 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      403 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       24 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 13:57:28.000000 celery_streaming_result-0.1.1/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-04-15 14:28:23.240302 celery_streaming_result-0.1.1/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1473 2024-04-15 01:21:50.000000 celery_streaming_result-0.1.1/setup.py
```

### Comparing `celery_streaming_result-0.1.0/LICENSE` & `celery_streaming_result-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_streaming_result-0.1.0/PKG-INFO` & `celery_streaming_result-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: celery_streaming_result
-Version: 0.1.0
-Summary: Celery任务结果分片管理
-Home-page: UNKNOWN
-Author: Zhou WeiKe
-Maintainer: Zhou WeiKe
-License: MIT
-Keywords: celery_streaming_result,celery,streaming result
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # celery-streaming-result
 
 Celery任务结果分片管理。
 
 ## 安装
 
 ```
@@ -48,32 +29,75 @@
         csrm.append_result_chunk(celery_task, i)
         result.append(i)
     csrm.append_ended_chunk(celery_task)
     return result
 
 ```
 
-## 客户端
+## 客户端（同步）
 
 ```python
 import redis
 from celery.app import app_or_default
 from celery_streaming_result import CeleryStreamingResultManager
-from test_server import task1 # 根据你的task定义，正确引用
+
+# 根据你的task定义，正确引用
+from test_server import task1
 
 app = app_or_default()
 redis_instance = redis.Redis()
 csrm = CeleryStreamingResultManager(redis_instance)
 
-atask1 = task1.delay() # 生成一个异步任务
-for chunk in csrm.get_result_chunks(atask1): # 读取该异步任务的结果分片
+# 生成一个异步任务
+atask1 = task1.delay()
+# 读取该异步任务的结果分片
+for chunk in csrm.get_result_chunks(atask1):
     print(chunk, end="-", flush=True)
+```
+
+## 客户端（异步）
 
+```python
+from redis import asyncio as aioredis
+from celery.app import app_or_default
+from celery_streaming_result import CeleryStreamingResultManager
+from celery_streaming_result import start_celery_task_async
+from celery_streaming_result import get_celery_task_result_async
+from test_server import task1  # 根据你的task定义，正确引用
+
+app = app_or_default()
+redis_instance = aioredis.Redis()
+csrm = CeleryStreamingResultManager(redis_instance)
+
+
+async def on_finished(
+    celery_task,
+):
+    print("on finished...")
+    task_result = await get_celery_task_result_async(
+        celery_task,
+    )
+    # 这里的task_result值是celery任务的返回值。
+    # 一般来说是所有结果分片的集合，但实际只取决于celery任务的实现。
+
+
+atask1 = await start_celery_task_async(
+    task1
+)  # task1.delay()是一个同步函数。需要使用`sync_to_async`进行转化。
+# 读取该异步任务的结果分片，如果任务结果，则回调on_finished函数。
+async for chunk in csrm.get_result_chunks(
+    atask1,
+    on_finished=on_finished,
+):
+    print(chunk, end="-", flush=True)
 ```
 
 ## 版本记录
 
 ### v0.1.0
 
 1. 首次发布。
 
+### v0.1.1
 
+1. 添加asyncio支持。
+1. 获取结果支持on_finished回调。
```

### Comparing `celery_streaming_result-0.1.0/celery_streaming_result/core.py` & `celery_streaming_result-0.1.1/celery_streaming_result/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import time
+import asyncio
+from asgiref.sync import sync_to_async
 import msgpack
 
 __all__ = [
     "DEFAULT_ENDED_CHUNK",
     "ReadCeleryStreamingResultTimeout",
     "CeleryStreamingResultManager",
+    "start_celery_task_async",
+    "get_celery_task_result_async",
 ]
 
 DEFAULT_ENDED_CHUNK = "this:is:the:celery:streaming:result:ended:chunk:b53127b4-ba43-4ff4-aba4-2134b17b9006"
 
 
 class ReadCeleryStreamingResultTimeout(RuntimeError):
     args = (124, "读取分片结果超时")
 
 
 class CeleryStreamingResultManager(object):
     """Celery任务结果分片管理类。
 
-    # 使用方法
+    ## 使用方法
 
     ```
     csrm = CeleryStreamingResultManager(redis_instance)
 
     # in task main
     csrm.append_result_chunk(celery_task_instance, result_chunk1)
     csrm.append_result_chunk(celery_task_instance, result_chunk2)
@@ -29,14 +33,22 @@
 
     # in task creator process
     async_result = celery_task.delay(*args, **kwargs)
     for chunk in csrm.get_result_chunks(async_result):
         yield chunk
     ```
 
+    ## 支持async_xxx方法
+
+    支持async_xxx方法的前提是store支持async方法。
+    要求store实例是由aioredis创建而来。
+
+    aioredis引用方法：
+    from redis import asyncio as aioredis
+
     """
 
     def __init__(
         self,
         store,
         result_key_template=None,
         ended_chunk=None,
@@ -76,37 +88,51 @@
 
     def append_result_chunk(self, task, chunk):
         """输出分片结果。"""
         result_key = self.result_key_template.format(task_id=task.request.id)
         self.store.lpush(result_key, self.encode(chunk))
         self.store.expire(result_key, self.expires)
 
+    async def async_append_result_chunk(self, task, chunk):
+        """输出分片结果。"""
+        result_key = self.result_key_template.format(task_id=task.request.id)
+        await self.store.lpush(result_key, self.encode(chunk))
+        await self.store.expire(result_key, self.expires)
+
     def append_ended_chunk(self, task):
         """输出分片结果结束标识。"""
         result_key = self.result_key_template.format(task_id=task.request.id)
         self.store.lpush(result_key, self.encode(self.ended_chunk))
         self.store.expire(result_key, self.expires)
 
+    async def async_append_ended_chunk(self, task):
+        """输出分片结果结束标识。"""
+        result_key = self.result_key_template.format(task_id=task.request.id)
+        await self.store.lpush(result_key, self.encode(self.ended_chunk))
+        await self.store.expire(result_key, self.expires)
+
     def get_result_chunks(
         self,
-        async_result,
+        celery_async_task,
         total_timeout=0,
         read_timeout=0,
         interval=1,
+        on_finished=None,
     ):
         """读取分片结果。
 
-        @parameter: async_result Celery task delay后返回的AsyncTask实例。
+        @parameter: celery_async_task Celery task delay后返回的AsyncTask实例。
         @parameter: total_timeout 总超时时长。超过后，强制结束。
         @parameter: read_timeout 连续没有响应导致的超时时长。超过后，强制结束。
         @parameter: interval 单次读取超时时间。
+        @parameter: on_finished 读取结束时的回调。
         """
         stime = time.time()
         rtime = None
-        result_key = self.result_key_template.format(task_id=async_result.task_id)
+        result_key = self.result_key_template.format(task_id=celery_async_task.task_id)
         while True:
             result = self.store.brpop(result_key, timeout=interval)
             if (total_timeout != 0) and (time.time() - stime > total_timeout):
                 raise ReadCeleryStreamingResultTimeout()
             if result is None:
                 if rtime is None:
                     rtime = time.time()
@@ -117,8 +143,55 @@
                 rtime = None
             if result is None:
                 continue
             result = self.decode(result[1])
             if result != self.ended_chunk:
                 yield result
             else:
+                if on_finished:
+                    on_finished(celery_async_task)
                 return
+
+    async def async_get_result_chunks(
+        self,
+        celery_async_task,
+        total_timeout=0,
+        read_timeout=0,
+        interval=1,
+        on_finished=None,
+    ):
+        stime = time.time()
+        rtime = None
+        result_key = self.result_key_template.format(task_id=celery_async_task.task_id)
+        while True:
+            result = await self.store.brpop(result_key, timeout=interval)
+            if (total_timeout != 0) and (time.time() - stime > total_timeout):
+                raise ReadCeleryStreamingResultTimeout()
+            if result is None:
+                if rtime is None:
+                    rtime = time.time()
+                else:
+                    if (read_timeout != 0) and (time.time() - rtime > read_timeout):
+                        raise ReadCeleryStreamingResultTimeout()
+            else:
+                rtime = None
+            if result is None:
+                continue
+            result = self.decode(result[1])
+            if result != self.ended_chunk:
+                yield result
+            else:
+                if on_finished:
+                    await on_finished(celery_async_task)
+                return
+
+
+async def start_celery_task_async(celery_task, *args, **kwargs):
+    """使用异步方法启动一个Celery任务。"""
+    result = await sync_to_async(celery_task.delay)(*args, **kwargs)
+    return result
+
+
+async def get_celery_task_result_async(celery_task_async, *args, **kwargs):
+    """获取celery TaskAsync的执行结果。"""
+    result = await sync_to_async(celery_task_async.get)(*args, **kwargs)
+    return result
```

### Comparing `celery_streaming_result-0.1.0/celery_streaming_result.egg-info/PKG-INFO` & `celery_streaming_result-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: celery-streaming-result
-Version: 0.1.0
+Name: celery_streaming_result
+Version: 0.1.1
 Summary: Celery任务结果分片管理
 Home-page: UNKNOWN
 Author: Zhou WeiKe
 Maintainer: Zhou WeiKe
 License: MIT
 Keywords: celery_streaming_result,celery,streaming result
 Platform: UNKNOWN
@@ -48,32 +48,77 @@
         csrm.append_result_chunk(celery_task, i)
         result.append(i)
     csrm.append_ended_chunk(celery_task)
     return result
 
 ```
 
-## 客户端
+## 客户端（同步）
 
 ```python
 import redis
 from celery.app import app_or_default
 from celery_streaming_result import CeleryStreamingResultManager
-from test_server import task1 # 根据你的task定义，正确引用
+
+# 根据你的task定义，正确引用
+from test_server import task1
 
 app = app_or_default()
 redis_instance = redis.Redis()
 csrm = CeleryStreamingResultManager(redis_instance)
 
-atask1 = task1.delay() # 生成一个异步任务
-for chunk in csrm.get_result_chunks(atask1): # 读取该异步任务的结果分片
+# 生成一个异步任务
+atask1 = task1.delay()
+# 读取该异步任务的结果分片
+for chunk in csrm.get_result_chunks(atask1):
     print(chunk, end="-", flush=True)
+```
+
+## 客户端（异步）
+
+```python
+from redis import asyncio as aioredis
+from celery.app import app_or_default
+from celery_streaming_result import CeleryStreamingResultManager
+from celery_streaming_result import start_celery_task_async
+from celery_streaming_result import get_celery_task_result_async
+from test_server import task1  # 根据你的task定义，正确引用
 
+app = app_or_default()
+redis_instance = aioredis.Redis()
+csrm = CeleryStreamingResultManager(redis_instance)
+
+
+async def on_finished(
+    celery_task,
+):
+    print("on finished...")
+    task_result = await get_celery_task_result_async(
+        celery_task,
+    )
+    # 这里的task_result值是celery任务的返回值。
+    # 一般来说是所有结果分片的集合，但实际只取决于celery任务的实现。
+
+
+atask1 = await start_celery_task_async(
+    task1
+)  # task1.delay()是一个同步函数。需要使用`sync_to_async`进行转化。
+# 读取该异步任务的结果分片，如果任务结果，则回调on_finished函数。
+async for chunk in csrm.get_result_chunks(
+    atask1,
+    on_finished=on_finished,
+):
+    print(chunk, end="-", flush=True)
 ```
 
 ## 版本记录
 
 ### v0.1.0
 
 1. 首次发布。
 
+### v0.1.1
+
+1. 添加asyncio支持。
+1. 获取结果支持on_finished回调。
+
```

### Comparing `celery_streaming_result-0.1.0/setup.py` & `celery_streaming_result-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery_streaming_result",
-    version="0.1.0",
+    version="0.1.1",
     description="Celery任务结果分片管理",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhou WeiKe",
     maintainer="Zhou WeiKe",
     license="MIT",
     license_files=("LICENSE",),
```

