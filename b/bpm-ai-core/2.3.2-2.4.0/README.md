# Comparing `tmp/bpm_ai_core-2.3.2.tar.gz` & `tmp/bpm_ai_core-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.3.2.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.4.0.tar", max compression
```

## Comparing `bpm_ai_core-2.3.2.tar` & `bpm_ai_core-2.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0       13 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1187 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     7217 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     3165 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6036 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7749 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     2919 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2085 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3018 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      827 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1428 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      909 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4370 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2267 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-04-11 18:28:46.931160 bpm_ai_core-2.3.2/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     1836 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     5233 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     1670 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    21191 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      675 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1014 2024-04-11 18:28:46.935160 bpm_ai_core-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1420 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6645 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     4774 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6141 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2445 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1455 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     7777 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     3340 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2698 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1220 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6259 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2085 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3018 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1096 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1428 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.404749 bpm_ai_core-2.4.0/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4381 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2347 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1572 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      475 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     2290 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     5945 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     3135 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    22412 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     5280 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/remote_object.py
+-rw-r--r--   0        0        0     2596 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      670 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/text.py
+-rw-r--r--   0        0        0      675 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1014 2024-04-15 20:58:46.408749 bpm_ai_core-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.4.0/PKG-INFO
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.4.0/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,34 @@
     """
 
     @abstractmethod
     async def _do_classify(
             self,
             text: str,
             classes: list[str],
-            hypothesis_template: str | None = None
+            hypothesis_template: str | None = None,
+            multi_label: bool = False
     ) -> ClassificationResult:
         pass
 
     @span(name="classifier")
     async def classify(
             self,
             text: str,
             classes: list[str],
             confidence_threshold: float | None = None,
-            hypothesis_template: str | None = None
+            hypothesis_template: str | None = None,
+            multi_label: bool = False
     ) -> ClassificationResult:
         result = await self._do_classify(
             text=text,
             classes=classes,
-            hypothesis_template=hypothesis_template
+            hypothesis_template=hypothesis_template,
+            multi_label=multi_label
         )
+        if multi_label:
+            result.labels_scores = [(l, s) for l, s in result.labels_scores if s > (confidence_threshold or -1)]
+
         # Only return if the score is above the threshold (if given)
         return result \
-            if not confidence_threshold or result.max_score > confidence_threshold \
+            if result.max_score > (confidence_threshold or -1) \
             else None
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import Dict, Any, Optional, List
 
 from typing_extensions import deprecated
 
 from bpm_ai_core.llm.anthropic_chat import get_anthropic_client
 from bpm_ai_core.llm.anthropic_chat._constants import DEFAULT_MODEL, DEFAULT_TEMPERATURE, \
     DEFAULT_MAX_RETRIES
-from bpm_ai_core.llm.anthropic_chat.util import messages_to_anthropic_dicts, json_schema_to_anthropic_tool
+from bpm_ai_core.llm.anthropic_chat.util import messages_to_anthropic_dicts, json_schema_to_anthropic_tool, \
+    tool_calls_to_tool_message
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.llm.common.message import ChatMessage, ToolCallMessage, AssistantMessage, SystemMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.tracing.tracing import Tracing
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 
@@ -87,57 +88,41 @@
         elif tools:
             return await self._run_tool_completion(messages, tools, current_try)
         else:
             completion = await self._run_completion(messages, stop, current_try)
             return AssistantMessage(content=completion.content[0].text.strip())
 
     async def _run_completion(self, messages: List[ChatMessage], stop: list[str] = None, current_try: int = None) -> Message:
+        messages = await messages_to_anthropic_dicts(messages)
         Tracing.tracers().start_llm_trace(self, messages, current_try, None)
         completion = await self.client.messages.create(
             max_tokens=4096,
             model=self.model,
             temperature=self.temperature,
-            system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
-            messages=await messages_to_anthropic_dicts(messages),
+            system=messages.pop(0)["content"] if (messages and messages[0]["role"] == "system") else "",
+            messages=messages,
             stop_sequences=stop
         )
-        Tracing.tracers().end_llm_trace(completion.content[0].text)
+        Tracing.tracers().end_llm_trace(completion)
         return completion
 
     async def _run_tool_completion(self, messages: list[ChatMessage], tools: list[Tool] = None, current_try: int = None) -> AssistantMessage:
-        anthropic_tools = [json_schema_to_anthropic_tool(f.name, f.description, f.args_schema) for f in tools] if tools else []
+        sanitized_key_mappings = {t.name: {} for t in tools}
+        anthropic_tools = [json_schema_to_anthropic_tool(t.name, t.description, t.args_schema, sanitized_key_mappings[t.name]) for t in tools] if tools else []
         Tracing.tracers().start_llm_trace(self, messages, current_try, anthropic_tools)
         completion = await self.client.beta.tools.messages.create(
             max_tokens=4096,
             model=self.model,
             temperature=self.temperature,
             system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
             messages=await messages_to_anthropic_dicts(messages),
             tools=anthropic_tools
         )
-        Tracing.tracers().end_llm_trace(completion.content)
-        return self._tool_calls_to_tool_message(completion, tools)
-
-    @staticmethod
-    def _tool_calls_to_tool_message(message: ToolsBetaMessage, tools: List[Tool]) -> AssistantMessage:
-        texts = [c.text for c in message.content if isinstance(c, TextBlock)]
-        tool_uses = [c for c in message.content if isinstance(c, ToolUseBlock)]
-        return AssistantMessage(
-            name=", ".join([t.name for t in tool_uses]),
-            content="\n".join(texts),
-            tool_calls=[
-                ToolCallMessage(
-                    id=t.id,
-                    name=t.name,
-                    payload=t.input,
-                    tool=next((item for item in tools if item.name == t.name), None)
-                )
-                for t in tool_uses
-            ]
-        )
+        Tracing.tracers().end_llm_trace(completion)
+        return tool_calls_to_tool_message(completion, tools, sanitized_key_mappings)
 
     @staticmethod
     def _output_schema_to_tool(output_schema: dict):
         output_schema = output_schema.copy()
         return Tool.create(
             name=output_schema.pop("name", None) or "record_result",
             description=output_schema.pop("description", None) or "Record your result into well-structured JSON.",
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,105 @@
 import logging
-from typing import List, Any
+from typing import List, Dict, Any
 
 from PIL.Image import Image
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.llm.common.message import ChatMessage, ToolResultMessage, AssistantMessage
 from bpm_ai_core.util.image import base64_encode_image, blob_as_images
 
 logger = logging.getLogger(__name__)
 
 ACCEPTED_IMAGE_FORMATS = ["jpeg", "png", "gif", "webp"]
 
 
-async def messages_to_anthropic_dicts(messages: List[ChatMessage]):
-    return [await message_to_anthropic_dict(m) for m in messages]
+def get_openai_tool_call_dict(message: AssistantMessage):
+    return {
+        "tool_calls": [
+            {
+                "type": "function",
+                "id": t.id,
+                "function": {
+                    "name": t.name,
+                    "arguments": t.payload
+                }
+            }
+            for t in message.tool_calls
+        ]
+    }
+
 
+async def messages_to_openai_dicts(messages: List[ChatMessage]):
+    return [await message_to_openai_dict(m) for m in messages]
 
-async def message_to_anthropic_dict(message: ChatMessage) -> dict:
+
+async def message_to_openai_dict(message: ChatMessage) -> dict:
     if isinstance(message, AssistantMessage) and message.has_tool_calls():
-        return tool_calls_message_to_anthropic_dict(message)
+        extra_dict = {
+            **get_openai_tool_call_dict(message)
+        }
     elif isinstance(message, ToolResultMessage):
-        return tool_result_message_to_anthropic_dict(message)
-    elif isinstance(message.content, str):
+        extra_dict = {
+            "tool_call_id": message.id
+        }
+    else:
+        extra_dict = {}
+
+    if isinstance(message.content, str):
         content = message.content
     elif isinstance(message.content, list):
         content = []
         for e in message.content:
             if isinstance(e, str):
-                content.append(str_to_anthropic_text_dict(e))
+                content.append(str_to_openai_text_dict(e))
             elif isinstance(e, Blob) and (e.is_image() or e.is_pdf()):
                 images = await blob_as_images(e, accept_formats=ACCEPTED_IMAGE_FORMATS)
-                for image in images:
-                    content.append(image_to_anthropic_image_dict(image))
+                for i, image in enumerate(images):
+                    content.append(str_to_openai_text_dict(f"Image / Page {i + 1}:"))
+                    content.append(image_to_openai_image_dict(image))
+            elif isinstance(e, Blob) and (e.is_text()):
+                text = (await e.as_bytes()).decode("utf-8")
+                filename = (" name='" + e.path + "'") if e.path else ''
+                text = f"<file{filename}>\n{text}\n</file>"
+                content.append(str_to_openai_text_dict(text))
             else:
                 raise ValueError(
-                    "Elements in ChatMessage.content must be str or image Blob"
+                    "Elements in ChatMessage.content must be str or Blob (image/pdf/text)"
                 )
     else:
         content = None
         logger.warning(
             "ChatMessage.content must be of type str or List[Union[str, PIL.Image]] if used for chat completions."
         )
     return {
         "role": message.role,
         **({"content": content} if content else {}),
+        **extra_dict,
         **({"name": message.name} if message.name else {})
     }
 
 
-def tool_calls_message_to_anthropic_dict(message: AssistantMessage) -> dict:
+def image_to_openai_image_dict(image: Image) -> dict:
     return {
-        "role": "assistant",
-        "content": ([{"type": "text", "text": message.content}] if message.content else [])
-                 + [{"type": "tool_use", "id": call.id, "name": call.name, "input": call.payload}
-                    for call in message.tool_calls]
-    }
-
-
-def tool_result_message_to_anthropic_dict(message: ToolResultMessage, is_error: bool = False) -> dict:
-    return {
-      "role": "user",
-      "content": [
-        {
-          "type": "tool_result",
-          "tool_use_id": message.id,
-          "content": message.content,
-          **({"is_error": True} if is_error else {})
+        "type": "image_url",
+        "image_url": {
+            "url": f"data:image/{image.format.lower()};base64,{base64_encode_image(image)}"
         }
-      ]
     }
 
 
-def image_to_anthropic_image_dict(image: Image) -> dict:
-    return {
-        "type": "image",
-        "source": {
-            "type": "base64",
-            "media_type": f"image/{image.format.lower()}",
-            "data": base64_encode_image(image),
-        }
-    }
-
-
-def str_to_anthropic_text_dict(text: str) -> dict:
+def str_to_openai_text_dict(text: str) -> dict:
     return {
         "type": "text",
         "text": text
     }
 
 
-def json_schema_to_anthropic_tool(name: str, desc: str, schema: dict[str, Any]) -> dict:
+def json_schema_to_openai_function(name: str, desc: str, schema: Dict[str, Any]) -> dict:
     return {
-        "name": name,
-        "description": desc,
-        "input_schema": schema
-    }
+        "type": "function",
+        "function": {
+            "name": name,
+            "description": desc,
+            "parameters": schema
+        }
+    }
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/common/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,21 @@
     def is_video(self) -> bool:
         return self.mimetype.startswith("video/") if self.mimetype else False
 
     def is_text(self) -> bool:
         app_text_mimetypes = [
             'application/json',
             'application/javascript',
-            'application/manifest+json',
             'application/xml',
             'application/x-sh',
             'application/x-python',
+            'application/x-httpd-php',
+            'application/x-httpd-php',
+            'application/x-latex',
+            'application/x-tex',
         ]
         return (self.mimetype.startswith("text/") or self.mimetype in app_text_mimetypes) if self.mimetype else False
 
     async def as_bytes(self) -> bytes:
         """Read data as bytes."""
         if self.data is None and (self.path.startswith('http://') or self.path.startswith('https://')):
             response = requests.get(self.path)
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.4.0/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,19 +148,20 @@
     async def _run_completion(
         self,
         messages: List[ChatMessage],
         tools: List[dict],
         stop: list[str] = None,
         current_try: int = None
     ) -> ChatCompletion:
+        messages = await messages_to_openai_dicts(messages)
         args = {
             "model": self.model,
             "temperature": self.temperature,
             **({"seed": self.seed} if self.seed else {}),
-            "messages": await messages_to_openai_dicts(messages),
+            "messages": messages,
             **({"stop": stop} if stop else {}),
             **({
                    "tool_choice": {
                        "type": "function",
                        "function": {"name": tools[0]["function"]["name"]}
                    } if (len(tools) == 1) else ("auto" if tools else "none"),
                    "tools": tools
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.4.0/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.4.0/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.4.0/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.4.0/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.4.0/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.4.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.4.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.4.0/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.4.0/bpm_ai_core/speech_recognition/asr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.4.0/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.4.0/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.4.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/langfuse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 from bpm_ai_core.tracing.tracer import Tracer
+from bpm_ai_core.util.image import replace_base64_values
 
 try:
     from langfuse import Langfuse
     from langfuse.client import StatefulTraceClient, StatefulSpanClient, StatefulGenerationClient
     has_langfuse = True
 except ImportError:
     has_langfuse = False
@@ -49,17 +50,19 @@
             status_message=error_msg
         )
         logger.info(f"[Langfuse Trace Finished] {self.trace.get_trace_url()}")
         self.trace = None
         self.span_stack = []
 
     def start_span(self, name: str, inputs: dict = None):
-        if not self.trace:
-            raise Exception("No trace started for this thread")
-        if self.span_stack:
+        if not self.trace and not self.span_stack:
+            self.start_trace("unnamed", inputs=inputs)
+            self.implicit_trace = True
+            client = self.trace
+        elif self.span_stack:
             client = self.span_stack[-1]
         else:
             client = self.trace
         span = client.span(name=name, input=inputs)
         self.span_stack.append(span)
 
     def end_span(self, output=None, error_msg: str = None):
@@ -67,21 +70,20 @@
             raise Exception("No span started for this thread")
         span = self.span_stack.pop()
         span.end(
             output=output,
             level="ERROR" if error_msg else None,
             status_message=error_msg
         )
+        if self.implicit_trace:
+            self.end_trace(outputs=output)
 
     def start_llm_trace(self, llm, messages: list, current_try: int, tools=None):
-        if not self.trace and not self.span_stack:
-            self.start_trace("unnamed", inputs=messages)
-            self.implicit_trace = True
-            client = self.trace
-        elif self.span_stack:
+        messages = replace_base64_values(messages)
+        if self.span_stack:
             client = self.span_stack[-1]
         else:
             client = self.trace
 
         self.generation = client.generation(
             model=llm.model,
             model_parameters={
@@ -99,16 +101,14 @@
         if not self.generation:
             raise Exception("No generation started for this thread")
         self.generation.end(
             output=completion,
             level="ERROR" if error_msg else None,
             status_message=error_msg
         )
-        if self.implicit_trace:
-            self.end_trace(outputs=completion)
 
     def start_tool_trace(self, tool, inputs: dict):
         self.start_span(tool.name, inputs)
 
     def end_tool_trace(self, outputs: dict | None = None, error_msg: str | None = None):
         self.end_span(outputs, error_msg)
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 from bpm_ai_core.tracing.tracer import Tracer
+from bpm_ai_core.util.image import replace_base64_values
 
 logger = logging.getLogger("logging-tracer")
 logger.setLevel(logging.INFO)
 
 
 class LoggingTracer(Tracer):
 
@@ -37,15 +38,15 @@
     def event(self, name: str, inputs: dict = None, outputs: dict = None, error_msg: str = None):
         if error_msg:
             logger.error(self._indent() + f"[EVENT] {error_msg}")
         else:
             logger.info(self._indent() + f"[EVENT] {name}, inputs={inputs}, outputs={outputs}")
 
     def start_llm_trace(self, llm, messages, current_try, tools=None):
-        logger.info(self._indent() + f"[LLM <] {llm.model}, current_try: {current_try}, tools={tools}, messages={messages}")
+        logger.info(self._indent() + f"[LLM <] {llm.model}, current_try: {current_try}, tools={tools}, messages={replace_base64_values(messages)}")
 
     def end_llm_trace(self, completion=None, error_msg=None):
         if error_msg:
             logger.error(self._indent() + f"[LLM COMPLETION ERROR] {error_msg}")
             return
         logger.info(self._indent() + f"[LLM >] {completion}")
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.4.0/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.4.0/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.4.0/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/file.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 from typing import List
 from urllib.parse import urlparse
 
 from bpm_ai_core.util.audio import audio_ext_map
 from bpm_ai_core.util.image import image_ext_map, pdf_ext_map
+from bpm_ai_core.util.text import text_ext_map
 
-supported_ext_map = {**audio_ext_map, **image_ext_map, **pdf_ext_map}
+supported_ext_map = {**audio_ext_map, **image_ext_map, **pdf_ext_map, **text_ext_map}
 supported_extensions = supported_ext_map.keys()
 
 
 def guess_mimetype(filename: str) -> str | None:
     if is_supported_file(filename, list(image_ext_map.keys())):
         return image_ext_map[_extract_extension(filename)]
+    elif is_supported_file(filename, list(text_ext_map.keys())):
+        return text_ext_map[_extract_extension(filename)]
     elif is_supported_file(filename, list(pdf_ext_map.keys())):
         return "application/pdf"
     elif is_supported_file(filename, list(audio_ext_map.keys())):
         return audio_ext_map[_extract_extension(filename)]
 
 
 def is_supported_file(url_or_path: str, extensions: List[str] = supported_extensions) -> bool:
@@ -30,19 +33,27 @@
     return is_supported_file(url_or_path, extensions=list(image_ext_map.keys()) + list(pdf_ext_map.keys()))
 
 
 def is_supported_audio_file(url_or_path: str) -> bool:
     return is_supported_file(url_or_path, extensions=list(audio_ext_map.keys()))
 
 
+def is_supported_text_file(url_or_path: str) -> bool:
+    return is_supported_file(url_or_path, extensions=list(text_ext_map.keys()))
+
+
 def _extract_extension(url_or_path):
     url_or_path = url_or_path.strip()
     # Extract the path from URL if it's a URL
     parsed_url = urlparse(url_or_path)
     path = parsed_url.path if parsed_url.scheme else url_or_path
     # Remove trailing slash if present
     if path.endswith('/'):
         path = path[:-1]
     # Extract the file extension
     _, file_extension = os.path.splitext(path)
     file_extension = file_extension.lower().lstrip('.')
     return file_extension
+
+
+def is_file(s: str) -> bool:
+    return s.startswith('http://') or s.startswith('https://') or os.path.exists(os.path.dirname(s))
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/image.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import io
 import logging
+import re
 import tempfile
 from io import BytesIO
 from typing import Union, Tuple
 
 from PIL import Image, ImageDraw
 from pdf2image import convert_from_path, convert_from_bytes
 
@@ -114,14 +115,40 @@
     """
     buffered = BytesIO()
     image.save(buffered, format=image.format or "JPEG")  # Assuming JPEG if format is not provided
     img_str = base64.b64encode(buffered.getvalue())
     return img_str.decode('utf-8')
 
 
+def replace_base64_values(data):
+    if isinstance(data, dict):
+        decoded_dict = {}
+        for key, value in data.items():
+            decoded_dict[key] = replace_base64_values(value)
+        return decoded_dict
+    elif isinstance(data, list):
+        decoded_list = []
+        for item in data:
+            decoded_list.append(replace_base64_values(item))
+        return decoded_list
+    elif isinstance(data, str) and len(data) > 1024 and is_base64(data):
+        return "..."
+    else:
+        return data
+
+
+def is_base64(s: str):
+    try:
+        s = re.sub(r"^data:image/.+;base64,", "", s)
+        base64.b64decode(s, validate=True)
+        return True
+    except:
+        return False
+
+
 def draw_boxes_on_image(image: Image, normalized_boxes: list[Tuple[float, float, float, float]]):
     """
     Draws bounding boxes on a given PIL image and displays the resulting image.
 
     Args:
         image (PIL.Image): The input image.
         normalized_boxes (list): A list of normalized bounding box coordinates.
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/linguistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,7 +180,22 @@
              'fuésemos', 'fueseis', 'fuesen', 'sintiendo', 'sentido', 'sentida', 'sentidos', 'sentidas', 'siente',
              'sentid', 'tengo', 'tienes', 'tiene', 'tenemos', 'tenéis', 'tienen', 'tenga', 'tengas', 'tengamos',
              'tengáis', 'tengan', 'tendré', 'tendrás', 'tendrá', 'tendremos', 'tendréis', 'tendrán', 'tendría',
              'tendrías', 'tendríamos', 'tendríais', 'tendrían', 'tenía', 'tenías', 'teníamos', 'teníais', 'tenían',
              'tuve', 'tuviste', 'tuvo', 'tuvimos', 'tuvisteis', 'tuvieron', 'tuviera', 'tuvieras', 'tuviéramos',
              'tuvierais', 'tuvieran', 'tuviese', 'tuvieses', 'tuviésemos', 'tuvieseis', 'tuviesen', 'teniendo',
              'tenido', 'tenida', 'tenidos', 'tenidas', 'tened']
+
+
+special_char_map = {'ä': 'ae', 'Ä': 'Ae', 'ö': 'oe', 'Ö': 'Oe', 'ü': 'ue', 'Ü': 'Ue', 'ß': 'ss', 'æ': 'ae', 'Æ': 'Ae',
+                    'ø': 'oe', 'Ø': 'Oe', 'ë': 'e', 'Ë': 'E', 'ï': 'i', 'Ï': 'I', 'à': 'a', 'À': 'A', 'â': 'a',
+                    'Â': 'A', 'ç': 'c', 'Ç': 'C', 'é': 'e', 'É': 'E', 'è': 'e', 'È': 'E', 'ê': 'e', 'Ê': 'E', 'î': 'i',
+                    'Î': 'I', 'ô': 'o', 'Ô': 'O', 'œ': 'oe', 'Œ': 'Oe', 'ù': 'u', 'Ù': 'U', 'û': 'u', 'Û': 'U',
+                    'ÿ': 'y', 'Ÿ': 'Y', 'ì': 'i', 'Ì': 'I', 'ò': 'o', 'Ò': 'O', 'ą': 'a', 'Ą': 'A', 'ć': 'c', 'Ć': 'C',
+                    'ę': 'e', 'Ę': 'E', 'ł': 'l', 'Ł': 'L', 'ń': 'n', 'Ń': 'N', 'ó': 'o', 'Ó': 'O', 'ś': 's', 'Ś': 'S',
+                    'ź': 'z', 'Ź': 'Z', 'ż': 'z', 'Ż': 'Z', 'á': 'a', 'Á': 'A', 'ã': 'a', 'Ã': 'A', 'í': 'i', 'Í': 'I',
+                    'õ': 'o', 'Õ': 'O', 'ú': 'u', 'Ú': 'U', 'ñ': 'n', 'Ñ': 'N', 'å': 'a', 'Å': 'A', 'ґ': 'g', 'Ґ': 'G',
+                    'є': 'ye', 'Є': 'Ye', 'і': 'i', 'І': 'I', 'ї': 'yi', 'Ї': 'Yi'}
+
+
+def replace_diacritics(text: str):
+    return ''.join([special_char_map.get(char, char) for char in text])
```

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/remote_object.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/remote_object.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.4.0/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.2/pyproject.toml` & `bpm_ai_core-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.3.2"
+version = "2.4.0"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai_core-2.3.2/PKG-INFO` & `bpm_ai_core-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.3.2
+Version: 2.4.0
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

