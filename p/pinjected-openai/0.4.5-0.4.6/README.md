# Comparing `tmp/pinjected_openai-0.4.5.tar.gz` & `tmp/pinjected_openai-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected_openai-0.4.5.tar", max compression
+gzip compressed data, was "pinjected_openai-0.4.6.tar", max compression
```

## Comparing `pinjected_openai-0.4.5.tar` & `pinjected_openai-0.4.6.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2024-01-25 04:47:59.248948 pinjected_openai-0.4.5/README.md
--rw-r--r--   0        0        0      227 2024-01-25 06:56:44.144365 pinjected_openai-0.4.5/pinjected_openai/__init__.py
--rw-r--r--   0        0        0     7160 2024-03-14 10:44:37.637306 pinjected_openai-0.4.5/pinjected_openai/vision_llm.py
--rw-r--r--   0        0        0      435 2024-03-20 14:01:22.837030 pinjected_openai-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 pinjected_openai-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-25 04:47:59.248948 pinjected_openai-0.4.6/README.md
+-rw-r--r--   0        0        0      380 2024-04-12 06:08:48.671473 pinjected_openai-0.4.6/pinjected_openai/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-15 03:17:41.134925 pinjected_openai-0.4.6/pinjected_openai/clients.py
+-rw-r--r--   0        0        0     6794 2024-04-12 06:08:48.682761 pinjected_openai-0.4.6/pinjected_openai/vision_llm.py
+-rw-r--r--   0        0        0     1358 2024-04-12 06:13:50.042530 pinjected_openai-0.4.6/pinjected_openai/whisper.py
+-rw-r--r--   0        0        0      453 2024-04-15 03:18:52.861961 pinjected_openai-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pinjected_openai-0.4.6/PKG-INFO
```

### Comparing `pinjected_openai-0.4.5/pinjected_openai/vision_llm.py` & `pinjected_openai-0.4.6/pinjected_openai/vision_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 import base64
 import io
 import json
-import os
 import re
 from pathlib import Path
 
 from PIL.Image import Image
 from injected_utils.injected_cache_utils import async_cached, sqlite_dict
 from loguru import logger
 from openai import AsyncOpenAI, RateLimitError
-from pinjected import injected, Injected, instances, instance
+from pinjected import injected, Injected, instances
 
 
 def to_content(img: Image):
     # convert Image into jpeg bytes
     jpg_bytes = io.BytesIO()
     img.convert('RGB').save(jpg_bytes, format='jpeg', quality=95)
     b64_image = base64.b64encode(jpg_bytes.getvalue()).decode('utf-8')
@@ -195,28 +194,14 @@
     return await a_json_llm__openai(
         text=text,
         max_completion_tokens=max_completion_tokens,
         model="gpt-4-turbo-preview"
     )
 
 
-@instance
-def async_openai_client(openai_api_key) -> AsyncOpenAI:
-    return AsyncOpenAI(
-        api_key=openai_api_key,
-    )
-
-
-@instance
-def openai_api_key() -> str:
-    if (api_key := os.environ.get('OPENAI_API_KEY', None)) is None:
-        api_key = Path(os.path.expanduser("~/.openai_api_key.txt")).read_text().strip()
-    return api_key
-
-
 test_vision_llm__gpt4 = a_vision_llm__gpt4(
     text="What are inside this image?",
     images=Injected.list(
     ),
 )
 """
 ('The image appears to be an advertisement or an informational graphic about '
```

### Comparing `pinjected_openai-0.4.5/PKG-INFO` & `pinjected_openai-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pinjected-openai
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: injected-utils (>=0.1.5,<0.2.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.9.0,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pinjected
+Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
```

