# Comparing `tmp/jy_lib-0.5.8.tar.gz` & `tmp/jy_lib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.5.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.5.8.tar` & `jy_lib-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.8/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.8/.pypirc
--rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.8/.vscode/launch.json
--rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.8/.vscode/settings.json
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.8/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.5.8/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.8/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.8/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.8/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-11 08:45:43.419981 jy_lib-0.5.8/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.8/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.8/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.8/jy_lib/base.py
--rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.8/jy_lib/cache.py
--rw-r--r--   0        0        0     3193 2024-04-11 08:45:28.687693 jy_lib-0.5.8/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.5.8/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.8/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.8/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.8/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.8/jy_lib/decorator.py
--rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.8/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.8/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.8/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.8/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.8/jy_lib/nav.py
--rw-r--r--   0        0        0    17343 2024-04-02 02:09:29.527247 jy_lib-0.5.8/jy_lib/smb_client.py
--rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.8/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.8/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.8/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.8/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.8/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.8/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-11 01:28:25.533916 jy_lib-0.5.8/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.9/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.9/.pypirc
+-rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.9/.vscode/launch.json
+-rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.9/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.5.9/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.9/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.9/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.9/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-15 07:07:38.678245 jy_lib-0.5.9/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.9/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.9/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.9/jy_lib/base.py
+-rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.9/jy_lib/cache.py
+-rw-r--r--   0        0        0     3207 2024-04-15 07:06:48.429065 jy_lib-0.5.9/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.5.9/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.9/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.9/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.9/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.9/jy_lib/decorator.py
+-rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.9/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.9/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.9/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.9/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.9/jy_lib/nav.py
+-rw-r--r--   0        0        0    18415 2024-04-15 07:06:48.429809 jy_lib-0.5.9/jy_lib/smb_client.py
+-rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.9/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.9/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.9/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.9/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.9/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.9/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.5.9/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.5.9/PKG-INFO
```

### Comparing `jy_lib-0.5.8/.gitignore` & `jy_lib-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/.vscode/settings.json` & `jy_lib-0.5.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/LICENSE` & `jy_lib-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/Pipfile` & `jy_lib-0.5.9/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/Pipfile.lock` & `jy_lib-0.5.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/__init__.py` & `jy_lib-0.5.9/jy_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     WarrantsType,
     BlockType,
     SpotType,
     SymbolType,
     SymbolFlag,
 )
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
```

### Comparing `jy_lib-0.5.8/jy_lib/auth_client.py` & `jy_lib-0.5.9/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/bank.py` & `jy_lib-0.5.9/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/base.py` & `jy_lib-0.5.9/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/cache.py` & `jy_lib-0.5.9/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/clickhouse.py` & `jy_lib-0.5.9/jy_lib/clickhouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,19 @@
         }
         self.execute = self.client.execute
 
     def bulk_insert(self, table_name: str, df: pl.DataFrame):
         columns: str = ', '.join([f'`{column}`' for column in df.columns])
         sql: str = f'INSERT INTO `{self.database_name}`.`{table_name}`({columns}) VALUES'
         with KeyboardInterruptProtect():
-            logger.debug(f'[{self.database_name}.{table_name}]准备插入{df.height}条数据')
+            logger.debug(f'[{self.database_name}.{table_name}]准备插入{df.height:12,d}条数据')
             t1: float = time.time()
             self.client.execute(query=sql, params=df.to_dicts())
             t2: float = time.time()
-            logger.success(f'[{self.database_name}.{table_name}]成功插入{df.height:7d}条数据 耗时{t2 - t1:0.0f}秒')
+            logger.success(f'[{self.database_name}.{table_name}]成功插入{df.height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
 
     def import_csv(self, table_name: str, csv: str, height: int = 0):
         sql: str = f'INSERT INTO `{self.database_name}`.`{table_name}` FORMAT CSVWithNames'
         params: Dict = {
             'query': sql,
             **self.credential,
             'enable_http_compression': 1,
@@ -51,29 +51,29 @@
             while sio.readline():
                 height += 1
         csv: bytes = csv.encode('utf-8')
         with ZstdStreamCompressor(size=len(csv), level=zstandard.STRATEGY_FAST) as sc:
             sc.update(data=csv)
             stream: io.BytesIO = sc.stream
         with KeyboardInterruptProtect():
-            logger.debug(f'[{self.database_name}.{table_name}]准备插入{height}条数据')
+            logger.debug(f'[{self.database_name}.{table_name}]准备插入{height:12,d}条数据')
             r = requests.post(
                 url=self.url_http,
                 params=params,
                 data=stream.getvalue(),
                 headers={
                     'Content-Encoding': 'zstd',
                     'Accept-Encoding': 'zstd',
                 },
             )
             t2: float = time.time()
         assert r.status_code == 200, f'[{r.status_code}]{r.text}'
         if r.text:
             logger.info(r.text)
-        logger.success(f'[{self.database_name}.{table_name}]成功插入{height:7d}条数据 耗时{t2 - t1:0.0f}秒')
+        logger.success(f'[{self.database_name}.{table_name}]成功插入{height:12,d}条数据 耗时{t2 - t1:0.0f}秒')
 
     def import_df(self, table_name: str, df: pl.DataFrame, datetime_format='%Y-%m-%d %H:%M:%S%.f'):
         assert self.database_name
         return self.import_csv(
             table_name=table_name,
             csv=df.write_csv(include_header=True, datetime_format=datetime_format),
             height=df.height
```

### Comparing `jy_lib-0.5.8/jy_lib/compressor.py` & `jy_lib-0.5.9/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/country.py` & `jy_lib-0.5.9/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/currency.py` & `jy_lib-0.5.9/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/date.py` & `jy_lib-0.5.9/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/decorator.py` & `jy_lib-0.5.9/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/exchange.py` & `jy_lib-0.5.9/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/interrupt_protect.py` & `jy_lib-0.5.9/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/lock.py` & `jy_lib-0.5.9/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/math.py` & `jy_lib-0.5.9/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/nav.py` & `jy_lib-0.5.9/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/smb_client.py` & `jy_lib-0.5.9/jy_lib/smb_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+import math
+
 import humanize
 import io
 import os
 import re
 import time
 import urllib.parse
 import uuid
@@ -403,7 +405,35 @@
             except (NotConnectedError, BrokenPipeError, ConnectionResetError):
                 self.reload()
                 logger.debug(f"SMB连接成功 PID={os.getpid()}")
                 continue
             except Exception as e:
                 logger.error(f"[{e.__class__.__name__}]{e}")
                 raise e
+
+    def getsize(self, path: AnyStr) -> int:
+        """获取文件大小"""
+        if not self.exists(path):
+            return -1
+        sf: SharedFile = self.getAttributes(service_name=self.service_name, path=path)
+        return sf.file_size
+
+    def getmtime(self, path: AnyStr) -> float:
+        """获取文件修改时间"""
+        if not self.exists(path):
+            return -math.inf
+        sf: SharedFile = self.getAttributes(service_name=self.service_name, path=path)
+        return sf.last_write_time
+
+    def getctime(self, path: AnyStr) -> float:
+        """获取文件创建时间"""
+        if not self.exists(path):
+            return -math.inf
+        sf: SharedFile = self.getAttributes(service_name=self.service_name, path=path)
+        return sf.create_time
+
+    def getatime(self, path: AnyStr) -> float:
+        """获取文件访问时间"""
+        if not self.exists(path):
+            return -math.inf
+        sf: SharedFile = self.getAttributes(service_name=self.service_name, path=path)
+        return sf.last_access_time
```

### Comparing `jy_lib-0.5.8/jy_lib/symbol.py` & `jy_lib-0.5.9/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/symbol_em.py` & `jy_lib-0.5.9/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/jy_lib/time.py` & `jy_lib-0.5.9/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.8/pyproject.toml` & `jy_lib-0.5.9/pyproject.toml`

 * *Files identical despite different names*

