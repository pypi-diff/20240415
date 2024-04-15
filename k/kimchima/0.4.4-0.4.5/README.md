# Comparing `tmp/kimchima-0.4.4.tar.gz` & `tmp/kimchima-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.4.4.tar", max compression
+gzip compressed data, was "kimchima-0.4.5.tar", max compression
```

## Comparing `kimchima-0.4.4.tar` & `kimchima-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11343 2024-04-13 08:10:01.851682 kimchima-0.4.4/LICENSE
--rw-r--r--   0        0        0      908 2024-04-13 08:10:01.851682 kimchima-0.4.4/README.md
--rw-r--r--   0        0        0     2595 2024-04-13 08:10:01.851682 kimchima-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1170 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/__init__.py
--rw-r--r--   0        0        0      684 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/chat_template/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/chat_template/chat_template_factory.py
--rw-r--r--   0        0        0        0 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-13 08:10:01.851682 kimchima-0.4.4/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0      674 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     2347 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1072 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3233 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/download_hub.py
--rw-r--r--   0        0        0     3222 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4727 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1838 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3558 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1504 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_chat.py
--rw-r--r--   0        0        0     2290 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_chat_template_factory.py
--rw-r--r--   0        0        0     1818 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     2032 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     2509 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0      653 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/utils/__init__.py
--rw-r--r--   0        0        0     2119 2024-04-13 08:10:01.855682 kimchima-0.4.4/src/kimchima/utils/chat.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-15 10:18:14.173492 kimchima-0.4.5/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-15 10:18:14.173492 kimchima-0.4.5/README.md
+-rw-r--r--   0        0        0     2595 2024-04-15 10:18:14.177492 kimchima-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/chat_template/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/chat_template/chat_template_factory.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     2347 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1015 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3222 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4727 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1838 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3558 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1966 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_chat.py
+-rw-r--r--   0        0        0     2290 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1818 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     2032 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     2509 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0      702 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/__init__.py
+-rw-r--r--   0        0        0     1817 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/chat.py
+-rw-r--r--   0        0        0     1384 2024-04-15 10:18:14.177492 kimchima-0.4.5/src/kimchima/utils/downloader.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.5/PKG-INFO
```

### Comparing `kimchima-0.4.4/LICENSE` & `kimchima-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/README.md` & `kimchima-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/pyproject.toml` & `kimchima-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.4.4"
+version = "0.4.5"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.4.4/src/kimchima/__init__.py` & `kimchima-0.4.5/src/kimchima/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__="0.3.1"
 
 from kimchima.pkg import (
     ModelFactory,
     TokenizerFactory,
     EmbeddingsFactory,
     QuantizationFactory,
     StreamerFactory,
-    Devices,
-    DownloadHub
+    Devices
     )
 
 from kimchima.pipelines import PipelinesFactory
 from kimchima.chat_template import ChatTemplateFactory
 
-from kimchima.utils import chat_summary
+from kimchima.utils import (
+    chat_summary,
+    Downloader
+    )
 
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'Devices',
     'PipelinesFactory',
     'ChatTemplateFactory',
-    'DownloadHub',
-    'chat_summary'
+    'chat_summary',
+    'Downloader'
     ]
```

### Comparing `kimchima-0.4.4/src/kimchima/chat_template/__init__.py` & `kimchima-0.4.5/src/kimchima/chat_template/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/chat_template/chat_template_factory.py` & `kimchima-0.4.5/src/kimchima/chat_template/chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/cmds/auto_cli.py` & `kimchima-0.4.5/src/kimchima/cmds/auto_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.4.5/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pipelines/__init__.py` & `kimchima-0.4.5/src/kimchima/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pipelines/pipelines_factory.py` & `kimchima-0.4.5/src/kimchima/pipelines/pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/__init__.py` & `kimchima-0.4.5/src/kimchima/pkg/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 from .model_factory import ModelFactory
 from .tokenizer_factory import TokenizerFactory
 from .embedding_factory import EmbeddingsFactory
 from .quantization_factory import QuantizationFactory
 from .streamer_factory import StreamerFactory
 
 from .devices import Devices
-from .download_hub import DownloadHub
 
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
 
-    'Devices',
-    'DownloadHub'
+    'Devices'
     ]
```

### Comparing `kimchima-0.4.4/src/kimchima/pkg/devices.py` & `kimchima-0.4.5/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.4.5/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/logging.py` & `kimchima-0.4.5/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/model_factory.py` & `kimchima-0.4.5/src/kimchima/pkg/model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.4.5/src/kimchima/pkg/quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.4.5/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.4.5/src/kimchima/pkg/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_chat.py` & `kimchima-0.4.5/src/kimchima/tests/test_chat.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,31 +10,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
+from kimchima.pipelines import PipelinesFactory
 from kimchima.utils.chat import chat_summary
 
 class TestChatSummary(unittest.TestCase):
         
+        # prepare test data
+        def setUp(self):
+            self.conversation_model="gpt2"
+            self.summarization_model="sshleifer/distilbart-cnn-12-6"
+            self.msg = "why Melbourne is a good place to travel?"
+            self.max_length = 10
+            self.prompt = "Melbourne is often considered one of the most livable cities globally, offering a high quality of life."
+
+            # Load conversation model by using pipeline
+            self.pipe_con=PipelinesFactory.customized_pipe(model=self.conversation_model, device_map='auto')
+
+            self.pipe_sum=PipelinesFactory.customized_pipe(model=self.summarization_model, device_map='auto')
+        
         @unittest.skip("skip test_chat_summary")
         def test_chat_summary(self):
             """
             Test chat_summary method
             """
-            conversation_model="gpt2"
-            summarization_model="sshleifer/distilbart-cnn-12-6"
-            msg = "why Melbourne is a good place to travel?"
-            prompt = "Melbourne is often considered one of the most livable cities globally, offering a high quality of life."
 
             res = chat_summary(
-                conversation_model=conversation_model,
-                summarization_model=summarization_model,
-                messages=msg,
-                prompt=prompt
+                pipe_con=self.pipe_con,
+                pipe_sum=self.pipe_sum,
+                messages=self.msg,
+                prompt=self.prompt,
+                max_length=self.max_length
                 )
 
             # res is str and should not be None
             self.assertIsNotNone(res)
             self.assertIsInstance(res, str)
```

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_chat_template_factory.py` & `kimchima-0.4.5/src/kimchima/tests/test_chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_devices.py` & `kimchima-0.4.5/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.4.5/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.4.5/src/kimchima/tests/test_pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.4.5/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.4/src/kimchima/utils/chat.py` & `kimchima-0.4.5/src/kimchima/utils/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,53 +12,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from kimchima.pkg import logging
-from kimchima.pipelines import PipelinesFactory
-
 
 logger=logging.get_logger(__name__)
 
 
-
 def chat_summary(*args,**kwargs)-> str:
         r"""
-        Create a chat response and summarization pipeline using the Huggingface Transformers library.
         """
-        conversation_model=kwargs.pop("conversation_model", None)
-        if conversation_model is None:
-            raise ValueError("conversation_model is required")
-        summarization_model=kwargs.pop("summarization_model", None)
+        pipe_con=kwargs.pop("pipe_con", None)
+        if pipe_con is None:
+            raise ValueError("conversation pipeline is required")
+        
+        pipe_sum=kwargs.pop("pipe_sum", None)
+        if pipe_sum is None:
+            raise ValueError("summarization pipeline is required")
+        
         messages=kwargs.pop("messages", None)
         if messages is None:
             raise ValueError("messages is required")
+
         prompt=kwargs.pop("prompt", None)
         max_length=kwargs.pop("max_length", None)
         
-        # text generation pipeline
-        pipe=PipelinesFactory.customized_pipe(
-             model=conversation_model, 
-             device_map='auto'
-        )
-        response = pipe(messages)
+        response = pipe_con(messages)
+
+        logger.info("Finish conversation pipeline")
         
         if prompt is None:
             return response[0].get('generated_text')
         
         raw_response = prompt + response[0].get('generated_text')
         
         if max_length is None:
             max_length = len(raw_response)
 
+        response = pipe_sum(raw_response, min_length=5, max_length=max_length)
 
-        # pipeline for summarization
-        pipe=PipelinesFactory.customized_pipe(
-             model=summarization_model, 
-             device_map='auto'
-        )
-
-        response = pipe(raw_response, min_length=5, max_length=max_length)
+        logger.info("Finish summarization pipeline")
 
         return response[0].get('summary_text')
```

### Comparing `kimchima-0.4.4/PKG-INFO` & `kimchima-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.4.4
+Version: 0.4.5
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

