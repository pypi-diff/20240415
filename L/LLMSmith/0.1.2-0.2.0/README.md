# Comparing `tmp/llmsmith-0.1.2.tar.gz` & `tmp/llmsmith-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.1.2.tar", max compression
+gzip compressed data, was "llmsmith-0.2.0.tar", max compression
```

## Comparing `llmsmith-0.1.2.tar` & `llmsmith-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.1.2/LICENSE
--rw-r--r--   0        0        0     1122 2024-04-03 10:55:28.746484 llmsmith-0.1.2/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.1.2/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.1.2/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.1.2/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.1.2/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-03-13 07:08:41.469795 llmsmith-0.1.2/llmsmith/llm/__init__.py
--rw-r--r--   0        0        0      840 2024-03-14 08:08:05.921578 llmsmith-0.1.2/llmsmith/llm/base.py
--rw-r--r--   0        0        0     4006 2024-04-03 10:52:50.577228 llmsmith-0.1.2/llmsmith/llm/claude.py
--rw-r--r--   0        0        0     4662 2024-04-03 10:53:07.060380 llmsmith-0.1.2/llmsmith/llm/gemini.py
--rw-r--r--   0        0        0      765 2024-03-15 12:55:51.327162 llmsmith-0.1.2/llmsmith/llm/models.py
--rw-r--r--   0        0        0     3548 2024-04-03 10:53:30.824465 llmsmith-0.1.2/llmsmith/llm/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.1.2/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.1.2/llmsmith/task/base.py
--rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.1.2/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.1.2/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.1.2/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0     3129 2024-04-03 10:53:39.882995 llmsmith-0.1.2/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.1.2/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.1.2/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0      649 2024-04-04 09:30:06.752488 llmsmith-0.1.2/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     4455 2024-04-04 09:30:06.752620 llmsmith-0.1.2/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     3185 2024-04-03 10:54:14.137132 llmsmith-0.1.2/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.1.2/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.1.2/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1466 2024-04-03 10:54:40.771025 llmsmith-0.1.2/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     2108 2024-04-03 10:54:48.638547 llmsmith-0.1.2/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1306 2024-04-04 09:37:14.232387 llmsmith-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 llmsmith-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1492 2024-04-15 06:09:18.276703 llmsmith-0.2.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.2.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.2.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.2.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.2.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.2.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.2.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.2.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.2.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.2.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-09 10:26:53.708807 llmsmith-0.2.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3667 2024-04-10 05:44:39.948855 llmsmith-0.2.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     4316 2024-04-11 04:01:18.457684 llmsmith-0.2.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.2.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.2.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0      649 2024-04-04 09:30:06.752488 llmsmith-0.2.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     4460 2024-04-13 10:05:58.713381 llmsmith-0.2.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     3185 2024-04-03 10:54:14.137132 llmsmith-0.2.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.2.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.2.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     1466 2024-04-03 10:54:40.771025 llmsmith-0.2.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     2108 2024-04-03 10:54:48.638547 llmsmith-0.2.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1845 2024-04-15 05:39:00.550872 llmsmith-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 llmsmith-0.2.0/PKG-INFO
```

### Comparing `llmsmith-0.1.2/LICENSE` & `llmsmith-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/job/base.py` & `llmsmith-0.2.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/job/job.py` & `llmsmith-0.2.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/base.py` & `llmsmith-0.2.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/claude.py` & `llmsmith-0.2.0/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/errors.py` & `llmsmith-0.2.0/llmsmith/task/textgen/errors.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/gemini.py` & `llmsmith-0.2.0/llmsmith/task/textgen/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             )
 
         log.debug(f"task_output value: {output_content}")
 
         return TaskOutput(content=output_content, raw_output=llm_reply)
 
     @classmethod
-    def _block_reason_str(llm_reply: GenerateContentResponse) -> str:
+    def _block_reason_str(cls, llm_reply: GenerateContentResponse) -> str:
         if (
             llm_reply.prompt_feedback.block_reason
             == llm_reply.prompt_feedback.BlockReason.SAFETY
         ):
             return "SAFETY_CHECK_FAILED"
 
         return "OTHER"
```

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/openai.py` & `llmsmith-0.2.0/llmsmith/task/textgen/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.2.0/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.2.0/llmsmith/task/textgen/options/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.2.0/llmsmith/task/textgen/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.2/pyproject.toml` & `llmsmith-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.1.2"
+version = "0.2.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.13"
 openai = {version = "^1.13.3", optional = true}
 anthropic = {version = "^0.19.2", optional = true}
 google-generativeai = {version = "^0.4.0", optional = true}
 chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
 protobuf = {version = "3.20.3", optional = true}
 tokenizers = {version = "^0.15.2", optional = true}
 python-dotenv = "^1.0.1"
+qdrant-client = {version = "^1.8.2", optional = true}
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
 chromadb = ["chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
-all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
+qdrant = ["qdrant-client"]
+all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
 black = "^24.2.0"
@@ -33,10 +42,21 @@
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.1.1"
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests"
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

