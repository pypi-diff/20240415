# Comparing `tmp/google_ai_studio_utils-0.1.2.tar.gz` & `tmp/google_ai_studio_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ai_studio_utils-0.1.2.tar", max compression
+gzip compressed data, was "google_ai_studio_utils-0.1.3.tar", max compression
```

## Comparing `google_ai_studio_utils-0.1.2.tar` & `google_ai_studio_utils-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.2/README.md
--rw-r--r--   0        0        0      214 2024-04-15 16:21:49.454447 google_ai_studio_utils-0.1.2/google_ai_studio_utils/config.py
--rwxr-xr-x   0        0        0     2720 2024-04-15 16:30:26.575670 google_ai_studio_utils-0.1.2/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
--rw-r--r--   0        0        0     1744 2024-04-15 16:31:29.925728 google_ai_studio_utils-0.1.2/google_ai_studio_utils/utils.py
--rw-r--r--   0        0        0      827 2024-04-15 16:36:29.062513 google_ai_studio_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.3/README.md
+-rw-r--r--   0        0        0      214 2024-04-15 16:21:49.454447 google_ai_studio_utils-0.1.3/google_ai_studio_utils/config.py
+-rwxr-xr-x   0        0        0     2720 2024-04-15 16:30:26.575670 google_ai_studio_utils-0.1.3/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
+-rw-r--r--   0        0        0     1786 2024-04-15 16:45:14.446099 google_ai_studio_utils-0.1.3/google_ai_studio_utils/utils.py
+-rw-r--r--   0        0        0      827 2024-04-15 16:55:07.966649 google_ai_studio_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.3/PKG-INFO
```

### Comparing `google_ai_studio_utils-0.1.2/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py` & `google_ai_studio_utils-0.1.3/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.2/google_ai_studio_utils/utils.py` & `google_ai_studio_utils-0.1.3/google_ai_studio_utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     import markdown
     html_template = google_ai_studio_html_template.read_text()
     
 
     content = ""
     for role, message in conversation:
         if role == "Model":
-            content += f'<div class="model-content">{markdown.markdown(message, extensions=['fenced_code', 'tables'])}</div><hr>'
+            content += f'<div class="model-content">{markdown.markdown(message, extensions=['footnotes', 'meta', 'toc', 'admonition', 'fenced_code', 'tables'])}</div><hr>'
         else:
             content += f'<div class="user-content"><pre>{message}</pre></div><hr>'
 
     # return html_template.format(content=content, font=font, title=title)
     return format_dunder_keys(html_template, content=content, font=font, title=title)
 
 def gist_create(p: PathLike) -> str:
```

### Comparing `google_ai_studio_utils-0.1.2/pyproject.toml` & `google_ai_studio_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "google-ai-studio-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/google-ai-studio-utils"
 repository = "https://github.com/tddschn/google-ai-studio-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `google_ai_studio_utils-0.1.2/PKG-INFO` & `google_ai_studio_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-studio-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/tddschn/google-ai-studio-utils
 License: MIT
 Keywords: chatgpt
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

