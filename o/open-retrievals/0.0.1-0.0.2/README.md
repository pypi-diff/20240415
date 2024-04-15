# Comparing `tmp/open-retrievals-0.0.1.tar.gz` & `tmp/open-retrievals-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-retrievals-0.0.1.tar", last modified: Mon Mar 18 01:32:28 2024, max compression
+gzip compressed data, was "open-retrievals-0.0.2.tar", last modified: Mon Apr 15 11:13:43 2024, max compression
```

## Comparing `open-retrievals-0.0.1.tar` & `open-retrievals-0.0.2.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11346 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-18 01:32:28.226098 open-retrievals-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.214098 open-retrievals-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.218098 open-retrievals-0.0.1/src/open_retrievals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 01:32:28.000000 open-retrievals-0.0.1/src/open_retrievals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.218098 open-retrievals-0.0.1/src/retrievals/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.218098 open-retrievals-0.0.1/src/retrievals/data/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/data/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/src/retrievals/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/bce.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/cosent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/infonce.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/r_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/simcse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/src/retrievals/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20620 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/embedding_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/match_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/models/rerank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/src/retrievals/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/corpus_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/prompter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/tools/web_retrievals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:32:28.222098 open-retrievals-0.0.1/src/retrievals/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/trainer/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/trainer/custom_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/trainer/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-18 01:32:08.000000 open-retrievals-0.0.1/src/retrievals/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11346 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 11:13:43.791568 open-retrievals-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.779568 open-retrievals-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/open_retrievals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/retrievals/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/retrievals/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/bce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/cosent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/infonce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/margin_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/pearson_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/r_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/simcse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/metrics/mrr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20893 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/embedding_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/retrieval_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/corpus_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/prompter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/custom_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/version.py
```

### Comparing `open-retrievals-0.0.1/LICENSE` & `open-retrievals-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/PKG-INFO` & `open-retrievals-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: open-retrievals
-Version: 0.0.1
-Summary: Text Embeddings for Retrieval and RAG based on transformers
-Home-page: https://github.com/LongxingTan/open-retrievals
-Author: Longxing Tan
-Author-email: tanlongxing888@163.com
-License: Apache 2.0 License
-Keywords: NLP retrieval RAG rerank text embedding contrastive
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [license-image]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
 [license-url]: https://opensource.org/licenses/Apache-2.0
 [pypi-image]: https://badge.fury.io/py/open-retrievals.svg
 [pypi-url]: https://pypi.org/project/open-retrievals
 [pepy-image]: https://pepy.tech/badge/retrievals/month
 [pepy-url]: https://pepy.tech/project/retrievals
 [build-image]: https://github.com/LongxingTan/open-retrievals/actions/workflows/test.yml/badge.svg?branch=master
@@ -57,15 +33,15 @@
 
 
 ## Installation
 
 **Prerequisites**
 ```shell
 pip install transformers
-pip install faiss
+pip install faiss-cpu
 pip install peft
 ```
 
 **With pip**
 ```shell
 pip install open-retrievals
 ```
@@ -74,96 +50,46 @@
 
 [//]: # (```shell)
 
 [//]: # (conda install open-retrievals -c conda-forge)
 
 [//]: # (```)
 
+## Quick-start
 
-## Usage
-
-**Use Pretrained sentence embedding**
 ```python
-from retrievals import AutoModelForEmbedding
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
-sentences = ["Hello world", "How are you?"]
-model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
-model = AutoModelForEmbedding(model_name_or_path, pooling_method="mean", normalize_embeddings=True)
-sentence_embeddings = model.encode(sentences, convert_to_tensor=True)
-print(sentence_embeddings)
-```
+# Example list of documents
+documents = [
+    "Open-retrievals is a text embedding libraries",
+    "I can use it simply with a SOTA RAG application.",
+]
 
-**Finetune transformers by contrastive learning**
-```python
-from transformers import AutoTokenizer
-from retrievals import AutoModelForEmbedding, AutoModelForMatch, RetrievalTrainer, PairCollator, TripletCollator
-from retrievals.losses import ArcFaceAdaptiveMarginLoss, InfoNCE, SimCSE, TripletLoss
-from retrievals.data import  RetrievalDataset, RerankDataset
-
-
-train_dataset = RetrievalDataset(args=data_args)
-tokenizer = AutoTokenizer.from_pretrained(model_args.tokenizer_name, use_fast=False)
-
-model = AutoModelForEmbedding(
-    model_args.model_name_or_path,
-    pooling_method="cls"
-)
-optimizer = get_optimizer(model, lr=5e-5, weight_decay=1e-3)
-
-lr_scheduler = get_scheduler(optimizer, num_train_steps=int(len(train_dataset) / 2 * 1))
-
-trainer = RetrievalTrainer(
-    model=model,
-    args=training_args,
-    train_dataset=train_dataset,
-    data_collator=TripletCollator(tokenizer, max_length=data_args.query_max_len),
-    loss_fn=TripletLoss(),
-)
-trainer.optimizer = optimizer
-trainer.scheduler = lr_scheduler
-trainer.train()
-```
-
-**Finetune LLM for embedding by Contrastive learning**
-```python
-
-from retrievals import AutoModelForEmbedding
+# This will trigger the model download and initialization
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path)
 
-model = AutoModelForEmbedding(
-    "mistralai/Mistral-7B-v0.1",
-    pooling_method='cls',
-    query_instruction=f'Instruct: Retrieve semantically similar text\nQuery: '
-)
+embeddings = model.encode(documents)
+len(embeddings) # Vector of 384 dimensions
 ```
 
-**Search by Cosine similarity/KNN**
-```python
-from retrievals import AutoModelForEmbedding, AutoModelForMatch
-
-query_texts = ['A dog is chasing car.']
-passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
-model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
-model = AutoModelForEmbedding('')
-query_embeddings = model.encode(query_texts, convert_to_tensor=True)
-passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
 
-matcher = AutoModelForMatch(method='cosine')
-dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
-```
+## Usage
 
-**Search by Faiss**
+**Build Index and Retrieval**
 ```python
-from retrievals import AutoModelForEmbedding, AutoModelForMatch
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
 sentences = ['A dog is chasing car.', 'A man is playing a guitar.']
 model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
 model = AutoModelForEmbedding(model_name_or_path)
 model.build_index(sentences)
 
-matcher = AutoModelForMatch()
+matcher = AutoModelForRetrieval()
 results = matcher.faiss_search("He plays guitar.")
 ```
 
 **Rerank**
 ```python
 from transformers import AutoTokenizer
 from retrievals import RerankCollator, RerankModel, RerankTrainer, RerankDataset
@@ -186,48 +112,146 @@
     data_collator=RerankCollator(tokenizer, max_length=data_args.query_max_len),
 )
 trainer.optimizer = optimizer
 trainer.scheduler = lr_scheduler
 trainer.train()
 ```
 
-[//]: # (**RAG with LangChain**)
-
-[//]: # ()
-[//]: # (- Prerequisites)
+**RAG with LangChain**
 
-[//]: # (```shell)
 
-[//]: # (pip install langchain)
+- Prerequisites
 
-[//]: # (```)
+```shell
+pip install langchain
+```
 
-[//]: # ()
-[//]: # (- Server)
 
-[//]: # (```python)
+- Server
 
-[//]: # ()
-[//]: # (```)
+```python
+from retrievals.tools.langchain import LangchainEmbedding, LangchainReranker
+from langchain.retrievers import ContextualCompressionRetriever
+from langchain_community.vectorstores import Chroma as Vectorstore
+
+
+class DenseRetrieval:
+    def __init__(self, persist_directory):
+        embeddings = LangchainEmbedding(model_name="BAAI/bge-large-zh-v1.5")
+        vectordb = Vectorstore(
+            persist_directory=persist_directory,
+            embedding_function=embeddings,
+        )
+        retrieval_args = {"search_type" :"similarity", "score_threshold": 0.15, "k": 30}
+        self.retriever = vectordb.as_retriever(retrieval_args)
+
+        reranker_args = {
+            "model": "../../inputs/bce-reranker-base_v1",
+            "top_n": 7,
+            "device": "cuda",
+            "use_fp16": True,
+        }
+        self.reranker = LangchainReranker(**reranker_args)
+        self.compression_retriever = ContextualCompressionRetriever(
+            base_compressor=self.reranker, base_retriever=self.retriever
+        )
+
+    def query(
+        self,
+        question: str
+    ):
+        docs = self.compression_retriever.get_relevant_documents(question)
+        return docs
+```
 
 [//]: # (**RAG with LLamaIndex**)
 
+[//]: # ()
 [//]: # (```shell)
 
 [//]: # (pip install llamaindex)
 
 [//]: # (```)
 
 [//]: # ()
+[//]: # ()
 [//]: # (```python)
 
 [//]: # ()
+[//]: # ()
 [//]: # (```)
 
+**Use Pretrained sentence embedding**
+```python
+from retrievals import AutoModelForEmbedding
+
+sentences = ["Hello world", "How are you?"]
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path, pooling_method="mean", normalize_embeddings=True)
+sentence_embeddings = model.encode(sentences, convert_to_tensor=True)
+print(sentence_embeddings)
+```
+
+
+**Finetune transformers by contrastive learning**
+```python
+from transformers import AutoTokenizer
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval, RetrievalTrainer, PairCollator, TripletCollator
+from retrievals.losses import ArcFaceAdaptiveMarginLoss, InfoNCE, SimCSE, TripletLoss
+from retrievals.data import  RetrievalDataset, RerankDataset
+
+
+train_dataset = RetrievalDataset(args=data_args)
+tokenizer = AutoTokenizer.from_pretrained(model_args.tokenizer_name, use_fast=False)
+
+model = AutoModelForEmbedding(
+    model_args.model_name_or_path,
+    pooling_method="cls"
+)
+optimizer = get_optimizer(model, lr=5e-5, weight_decay=1e-3)
+
+lr_scheduler = get_scheduler(optimizer, num_train_steps=int(len(train_dataset) / 2 * 1))
+
+trainer = RetrievalTrainer(
+    model=model,
+    args=training_args,
+    train_dataset=train_dataset,
+    data_collator=TripletCollator(tokenizer, max_length=data_args.query_max_len),
+    loss_fn=TripletLoss(),
+)
+trainer.optimizer = optimizer
+trainer.scheduler = lr_scheduler
+trainer.train()
+```
+
+**Finetune LLM for embedding by Contrastive learning**
+```python
+
+from retrievals import AutoModelForEmbedding
+
+model = AutoModelForEmbedding(
+    "mistralai/Mistral-7B-v0.1",
+    pooling_method='cls',
+    query_instruction=f'Instruct: Retrieve semantically similar text\nQuery: '
+)
+```
+
+**Search by Cosine similarity/KNN**
+```python
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
+
+query_texts = ['A dog is chasing car.']
+passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path)
+query_embeddings = model.encode(query_texts, convert_to_tensor=True)
+passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
+
+matcher = AutoModelForRetrieval(method='cosine')
+dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
+```
 
 ## Reference & Acknowledge
 - [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
 - [FlagEmbedding](https://github.com/FlagOpen/FlagEmbedding)
 - [uniem](https://github.com/wangyuxinwhy/uniem)
 - [BCEmbedding](https://github.com/netease-youdao/BCEmbedding)
-
-
```

### Comparing `open-retrievals-0.0.1/setup.cfg` & `open-retrievals-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/setup.py` & `open-retrievals-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/open_retrievals.egg-info/PKG-INFO` & `open-retrievals-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-retrievals
-Version: 0.0.1
+Version: 0.0.2
 Summary: Text Embeddings for Retrieval and RAG based on transformers
 Home-page: https://github.com/LongxingTan/open-retrievals
 Author: Longxing Tan
 Author-email: tanlongxing888@163.com
 License: Apache 2.0 License
 Keywords: NLP retrieval RAG rerank text embedding contrastive
 Platform: UNKNOWN
@@ -57,15 +57,15 @@
 
 
 ## Installation
 
 **Prerequisites**
 ```shell
 pip install transformers
-pip install faiss
+pip install faiss-cpu
 pip install peft
 ```
 
 **With pip**
 ```shell
 pip install open-retrievals
 ```
@@ -74,96 +74,46 @@
 
 [//]: # (```shell)
 
 [//]: # (conda install open-retrievals -c conda-forge)
 
 [//]: # (```)
 
+## Quick-start
 
-## Usage
-
-**Use Pretrained sentence embedding**
-```python
-from retrievals import AutoModelForEmbedding
-
-sentences = ["Hello world", "How are you?"]
-model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
-model = AutoModelForEmbedding(model_name_or_path, pooling_method="mean", normalize_embeddings=True)
-sentence_embeddings = model.encode(sentences, convert_to_tensor=True)
-print(sentence_embeddings)
-```
-
-**Finetune transformers by contrastive learning**
 ```python
-from transformers import AutoTokenizer
-from retrievals import AutoModelForEmbedding, AutoModelForMatch, RetrievalTrainer, PairCollator, TripletCollator
-from retrievals.losses import ArcFaceAdaptiveMarginLoss, InfoNCE, SimCSE, TripletLoss
-from retrievals.data import  RetrievalDataset, RerankDataset
-
-
-train_dataset = RetrievalDataset(args=data_args)
-tokenizer = AutoTokenizer.from_pretrained(model_args.tokenizer_name, use_fast=False)
-
-model = AutoModelForEmbedding(
-    model_args.model_name_or_path,
-    pooling_method="cls"
-)
-optimizer = get_optimizer(model, lr=5e-5, weight_decay=1e-3)
-
-lr_scheduler = get_scheduler(optimizer, num_train_steps=int(len(train_dataset) / 2 * 1))
-
-trainer = RetrievalTrainer(
-    model=model,
-    args=training_args,
-    train_dataset=train_dataset,
-    data_collator=TripletCollator(tokenizer, max_length=data_args.query_max_len),
-    loss_fn=TripletLoss(),
-)
-trainer.optimizer = optimizer
-trainer.scheduler = lr_scheduler
-trainer.train()
-```
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
-**Finetune LLM for embedding by Contrastive learning**
-```python
+# Example list of documents
+documents = [
+    "Open-retrievals is a text embedding libraries",
+    "I can use it simply with a SOTA RAG application.",
+]
 
-from retrievals import AutoModelForEmbedding
+# This will trigger the model download and initialization
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path)
 
-model = AutoModelForEmbedding(
-    "mistralai/Mistral-7B-v0.1",
-    pooling_method='cls',
-    query_instruction=f'Instruct: Retrieve semantically similar text\nQuery: '
-)
+embeddings = model.encode(documents)
+len(embeddings) # Vector of 384 dimensions
 ```
 
-**Search by Cosine similarity/KNN**
-```python
-from retrievals import AutoModelForEmbedding, AutoModelForMatch
-
-query_texts = ['A dog is chasing car.']
-passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
-model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
-model = AutoModelForEmbedding('')
-query_embeddings = model.encode(query_texts, convert_to_tensor=True)
-passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
 
-matcher = AutoModelForMatch(method='cosine')
-dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
-```
+## Usage
 
-**Search by Faiss**
+**Build Index and Retrieval**
 ```python
-from retrievals import AutoModelForEmbedding, AutoModelForMatch
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
 sentences = ['A dog is chasing car.', 'A man is playing a guitar.']
 model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
 model = AutoModelForEmbedding(model_name_or_path)
 model.build_index(sentences)
 
-matcher = AutoModelForMatch()
+matcher = AutoModelForRetrieval()
 results = matcher.faiss_search("He plays guitar.")
 ```
 
 **Rerank**
 ```python
 from transformers import AutoTokenizer
 from retrievals import RerankCollator, RerankModel, RerankTrainer, RerankDataset
@@ -186,47 +136,147 @@
     data_collator=RerankCollator(tokenizer, max_length=data_args.query_max_len),
 )
 trainer.optimizer = optimizer
 trainer.scheduler = lr_scheduler
 trainer.train()
 ```
 
-[//]: # (**RAG with LangChain**)
-
-[//]: # ()
-[//]: # (- Prerequisites)
+**RAG with LangChain**
 
-[//]: # (```shell)
 
-[//]: # (pip install langchain)
+- Prerequisites
 
-[//]: # (```)
+```shell
+pip install langchain
+```
 
-[//]: # ()
-[//]: # (- Server)
 
-[//]: # (```python)
+- Server
 
-[//]: # ()
-[//]: # (```)
+```python
+from retrievals.tools.langchain import LangchainEmbedding, LangchainReranker
+from langchain.retrievers import ContextualCompressionRetriever
+from langchain_community.vectorstores import Chroma as Vectorstore
+
+
+class DenseRetrieval:
+    def __init__(self, persist_directory):
+        embeddings = LangchainEmbedding(model_name="BAAI/bge-large-zh-v1.5")
+        vectordb = Vectorstore(
+            persist_directory=persist_directory,
+            embedding_function=embeddings,
+        )
+        retrieval_args = {"search_type" :"similarity", "score_threshold": 0.15, "k": 30}
+        self.retriever = vectordb.as_retriever(retrieval_args)
+
+        reranker_args = {
+            "model": "../../inputs/bce-reranker-base_v1",
+            "top_n": 7,
+            "device": "cuda",
+            "use_fp16": True,
+        }
+        self.reranker = LangchainReranker(**reranker_args)
+        self.compression_retriever = ContextualCompressionRetriever(
+            base_compressor=self.reranker, base_retriever=self.retriever
+        )
+
+    def query(
+        self,
+        question: str
+    ):
+        docs = self.compression_retriever.get_relevant_documents(question)
+        return docs
+```
 
 [//]: # (**RAG with LLamaIndex**)
 
+[//]: # ()
 [//]: # (```shell)
 
 [//]: # (pip install llamaindex)
 
 [//]: # (```)
 
 [//]: # ()
+[//]: # ()
 [//]: # (```python)
 
 [//]: # ()
+[//]: # ()
 [//]: # (```)
 
+**Use Pretrained sentence embedding**
+```python
+from retrievals import AutoModelForEmbedding
+
+sentences = ["Hello world", "How are you?"]
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path, pooling_method="mean", normalize_embeddings=True)
+sentence_embeddings = model.encode(sentences, convert_to_tensor=True)
+print(sentence_embeddings)
+```
+
+
+**Finetune transformers by contrastive learning**
+```python
+from transformers import AutoTokenizer
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval, RetrievalTrainer, PairCollator, TripletCollator
+from retrievals.losses import ArcFaceAdaptiveMarginLoss, InfoNCE, SimCSE, TripletLoss
+from retrievals.data import  RetrievalDataset, RerankDataset
+
+
+train_dataset = RetrievalDataset(args=data_args)
+tokenizer = AutoTokenizer.from_pretrained(model_args.tokenizer_name, use_fast=False)
+
+model = AutoModelForEmbedding(
+    model_args.model_name_or_path,
+    pooling_method="cls"
+)
+optimizer = get_optimizer(model, lr=5e-5, weight_decay=1e-3)
+
+lr_scheduler = get_scheduler(optimizer, num_train_steps=int(len(train_dataset) / 2 * 1))
+
+trainer = RetrievalTrainer(
+    model=model,
+    args=training_args,
+    train_dataset=train_dataset,
+    data_collator=TripletCollator(tokenizer, max_length=data_args.query_max_len),
+    loss_fn=TripletLoss(),
+)
+trainer.optimizer = optimizer
+trainer.scheduler = lr_scheduler
+trainer.train()
+```
+
+**Finetune LLM for embedding by Contrastive learning**
+```python
+
+from retrievals import AutoModelForEmbedding
+
+model = AutoModelForEmbedding(
+    "mistralai/Mistral-7B-v0.1",
+    pooling_method='cls',
+    query_instruction=f'Instruct: Retrieve semantically similar text\nQuery: '
+)
+```
+
+**Search by Cosine similarity/KNN**
+```python
+from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
+
+query_texts = ['A dog is chasing car.']
+passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
+model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
+model = AutoModelForEmbedding(model_name_or_path)
+query_embeddings = model.encode(query_texts, convert_to_tensor=True)
+passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
+
+matcher = AutoModelForRetrieval(method='cosine')
+dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
+```
 
 ## Reference & Acknowledge
 - [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
 - [FlagEmbedding](https://github.com/FlagOpen/FlagEmbedding)
 - [uniem](https://github.com/wangyuxinwhy/uniem)
 - [BCEmbedding](https://github.com/netease-youdao/BCEmbedding)
```

### Comparing `open-retrievals-0.0.1/src/open_retrievals.egg-info/SOURCES.txt` & `open-retrievals-0.0.2/src/open_retrievals.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,37 @@
 src/retrievals/data/__init__.py
 src/retrievals/data/collator.py
 src/retrievals/data/dataset.py
 src/retrievals/data/sampler.py
 src/retrievals/losses/__init__.py
 src/retrievals/losses/arcface.py
 src/retrievals/losses/bce.py
+src/retrievals/losses/bpr.py
 src/retrievals/losses/circle.py
 src/retrievals/losses/cosent.py
 src/retrievals/losses/cosine_similarity.py
 src/retrievals/losses/dice.py
 src/retrievals/losses/focal_loss.py
 src/retrievals/losses/infonce.py
+src/retrievals/losses/margin_mse.py
+src/retrievals/losses/pearson_loss.py
 src/retrievals/losses/r_drop.py
 src/retrievals/losses/simcse.py
 src/retrievals/losses/triplet.py
+src/retrievals/metrics/__init__.py
+src/retrievals/metrics/mrr.py
 src/retrievals/models/__init__.py
 src/retrievals/models/embedding_auto.py
-src/retrievals/models/match_auto.py
 src/retrievals/models/pooling.py
 src/retrievals/models/rag.py
 src/retrievals/models/rerank.py
+src/retrievals/models/retrieval_auto.py
 src/retrievals/tools/__init__.py
 src/retrievals/tools/corpus_processor.py
 src/retrievals/tools/langchain.py
 src/retrievals/tools/llama_index.py
 src/retrievals/tools/parser.py
 src/retrievals/tools/prompter.py
-src/retrievals/tools/web_retrievals.py
 src/retrievals/trainer/__init__.py
 src/retrievals/trainer/adversarial.py
 src/retrievals/trainer/custom_trainer.py
 src/retrievals/trainer/trainer.py
```

### Comparing `open-retrievals-0.0.1/src/retrievals/__init__.py` & `open-retrievals-0.0.2/src/retrievals/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from src.retrievals.data.collator import PairCollator, RerankCollator, TripletCollator
 from src.retrievals.data.dataset import RerankDataset, RetrievalDataset
 from src.retrievals.models.embedding_auto import AutoModelForEmbedding, PairwiseModel
-from src.retrievals.models.match_auto import AutoModelForMatch
 from src.retrievals.models.pooling import AutoPooling
 from src.retrievals.models.rerank import RerankModel
+from src.retrievals.models.retrieval_auto import AutoModelForRetrieval
 from src.retrievals.trainer.custom_trainer import CustomTrainer
 from src.retrievals.trainer.trainer import RerankTrainer, RetrievalTrainer
```

### Comparing `open-retrievals-0.0.1/src/retrievals/data/collator.py` & `open-retrievals-0.0.2/src/retrievals/data/collator.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,21 +147,24 @@
         else:
             self.query_max_length = tokenizer.model_max_length
             self.passage_max_length = tokenizer.model_max_length
 
         if passage_max_length:
             self.passage_max_length = passage_max_length
 
-    def __call__(self, features: List[Dict[str, Any]]) -> BatchEncoding:
-        assert (
-            'query' in features and 'passage' in features
-        ), "RerankCollator should have 'query' and 'passage' keys in features dict, and 'labels' during training"
-
-        query_texts = [feature["query"] for feature in features]
-        passage_texts = [feature['passage'] for feature in features]
+    def __call__(self, features: Union[List[Dict[str, Any]], List]) -> BatchEncoding:
+        if isinstance(features[0], dict):
+            assert (
+                'query' in features[0] and 'passage' in features[0]
+            ), "RerankCollator should have 'query' and 'passage' keys in features dict, and 'labels' during training"
+            query_texts = [feature["query"] for feature in features]
+            passage_texts = [feature['passage'] for feature in features]
+        else:
+            query_texts = [feature[0] for feature in features]
+            passage_texts = [feature[1] for feature in features]
 
         labels = None
         if 'labels' in features[0].keys():
             labels = [feature['labels'] for feature in features]
 
         batch = self.tokenizer(
             text=query_texts, text_pair=passage_texts, truncation=True, max_length=self.max_length, return_tensors="pt"
```

### Comparing `open-retrievals-0.0.1/src/retrievals/data/dataset.py` & `open-retrievals-0.0.2/src/retrievals/data/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 import os
 import random
 from dataclasses import dataclass
 from typing import Iterable, List, Tuple
 
 import datasets
 from torch.utils.data import Dataset
 from transformers import DataCollatorWithPadding, PreTrainedTokenizer
 
+logger = logging.getLogger(__name__)
+
 
 class RetrievalDataset(Dataset):
     def __init__(self, args):
         self.args = args
         if os.path.isdir(args.data_dir):
             train_datasets = []
             for file in os.listdir(args.data_dir):
@@ -23,14 +26,15 @@
 
                 train_datasets.append(temp_dataset)
             self.dataset = datasets.concatenate_datasets(train_datasets)
         else:
             self.dataset = datasets.load_dataset("json", data_files=args.train_data, split="train")
 
         # self.tokenizer = tokenizer
+        logger.info("Loaded {} retrieval data.".format(len(self.dataset)))
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, item):
         query = self.dataset[item]["query"]
         if isinstance(self.dataset[item]["pos"], Iterable):
@@ -59,14 +63,16 @@
                 )
 
                 train_datasets.append(temp_dataset)
             self.dataset = datasets.concatenate_datasets(train_datasets)
         else:
             self.dataset = datasets.load_dataset("json", data_files=args.train_data, split="train")
 
+        logger.info("Loaded {} rerank data.".format(len(self.dataset)))
+
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, item):
         query = self.dataset[item]["query"]
         passage = self.dataset[item]['passage']
         labels = self.dataset[item]['labels']
```

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/arcface.py` & `open-retrievals-0.0.2/src/retrievals/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/bce.py` & `open-retrievals-0.0.2/src/retrievals/losses/bce.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
         bce = 1 * bce1 * labels + bce2 * (1 - labels)
         if mask is not None:
             # mask = torch.where(targets >= 0, torch.ones_like(bce), torch.zeros_like(bce))
             bce = bce * mask
 
         if sample_weight is not None:
             bce = bce * sample_weight.unsqueeze(1)
-        loss = torch.sum(bce, dim=1) / torch.sum(mask, dim=1)
+        loss = torch.sum(bce, dim=1)  # / torch.sum(mask, dim=1)
         loss = loss.mean()
         return loss
```

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/cosine_similarity.py` & `open-retrievals-0.0.2/src/retrievals/losses/cosine_similarity.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import torch
 from torch import nn
 
 logger = logging.getLogger(__name__)
 
 
 class CosineSimilarity(nn.Module):
-    def __init__(self, temperature: float = 0.0):
+    def __init__(self, temperature: float = 0.0, dynamic_temperature=False):
         super().__init__()
         self.temperature = temperature
+        self.dynamic_temperature = dynamic_temperature
 
     def forward(self, query_embeddings: torch.Tensor, passage_embeddings: torch.Tensor):
         sim_pos_vector = torch.cosine_similarity(query_embeddings, passage_embeddings, dim=-1)
         sim_pos_vector = sim_pos_vector / self.temperature
         sim_neg_matrix = torch.cosine_similarity(
             query_embeddings.unsqueeze(1),
             passage_embeddings.unsqueeze(0),
```

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/focal_loss.py` & `open-retrievals-0.0.2/src/retrievals/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/infonce.py` & `open-retrievals-0.0.2/src/retrievals/losses/infonce.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/r_drop.py` & `open-retrievals-0.0.2/src/retrievals/losses/r_drop.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/simcse.py` & `open-retrievals-0.0.2/src/retrievals/losses/simcse.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/losses/triplet.py` & `open-retrievals-0.0.2/src/retrievals/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/models/embedding_auto.py` & `open-retrievals-0.0.2/src/retrievals/models/embedding_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Callable, Dict, Iterable, List, Literal, Optional, Tuple, Union
 
 import faiss
 import numpy as np
 import torch
 import torch.nn as nn
 from numpy import ndarray
-from torch.utils.data import DataLoader, Dataset
+from torch.utils.data import DataLoader
 from tqdm.autonotebook import trange
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoTokenizer,
     BatchEncoding,
     GenerationConfig,
@@ -49,15 +49,15 @@
             print(batch[key])
             batch[key] = torch.tensor(batch[key], dtype=torch.long).to(target_device)
     return batch
 
 
 class AutoModelForEmbedding(nn.Module):
     """
-    Loads or creates a Embedding model that can be used to map sentences / text.
+    Loads or creates an Embedding model that can be used to map sentences / text.
 
     :param model_name_or_path: If it is a filepath on disc, it loads the model from that path. If it is not a path,
         it first tries to download a pre-trained SentenceTransformer model. If that fails, tries to construct a model
         from the Hugging Face Hub with that name.
     """
 
     encode_kwargs: Dict[str, Any] = dict()
@@ -75,15 +75,15 @@
         query_instruction: Optional[str] = None,
         passage_instruction: Optional[str] = None,
         generation_args: Dict = None,
         use_fp16: bool = False,
         use_lora: bool = False,
         lora_config=None,
         device: Optional[str] = None,
-        trust_remote_code: bool = False,
+        trust_remote_code: bool = True,
     ):
         super().__init__()
 
         self.tokenizer = AutoTokenizer.from_pretrained(
             model_name_or_path, return_tensors=False, trust_remote_code=trust_remote_code
         )
 
@@ -197,24 +197,24 @@
         batch_dict["input_ids"] = [input_ids + [self.tokenizer.eos_token_id] for input_ids in batch_dict["input_ids"]]
         batch_dict = self.tokenizer.pad(batch_dict, padding=True, return_attention_mask=True, return_tensors="pt")
         batch_dict.pop("token_type_ids")
         return self.forward_from_loader(batch_dict)
 
     def encode(
         self,
-        inputs,
-        batch_size: int = 32,
+        inputs: Union[DataLoader, Dict, List, str],
+        batch_size: int = 128,
         show_progress_bar: bool = None,
         output_value: str = "sentence_embedding",
         convert_to_numpy: bool = True,
         convert_to_tensor: bool = False,
         device: str = None,
         normalize_embeddings: bool = False,
     ):
-        if isinstance(inputs, (BatchEncoding, Dict)):
+        if isinstance(inputs, (DataLoader, BatchEncoding, Dict)):
             return self.encode_from_loader(
                 loader=inputs,
                 batch_size=batch_size,
                 show_progress_bar=show_progress_bar,
                 output_value=output_value,
                 convert_to_numpy=convert_to_numpy,
                 convert_to_tensor=convert_to_tensor,
@@ -241,47 +241,41 @@
         return embeddings.tolist()
 
     def embed_query(self, text: str) -> List[float]:
         """Compute query embeddings using a HuggingFace transformer model."""
         return self.embed_documents([text])[0]
 
     def encode_from_loader(
-        self,
-        loader,
-        batch_size: int = 32,
-        show_progress_bar: bool = None,
-        output_value: str = "sentence_embedding",
-        convert_to_numpy: bool = True,
-        convert_to_tensor: bool = False,
-        device: str = None,
-        normalize_embeddings: bool = False,
+        self, loader, convert_to_numpy: bool = True, device: str = None, normalize_embeddings: bool = False, **kwargs
     ) -> Union[List[torch.Tensor], ndarray, torch.Tensor]:
         self.model.eval()
         self.model.to(device or self.device)
         all_embeddings = []
 
         with torch.no_grad():
             for idx, inputs in enumerate(loader):
                 for k, v in inputs.items():
                     inputs[k] = v.to(self.device)
-                embed = self.forward_from_loader(inputs)
-                embed = embed.detach().cpu()
+                embeddings = self.forward_from_loader(inputs)
+                embeddings = embeddings.detach()
+                if normalize_embeddings:
+                    embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
                 if convert_to_numpy:
-                    embed = embed.numpy()
-                all_embeddings.append(embed.numpy())
+                    embeddings = embeddings.cpu()
+                all_embeddings.append(embeddings)
         if convert_to_numpy:
-            all_embeddings = np.concatenate(all_embeddings)
+            all_embeddings = np.asarray([emb.numpy() for emb in all_embeddings])
         else:
             all_embeddings = torch.concat(all_embeddings)
         return all_embeddings
 
     def encode_from_text(
         self,
         sentences: Union[str, List[str]],
-        batch_size: int = 32,
+        batch_size: int = 128,
         show_progress_bar: bool = None,
         output_value: str = "sentence_embedding",
         convert_to_numpy: bool = True,
         convert_to_tensor: bool = False,
         device: str = None,
         normalize_embeddings: bool = False,
     ) -> Union[List[torch.Tensor], ndarray, torch.Tensor]:
@@ -382,15 +376,15 @@
             all_embeddings = np.asarray([emb.numpy() for emb in all_embeddings])
 
         if input_was_string:
             all_embeddings = all_embeddings[0]
 
         return all_embeddings
 
-    def build_index(self, inputs: BatchEncoding, batch_size: int = 64, use_gpu: bool = True):
+    def build_index(self, inputs: BatchEncoding, batch_size: int = 128, use_gpu: bool = True):
         embeddings = self.encode(inputs, batch_size=batch_size)
         embeddings = np.asarray(embeddings, dtype=np.float32)
         index = faiss.IndexFlatL2(len(embeddings[0]))
         if use_gpu:
             co = faiss.GpuMultipleClonerOptions()
             co.shard = True
             co.useFloat16 = True
@@ -403,16 +397,24 @@
 
     def search(self):
         return
 
     def similarity(self, queries: Union[str, List[str]], keys: Union[str, List[str], ndarray]):
         return
 
-    def save(self):
-        pass
+    def save(self, path: str):
+        """
+        Saves all model and tokenizer to path
+        """
+        if path is None:
+            return
+
+        logger.info("Save model to {}".format(path))
+        self.model.save_pretrained(path)
+        self.tokenizer.save_pretrained(path)
 
     @classmethod
     def from_pretrained(cls, model_name_or_path: str, **kwargs):
         embedder = AutoModel.from_pretrained(model_name_or_path)
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
         return cls(embedder, tokenizer, **kwargs)
```

### Comparing `open-retrievals-0.0.1/src/retrievals/models/match_auto.py` & `open-retrievals-0.0.2/src/retrievals/models/retrieval_auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,96 @@
 import logging
-from typing import Union
+from typing import Optional, Union
 
 import faiss
 import numpy as np
+import pandas as pd
 import torch
 from sklearn.neighbors import NearestNeighbors
 from tqdm import tqdm
+from tqdm.autonotebook import trange
 
 logger = logging.getLogger(__name__)
 
 
-class AutoModelForMatch(object):
+class AutoModelForRetrieval(object):
     def __init__(self, method: str = "cosine") -> None:
         super().__init__()
         self.method = method
 
     def similarity_search(
         self,
         query_embed: torch.Tensor,
-        passage_embed: torch.Tensor,
+        passage_embed: Optional[torch.Tensor] = None,
+        index_path: Optional[str] = None,
         top_k: int = 1,
-        batch_size: int = 0,
+        batch_size: int = -1,
         convert_to_numpy: bool = True,
+        convert_to_pandas: bool = False,
         **kwargs,
     ):
-        if self.method == "knn":
+        if passage_embed is None and index_path is None:
+            logging.warning('Please provide passage_embed for knn/tensor search or index_path for faiss search')
+            return
+        if index_path is not None:
+            faiss_index = faiss.read_index(index_path)
+            dists, indices = faiss_search(
+                query_embeddings=query_embed,
+                faiss_index=faiss_index,
+                top_k=top_k,
+                batch_size=batch_size,
+            )
+
+        elif self.method == "knn":
             neighbors_model = NearestNeighbors(n_neighbors=top_k, metric="cosine", n_jobs=-1)
             neighbors_model.fit(passage_embed)
             dists, indices = neighbors_model.kneighbors(query_embed)
-            return dists, indices
 
         elif self.method == "cosine":
             dists, indices = cosine_similarity_search(
                 query_embed, passage_embed, top_k=top_k, batch_size=batch_size, convert_to_numpy=convert_to_numpy
             )
-            return dists, indices
 
         else:
             raise ValueError(f"Only cosine and knn method are supported by similarity_search, while get {self.method}")
 
-    def faiss_search(
-        self,
-        query_embed: torch.Tensor,
-        index_path: str = "/faiss.index",
-        top_k: int = 1,
-        batch_size: int = 256,
-        max_length: int = 512,
-    ):
-        faiss_index = faiss.read_index(index_path)
-        dists, indices = faiss_search(
-            query_embeddings=query_embed,
-            faiss_index=faiss_index,
-            top_k=top_k,
-            batch_size=batch_size,
-        )
-        return dists, indices
-
-    def get_match_df(self):
-        rerank_data = dict({'query': [], 'passage': [], 'labels': []})
-        return rerank_data
+        if not convert_to_pandas:
+            return dists, indices
+
+        retrieval = dict({'query': [], 'passage': [], 'labels': []})
+        return pd.from_dict(retrieval)
+
+
+class EnsembleRetriever(object):
+    def __init__(self, retrievers, weights=None):
+        pass
 
 
 def cosine_similarity_search(
     query_embed: torch.Tensor,
     passage_embed: torch.Tensor,
     top_k: int = 1,
-    batch_size: int = 512,
+    batch_size: int = 128,
     penalty: bool = True,
     temperature: float = 0,
     convert_to_numpy: bool = True,
+    show_progress_bar: bool = None,
 ):
     if len(query_embed.size()) == 1:
         query_embed = query_embed.view(1, -1)
     assert query_embed.size()[1] == passage_embed.size()[1], (
         f"The embed Shape of query_embed and passage_embed should be same, "
         f"while received query {query_embed.size()} and passage {passage_embed.size()}"
     )
     chunk = batch_size if batch_size > 0 else len(query_embed)
     embeddings_chunks = query_embed.split(chunk)
 
     dists = []
     indices = []
-    for idx in range(len(embeddings_chunks)):
+    for idx in trange(0, len(embeddings_chunks), desc="Batches", disable=not show_progress_bar):
         cos_sim_chunk = torch.matmul(embeddings_chunks[idx], passage_embed.transpose(0, 1))
         cos_sim_chunk = torch.nan_to_num(cos_sim_chunk, nan=0.0)
         # if penalty:
         #     pen = ((contents["old_source_count"].values==0) & (contents["old_nonsource_count"].values==1))
         #     cos_sim_chunk = cos_sim_chunk.clamp(0,1) ** torch.Tensor((1 + pen*0.5).reshape(1,-1)).to(DEVICE)
         #     cos_sim_chunk = cos_sim_chunk.clamp(0,1) ** torch.Tensor((1-(contents["old_count"].values==0)*0.1).
         #     reshape(1,-1)).to(DEVICE)
@@ -103,15 +108,15 @@
     return dists, indices
 
 
 def faiss_search(
     query_embeddings,
     faiss_index: faiss.Index,
     top_k: int = 100,
-    batch_size: int = 256,
+    batch_size: int = 128,
     max_length: int = 512,
 ):
     """
     1. Encode queries into dense embeddings;
     2. Search through faiss index
     """
     # query_embeddings = model.encode_queries(
```

### Comparing `open-retrievals-0.0.1/src/retrievals/models/pooling.py` & `open-retrievals-0.0.2/src/retrievals/models/pooling.py`

 * *Files 11% similar despite different names*

```diff
@@ -170,7 +170,41 @@
         self.eps = eps
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         return F.adaptive_avg_pool2d(x.clamp(min=self.eps).pow(self.p), self.size).pow(1.0 / self.p)
 
     def __repr__(self):
         return f"AdaptiveGeM(size={self.size}, p={self.p}, eps={self.eps})"
+
+
+class TopKPooling(nn.Module):
+    def __init__(self):
+        super().__init__()
+
+    def forward(self):
+        return
+
+
+class SumPooling(nn.Module):
+    def forward(self, x, x_mask=None):
+        if x_mask is None or x_mask.data.sum() == 0:
+            return torch.sum(x, 1)
+        else:
+            x_mask = x_mask.unsqueeze(-1).expand(x.size())
+            x.data.masked_fill_(x_mask.data, 0.0)
+            return torch.sum(x, 1)
+
+
+class FMPooling(nn.Module):
+    def __init__(self):
+        super(FMPooling, self).__init__()
+        self.sum_pooling = SumPooling()
+
+    def forward(self, x, x_mask=None):
+        summed_emb = self.sum_pooling(x, x_mask)
+        summed_emb_square = summed_emb**2
+
+        squared_emb = x**2
+        squared_sum_emb = self.sum_pooling(squared_emb, x_mask)
+
+        y_second_order = 0.5 * (summed_emb_square - squared_sum_emb)
+        return y_second_order
```

### Comparing `open-retrievals-0.0.1/src/retrievals/models/rag.py` & `open-retrievals-0.0.2/src/retrievals/models/rag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, TypeVar, Union
 
 from transformers import AutoModel
 
+logger = logging.getLogger(__name__)
 
-class RAG(object):
+
+class SimpleRAG(object):
     def __init__(self):
         pass
 
     @classmethod
     def from_pretrained(
         cls,
         model_name_or_path: Union[str, Path],
@@ -38,9 +41,18 @@
         return
 
     def search(self):
         return
 
 
 class Generator(object):
-    def __init__(self):
+    def __init__(self, config_path: str):
+        self.config_path = config_path
+
+    def _load_config(self):
+        # with open(self.config_path, encoding='utf8') as f:
+        #     config = pytoml.load(f)
+        #     return config['llm']
+        pass
+
+    def generate(self, prompt, history=None, remote=False):
         pass
```

### Comparing `open-retrievals-0.0.1/src/retrievals/models/rerank.py` & `open-retrievals-0.0.2/src/retrievals/models/rerank.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import logging
 from typing import Callable, Dict, List, Optional, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
-from transformers import AutoConfig, AutoModel, AutoTokenizer
+from transformers import (
+    AutoConfig,
+    AutoModel,
+    AutoModelForSequenceClassification,
+    AutoTokenizer,
+)
 
 from src.retrievals.data.collator import RerankCollator
 from src.retrievals.models.embedding_auto import get_device_name
 from src.retrievals.models.pooling import AutoPooling
 
 logger = logging.getLogger(__name__)
 
@@ -29,15 +34,17 @@
         **kwargs,
     ):
         super().__init__()
         self.tokenizer = AutoTokenizer.from_pretrained(
             model_name_or_path, return_tensors=False, trust_remote_code=trust_remote_code
         )
 
-        self.model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code)
+        self.model = AutoModelForSequenceClassification.from_pretrained(
+            model_name_or_path, trust_remote_code=trust_remote_code
+        )
         if gradient_checkpointing:
             self.model.graident_checkpointing_enable()
         if device is None:
             self.device = get_device_name()
         else:
             self.device = device
 
@@ -49,17 +56,17 @@
 
             if not lora_config:
                 raise ValueError("If use_lora is true, please provide a valid lora_config")
             self.model = get_peft_model(self.model, lora_config)
             self.model.print_trainable_parameters()
 
         self.pooling = AutoPooling(pooling_method)
-        num_features = self.backbone.config.hidden_size
+        num_features = self.model.config.hidden_size
         self.classifier = nn.Linear(num_features, 1)
-        self._init_weights(self.classifier)
+        # self._init_weights(self.classifier)
         self.loss_fn = loss_fn
 
         if max_length is None:
             if (
                 hasattr(self.model, "config")
                 and hasattr(self.model.config, "max_position_embeddings")
                 and hasattr(self.tokenizer, "model_max_length")
@@ -94,26 +101,31 @@
         labels: Optional[torch.Tensor] = None,
         return_dict: Optional[bool] = False,
         **kwargs,
     ) -> Union[Dict[str, torch.Tensor], torch.Tensor]:
         features = self.encode(input_ids=input_ids, attention_mask=attention_mask)
         logits = self.classifier(features).reshape(-1)
 
+        if return_dict:
+            outputs_dict = dict()
+            outputs_dict['logits'] = logits
+
         if labels is not None:
             if not self.loss_fn:
                 logger.warning('loss_fn is not setup, use BCEWithLogitsLoss')
                 self.loss_fn = nn.BCEWithLogitsLoss(reduction='mean')
 
-        loss = self.loss_fn(logits, labels)
-        if return_dict:
-            outputs_dict = dict()
-            outputs_dict['loss'] = loss
-            outputs_dict['logits'] = logits
-            return outputs_dict
-        return loss
+            loss = self.loss_fn(logits, labels)
+            if return_dict:
+                outputs_dict['loss'] = loss
+                return outputs_dict
+            else:
+                return logits, loss
+        else:
+            return logits
 
     def compute_score(
         self,
         text: Union[List[str], str],
         text_pair: Union[List[str], str],
         data_collator: Optional[RerankCollator] = None,
         batch_size: int = 128,
@@ -121,53 +133,59 @@
         **kwargs,
     ):
         if isinstance(text, str):
             text = [text]
         if isinstance(text_pair, str):
             text_pair = [text_pair]
         assert len(text) == len(text_pair), f"Length of text {len(text)} and text_pair {len(text_pair)} should be same"
+        batch_size = min(batch_size, len(text))
 
         if not data_collator:
             data_collator = RerankCollator(tokenizer=self.tokenizer)
 
         with torch.no_grad():
             scores_list: List = []
             for i in range(0, len(text), batch_size):
                 text_batch = [{'query': text[i], 'passage': text_pair[i]} for i in range(i, i + batch_size)]
                 batch = data_collator(text_batch)
-                scores = self.model(batch, return_dict=True).logits.view(-1).float()
+                scores = (
+                    self.model(batch['input_ids'], batch['attention_mask'], return_dict=True).logits.view(-1).float()
+                )
                 scores = torch.sigmoid(scores)
                 scores_list.extend(scores.cpu().numpy().tolist())
 
         return scores_list
 
     def rerank(
         self,
         query: Union[List[str], str],
         passages: List[str],
         data_collator: Optional[RerankCollator] = None,
         batch_size: int = 32,
         show_progress_bar: bool = None,
+        return_dict: bool = True,
         **kwargs,
     ):
-
         merge_scores = self.compute_score(query, passages, data_collator, batch_size, show_progress_bar)
 
         merge_scores_argsort = np.argsort(merge_scores)[::-1]
         sorted_passages = []
         sorted_scores = []
         for mid in merge_scores_argsort:
             sorted_scores.append(merge_scores[mid])
             sorted_passages.append(passages[mid])
 
-        return {
-            'rerank_passages': sorted_passages,
-            'rerank_scores': sorted_scores,
-            'rerank_ids': merge_scores_argsort.tolist(),
-        }
+        if return_dict:
+            return {
+                'rerank_passages': sorted_passages,
+                'rerank_scores': sorted_scores,
+                'rerank_ids': merge_scores_argsort.tolist(),
+            }
+        else:
+            return sorted_passages
 
     def save(self, path: str):
         """
         Saves all model and tokenizer to path
         """
         if path is None:
             return
```

### Comparing `open-retrievals-0.0.1/src/retrievals/tools/langchain.py` & `open-retrievals-0.0.2/src/retrievals/tools/langchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,12 +88,7 @@
             final_results.append(doc)
         for doc in invalid_doc_list:
             doc.metadata["relevance_score"] = 0
             final_results.append(doc)
 
         final_results = final_results[: self.top_n]
         return final_results
-
-
-class RagFeature(object):
-    def __init__(self, config_path: str = 'config.ini'):
-        pass
```

### Comparing `open-retrievals-0.0.1/src/retrievals/tools/llama_index.py` & `open-retrievals-0.0.2/src/retrievals/tools/llama_index.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/tools/prompter.py` & `open-retrievals-0.0.2/src/retrievals/tools/prompter.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/trainer/adversarial.py` & `open-retrievals-0.0.2/src/retrievals/trainer/adversarial.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/trainer/custom_trainer.py` & `open-retrievals-0.0.2/src/retrievals/trainer/custom_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,22 +136,25 @@
                 ema_inst.restore()
 
     return losses.avg
 
 
 @torch.no_grad()
 def valid_fn(
+    epoch,
     valid_loader,
     model,
     criterion,
     eval_metrics=None,
     apex: bool = False,
     device="cuda",
     data_collator=None,
+    print_freq: int = 100,
 ):
+    start = time.time()
     model.eval()
     losses = AverageMeter()
     pred_array = torch.tensor([], device=device)
     label_array = np.array([])
 
     for step, (inputs, labels) in enumerate(valid_loader):
         if data_collator:
@@ -176,16 +179,33 @@
                 loss = criterion(preds, labels)
                 pred = preds
 
         losses.update(loss.item(), batch_size)
         pred_array = torch.cat((pred_array, pred), dim=0)
         label_array = np.append(label_array, np.array(labels))
 
+        if step % print_freq == 0 or step == (len(valid_loader) - 1):
+            print(
+                "Epoch: [{0}][{1}/{2}] "
+                "Elapsed {remain:s} "
+                "Loss: {loss.val:.4f}({loss.avg:.4f}) "
+                # "ACC: {acc: .4f}"
+                .format(
+                    epoch + 1,
+                    step,
+                    len(valid_loader),
+                    remain=timeSince(start, float(step + 1) / len(valid_loader)),
+                    loss=losses,
+                    # acc=np.mean(acc_list),
+                )
+            )
+
     if eval_metrics is not None:
         score = eval_metrics(label_array, pred_array)
+        print(f"Epoch {epoch}, Score: {score}")
         return losses.avg, score
 
     return losses.avg
 
 
 def inference_fn(test_loader, model, device):
     preds = []
@@ -217,32 +237,37 @@
         self,
         train_loader,
         optimizer,
         epochs=10,
         criterion=None,
         scheduler=None,
         valid_loader=None,
-        eval_metric=None,
+        eval_metrics=None,
         data_collator=None,
         max_grad_norm=10,
         **kwargs,
     ):
         # best_score = 0
         # fgm = FGM(model)
         # awp = None
         # ema_inst = EMA(model, 0.999)
         # ema_inst.register()
 
         for epoch in range(epochs):
             if "dynamic_margin" in kwargs.keys():
+                margin = min(0.1 + epoch * 0.02, 0.4)
+                logger.info(f"Epoch: {epoch}, Margin: {margin}")
                 if criterion:
-                    criterion.set_margin(0.1 + epoch * 0.02)
+                    criterion.set_margin(margin)
+                elif self.model.loss_fn is not None:
+                    self.model.loss_fn.set_margin(margin)
                 else:
-                    self.model.loss_fn.set_margin(0.1 + epoch * 0.02)
-                    logger.info(f"Epoch: {epoch}, Margin: {0.1 + epoch * 0.02}")
+                    raise ValueError(
+                        'dynamic margin is True, but criterion of trainer and loss_fn of model are both none'
+                    )
 
             # lr = scheduler(optimizer, epoch)
 
             # 放在这里, 是因为前面的set_margin也会产生新的参数位于cpu
             # 如果把参数直接放在cuda, 则导致parameter里没有出现该参数，无法分别设置学习率
             self.model = self.model.to(self.device)
             optimizer.zero_grad()
@@ -259,17 +284,19 @@
                 valid_loader=valid_loader,
                 data_collator=data_collator,
                 device=self.device,
             )
 
             if valid_loader is not None:
                 self.valid_step(
-                    valid_loader,
-                    self.model,
+                    epoch=epoch,
+                    valid_loader=valid_loader,
+                    model=self.model,
                     criterion=criterion,
+                    eval_metrics=eval_metrics,
                     apex=self.apex,
                     device=self.device,
                     data_collator=None,
                 )
 
         torch.cuda.empty_cache()
         gc.collect()
```

### Comparing `open-retrievals-0.0.1/src/retrievals/trainer/trainer.py` & `open-retrievals-0.0.2/src/retrievals/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.1/src/retrievals/version.py` & `open-retrievals-0.0.2/src/retrievals/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Longxing Tan.
 
 import sys
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 short_version = __version__
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
```

