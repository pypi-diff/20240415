# Comparing `tmp/openplugin-0.1.6.tar.gz` & `tmp/openplugin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.1.6.tar", max compression
+gzip compressed data, was "openplugin-0.1.7.tar", max compression
```

## Comparing `openplugin-0.1.6.tar` & `openplugin-0.1.7.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0     3757 2024-03-29 18:25:14.375472 openplugin-0.1.6/LICENSE
--rw-r--r--   0        0        0     6105 2024-03-29 18:25:14.375472 openplugin-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/__init__.py
--rw-r--r--   0        0        0       51 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/__main__.py
--rw-r--r--   0        0        0     1482 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/__init__.py
--rw-r--r--   0        0        0       59 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/application.py
--rw-r--r--   0        0        0     1506 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/auth.py
--rw-r--r--   0        0        0      490 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/http_error.py
--rw-r--r--   0        0        0     1179 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/info.py
--rw-r--r--   0        0        0     1121 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/operation_execution.py
--rw-r--r--   0        0        0     4555 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/operation_signature_builder.py
--rw-r--r--   0        0        0     2979 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/plugin_execution_pipeline.py
--rw-r--r--   0        0        0     2751 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/api/plugin_selector.py
--rw-r--r--   0        0        0      903 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/__init__.py
--rw-r--r--   0        0        0     7959 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/execution/implementations/operation_execution_with_imprompt.py
--rw-r--r--   0        0        0     1567 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/execution/operation_execution.py
--rw-r--r--   0        0        0     2925 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/flow_path.py
--rw-r--r--   0        0        0    11968 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/functions.py
--rw-r--r--   0        0        0     1189 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/helper.py
--rw-r--r--   0        0        0     4057 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/llms.py
--rw-r--r--   0        0        0      757 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/messages.py
--rw-r--r--   0        0        0     7086 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_imprompt.py
--rw-r--r--   0        0        0     5518 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_langchain.py
--rw-r--r--   0        0        0     8197 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_openai.py
--rw-r--r--   0        0        0     1706 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/operations/operation_signature_builder.py
--rw-r--r--   0        0        0     8317 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/plugin.py
--rw-r--r--   0        0        0     1139 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/plugin_detected.py
--rw-r--r--   0        0        0    13301 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/plugin_execution_pipeline.py
--rw-r--r--   0        0        0     2385 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/plugin_runner.py
--rw-r--r--   0        0        0     3586 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/port.py
--rw-r--r--   0        0        0     9031 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_imprompt.py
--rw-r--r--   0        0        0     6131 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_langchain.py
--rw-r--r--   0        0        0     4476 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_openai.py
--rw-r--r--   0        0        0     1843 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/core/selectors/plugin_selector.py
--rw-r--r--   0        0        0     2069 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/main.py
--rw-r--r--   0        0        0      424 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/__init__.py
--rw-r--r--   0        0        0     1066 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/audio_to_text/audio_to_text.py
--rw-r--r--   0        0        0      550 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/audio_to_text/audio_to_text_factory.py
--rw-r--r--   0        0        0      737 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/audio_to_text/implementations/audio_to_text_with_whisper.py
--rw-r--r--   0        0        0     1118 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_cloud/file_to_cloud.py
--rw-r--r--   0        0        0      505 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_cloud/file_to_cloud_factory.py
--rw-r--r--   0        0        0      974 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_cloud/implementations/file_to_cloud_with_s3.py
--rw-r--r--   0        0        0     1123 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_text/file_to_text.py
--rw-r--r--   0        0        0      550 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_text/file_to_text_factory.py
--rw-r--r--   0        0        0        0 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_text/implementations/file_to_text_from_S3.py
--rw-r--r--   0        0        0      686 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/file_to_text/implementations/file_to_text_with_langchain.py
--rw-r--r--   0        0        0     1115 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/html_to_text/html_to_text.py
--rw-r--r--   0        0        0      497 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/html_to_text/html_to_text_factory.py
--rw-r--r--   0        0        0      566 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/html_to_text/implementations/html_to_text_with_bs.py
--rw-r--r--   0        0        0      927 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/llm_engine/implementations/llm_engine_with_openai.py
--rw-r--r--   0        0        0     1145 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/llm_engine/llm_engine.py
--rw-r--r--   0        0        0      501 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/llm_engine/llm_engine_factory.py
--rw-r--r--   0        0        0     3705 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/processor.py
--rw-r--r--   0        0        0     3096 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/processor_factory.py
--rw-r--r--   0        0        0      841 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/template_engine/implementations/template_engine_with_jinja.py
--rw-r--r--   0        0        0      683 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/template_engine/implementations/template_engine_with_jsx.py
--rw-r--r--   0        0        0     1167 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/template_engine/template_engine.py
--rw-r--r--   0        0        0      782 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/template_engine/template_engine_factory.py
--rw-r--r--   0        0        0     2925 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_audio/implementations/text_to_audio_with_azure.py
--rw-r--r--   0        0        0     1126 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_audio/text_to_audio.py
--rw-r--r--   0        0        0      528 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_audio/text_to_audio_factory.py
--rw-r--r--   0        0        0      846 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_file/implementations/text_to_file_with_default.py
--rw-r--r--   0        0        0     1123 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_file/text_to_file.py
--rw-r--r--   0        0        0      517 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/text_to_file/text_to_file_factory.py
--rw-r--r--   0        0        0      588 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/url_to_html/implementations/url_to_html_with_request.py
--rw-r--r--   0        0        0     1067 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/url_to_html/url_to_html.py
--rw-r--r--   0        0        0      509 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/processors/url_to_html/url_to_html_factory.py
--rw-r--r--   0        0        0      284 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/settings.py
--rw-r--r--   0        0        0      199 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/utils/__init__.py
--rw-r--r--   0        0        0     2270 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/utils/langchain_helpers.py
--rw-r--r--   0        0        0     4318 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/utils/llm_manager_handler.py
--rw-r--r--   0        0        0     3431 2024-03-29 18:25:14.387472 openplugin-0.1.6/openplugin/utils/manifest_handler.py
--rw-r--r--   0        0        0      678 2024-03-29 18:25:14.391472 openplugin-0.1.6/openplugin/utils/openai_helpers.py
--rw-r--r--   0        0        0     3917 2024-03-29 18:25:14.391472 openplugin-0.1.6/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0     2078 2024-03-29 18:25:14.391472 openplugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7351 1970-01-01 00:00:00.000000 openplugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3757 2024-04-15 21:45:27.594246 openplugin-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4189 2024-04-15 21:45:27.594246 openplugin-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/__main__.py
+-rw-r--r--   0        0        0     2057 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/application.py
+-rw-r--r--   0        0        0     1506 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/auth.py
+-rw-r--r--   0        0        0      490 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/http_error.py
+-rw-r--r--   0        0        0     1179 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/info.py
+-rw-r--r--   0        0        0     1121 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/operation_execution.py
+-rw-r--r--   0        0        0     4555 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/operation_signature_builder.py
+-rw-r--r--   0        0        0     2979 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/plugin_execution_pipeline.py
+-rw-r--r--   0        0        0     2751 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/plugin_selector.py
+-rw-r--r--   0        0        0      572 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/api/processors.py
+-rw-r--r--   0        0        0      903 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/__init__.py
+-rw-r--r--   0        0        0     7959 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/execution/implementations/operation_execution_with_imprompt.py
+-rw-r--r--   0        0        0     1567 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/execution/operation_execution.py
+-rw-r--r--   0        0        0     2925 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/flow_path.py
+-rw-r--r--   0        0        0    12459 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/functions.py
+-rw-r--r--   0        0        0     1189 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/helper.py
+-rw-r--r--   0        0        0     4057 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/llms.py
+-rw-r--r--   0        0        0      757 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/messages.py
+-rw-r--r--   0        0        0     7086 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_imprompt.py
+-rw-r--r--   0        0        0     5518 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_langchain.py
+-rw-r--r--   0        0        0     8447 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_openai.py
+-rw-r--r--   0        0        0     1706 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/operations/operation_signature_builder.py
+-rw-r--r--   0        0        0     8317 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/plugin.py
+-rw-r--r--   0        0        0     1139 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/plugin_detected.py
+-rw-r--r--   0        0        0    13970 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/plugin_execution_pipeline.py
+-rw-r--r--   0        0        0     2385 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/plugin_runner.py
+-rw-r--r--   0        0        0     3586 2024-04-15 21:45:27.602246 openplugin-0.1.7/openplugin/core/port.py
+-rw-r--r--   0        0        0     9031 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_imprompt.py
+-rw-r--r--   0        0        0     6131 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_langchain.py
+-rw-r--r--   0        0        0     4725 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_openai.py
+-rw-r--r--   0        0        0     1843 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/core/selectors/plugin_selector.py
+-rw-r--r--   0        0        0     1945 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/main.py
+-rw-r--r--   0        0        0      424 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/audio_to_text/audio_to_text.py
+-rw-r--r--   0        0        0      550 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/audio_to_text/audio_to_text_factory.py
+-rw-r--r--   0        0        0      737 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/audio_to_text/implementations/audio_to_text_with_whisper.py
+-rw-r--r--   0        0        0     1118 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_cloud/file_to_cloud.py
+-rw-r--r--   0        0        0      505 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_cloud/file_to_cloud_factory.py
+-rw-r--r--   0        0        0      974 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_cloud/implementations/file_to_cloud_with_s3.py
+-rw-r--r--   0        0        0     1123 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_text/file_to_text.py
+-rw-r--r--   0        0        0      550 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_text/file_to_text_factory.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_text/implementations/file_to_text_from_S3.py
+-rw-r--r--   0        0        0      686 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/file_to_text/implementations/file_to_text_with_langchain.py
+-rw-r--r--   0        0        0     1115 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/html_to_text/html_to_text.py
+-rw-r--r--   0        0        0      497 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/html_to_text/html_to_text_factory.py
+-rw-r--r--   0        0        0      566 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/html_to_text/implementations/html_to_text_with_bs.py
+-rw-r--r--   0        0        0      927 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/llm_engine/implementations/llm_engine_with_openai.py
+-rw-r--r--   0        0        0     1145 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/llm_engine/llm_engine.py
+-rw-r--r--   0        0        0      501 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/llm_engine/llm_engine_factory.py
+-rw-r--r--   0        0        0     3705 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/processor.py
+-rw-r--r--   0        0        0     3096 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/processor_factory.py
+-rw-r--r--   0        0        0      841 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/template_engine/implementations/template_engine_with_jinja.py
+-rw-r--r--   0        0        0      683 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/template_engine/implementations/template_engine_with_jsx.py
+-rw-r--r--   0        0        0     1167 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/template_engine/template_engine.py
+-rw-r--r--   0        0        0      782 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/template_engine/template_engine_factory.py
+-rw-r--r--   0        0        0     2925 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_audio/implementations/text_to_audio_with_azure.py
+-rw-r--r--   0        0        0     1126 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_audio/text_to_audio.py
+-rw-r--r--   0        0        0      528 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_audio/text_to_audio_factory.py
+-rw-r--r--   0        0        0      846 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_file/implementations/text_to_file_with_default.py
+-rw-r--r--   0        0        0     1123 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_file/text_to_file.py
+-rw-r--r--   0        0        0      517 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/text_to_file/text_to_file_factory.py
+-rw-r--r--   0        0        0      588 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/url_to_html/implementations/url_to_html_with_request.py
+-rw-r--r--   0        0        0     1067 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/url_to_html/url_to_html.py
+-rw-r--r--   0        0        0      509 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/processors/url_to_html/url_to_html_factory.py
+-rw-r--r--   0        0        0     9735 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/resources/processors.json
+-rw-r--r--   0        0        0      284 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/settings.py
+-rw-r--r--   0        0        0      199 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/__init__.py
+-rw-r--r--   0        0        0     2270 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/langchain_helpers.py
+-rw-r--r--   0        0        0     4318 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/llm_manager_handler.py
+-rw-r--r--   0        0        0     3431 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/manifest_handler.py
+-rw-r--r--   0        0        0      678 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/openai_helpers.py
+-rw-r--r--   0        0        0     3917 2024-04-15 21:45:27.606246 openplugin-0.1.7/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0     2078 2024-04-15 21:45:27.610246 openplugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 openplugin-0.1.7/PKG-INFO
```

### Comparing `openplugin-0.1.6/LICENSE` & `openplugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/README.md` & `openplugin-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,78 @@
+Metadata-Version: 2.1
+Name: openplugin
+Version: 0.1.7
+Summary: 
+Author: shrikant
+Author-email: shrikant.pm14@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: azure-cognitiveservices-speech (==1.35.0)
+Requires-Dist: boto3 (>=1.29.3,<2.0.0)
+Requires-Dist: fastapi (==0.109.2)
+Requires-Dist: google-cloud-aiplatform (==1.35.0)
+Requires-Dist: langchain (>=0.1.12,<0.2.0)
+Requires-Dist: langchain-fireworks (>=0.1.1,<0.2.0)
+Requires-Dist: langchain-mistralai (>=0.0.5,<0.0.6)
+Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
+Requires-Dist: litellm (==1.23.14)
+Requires-Dist: load-dotenv (>=0.1.0,<0.2.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: openai (==1.12.0)
+Requires-Dist: pydantic (==2.6.1)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pydub (>=0.25.1,<0.26.0)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0)
+Description-Content-Type: text/markdown
+
 <h1 align="center">
         OpenPlugin
     </h1>
     <p align="center">
         <p align="center">:open_hands::electric_plug: Multimodal API Bridge - make APIs into chat and multimodal ready interfaces
         <br>
     </p>
 <h4 align="center">
     <a href="https://openplugin.com/" target="_blank">
         <img src="https://img.shields.io/badge/view-documentation-blue" alt="View Documentation">
     </a>
     <a href="https://pypi.org/project/openplugin/" target="_blank">
         <img src="https://img.shields.io/pypi/v/openplugin.svg" alt="PyPI Version">
     </a>
+    <a href="https://pypi.org/project/openplugin/" target="_blank">
+        <img src="https://img.shields.io/badge/Python-3.9-blue" alt="python">
+    </a>
 </h4>
 
 ![Openplugin banner image](docs/source/_images/openplugin_hero_header.png)
 
 
 This is an open source effort to create an ecosystem around LLM enabled APIs. We make it easy to "chat with an API", that is, to send natural language as the input to the API and have it process it. Then, we offer several options to easily transform the APIs response into something better suited for human consumption like text, markdown, HTML, JSX, voice, video, etc.
 
 ---
 
-**Design Decisions:**
-- LLM neutral (LLMs leapfrog each other in capability; swap easily, support many)
-- Framework neutral (langchain, semantic kernel, ...)
-- Deployment model neutral (serverless, containers, k8, ... )
-- Language neutral (our manifest is declarative JSON)
-- Client neutral (e.g., we're not hard coded to ChatGPT or Gemini, ...)
-- Multimodal opinionated (it's built into our architecture from day 1, but you choose providers)
-- Flow / agent neutral (it's a layer above us)
-- Quality control opinionated (we encourage regression tests for plugins)
-- Cloud neutral (offer containers, offer serverless, ...)
-
-**NOTE**: Please see the complete documentation here: https://openplugin.com/
-
-## About OpenPlugin Manifest:
-
-The OpenPlugin Manifest is a superset of the OpenAPI effort. It focuses on improving a few key areas including:
-- Accuracy is a core element
-- Emphasis on quality: linked to regression tests
-- Integration w/marketplace a priority
-- Ensure security; agent oriented reputation
-
-**Why not use OpenAPI/Swagger?**
-
-OpenAPI (previously, Swagger) was released over a decade ago as a replacement to WSDL, where they switched the interface description from XML to JSON. Both WSDL and OpenAPI focused on the machine-to-machine use case. They answered the question, how can we describe an API in a formal manner to bind a client with a service. OpenAPI describes many of the concepts needed, but falls short in the new GPT oriented requirements.
-
-## Architecture
-
-<div align="center">
-    <img src="docs/source/_images/architecture.png" alt="Openplugin banner image" height="300">
-</div>
-
-### Basic Scenario
- 
- Target Plugin: Google Finance API
- 
- Input Request: "get the stock price for Amazon."
- 
- Optional Responses:
- 1. standard JSON response object
- 2. a formatted response (HTML, Markdown, JSX, ...)
- 3. a multimodal response (text-to-voice, image, ...)
+### Starting a Server
 
-
-### Usage: starting an openplugin server
-
-#### 1. Starting Openplugin server from PyPI
+#### 1. Starting an OpenPlugin Server from PyPI
 
 ```
 pip install openplugin
 openplugin --help
 export OPENAI_API_KEY=<your key>
 openplugin start-server
 ```
 
-#### 2. Starting Openplugin server from docker
+#### 2. Starting OpenPlugin Server from Docker
 
 ```
 # Passing environment variables in the startup script
 docker run --name openplugin_container -p 8006:8006 -e "OPENAI_API_KEY=<your_key>" -e "COHERE_API_KEY=<your_key>" -e "GOOGLE_APPLICATION_CREDENTIALS=<your_key>" -d shrikant14/openplugin:latest
   
 
 # Passing environment variables as a file
@@ -88,45 +81,36 @@
     [variable1-name]=[value1]
     [variable2-name]=[value2]
     [variable3-name]=[value3]
 docker run --name openplugin_container -p 8006:8006 --env-file my_env.env -d shrikant14/openplugin:latest
 
 ```
 
-#### 3. Starting OpenPlugin server from code
+#### 3. Starting an OpenPlugin Server from code
 
 ```
 git clone <openplugin>
 cd openplugin
 poetry install
 python openplugin/main.py run-plugin --openplugin manifests/sample_klarna.json --prompt sample_prompt.txt --log-level="FLOW"
 ```
 
-### Usage: build an OpenPlugin
-
-##### Build an OpenPlugin manifest in your text editor
-
-```
-COMING SOON
-```
-
-
-### Usage: run an OpenPlugin
+### Run an OpenPlugin
 
 #### 1. Run an OpenPlugin using PyPI
 
 ```
 pip install openplugin
 openplugin --help
 export OPENAI_API_KEY=<your key>
 openplugin start-servero
 openplugin run-plugin --openplugin manifests/sample_klarna.json --prompt sample_prompt.txt --log-level="FLOW"
 ```
 
-#### 2. Run an OpenPlugin using server API
+#### 2. Run via an API call 
 
 ```
 curl --location 'https://api.imprompt.ai/openplugin/api/plugin-execution-pipeline' \
            --header 'Content-Type: application/json' \
            --header 'x-api-key: 'YOUR-API-KEY' \
            --data '{
             "prompt": "USER_PROMPT",
@@ -147,26 +131,26 @@
               "name": "OAI functions-OpenAI",
               "pre_prompt": null
             },
             "output_module_names":["default_cleanup_response"]
             }'
 ```
 
-#### 3. Run an OpenPlugin using code
+#### 3. Run via Code
 
 ```
 pip install openplugin
 
 from openplugin.core.plugin_runner import run_prompt_on_plugin
 openplugin=""
 prompt=""
 response =await run_prompt_on_plugin(openplugin, prompt)
 ```
 
-#### 4. Run an OpenPlugin using openplugin-sdk
+#### 4. Run via SDK
 
 **NOTE:** Learn more about openplugin-sdk at: https://github.com/ImpromptAI/openplugin-sdk
 
 ```
 pip install openplugin-sdk
 
 remote_server_endpoint = "...."
@@ -187,7 +171,8 @@
 print(f"Response={response.value}")
 ```
 
 
 
 
 
+
```

#### html2text {}

```diff
@@ -1,73 +1,63 @@
+Metadata-Version: 2.1 Name: openplugin Version: 0.1.7 Summary: Author: shrikant
+Author-email: shrikant.pm14@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: azure-cognitiveservices-
+speech (==1.35.0) Requires-Dist: boto3 (>=1.29.3,<2.0.0) Requires-Dist: fastapi
+(==0.109.2) Requires-Dist: google-cloud-aiplatform (==1.35.0) Requires-Dist:
+langchain (>=0.1.12,<0.2.0) Requires-Dist: langchain-fireworks (>=0.1.1,<0.2.0)
+Requires-Dist: langchain-mistralai (>=0.0.5,<0.0.6) Requires-Dist: langchain-
+openai (>=0.0.8,<0.0.9) Requires-Dist: litellm (==1.23.14) Requires-Dist: load-
+dotenv (>=0.1.0,<0.2.0) Requires-Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist:
+openai (==1.12.0) Requires-Dist: pydantic (==2.6.1) Requires-Dist: pydantic-
+settings (>=2.2.1,<3.0.0) Requires-Dist: pydub (>=0.25.1,<0.26.0) Requires-
+Dist: requests (==2.31.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist:
+typer[all] (>=0.9.0,<0.10.0) Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0) Description-Content-Type: text/
+markdown
                            ************ OOppeennPPlluuggiinn ************
   :open_hands::electric_plug: Multimodal API Bridge - make APIs into chat and
                           multimodal ready interfaces
-                  ****** _[[_VV_ii_ee_ww_ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_]]_[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]] ******
+              ****** _[[_VV_ii_ee_ww_ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_]]_[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_pp_yy_tt_hh_oo_nn_]] ******
 ![Openplugin banner image](docs/source/_images/openplugin_hero_header.png) This
 is an open source effort to create an ecosystem around LLM enabled APIs. We
 make it easy to "chat with an API", that is, to send natural language as the
 input to the API and have it process it. Then, we offer several options to
 easily transform the APIs response into something better suited for human
-consumption like text, markdown, HTML, JSX, voice, video, etc. --- **Design
-Decisions:** - LLM neutral (LLMs leapfrog each other in capability; swap
-easily, support many) - Framework neutral (langchain, semantic kernel, ...) -
-Deployment model neutral (serverless, containers, k8, ... ) - Language neutral
-(our manifest is declarative JSON) - Client neutral (e.g., we're not hard coded
-to ChatGPT or Gemini, ...) - Multimodal opinionated (it's built into our
-architecture from day 1, but you choose providers) - Flow / agent neutral (it's
-a layer above us) - Quality control opinionated (we encourage regression tests
-for plugins) - Cloud neutral (offer containers, offer serverless, ...)
-**NOTE**: Please see the complete documentation here: https://openplugin.com/
-## About OpenPlugin Manifest: The OpenPlugin Manifest is a superset of the
-OpenAPI effort. It focuses on improving a few key areas including: - Accuracy
-is a core element - Emphasis on quality: linked to regression tests -
-Integration w/marketplace a priority - Ensure security; agent oriented
-reputation **Why not use OpenAPI/Swagger?** OpenAPI (previously, Swagger) was
-released over a decade ago as a replacement to WSDL, where they switched the
-interface description from XML to JSON. Both WSDL and OpenAPI focused on the
-machine-to-machine use case. They answered the question, how can we describe an
-API in a formal manner to bind a client with a service. OpenAPI describes many
-of the concepts needed, but falls short in the new GPT oriented requirements.
-## Architecture
-                           [Openplugin banner image]
-### Basic Scenario Target Plugin: Google Finance API Input Request: "get the
-stock price for Amazon." Optional Responses: 1. standard JSON response object
-2. a formatted response (HTML, Markdown, JSX, ...) 3. a multimodal response
-(text-to-voice, image, ...) ### Usage: starting an openplugin server #### 1.
-Starting Openplugin server from PyPI ``` pip install openplugin openplugin --
-help export OPENAI_API_KEY= openplugin start-server ``` #### 2. Starting
-Openplugin server from docker ``` # Passing environment variables in the
-startup script docker run --name openplugin_container -p 8006:8006 -
-e "OPENAI_API_KEY=" -e "COHERE_API_KEY=" -e "GOOGLE_APPLICATION_CREDENTIALS=" -
-d shrikant14/openplugin:latest # Passing environment variables as a file nano
-[env-filename] Add to file [variable1-name]=[value1] [variable2-name]=[value2]
-[variable3-name]=[value3] docker run --name openplugin_container -p 8006:8006 -
--env-file my_env.env -d shrikant14/openplugin:latest ``` #### 3. Starting
-OpenPlugin server from code ``` git clone cd openplugin poetry install python
-openplugin/main.py run-plugin --openplugin manifests/sample_klarna.json --
-prompt sample_prompt.txt --log-level="FLOW" ``` ### Usage: build an OpenPlugin
-##### Build an OpenPlugin manifest in your text editor ``` COMING SOON ``` ###
-Usage: run an OpenPlugin #### 1. Run an OpenPlugin using PyPI ``` pip install
-openplugin openplugin --help export OPENAI_API_KEY= openplugin start-servero
-openplugin run-plugin --openplugin manifests/sample_klarna.json --prompt
-sample_prompt.txt --log-level="FLOW" ``` #### 2. Run an OpenPlugin using server
-API ``` curl --location 'https://api.imprompt.ai/openplugin/api/plugin-
-execution-pipeline' \ --header 'Content-Type: application/json' \ --header 'x-
-api-key: 'YOUR-API-KEY' \ --data '{ "prompt": "USER_PROMPT", "conversation":
-[], "openplugin_manifest_url": "MANIFEST_URL", "header":{}, "approach":
+consumption like text, markdown, HTML, JSX, voice, video, etc. --- ### Starting
+a Server #### 1. Starting an OpenPlugin Server from PyPI ``` pip install
+openplugin openplugin --help export OPENAI_API_KEY= openplugin start-server ```
+#### 2. Starting OpenPlugin Server from Docker ``` # Passing environment
+variables in the startup script docker run --name openplugin_container -p 8006:
+8006 -e "OPENAI_API_KEY=" -e "COHERE_API_KEY=" -
+e "GOOGLE_APPLICATION_CREDENTIALS=" -d shrikant14/openplugin:latest # Passing
+environment variables as a file nano [env-filename] Add to file [variable1-
+name]=[value1] [variable2-name]=[value2] [variable3-name]=[value3] docker run -
+-name openplugin_container -p 8006:8006 --env-file my_env.env -d shrikant14/
+openplugin:latest ``` #### 3. Starting an OpenPlugin Server from code ``` git
+clone cd openplugin poetry install python openplugin/main.py run-plugin --
+openplugin manifests/sample_klarna.json --prompt sample_prompt.txt --log-
+level="FLOW" ``` ### Run an OpenPlugin #### 1. Run an OpenPlugin using PyPI ```
+pip install openplugin openplugin --help export OPENAI_API_KEY= openplugin
+start-servero openplugin run-plugin --openplugin manifests/sample_klarna.json -
+-prompt sample_prompt.txt --log-level="FLOW" ``` #### 2. Run via an API call
+``` curl --location 'https://api.imprompt.ai/openplugin/api/plugin-execution-
+pipeline' \ --header 'Content-Type: application/json' \ --header 'x-api-key:
+'YOUR-API-KEY' \ --data '{ "prompt": "USER_PROMPT", "conversation": [],
+"openplugin_manifest_url": "MANIFEST_URL", "header":{}, "approach":
 { "base_strategy": "oai functions", "llm": { "frequency_penalty": 0,
 "max_tokens": 2048, "model_name": "gpt-3.5-turbo-0613", "presence_penalty": 0,
 "provider": "OpenAI", "temperature": 0, "top_p": 1 }, "name": "OAI functions-
 OpenAI", "pre_prompt": null }, "output_module_names":
-["default_cleanup_response"] }' ``` #### 3. Run an OpenPlugin using code ```
-pip install openplugin from openplugin.core.plugin_runner import
-run_prompt_on_plugin openplugin="" prompt="" response =await
-run_prompt_on_plugin(openplugin, prompt) ``` #### 4. Run an OpenPlugin using
-openplugin-sdk **NOTE:** Learn more about openplugin-sdk at: https://
-github.com/ImpromptAI/openplugin-sdk ``` pip install openplugin-sdk
+["default_cleanup_response"] }' ``` #### 3. Run via Code ``` pip install
+openplugin from openplugin.core.plugin_runner import run_prompt_on_plugin
+openplugin="" prompt="" response =await run_prompt_on_plugin(openplugin,
+prompt) ``` #### 4. Run via SDK **NOTE:** Learn more about openplugin-sdk at:
+https://github.com/ImpromptAI/openplugin-sdk ``` pip install openplugin-sdk
 remote_server_endpoint = "...." openplugin_api_key = "...." svc =
 OpenpluginService( remote_server_endpoint=remote_server_endpoint,
 api_key=openplugin_api_key ) openplugin_manifest_url = "...." prompt = "..."
 output_module_name="..." response = svc.run
 ( openplugin_manifest_url=openplugin_manifest_url, prompt=prompt,
 output_module_names=[output_module_name], ) print(f"Response={response.value}")
 ```
```

### Comparing `openplugin-0.1.6/openplugin/api/auth.py` & `openplugin-0.1.7/openplugin/api/auth.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/api/info.py` & `openplugin-0.1.7/openplugin/api/info.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/api/operation_execution.py` & `openplugin-0.1.7/openplugin/api/operation_execution.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/api/operation_signature_builder.py` & `openplugin-0.1.7/openplugin/api/operation_signature_builder.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/api/plugin_execution_pipeline.py` & `openplugin-0.1.7/openplugin/api/plugin_execution_pipeline.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/api/plugin_selector.py` & `openplugin-0.1.7/openplugin/api/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/__init__.py` & `openplugin-0.1.7/openplugin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/execution/implementations/operation_execution_with_imprompt.py` & `openplugin-0.1.7/openplugin/core/execution/implementations/operation_execution_with_imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/execution/operation_execution.py` & `openplugin-0.1.7/openplugin/core/execution/operation_execution.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/flow_path.py` & `openplugin-0.1.7/openplugin/core/flow_path.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/functions.py` & `openplugin-0.1.7/openplugin/core/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any, Dict, List, Optional
 
 import requests
 from pydantic import BaseModel
 
 from .plugin import Plugin
-
+import re
 
 class API(BaseModel):
     url: str
     method: str
 
     def call(self, params):
         if self.method.lower() == "get":
@@ -71,16 +71,21 @@
                 obj["items"] = param_property.items
             if param_property.enum:
                 obj["enum"] = param_property.enum
             map[param_property.name] = obj
         return map
 
     def get_openai_function_json(self):
+        # validate for litellm character restrictions: r"^[a-zA-Z0-9_-]{1,64}$"
+        pattern = re.compile("[a-zA-Z0-9_-]{1,64}")
+        matches = pattern.findall(self.name)
+        validated_name = ''.join(matches)
+
         json = {
-            "name": self.name,
+            "name": validated_name,
             "description": self.description,
             "parameters": {
                 "type": self.param_type,
                 "properties": self.get_property_map(),
                 "required": self.get_required_properties(),
             },
         }
@@ -192,15 +197,20 @@
             for method in paths[path]:
                 if valid_operations is not None:
                     if f"{path}_{method}" not in valid_operations:
                         continue
                 details = paths[path][method]
                 function_values: Dict[str, Any] = {}
                 function_values["api"] = API(url=f"{server_url}{path}", method=method)
-                function_values["name"] = f"{method}{path.replace('/', '_')}"
+
+                # validate for litellm character restrictions: r"^[a-zA-Z0-9_-]{1,64}$"
+                pattern = re.compile("[a-zA-Z0-9_-]{1,64}")
+                matches = pattern.findall(f"{method}{path.replace('/', '_')}")
+                validated_name = ''.join(matches)
+                function_values["name"] = validated_name
                 if details.get("summary") is None:
                     function_values["description"] = function_values["name"]
                 else:
                     function_values["description"] = details.get("summary")
                 function_values["param_type"] = "object"
                 if method.lower() == "get":
                     g_properties = []
```

### Comparing `openplugin-0.1.6/openplugin/core/helper.py` & `openplugin-0.1.7/openplugin/core/helper.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/llms.py` & `openplugin-0.1.7/openplugin/core/llms.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/messages.py` & `openplugin-0.1.7/openplugin/core/messages.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_imprompt.py` & `openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_langchain.py` & `openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/operations/implementations/operation_signature_builder_with_openai.py` & `openplugin-0.1.7/openplugin/core/operations/implementations/operation_signature_builder_with_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import time
 from typing import List, Optional
+import re
 import litellm
 
 from openplugin.core import (
     LLM,
     Config,
     Functions,
     Message,
@@ -172,15 +173,19 @@
         message = response["choices"][0]["message"]
         message_json = message.json()
         if (
             message_json
             and isinstance(message_json, dict)
             and message_json.get("function_call")
         ):
-            function_name = message_json["function_call"]["name"]
+            # validate for litellm character restrictions: r"^[a-zA-Z0-9_-]{1,64}$"
+            pattern = re.compile("[a-zA-Z0-9_-]{1,64}")
+            matches = pattern.findall(message_json["function_call"]["name"])
+            validated_name = ''.join(matches)
+            function_name = validated_name
             detected_plugin = functions.get_plugin_from_func_name(function_name)
             detected_function = functions.get_function_from_func_name(function_name)
             arguments = json.loads(message_json["function_call"]["arguments"])
             p_detected = PluginDetectedParams(
                 plugin=detected_plugin,
                 api_called=detected_function.get_api_url(),
                 method=detected_function.get_api_method(),
```

### Comparing `openplugin-0.1.6/openplugin/core/operations/operation_signature_builder.py` & `openplugin-0.1.7/openplugin/core/operations/operation_signature_builder.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/plugin.py` & `openplugin-0.1.7/openplugin/core/plugin.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/plugin_detected.py` & `openplugin-0.1.7/openplugin/core/plugin_detected.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/plugin_execution_pipeline.py` & `openplugin-0.1.7/openplugin/core/plugin_execution_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from .operations.implementations.operation_signature_builder_with_langchain import (
     LangchainOperationSignatureBuilder,
 )
 from .plugin import Plugin, PreferredApproach
 from .port import Port, PortMetadata, PortType, PortValueError
 
+import re
 
 async def run_module(output_module, flow_port):
     logger.info(f"\n[RUNNING_OUTPUT_MODULE] {output_module}")
     output_port = await output_module.run(flow_port)
     output_port.name = output_module.name
     if output_module.default_module:
         output_port.add_metadata(PortMetadata.DEFAULT_OUTPUT_MODULE, True)
@@ -278,18 +279,33 @@
         auth_query_param: Optional[dict],
         preferred_approach: PreferredApproach,
     ) -> APIExecutionStepResponse:
         if input.data_type != PortType.JSON:
             raise Exception("Input data type to plugin must be JSON.")
         if input.value is None:
             raise PortValueError("Input value cannot be None")
-
-        api_called = input.value.get("api_called")
+        
+        api_called = input.value.get("api_called") 
         method = input.value.get("method")
         query_params = input.value.get("mapped_operation_parameters")
+
+        # identify path parameters
+        pattern = re.compile(r'\{([^}]+)\}')
+        path_params = pattern.findall(api_called)
+
+        # use path parameter values instead of names in endpoint
+            # "example.com/path/{id}" >> "example.com/path/1"
+        for param_name in path_params:
+            if param_name in query_params:
+                parameter_key = f'{{{param_name}}}'
+                parameter_value = str(query_params[param_name])
+                api_called = api_called.replace(parameter_key, parameter_value)
+
+                # remove matched path parameters from query_params
+                del query_params[param_name]
         logger.info(
             f"\n[RUNNING_PLUGIN_EXECUTION] url={api_called}, method={method}"
         )
         if auth_query_param:
             query_params.update(auth_query_param)
         params = OperationExecutionParams(
             config=config,
```

### Comparing `openplugin-0.1.6/openplugin/core/plugin_runner.py` & `openplugin-0.1.7/openplugin/core/plugin_runner.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/port.py` & `openplugin-0.1.7/openplugin/core/port.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_imprompt.py` & `openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_langchain.py` & `openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/core/selectors/implementations/plugin_selector_with_openai.py` & `openplugin-0.1.7/openplugin/core/selectors/implementations/plugin_selector_with_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Message,
     Plugin,
     PluginDetected,
     SelectedPluginsResponse,
 )
 
 from ..plugin_selector import PluginSelector
-
+import re
 
 class OpenAIPluginSelector(PluginSelector):
     def __init__(
         self,
         plugins: List[Plugin],
         config: Optional[Config],
         llm: Optional[LLM],
@@ -82,15 +82,19 @@
             messages=f_messages,
             functions=function_json,
             function_call="auto",
         )
         message = response["choices"][0]["message"]
         detected_plugins = []
         if message.get("function_call"):
-            function_name = message.get("function_call").name
+            # validate for litellm character restrictions: r"^[a-zA-Z0-9_-]{1,64}$"
+            pattern = re.compile("[a-zA-Z0-9_-]{1,64}")
+            matches = pattern.findall(message.get("function_call").name)
+            validated_name = ''.join(matches)
+            function_name = validated_name
             detected_plugin = functions.get_plugin_from_func_name(function_name)
             detected_function = functions.get_function_from_func_name(function_name)
             p_detected = PluginDetected(
                 plugin=detected_plugin,
                 api_called=detected_function.get_api_url(),
                 method=detected_function.get_api_method(),
             )
```

### Comparing `openplugin-0.1.6/openplugin/core/selectors/plugin_selector.py` & `openplugin-0.1.7/openplugin/core/selectors/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/main.py` & `openplugin-0.1.7/openplugin/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,36 +17,31 @@
     """
     Permutate is an automated testing framework for LLM Plugins.
     """
 
 
 @app.command()
 def start_server(
-    openai_api_key: Optional[
+    env_file: Optional[
         Annotated[
             str,
             typer.Option(
-                help="OpenAI API Key", rich_help_panel="Customization and Utils"
+                help="ENV File Location", rich_help_panel="Customization and Utils"
             ),
         ]
     ]
 ):
     """
     Start the openplugin server
     """
-    if openai_api_key is None:
-        if os.environ.get("OPENAI_API_KEY") is None:
-            typer.echo("OPENAI_API_KEY is not set.")
-            raise typer.Exit(code=1)
-    else:
-        load_dotenv()
-        os.environ["OPENAI_API_KEY"] = openai_api_key
-
+    if env_file is None:
+        typer.echo("Please pass environment file path.")
+        raise typer.Exit(code=1)
+    load_dotenv(env_file)
     from openplugin.api import create_app
-
     app = create_app()
     uvicorn.run(
         app,
         host=os.environ.get("HOST", "0.0.0.0"),
         port=int(os.environ.get("PORT", 8012)),
     )
```

### Comparing `openplugin-0.1.6/openplugin/processors/audio_to_text/audio_to_text.py` & `openplugin-0.1.7/openplugin/processors/audio_to_text/audio_to_text.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/audio_to_text/audio_to_text_factory.py` & `openplugin-0.1.7/openplugin/processors/audio_to_text/audio_to_text_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/audio_to_text/implementations/audio_to_text_with_whisper.py` & `openplugin-0.1.7/openplugin/processors/audio_to_text/implementations/audio_to_text_with_whisper.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/file_to_cloud/file_to_cloud.py` & `openplugin-0.1.7/openplugin/processors/file_to_cloud/file_to_cloud.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/file_to_cloud/implementations/file_to_cloud_with_s3.py` & `openplugin-0.1.7/openplugin/processors/file_to_cloud/implementations/file_to_cloud_with_s3.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/file_to_text/file_to_text.py` & `openplugin-0.1.7/openplugin/processors/file_to_text/file_to_text.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/file_to_text/file_to_text_factory.py` & `openplugin-0.1.7/openplugin/processors/file_to_text/file_to_text_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/file_to_text/implementations/file_to_text_with_langchain.py` & `openplugin-0.1.7/openplugin/processors/file_to_text/implementations/file_to_text_with_langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/html_to_text/html_to_text.py` & `openplugin-0.1.7/openplugin/processors/html_to_text/html_to_text.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/html_to_text/implementations/html_to_text_with_bs.py` & `openplugin-0.1.7/openplugin/processors/html_to_text/implementations/html_to_text_with_bs.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/llm_engine/implementations/llm_engine_with_openai.py` & `openplugin-0.1.7/openplugin/processors/llm_engine/implementations/llm_engine_with_openai.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/llm_engine/llm_engine.py` & `openplugin-0.1.7/openplugin/processors/llm_engine/llm_engine.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/processor.py` & `openplugin-0.1.7/openplugin/processors/processor.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/processor_factory.py` & `openplugin-0.1.7/openplugin/processors/processor_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/template_engine/implementations/template_engine_with_jinja.py` & `openplugin-0.1.7/openplugin/processors/template_engine/implementations/template_engine_with_jinja.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/template_engine/implementations/template_engine_with_jsx.py` & `openplugin-0.1.7/openplugin/processors/template_engine/implementations/template_engine_with_jsx.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/template_engine/template_engine.py` & `openplugin-0.1.7/openplugin/processors/template_engine/template_engine.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/template_engine/template_engine_factory.py` & `openplugin-0.1.7/openplugin/processors/template_engine/template_engine_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_audio/implementations/text_to_audio_with_azure.py` & `openplugin-0.1.7/openplugin/processors/text_to_audio/implementations/text_to_audio_with_azure.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_audio/text_to_audio.py` & `openplugin-0.1.7/openplugin/processors/text_to_audio/text_to_audio.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_audio/text_to_audio_factory.py` & `openplugin-0.1.7/openplugin/processors/text_to_audio/text_to_audio_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_file/implementations/text_to_file_with_default.py` & `openplugin-0.1.7/openplugin/processors/text_to_file/implementations/text_to_file_with_default.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_file/text_to_file.py` & `openplugin-0.1.7/openplugin/processors/text_to_file/text_to_file.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/text_to_file/text_to_file_factory.py` & `openplugin-0.1.7/openplugin/processors/text_to_file/text_to_file_factory.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/url_to_html/implementations/url_to_html_with_request.py` & `openplugin-0.1.7/openplugin/processors/url_to_html/implementations/url_to_html_with_request.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/processors/url_to_html/url_to_html.py` & `openplugin-0.1.7/openplugin/processors/url_to_html/url_to_html.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/utils/langchain_helpers.py` & `openplugin-0.1.7/openplugin/utils/langchain_helpers.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/utils/llm_manager_handler.py` & `openplugin-0.1.7/openplugin/utils/llm_manager_handler.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/utils/manifest_handler.py` & `openplugin-0.1.7/openplugin/utils/manifest_handler.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/utils/openai_helpers.py` & `openplugin-0.1.7/openplugin/utils/openai_helpers.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/openplugin/utils/run_plugin_selector.py` & `openplugin-0.1.7/openplugin/utils/run_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.1.6/pyproject.toml` & `openplugin-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.1.12"
```

