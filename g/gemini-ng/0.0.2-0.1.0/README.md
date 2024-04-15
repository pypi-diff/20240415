# Comparing `tmp/gemini_ng-0.0.2.tar.gz` & `tmp/gemini_ng-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ng-0.0.2.tar", last modified: Mon Apr 15 10:29:14 2024, max compression
+gzip compressed data, was "gemini_ng-0.1.0.tar", last modified: Mon Apr 15 16:44:16 2024, max compression
```

## Comparing `gemini_ng-0.0.2.tar` & `gemini_ng-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.434310 gemini_ng-0.0.2/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 14:47:07.000000 gemini_ng-0.0.2/LICENSE
--rw-r--r--   0 viv        (501) staff       (20)     1236 2024-04-15 10:29:14.434039 gemini_ng-0.0.2/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      374 2024-04-14 19:20:17.000000 gemini_ng-0.0.2/README.md
--rw-r--r--   0 viv        (501) staff       (20)      988 2024-04-15 10:21:37.000000 gemini_ng-0.0.2/pyproject.toml
--rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-15 10:29:14.434365 gemini_ng-0.0.2/setup.cfg
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.426404 gemini_ng-0.0.2/src/
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.427996 gemini_ng-0.0.2/src/gemini_ng/
--rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-15 10:28:45.000000 gemini_ng-0.0.2/src/gemini_ng/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     1598 2024-04-14 19:06:40.000000 gemini_ng-0.0.2/src/gemini_ng/chat.py
--rw-r--r--   0 viv        (501) staff       (20)     5820 2024-04-15 10:27:50.000000 gemini_ng-0.0.2/src/gemini_ng/client.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.431876 gemini_ng-0.0.2/src/gemini_ng/schemas/
--rw-r--r--   0 viv        (501) staff       (20)      386 2024-04-14 18:22:25.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/base.py
--rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/harm.py
--rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/part.py
--rw-r--r--   0 viv        (501) staff       (20)     2838 2024-04-14 16:23:27.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/request.py
--rw-r--r--   0 viv        (501) staff       (20)     1209 2024-04-14 16:16:33.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/response.py
--rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.0.2/src/gemini_ng/schemas/upload.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.432890 gemini_ng-0.0.2/src/gemini_ng/utils/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.0.2/src/gemini_ng/utils/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     2417 2024-04-15 10:18:45.000000 gemini_ng-0.0.2/src/gemini_ng/utils/video.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 10:29:14.433603 gemini_ng-0.0.2/src/gemini_ng.egg-info/
--rw-r--r--   0 viv        (501) staff       (20)     1236 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      582 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/SOURCES.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/dependency_links.txt
--rw-r--r--   0 viv        (501) staff       (20)      120 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/requires.txt
--rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-15 10:29:14.000000 gemini_ng-0.0.2/src/gemini_ng.egg-info/top_level.txt
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.151928 gemini_ng-0.1.0/
+-rw-r--r--   0 viv        (501) staff       (20)     1053 2024-04-15 16:41:45.000000 gemini_ng-0.1.0/LICENSE
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-15 16:44:16.151682 gemini_ng-0.1.0/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)     1019 2024-04-15 16:43:10.000000 gemini_ng-0.1.0/README.md
+-rw-r--r--   0 viv        (501) staff       (20)     1012 2024-04-15 16:16:28.000000 gemini_ng-0.1.0/pyproject.toml
+-rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-15 16:44:16.151977 gemini_ng-0.1.0/setup.cfg
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.145821 gemini_ng-0.1.0/src/
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.147116 gemini_ng-0.1.0/src/gemini_ng/
+-rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-15 16:39:05.000000 gemini_ng-0.1.0/src/gemini_ng/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     1684 2024-04-15 16:14:47.000000 gemini_ng-0.1.0/src/gemini_ng/chat.py
+-rw-r--r--   0 viv        (501) staff       (20)     7327 2024-04-15 16:37:20.000000 gemini_ng-0.1.0/src/gemini_ng/client.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.150063 gemini_ng-0.1.0/src/gemini_ng/schemas/
+-rw-r--r--   0 viv        (501) staff       (20)      386 2024-04-14 18:22:25.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/base.py
+-rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/harm.py
+-rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/part.py
+-rw-r--r--   0 viv        (501) staff       (20)     2838 2024-04-14 16:23:27.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/request.py
+-rw-r--r--   0 viv        (501) staff       (20)     1441 2024-04-15 16:14:16.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/response.py
+-rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.1.0/src/gemini_ng/schemas/upload.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.150768 gemini_ng-0.1.0/src/gemini_ng/utils/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.1.0/src/gemini_ng/utils/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      509 2024-04-15 16:23:14.000000 gemini_ng-0.1.0/src/gemini_ng/utils/cache.py
+-rw-r--r--   0 viv        (501) staff       (20)     1435 2024-04-15 15:33:21.000000 gemini_ng-0.1.0/src/gemini_ng/utils/error.py
+-rw-r--r--   0 viv        (501) staff       (20)     2417 2024-04-15 10:18:45.000000 gemini_ng-0.1.0/src/gemini_ng/utils/video.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-15 16:44:16.151323 gemini_ng-0.1.0/src/gemini_ng.egg-info/
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-15 16:44:16.000000 gemini_ng-0.1.0/src/gemini_ng.egg-info/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      640 2024-04-15 16:44:16.000000 gemini_ng-0.1.0/src/gemini_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-15 16:44:16.000000 gemini_ng-0.1.0/src/gemini_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 viv        (501) staff       (20)      137 2024-04-15 16:44:16.000000 gemini_ng-0.1.0/src/gemini_ng.egg-info/requires.txt
+-rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-15 16:44:16.000000 gemini_ng-0.1.0/src/gemini_ng.egg-info/top_level.txt
```

### Comparing `gemini_ng-0.0.2/pyproject.toml` & `gemini_ng-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "google-api-python-client>=2.125.0",
     "requests>=2.31.0",
     "pydantic>=2.7.0",
     "av>=12.0.0",
     "pillow>=10.3.0",
     "numpy>=1.26.4",
     "tqdm>=4.66.2",
+    "diskcache>=5.6.3",
 ]
 
 [project.urls]
 Documentation = "https://github.com/vivym/gemini-ng#readme"
 Issues = "https://github.com/vivym/gemini-ng/issues"
 Source = "https://github.com/vivym/gemini-ng"
```

### Comparing `gemini_ng-0.0.2/src/gemini_ng/chat.py` & `gemini_ng-0.1.0/src/gemini_ng/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 
         rsp = self.client.generate(
             self.model,
             ChatHistory(messages=self.history),
             generation_config=generation_config or self.generation_config,
             safety_settings=safety_settings or self.safety_settings,
         )
-        rsp_parts = rsp.candidates[0].content.parts
-        self.history.append(ChatMessage(role="model", parts=rsp_parts))
+        if len(rsp.candidates) > 0 and rsp.candidates[0].content is not None:
+            rsp_parts = rsp.candidates[0].content.parts
+            self.history.append(ChatMessage(role="model", parts=rsp_parts))
 
         return rsp
 
     def clear(self):
         self.history = []
 
     def __enter__(self):
```

### Comparing `gemini_ng-0.0.2/src/gemini_ng/client.py` & `gemini_ng-0.1.0/src/gemini_ng/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import hashlib
 import os
 import tempfile
-from pathlib import Path
 
 import requests
 import googleapiclient.discovery as g_discovery
 from tqdm import tqdm
 
 from .chat import ChatSession
 from .schemas import (
@@ -18,27 +18,31 @@
     TextPart,
     ImagePart,
     FilePart,
     VideoPart,
     UploadFile,
     UploadedFile,
 )
+from .utils.cache import get_cache_instance
+from .utils.error import handle_http_exception
 from .utils.video import extract_video_frames
 
 
 class GeminiClient:
     def __init__(
         self,
         api_key: str | None = None,
         version: str = "v1beta",
     ):
-        api_key = api_key or os.getenv("GEMINI_API_KEY")
+        api_key = api_key or os.getenv("GEMINI_NG_API_KEY")
 
         if api_key is None:
-            raise ValueError("Gemini API (`GEMINI_API_KEY`) key must be provided")
+            raise ValueError("Gemini API (`GEMINI_NG_API_KEY`) key must be provided")
+
+        self.api_key = api_key
 
         rsp = requests.get(
             "https://generativelanguage.googleapis.com/$discovery/rest",
             params={"version": version, "key": api_key},
         )
         rsp.raise_for_status()
 
@@ -49,26 +53,47 @@
     @staticmethod
     def normalize_prompt(prompt: list | str) -> list:
         parts = []
 
         if isinstance(prompt, str):
             prompt = [prompt]
 
-        for part in prompt:
+        for i, part in enumerate(prompt):
             if isinstance(part, str):
-                parts.append(TextPart(text=f"\n{part}\n"))  # Take care of the newline more elegantly
-            elif isinstance(part, (FilePart, ImagePart)):
+                parts.append(TextPart(text=part if i == 0 else "\n" + part))
+            elif isinstance(part, (TextPart, FilePart, ImagePart)):
                 parts.append(part)
             elif isinstance(part, VideoPart):
                 parts.extend(part.content_parts())
             else:
                 raise ValueError(f"Invalid prompt part type: {type(part)} ({part})")
 
         return parts
 
+    @handle_http_exception
+    def get_token_count(self, model: str, prompt: GenerationRequest | list) -> int:
+        if isinstance(prompt, GenerationRequest):
+            request = prompt
+        else:
+            parts = self.normalize_prompt(prompt)
+            request = GenerationRequest(contents=[GenerationRequestParts(parts=parts)])
+
+        rsp = (
+            self.genai_service
+                .models()
+                .getTokenCount(
+                    model=model,
+                    body=request.model_dump(by_alias=True, exclude_none=True),
+                )
+                .execute()
+        )
+
+        return rsp["totalTokens"]
+
+    @handle_http_exception
     def generate(
         self,
         model: str,
         prompt: GenerationRequest | ChatHistory | list | str,
         generation_config: GenerationConfig | dict | None = None,
         safety_settings: SafetySettings | dict | None = None,
     ) -> GenerationResponse:
@@ -133,23 +158,28 @@
             if not isinstance(safety_settings, SafetySettings):
                 safety_settings = SafetySettings.model_validate(safety_settings)
             request.safety_settings = safety_settings
 
         return request
 
     def upload_image(self, image_path: str) -> ImagePart:
-        if not Path(image_path).exists():
+        if not os.path.exists(image_path):
             raise FileNotFoundError(f"Image file not found: {image_path}")
 
-        uploaded_file = self._upload_file(UploadFile.from_path(image_path))
+        uploaded_file = self._upload_file(
+            UploadFile.from_path(
+                image_path,
+                body={"file": {"displayName": os.path.basename(image_path)}},
+            )
+        )
 
         return uploaded_file.to_file_part()
 
     def upload_video(self, video_path: str, verbose: bool = False) -> VideoPart:
-        if not Path(video_path).exists():
+        if not os.path.exists(video_path):
             raise FileNotFoundError(f"Video file not found: {video_path}")
 
         with tempfile.TemporaryDirectory() as temp_dir:
             frame_paths = extract_video_frames(video_path, save_dir=temp_dir, sample_fps=1)
 
             image_parts = [
                 self.upload_image(frame_path)
@@ -160,22 +190,40 @@
             time_spans=[
                 TextPart(text=f"{i // 60:02d}:{i % 60:02d}")
                 for i in range(len(image_parts))
             ],
             frames=image_parts,
         )
 
+    @handle_http_exception
     def _upload_file(self, file: UploadFile) -> UploadedFile:
+        m = hashlib.sha256()
+        with open(file.file_path, "rb") as f:
+            for chunk in iter(lambda: f.read(4096), b""):
+                m.update(chunk)
+
+        sha256_hash = m.hexdigest()
+        cache_key = f"{self.api_key}_file_{sha256_hash}"
+
+        cache = get_cache_instance()
+        cached_obj = cache.get(cache_key)
+        if cached_obj:
+            return UploadedFile.model_validate(cached_obj)
+
         rsp = (
             self.genai_service.media()
             .upload(
                 media_body=file.file_path,
                 media_mime_type=file.mime_type,
                 body=file.body,
             )
             .execute()
         )
 
-        return UploadedFile.model_validate(rsp["file"])
+        uploaded_file = UploadedFile.model_validate(rsp["file"])
+
+        cache.set(cache_key, uploaded_file.model_dump(by_alias=True, exclude_none=True))
+
+        return uploaded_file
 
     def _upload_files(self, *files: list[UploadFile]) -> list[UploadedFile]:
         return [self._upload_file(file) for file in files]
```

### Comparing `gemini_ng-0.0.2/src/gemini_ng/schemas/harm.py` & `gemini_ng-0.1.0/src/gemini_ng/schemas/harm.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.2/src/gemini_ng/schemas/part.py` & `gemini_ng-0.1.0/src/gemini_ng/schemas/part.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.2/src/gemini_ng/schemas/request.py` & `gemini_ng-0.1.0/src/gemini_ng/schemas/request.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.2/src/gemini_ng/schemas/response.py` & `gemini_ng-0.1.0/src/gemini_ng/schemas/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,12 +30,18 @@
         None, alias="finishReason", description="The reason the generation stopped."
     )
 
     safety_ratings: list[SafetyRating] | None = Field(
         None, alias="safetyRatings", description="Safety ratings of the content."
     )
 
+    @property
+    def text(self) -> str:
+        if self.content is None:
+            raise ValueError("No content to get text from. " + str(self.model_dump_json()))
+        return "".join(part.text for part in self.content.parts)
+
 
 class GenerationResponse(BaseModel):
     candidates: list[GenerationCandidate] = Field(
         [], description="The generated responses."
     )
```

### Comparing `gemini_ng-0.0.2/src/gemini_ng/schemas/upload.py` & `gemini_ng-0.1.0/src/gemini_ng/schemas/upload.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.2/src/gemini_ng/utils/video.py` & `gemini_ng-0.1.0/src/gemini_ng/utils/video.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.0.2/src/gemini_ng.egg-info/SOURCES.txt` & `gemini_ng-0.1.0/src/gemini_ng.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 src/gemini_ng/schemas/base.py
 src/gemini_ng/schemas/harm.py
 src/gemini_ng/schemas/part.py
 src/gemini_ng/schemas/request.py
 src/gemini_ng/schemas/response.py
 src/gemini_ng/schemas/upload.py
 src/gemini_ng/utils/__init__.py
+src/gemini_ng/utils/cache.py
+src/gemini_ng/utils/error.py
 src/gemini_ng/utils/video.py
```

