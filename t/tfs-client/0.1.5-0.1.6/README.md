# Comparing `tmp/tfs-client-0.1.5.tar.gz` & `tmp/tfs_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfs-client-0.1.5.tar", last modified: Wed Mar 20 16:34:26 2024, max compression
+gzip compressed data, was "tfs_client-0.1.6.tar", last modified: Mon Apr 15 18:37:43 2024, max compression
```

## Comparing `tfs-client-0.1.5.tar` & `tfs_client-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-03-20 16:34:26.375571 tfs-client-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-03-15 10:11:13.000000 tfs-client-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      461 2024-03-20 16:34:23.000000 tfs-client-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-03-20 16:34:26.375571 tfs-client-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/src/tfs_client/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-17 18:31:13.000000 tfs-client-0.1.5/src/tfs_client/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      761 2024-03-16 14:16:09.000000 tfs-client-0.1.5/src/tfs_client/http.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/src/tfs_client/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       52 2024-03-16 14:17:28.000000 tfs-client-0.1.5/src/tfs_client/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/src/tfs_client/util/cit_images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       80 2024-03-16 14:18:51.000000 tfs-client-0.1.5/src/tfs_client/util/cit_images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1498 2024-03-19 10:06:52.000000 tfs-client-0.1.5/src/tfs_client/util/cit_images/cit_images.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-03-19 10:05:24.000000 tfs-client-0.1.5/src/tfs_client/util/postprocessing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-20 16:34:26.375571 tfs-client-0.1.5/src/tfs_client.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-03-20 16:34:26.000000 tfs-client-0.1.5/src/tfs_client.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      421 2024-03-20 16:34:26.000000 tfs-client-0.1.5/src/tfs_client.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-03-20 16:34:26.000000 tfs-client-0.1.5/src/tfs_client.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-03-20 16:34:26.000000 tfs-client-0.1.5/src/tfs_client.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-03-20 16:34:26.000000 tfs-client-0.1.5/src/tfs_client.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-15 18:37:43.502496 tfs_client-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-03-15 10:11:13.000000 tfs_client-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-15 18:37:40.000000 tfs_client-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 18:37:43.502496 tfs_client-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-17 18:31:13.000000 tfs_client-0.1.6/src/tfs_client/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      761 2024-03-16 14:16:09.000000 tfs_client-0.1.6/src/tfs_client/http.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       52 2024-03-16 14:17:28.000000 tfs_client-0.1.6/src/tfs_client/util/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/util/cit_images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       80 2024-03-16 14:18:51.000000 tfs_client-0.1.6/src/tfs_client/util/cit_images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1498 2024-03-19 10:06:52.000000 tfs_client-0.1.6/src/tfs_client/util/cit_images/cit_images.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-04-15 18:35:38.000000 tfs_client-0.1.6/src/tfs_client/util/postprocessing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      421 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/top_level.txt
```

### Comparing `tfs-client-0.1.5/src/tfs_client/http.py` & `tfs_client-0.1.6/src/tfs_client/http.py`

 * *Files identical despite different names*

### Comparing `tfs-client-0.1.5/src/tfs_client/util/cit_images/cit_images.py` & `tfs_client-0.1.6/src/tfs_client/util/cit_images/cit_images.py`

 * *Files identical despite different names*

### Comparing `tfs-client-0.1.5/src/tfs_client/util/postprocessing.py` & `tfs_client-0.1.6/src/tfs_client/util/postprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import haskellian as hk
+import haskellian.iterables as hk
+from haskellian.core import pipe
 from ..http import SamplePreds, predict, Params
 
 def transpose(sample: SamplePreds) -> list[tuple[str, float]]:
   return list(zip(sample.preds, sample.logprobs))
 
 async def multi_predict(b64_multibatch: list[tuple[str, ...]], **params: Params) -> list[list[list[tuple[str, float]]]]:
     """Returns an array of shape `BATCH x PLAYERS x TOP_PREDS` of `(pred, logprob)`"""
     if len(b64_multibatch) == 0:
         return []
     num_players = len(b64_multibatch[0])
     flatbatch = list(hk.flatten(b64_multibatch))
     flatpreds = await predict(flatbatch, **params)
-    return hk.vpipe(
+    return pipe(
         hk.map(transpose, flatpreds),
         hk.batch(num_players),
         list
     )
```

