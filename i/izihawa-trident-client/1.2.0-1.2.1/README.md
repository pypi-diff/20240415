# Comparing `tmp/izihawa_trident_client-1.2.0.tar.gz` & `tmp/izihawa_trident_client-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.2.0.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.2.1.tar", max compression
```

## Comparing `izihawa_trident_client-1.2.0.tar` & `izihawa_trident_client-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.0/README.md
--rw-r--r--   0        0        0      348 2024-04-14 17:14:42.598735 izihawa_trident_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.0/trident/__init__.py
--rw-r--r--   0        0        0     4381 2024-04-14 17:13:23.892915 izihawa_trident_client-1.2.0/trident/client.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.1/README.md
+-rw-r--r--   0        0        0      348 2024-04-14 19:09:28.236421 izihawa_trident_client-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.1/trident/__init__.py
+-rw-r--r--   0        0        0     4386 2024-04-14 19:09:07.214280 izihawa_trident_client-1.2.1/trident/client.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.1/PKG-INFO
```

### Comparing `izihawa_trident_client-1.2.0/trident/client.py` & `izihawa_trident_client-1.2.1/trident/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,9 +120,9 @@
 
     async def table_exists(self, table: str, key: str) -> dict | None:
         url = f"/tables/{table}/{key}"
         response = await self.head(url)
         if response is not None:
             return {
                 'iroh_hash': response.headers['X-Iroh-Hash'],
-                'size': response.headers['Content-Length'],
+                'size': int(response.headers['Content-Length']),
             }
```

### Comparing `izihawa_trident_client-1.2.0/PKG-INFO` & `izihawa_trident_client-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

