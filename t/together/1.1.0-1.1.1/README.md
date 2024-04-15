# Comparing `tmp/together-1.1.0.tar.gz` & `tmp/together-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.1.0.tar", max compression
+gzip compressed data, was "together-1.1.1.tar", max compression
```

## Comparing `together-1.1.0.tar` & `together-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-10 23:34:18.446826 together-1.1.0/LICENSE
--rw-r--r--   0        0        0     9667 2024-04-10 23:34:18.446826 together-1.1.0/README.md
--rw-r--r--   0        0        0     2439 2024-04-10 23:34:18.446826 together-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-10 23:34:18.446826 together-1.1.0/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-04-10 23:34:18.446826 together-1.1.0/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-04-10 23:34:18.450826 together-1.1.0/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     7838 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     3691 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/files.py
--rw-r--r--   0        0        0     4954 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-04-10 23:34:18.450826 together-1.1.0/src/together/client.py
--rw-r--r--   0        0        0      908 2024-04-10 23:34:18.450826 together-1.1.0/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-04-10 23:34:18.450826 together-1.1.0/src/together/error.py
--rw-r--r--   0        0        0    11438 2024-04-10 23:34:18.450826 together-1.1.0/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0     8403 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/files.py
--rw-r--r--   0        0        0    12424 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-04-10 23:34:18.450826 together-1.1.0/src/together/together_response.py
--rw-r--r--   0        0        0     1432 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/abstract.py
--rw-r--r--   0        0        0     3630 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/common.py
--rw-r--r--   0        0        0     2173 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/error.py
--rw-r--r--   0        0        0     1954 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/files.py
--rw-r--r--   0        0        0     5779 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     7186 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-04-10 23:34:18.454826 together-1.1.0/src/together/version.py
--rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 together-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 16:35:07.303589 together-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9667 2024-04-15 16:35:07.303589 together-1.1.1/README.md
+-rw-r--r--   0        0        0     2439 2024-04-15 16:35:07.303589 together-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-15 16:35:07.303589 together-1.1.1/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-15 16:35:07.303589 together-1.1.1/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-04-15 16:35:07.303589 together-1.1.1/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     7838 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     3691 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     4954 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-04-15 16:35:07.303589 together-1.1.1/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-04-15 16:35:07.303589 together-1.1.1/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-04-15 16:35:07.303589 together-1.1.1/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-04-15 16:35:07.303589 together-1.1.1/src/together/error.py
+-rw-r--r--   0        0        0    11438 2024-04-15 16:35:07.303589 together-1.1.1/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-04-15 16:35:07.303589 together-1.1.1/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-04-15 16:35:07.303589 together-1.1.1/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0     8403 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/files.py
+-rw-r--r--   0        0        0    12424 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-04-15 16:35:07.307590 together-1.1.1/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-04-15 16:35:07.307590 together-1.1.1/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/abstract.py
+-rw-r--r--   0        0        0     3630 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/common.py
+-rw-r--r--   0        0        0     2173 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/files.py
+-rw-r--r--   0        0        0     5779 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-04-15 16:35:07.307590 together-1.1.1/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-04-15 16:35:07.307590 together-1.1.1/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-15 16:35:07.307590 together-1.1.1/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-04-15 16:35:07.307590 together-1.1.1/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7165 2024-04-15 16:35:07.307590 together-1.1.1/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-04-15 16:35:07.307590 together-1.1.1/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-04-15 16:35:07.307590 together-1.1.1/src/together/version.py
+-rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 together-1.1.1/PKG-INFO
```

### Comparing `together-1.1.0/LICENSE` & `together-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.1.0/README.md` & `together-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `together-1.1.0/pyproject.toml` & `together-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "oldest-supported-numpy>=0.14; python_version<'3.9'",
     "numpy>=1.25; python_version>='3.9'",
 ]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `together-1.1.0/src/together/__init__.py` & `together-1.1.1/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/abstract/api_requestor.py` & `together-1.1.1/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/chat.py` & `together-1.1.1/src/together/cli/api/chat.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/completions.py` & `together-1.1.1/src/together/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/files.py` & `together-1.1.1/src/together/cli/api/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/finetune.py` & `together-1.1.1/src/together/cli/api/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/images.py` & `together-1.1.1/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/api/models.py` & `together-1.1.1/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/cli/cli.py` & `together-1.1.1/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/client.py` & `together-1.1.1/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/constants.py` & `together-1.1.1/src/together/constants.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/error.py` & `together-1.1.1/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/filemanager.py` & `together-1.1.1/src/together/filemanager.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/base.py` & `together-1.1.1/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/complete.py` & `together-1.1.1/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/embeddings.py` & `together-1.1.1/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/files.py` & `together-1.1.1/src/together/legacy/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/finetune.py` & `together-1.1.1/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/images.py` & `together-1.1.1/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/legacy/models.py` & `together-1.1.1/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/__init__.py` & `together-1.1.1/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/chat/__init__.py` & `together-1.1.1/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/chat/completions.py` & `together-1.1.1/src/together/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/completions.py` & `together-1.1.1/src/together/resources/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/embeddings.py` & `together-1.1.1/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/files.py` & `together-1.1.1/src/together/resources/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/finetune.py` & `together-1.1.1/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/images.py` & `together-1.1.1/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/resources/models.py` & `together-1.1.1/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/together_response.py` & `together-1.1.1/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/__init__.py` & `together-1.1.1/src/together/types/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/abstract.py` & `together-1.1.1/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/chat_completions.py` & `together-1.1.1/src/together/types/chat_completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/common.py` & `together-1.1.1/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/completions.py` & `together-1.1.1/src/together/types/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/embeddings.py` & `together-1.1.1/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/files.py` & `together-1.1.1/src/together/types/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/finetune.py` & `together-1.1.1/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/images.py` & `together-1.1.1/src/together/types/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/types/models.py` & `together-1.1.1/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/utils/__init__.py` & `together-1.1.1/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/utils/_log.py` & `together-1.1.1/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/utils/api_helpers.py` & `together-1.1.1/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/src/together/utils/files.py` & `together-1.1.1/src/together/utils/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,19 +145,19 @@
                 )
             else:
                 report_dict["message"] = (
                     f"Error parsing json payload. Unexpected format on line {idx + 1}."
                 )
             report_dict["is_check_passed"] = False
 
-    if report_dict["text_field"] is not False:
+    if "text_field" not in report_dict:
         report_dict["text_field"] = True
-    if report_dict["line_type"] is not False:
+    if "line_type" not in report_dict:
         report_dict["line_type"] = True
-    if report_dict["key_value"] is not False:
+    if "key_value" not in report_dict:
         report_dict["key_value"] = True
     return report_dict
 
 
 def _check_parquet(file: Path) -> Dict[str, Any]:
     report_dict: Dict[str, Any] = {}
```

### Comparing `together-1.1.0/src/together/utils/tools.py` & `together-1.1.1/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.1.0/PKG-INFO` & `together-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client for Together's Cloud Platform!
 Home-page: https://github.com/togethercomputer/together-python
 License: Apache-2.0
 Author: Together AI
 Author-email: support@together.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

