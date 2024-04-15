# Comparing `tmp/google_ai_studio_utils-0.1.1.tar.gz` & `tmp/google_ai_studio_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ai_studio_utils-0.1.1.tar", max compression
+gzip compressed data, was "google_ai_studio_utils-0.1.2.tar", max compression
```

## Comparing `google_ai_studio_utils-0.1.1.tar` & `google_ai_studio_utils-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.1/README.md
--rw-r--r--   0        0        0      187 2024-04-15 13:00:57.757722 google_ai_studio_utils-0.1.1/google_ai_studio_utils/config.py
--rwxr-xr-x   0        0        0     1275 2024-04-15 15:55:23.774983 google_ai_studio_utils-0.1.1/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
--rw-r--r--   0        0        0     1212 2024-04-15 15:53:40.501652 google_ai_studio_utils-0.1.1/google_ai_studio_utils/utils.py
--rw-r--r--   0        0        0      788 2024-04-15 16:00:00.279765 google_ai_studio_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.2/README.md
+-rw-r--r--   0        0        0      214 2024-04-15 16:21:49.454447 google_ai_studio_utils-0.1.2/google_ai_studio_utils/config.py
+-rwxr-xr-x   0        0        0     2720 2024-04-15 16:30:26.575670 google_ai_studio_utils-0.1.2/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
+-rw-r--r--   0        0        0     1744 2024-04-15 16:31:29.925728 google_ai_studio_utils-0.1.2/google_ai_studio_utils/utils.py
+-rw-r--r--   0        0        0      827 2024-04-15 16:36:29.062513 google_ai_studio_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.2/PKG-INFO
```

### Comparing `google_ai_studio_utils-0.1.1/pyproject.toml` & `google_ai_studio_utils-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "google-ai-studio-utils"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/google-ai-studio-utils"
 repository = "https://github.com/tddschn/google-ai-studio-utils"
 classifiers = ["Topic :: Utilities"]
@@ -13,14 +13,16 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/google-ai-studio-utils/issues"
 [tool.poetry.scripts]
 gai2html = "google_ai_studio_utils.google_ai_studio_conversation_csv_to_html:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
+pyperclip = "^1.8.2"
+markdown = "^3.6"
 
 
 [tool.poetry.group.dev.dependencies]
 better-exceptions = "^0.3.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `google_ai_studio_utils-0.1.1/PKG-INFO` & `google_ai_studio_utils-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: google-ai-studio-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/tddschn/google-ai-studio-utils
 License: MIT
 Keywords: chatgpt
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
+Requires-Dist: markdown (>=3.6,<4.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/google-ai-studio-utils/issues
 Project-URL: Repository, https://github.com/tddschn/google-ai-studio-utils
 Description-Content-Type: text/markdown
 
 # google-ai-studio-utils
```

