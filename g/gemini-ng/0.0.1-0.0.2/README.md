# Comparing `tmp/gemini_ng-0.0.1.tar.gz` & `tmp/gemini_ng-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ng-0.0.1.tar", last modified: Sun Apr 14 19:23:24 2024, max compression
+gzip compressed data, was "gemini_ng-0.0.2.tar", last modified: Mon Apr 15 10:29:14 2024, max compression
```

## Comparing `gemini_ng-0.0.1.tar` & `gemini_ng-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.250575 gemini_ng-0.0.1/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 14:47:07.000000 gemini_ng-0.0.1/LICENSE
--rw-r--r--   0 viv        (501) staff       (20)     1123 2024-04-14 19:23:24.250336 gemini_ng-0.0.1/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      374 2024-04-14 19:20:17.000000 gemini_ng-0.0.1/README.md
--rw-r--r--   0 viv        (501) staff       (20)      907 2024-04-14 15:10:57.000000 gemini_ng-0.0.1/pyproject.toml
--rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-14 19:23:24.250619 gemini_ng-0.0.1/setup.cfg
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.243381 gemini_ng-0.0.1/src/
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.246889 gemini_ng-0.0.1/src/gemini_ng/
--rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-14 16:52:15.000000 gemini_ng-0.0.1/src/gemini_ng/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     1598 2024-04-14 19:06:40.000000 gemini_ng-0.0.1/src/gemini_ng/chat.py
--rw-r--r--   0 viv        (501) staff       (20)     5226 2024-04-14 19:17:42.000000 gemini_ng-0.0.1/src/gemini_ng/client.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.249641 gemini_ng-0.0.1/src/gemini_ng/schemas/
--rw-r--r--   0 viv        (501) staff       (20)      386 2024-04-14 18:22:25.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/base.py
--rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/harm.py
--rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/part.py
--rw-r--r--   0 viv        (501) staff       (20)     2838 2024-04-14 16:23:27.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/request.py
--rw-r--r--   0 viv        (501) staff       (20)     1209 2024-04-14 16:16:33.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/response.py
--rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.0.1/src/gemini_ng/schemas/upload.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.249907 gemini_ng-0.0.1/src/gemini_ng/utils/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.0.1/src/gemini_ng/utils/__init__.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-14 19:23:24.250071 gemini_ng-0.0.1/src/gemini_ng.egg-info/
--rw-r--r--   0 viv        (501) staff       (20)     1123 2024-04-14 19:23:24.000000 gemini_ng-0.0.1/src/gemini_ng.egg-info/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      553 2024-04-14 19:23:24.000000 gemini_ng-0.0.1/src/gemini_ng.egg-info/SOURCES.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-14 19:23:24.000000 gemini_ng-0.0.1/src/gemini_ng.egg-info/dependency_links.txt
--rw-r--r--   0 viv        (501) staff       (20)       67 2024-04-14 19:23:24.000000 gemini_ng-0.0.1/src/gemini_ng.egg-info/requires.txt
--rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-14 19:23:24.000000 gemini_ng-0.0.1/src/gemini_ng.egg-info/top_level.txt
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.434310 gemini_ng-0.0.2/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 14:47:07.000000 gemini_ng-0.0.2/LICENSE
+-rw-r--r--   0 viv        (501) staff       (20)     1236 2024-04-15 10:29:14.434039 gemini_ng-0.0.2/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      374 2024-04-14 19:20:17.000000 gemini_ng-0.0.2/README.md
+-rw-r--r--   0 viv        (501) staff       (20)      988 2024-04-15 10:21:37.000000 gemini_ng-0.0.2/pyproject.toml
+-rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-15 10:29:14.434365 gemini_ng-0.0.2/setup.cfg
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.426404 gemini_ng-0.0.2/src/
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.427996 gemini_ng-0.0.2/src/gemini_ng/
+-rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-15 10:28:45.000000 gemini_ng-0.0.2/src/gemini_ng/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     1598 2024-04-14 19:06:40.000000 gemini_ng-0.0.2/src/gemini_ng/chat.py
+-rw-r--r--   0 viv        (501) staff       (20)     5820 2024-04-15 10:27:50.000000 gemini_ng-0.0.2/src/gemini_ng/client.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.431876 gemini_ng-0.0.2/src/gemini_ng/schemas/
+-rw-r--r--   0 viv        (501) staff       (20)      386 2024-04-14 18:22:25.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/base.py
+-rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/harm.py
+-rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/part.py
+-rw-r--r--   0 viv        (501) staff       (20)     2838 2024-04-14 16:23:27.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/request.py
+-rw-r--r--   0 viv        (501) staff       (20)     1209 2024-04-14 16:16:33.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/response.py
+-rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/upload.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.432890 gemini_ng-0.0.2/src/gemini_ng/utils/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.0.2/src/gemini_ng/utils/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     2417 2024-04-15 10:18:45.000000 gemini_ng-0.0.2/src/gemini_ng/utils/video.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.433603 gemini_ng-0.0.2/src/gemini_ng.egg-info/
+-rw-r--r--   0 viv        (501) staff       (20)     1236 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      582 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 viv        (501) staff       (20)      120 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/requires.txt
+-rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/top_level.txt
```

### Comparing `gemini_ng-0.0.1/PKG-INFO` & `gemini_ng-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.0.1
+Version: 0.0.2
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 Project-URL: Documentation, https://github.com/vivym/gemini-ng#readme
 Project-URL: Issues, https://github.com/vivym/gemini-ng/issues
 Project-URL: Source, https://github.com/vivym/gemini-ng
 Keywords: Gemini
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-api-python-client>=2.125.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=2.7.0
+Requires-Dist: av>=12.0.0
+Requires-Dist: pillow>=10.3.0
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: tqdm>=4.66.2
 
 # Next-generation Gemini API Client
 
 ```python
 from gemini_ng import GeminiClient
 
 client = GeminiClient() # api key from environment variable `GEMINI_API_KEY`
```

### Comparing `gemini_ng-0.0.1/pyproject.toml` & `gemini_ng-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,18 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
     "google-api-python-client>=2.125.0",
     "requests>=2.31.0",
     "pydantic>=2.7.0",
+    "av>=12.0.0",
+    "pillow>=10.3.0",
+    "numpy>=1.26.4",
+    "tqdm>=4.66.2",
 ]
 
 [project.urls]
 Documentation = "https://github.com/vivym/gemini-ng#readme"
 Issues = "https://github.com/vivym/gemini-ng/issues"
 Source = "https://github.com/vivym/gemini-ng"
```

### Comparing `gemini_ng-0.0.1/src/gemini_ng/chat.py` & `gemini_ng-0.0.2/src/gemini_ng/chat.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng/client.py` & `gemini_ng-0.0.2/src/gemini_ng/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
+import tempfile
 from pathlib import Path
 
 import requests
 import googleapiclient.discovery as g_discovery
+from tqdm import tqdm
 
 from .chat import ChatSession
 from .schemas import (
     ChatMessage,
     ChatHistory,
     GenerationConfig,
     GenerationRequest,
@@ -16,14 +18,15 @@
     TextPart,
     ImagePart,
     FilePart,
     VideoPart,
     UploadFile,
     UploadedFile,
 )
+from .utils.video import extract_video_frames
 
 
 class GeminiClient:
     def __init__(
         self,
         api_key: str | None = None,
         version: str = "v1beta",
@@ -137,19 +140,33 @@
         if not Path(image_path).exists():
             raise FileNotFoundError(f"Image file not found: {image_path}")
 
         uploaded_file = self._upload_file(UploadFile.from_path(image_path))
 
         return uploaded_file.to_file_part()
 
-    def upload_video(self, video_path: str) -> VideoPart:
+    def upload_video(self, video_path: str, verbose: bool = False) -> VideoPart:
         if not Path(video_path).exists():
             raise FileNotFoundError(f"Video file not found: {video_path}")
 
-        raise NotImplementedError("Video upload is not yet implemented")
+        with tempfile.TemporaryDirectory() as temp_dir:
+            frame_paths = extract_video_frames(video_path, save_dir=temp_dir, sample_fps=1)
+
+            image_parts = [
+                self.upload_image(frame_path)
+                for frame_path in tqdm(frame_paths, disable=not verbose, desc="Uploading video frames")
+            ]
+
+        return VideoPart(
+            time_spans=[
+                TextPart(text=f"{i // 60:02d}:{i % 60:02d}")
+                for i in range(len(image_parts))
+            ],
+            frames=image_parts,
+        )
 
     def _upload_file(self, file: UploadFile) -> UploadedFile:
         rsp = (
             self.genai_service.media()
             .upload(
                 media_body=file.file_path,
                 media_mime_type=file.mime_type,
```

### Comparing `gemini_ng-0.0.1/src/gemini_ng/schemas/harm.py` & `gemini_ng-0.0.2/src/gemini_ng/schemas/harm.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng/schemas/part.py` & `gemini_ng-0.0.2/src/gemini_ng/schemas/part.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng/schemas/request.py` & `gemini_ng-0.0.2/src/gemini_ng/schemas/request.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng/schemas/response.py` & `gemini_ng-0.0.2/src/gemini_ng/schemas/response.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng/schemas/upload.py` & `gemini_ng-0.0.2/src/gemini_ng/schemas/upload.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.1/src/gemini_ng.egg-info/PKG-INFO` & `gemini_ng-0.0.2/src/gemini_ng.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.0.1
+Version: 0.0.2
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 Project-URL: Documentation, https://github.com/vivym/gemini-ng#readme
 Project-URL: Issues, https://github.com/vivym/gemini-ng/issues
 Project-URL: Source, https://github.com/vivym/gemini-ng
 Keywords: Gemini
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-api-python-client>=2.125.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=2.7.0
+Requires-Dist: av>=12.0.0
+Requires-Dist: pillow>=10.3.0
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: tqdm>=4.66.2
 
 # Next-generation Gemini API Client
 
 ```python
 from gemini_ng import GeminiClient
 
 client = GeminiClient() # api key from environment variable `GEMINI_API_KEY`
```

### Comparing `gemini_ng-0.0.1/src/gemini_ng.egg-info/SOURCES.txt` & `gemini_ng-0.0.2/src/gemini_ng.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/gemini_ng/schemas/__init__.py
 src/gemini_ng/schemas/base.py
 src/gemini_ng/schemas/harm.py
 src/gemini_ng/schemas/part.py
 src/gemini_ng/schemas/request.py
 src/gemini_ng/schemas/response.py
 src/gemini_ng/schemas/upload.py
-src/gemini_ng/utils/__init__.py
+src/gemini_ng/utils/__init__.py
+src/gemini_ng/utils/video.py
```

