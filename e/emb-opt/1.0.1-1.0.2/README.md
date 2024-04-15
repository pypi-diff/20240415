# Comparing `tmp/emb_opt-1.0.1.tar.gz` & `tmp/emb_opt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emb_opt-1.0.1.tar", last modified: Sat Oct 21 21:54:18 2023, max compression
+gzip compressed data, was "emb_opt-1.0.2.tar", last modified: Mon Apr 15 21:11:28 2024, max compression
```

## Comparing `emb_opt-1.0.1.tar` & `emb_opt-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-10-21 21:54:18.069454 emb_opt-1.0.1/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    11337 2023-01-20 02:50:04.000000 emb_opt-1.0.1/LICENSE
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      111 2023-01-20 02:50:04.000000 emb_opt-1.0.1/MANIFEST.in
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1318 2023-10-21 21:54:18.069454 emb_opt-1.0.1/PKG-INFO
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      616 2023-10-21 21:48:03.000000 emb_opt-1.0.1/README.md
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-10-21 21:54:18.069454 emb_opt-1.0.1/emb_opt/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       22 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/__init__.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    27125 2023-10-21 21:47:59.000000 emb_opt-1.0.1/emb_opt/_modidx.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     9261 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/data_source.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     4942 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/executor.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2870 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/filter.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      351 2023-10-21 21:46:30.000000 emb_opt-1.0.1/emb_opt/imports.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3915 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/log.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1597 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/module.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-10-21 21:54:18.069454 emb_opt-1.0.1/emb_opt/plugins/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/plugins/__init__.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3892 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/plugins/faiss.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     4879 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/plugins/huggingface.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3739 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/plugins/qdrant.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     5726 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/prune.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3145 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/runner.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    11651 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/schemas.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     3277 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/score.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     9785 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/update.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     6199 2023-10-21 21:47:58.000000 emb_opt-1.0.1/emb_opt/utils.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2023-10-21 21:54:18.069454 emb_opt-1.0.1/emb_opt.egg-info/
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1318 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/PKG-INFO
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      637 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/SOURCES.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/dependency_links.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       36 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/entry_points.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-04 21:43:10.000000 emb_opt-1.0.1/emb_opt.egg-info/not-zip-safe
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       83 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/requires.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)        8 2023-10-21 21:54:18.000000 emb_opt-1.0.1/emb_opt.egg-info/top_level.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      931 2023-10-21 21:46:30.000000 emb_opt-1.0.1/settings.ini
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       38 2023-10-21 21:54:18.069454 emb_opt-1.0.1/setup.cfg
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2560 2023-01-20 02:50:04.000000 emb_opt-1.0.1/setup.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2024-04-15 21:11:28.243440 emb_opt-1.0.2/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    11337 2023-01-20 02:50:04.000000 emb_opt-1.0.2/LICENSE
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      111 2023-01-20 02:50:04.000000 emb_opt-1.0.2/MANIFEST.in
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1318 2024-04-15 21:11:28.243440 emb_opt-1.0.2/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      616 2023-10-21 21:48:03.000000 emb_opt-1.0.2/README.md
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2024-04-15 21:11:28.243440 emb_opt-1.0.2/emb_opt/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       22 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    27125 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/_modidx.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     9261 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/data_source.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     4942 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/executor.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2870 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/filter.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      351 2023-10-21 21:46:30.000000 emb_opt-1.0.2/emb_opt/imports.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3915 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/log.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1597 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/module.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2024-04-15 21:11:28.243440 emb_opt-1.0.2/emb_opt/plugins/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        0 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/plugins/__init__.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3892 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/plugins/faiss.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     4879 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/plugins/huggingface.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3739 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/plugins/qdrant.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     5726 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/prune.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3145 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/runner.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)    11651 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/schemas.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     3277 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/score.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     9929 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/update.py
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     6199 2024-04-15 21:06:32.000000 emb_opt-1.0.2/emb_opt/utils.py
+drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2024-04-15 21:11:28.243440 emb_opt-1.0.2/emb_opt.egg-info/
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     1318 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/PKG-INFO
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      637 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       36 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/entry_points.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        1 2023-04-04 21:43:10.000000 emb_opt-1.0.2/emb_opt.egg-info/not-zip-safe
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       83 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/requires.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)        8 2024-04-15 21:11:28.000000 emb_opt-1.0.2/emb_opt.egg-info/top_level.txt
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)      931 2024-04-15 21:06:05.000000 emb_opt-1.0.2/settings.ini
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)       38 2024-04-15 21:11:28.243440 emb_opt-1.0.2/setup.cfg
+-rw-rw-r--   0 dmai      (1000) dmai      (1000)     2560 2023-01-20 02:50:04.000000 emb_opt-1.0.2/setup.py
```

### Comparing `emb_opt-1.0.1/LICENSE` & `emb_opt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/PKG-INFO` & `emb_opt-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emb_opt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight framework to efficiently screen vector databases
 Home-page: https://github.com/DarkMatterAI/emb_opt
 Author: Karl Heyer
 Author-email: karl@darkmatterai.co
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `emb_opt-1.0.1/README.md` & `emb_opt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/_modidx.py` & `emb_opt-1.0.2/emb_opt/_modidx.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/data_source.py` & `emb_opt-1.0.2/emb_opt/data_source.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/executor.py` & `emb_opt-1.0.2/emb_opt/executor.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/filter.py` & `emb_opt-1.0.2/emb_opt/filter.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/log.py` & `emb_opt-1.0.2/emb_opt/log.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/module.py` & `emb_opt-1.0.2/emb_opt/module.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/plugins/faiss.py` & `emb_opt-1.0.2/emb_opt/plugins/faiss.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/plugins/huggingface.py` & `emb_opt-1.0.2/emb_opt/plugins/huggingface.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/plugins/qdrant.py` & `emb_opt-1.0.2/emb_opt/plugins/qdrant.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/prune.py` & `emb_opt-1.0.2/emb_opt/prune.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/runner.py` & `emb_opt-1.0.2/emb_opt/runner.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/schemas.py` & `emb_opt-1.0.2/emb_opt/schemas.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/score.py` & `emb_opt-1.0.2/emb_opt/score.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt/update.py` & `emb_opt-1.0.2/emb_opt/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,17 +153,18 @@
                 ):
         self.k = k
         
     def __call__(self, inputs: List[Query]) -> List[UpdateResponse]:
         outputs = []
         
         for query in inputs:
-            result_scores = np.array([i.score for i in query.valid_results()])
+            valid_results = [i for i in query.valid_results()]
+            result_scores = np.array([i.score for i in valid_results])
             topk_idxs = result_scores.argsort()[::-1][:self.k]
-            top_items = [query[i] for i in topk_idxs]
+            top_items = [valid_results[i] for i in topk_idxs]
             outputs += top_items
             
         outputs = [UpdateResponse(query=Query.from_item(i), parent_id=i.internal.parent_id) 
                                   for i in outputs]
         return outputs
 
 # %% ../nbs/08_update.ipynb 14
@@ -178,24 +179,27 @@
                 ):
         self.k = k
         
     def __call__(self, inputs: List[Query]) -> List[UpdateResponse]:
         outputs = []
         
         for query in inputs:
-            result_scores = np.array([i.score for i in query.valid_results()])
+            valid_results = [i for i in query.valid_results()]
+            result_scores = np.array([i.score for i in valid_results])
+            
             topk_idxs = result_scores.argsort()[::-1][:self.k]
-            topk_embs = np.array([query[i].embedding for i in topk_idxs])
+            topk_embs = np.array([valid_results[i].embedding for i in topk_idxs])
             
             new_embedding = np.average(topk_embs, 0)
             output = UpdateResponse(query=Query.from_parent_query(embedding=new_embedding, 
                                                                   parent_query=query),
                                     parent_id=query.id)
             outputs.append(output)
         return outputs
+    
 
 # %% ../nbs/08_update.ipynb 16
 class RLUpdate():
     '''
     RLUpdate - uses reinforcement learning to update queries
     
     To compute the gradient with RL:
```

### Comparing `emb_opt-1.0.1/emb_opt/utils.py` & `emb_opt-1.0.2/emb_opt/utils.py`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/emb_opt.egg-info/PKG-INFO` & `emb_opt-1.0.2/emb_opt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emb-opt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight framework to efficiently screen vector databases
 Home-page: https://github.com/DarkMatterAI/emb_opt
 Author: Karl Heyer
 Author-email: karl@darkmatterai.co
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `emb_opt-1.0.1/emb_opt.egg-info/SOURCES.txt` & `emb_opt-1.0.2/emb_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emb_opt-1.0.1/settings.ini` & `emb_opt-1.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = emb_opt
 lib_name = emb_opt
-version = 1.0.1
+version = 1.0.2
 min_python = 3.9
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = emb_opt
 nbs_path = nbs
 recursive = True
```

### Comparing `emb_opt-1.0.1/setup.py` & `emb_opt-1.0.2/setup.py`

 * *Files identical despite different names*

