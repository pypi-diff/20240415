# Comparing `tmp/qianfan-0.3.8.tar.gz` & `tmp/qianfan-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianfan-0.3.8.tar", max compression
+gzip compressed data, was "qianfan-0.3.8.1.tar", max compression
```

## Comparing `qianfan-0.3.8.tar` & `qianfan-0.3.8.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
--rw-r--r--   0        0        0     6443 2024-04-13 13:35:38.755281 qianfan-0.3.8/README.pypi.md
--rw-r--r--   0        0        0     3772 2024-04-13 13:35:38.755281 qianfan-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1578 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/__init__.py
--rw-r--r--   0        0        0      659 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/__init__.py
--rw-r--r--   0        0        0     2451 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/context.py
--rw-r--r--   0        0        0     4502 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/launcher.py
--rw-r--r--   0        0        0      847 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/base.py
--rw-r--r--   0        0        0     6028 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/infer_runner.py
--rw-r--r--   0        0        0     6278 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/qianfan_runner.py
--rw-r--r--   0        0        0     1460 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/space.py
--rw-r--r--   0        0        0      784 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/__init__.py
--rw-r--r--   0        0        0     3370 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/base.py
--rw-r--r--   0        0        0     3356 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/random_suggestor.py
--rw-r--r--   0        0        0     3973 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/tune.py
--rw-r--r--   0        0        0     1357 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/utils.py
--rw-r--r--   0        0        0      699 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/__init__.py
--rw-r--r--   0        0        0    15290 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/chat.py
--rw-r--r--   0        0        0     7120 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/completion.py
--rw-r--r--   0        0        0    14564 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/dataset.py
--rw-r--r--   0        0        0      790 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/embedding.py
--rw-r--r--   0        0        0     9595 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/evaluation.py
--rw-r--r--   0        0        0     6437 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/main.py
--rw-r--r--   0        0        0     4107 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/openai_adapter.py
--rw-r--r--   0        0        0    17018 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/plugin.py
--rw-r--r--   0        0        0    24762 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/trainer.py
--rw-r--r--   0        0        0     3265 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/txt2img.py
--rw-r--r--   0        0        0     9991 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/utils.py
--rw-r--r--   0        0        0        1 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/hub.py
--rw-r--r--   0        0        0     3512 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/interface.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/__init__.py
--rw-r--r--   0        0        0      963 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/base.py
--rw-r--r--   0        0        0     2982 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/persist.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/__init__.py
--rw-r--r--   0        0        0    30862 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/prompt.py
--rw-r--r--   0        0        0     2215 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/template.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/runnable/__init__.py
--rw-r--r--   0        0        0     7049 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/runnable/base.py
--rw-r--r--   0        0        0     3698 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/baidu_search_tool.py
--rw-r--r--   0        0        0     7561 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/base_tool.py
--rw-r--r--   0        0        0     2962 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/duckduckgo_search_tool.py
--rw-r--r--   0        0        0     3312 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/wikipedia_tool.py
--rw-r--r--   0        0        0     9582 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/config.py
--rw-r--r--   0        0        0    12267 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/consts.py
--rw-r--r--   0        0        0     1367 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/dataset/__init__.py
--rw-r--r--   0        0        0     2786 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/consts.py
--rw-r--r--   0        0        0      600 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/__init__.py
--rw-r--r--   0        0        0     2369 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/assets/index.html
--rw-r--r--   0        0        0      841 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/data_insight_utils.py
--rw-r--r--   0        0        0     8768 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/insight.py
--rw-r--r--   0        0        0     4363 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_operator.py
--rw-r--r--   0        0        0     1013 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/__init__.py
--rw-r--r--   0        0        0    27521 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/baidu_qianfan.py
--rw-r--r--   0        0        0     2701 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/base.py
--rw-r--r--   0        0        0    13584 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/bos.py
--rw-r--r--   0        0        0     9420 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/chunk_reader.py
--rw-r--r--   0        0        0     9532 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/file.py
--rw-r--r--   0        0        0    26192 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/utils.py
--rw-r--r--   0        0        0    71978 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/dataset.py
--rw-r--r--   0        0        0    17893 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/dataset_utils.py
--rw-r--r--   0        0        0     1139 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/__init__.py
--rw-r--r--   0        0        0     2237 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/base.py
--rw-r--r--   0        0        0     3942 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
--rw-r--r--   0        0        0     4482 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_flagged_words.py
--rw-r--r--   0        0        0     2443 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
--rw-r--r--   0        0        0     2504 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_special_characters.py
--rw-r--r--   0        0        0     4313 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_stopwords.py
--rw-r--r--   0        0        0     3085 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_number.py
--rw-r--r--   0        0        0     3910 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
--rw-r--r--   0        0        0     4483 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/consts.py
--rw-r--r--   0        0        0     4693 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/utils.py
--rw-r--r--   0        0        0   136258 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/word_list.py
--rw-r--r--   0        0        0     2832 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/process_interface.py
--rw-r--r--   0        0        0     4363 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/qianfan_data_operators.py
--rw-r--r--   0        0        0    10622 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/schema.py
--rw-r--r--   0        0        0     2010 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/summarization_method.py
--rw-r--r--   0        0        0    49904 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/table.py
--rw-r--r--   0        0        0     1302 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/table_utils.py
--rw-r--r--   0        0        0     2334 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/errors.py
--rw-r--r--   0        0        0      878 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/__init__.py
--rw-r--r--   0        0        0     2748 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/consts.py
--rw-r--r--   0        0        0    26228 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluation_manager.py
--rw-r--r--   0        0        0     1325 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluation_result.py
--rw-r--r--   0        0        0     4484 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluator.py
--rw-r--r--   0        0        0     4379 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/local_evaluator.py
--rw-r--r--   0        0        0     2468 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/opencompass_evaluator.py
--rw-r--r--   0        0        0       66 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/README.md
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/__init__.py
--rw-r--r--   0        0        0      200 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/__init__.py
--rw-r--r--   0        0        0      212 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/agents/__init__.py
--rw-r--r--   0        0        0    13709 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/openai/__init__.py
--rw-r--r--   0        0        0    18554 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/openai/adapter.py
--rw-r--r--   0        0        0     1602 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0     7804 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
--rw-r--r--   0        0        0     1627 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
--rw-r--r--   0        0        0     5365 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
--rw-r--r--   0        0        0     4056 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
--rw-r--r--   0        0        0     2577 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/fake_pyarrow_replacer.py
--rw-r--r--   0        0        0      742 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/__init__.py
--rw-r--r--   0        0        0      923 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/configs.py
--rw-r--r--   0        0        0      938 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/consts.py
--rw-r--r--   0        0        0    23100 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/model.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/py.typed
--rw-r--r--   0        0        0     1648 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/iam.py
--rw-r--r--   0        0        0    15255 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/oauth.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/__init__.py
--rw-r--r--   0        0        0     4183 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/charge.py
--rw-r--r--   0        0        0     7533 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/consts.py
--rw-r--r--   0        0        0    30894 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/data.py
--rw-r--r--   0        0        0    16673 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/finetune.py
--rw-r--r--   0        0        0    23132 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/model.py
--rw-r--r--   0        0        0    19491 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/prompt.py
--rw-r--r--   0        0        0     5607 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/service.py
--rw-r--r--   0        0        0     4941 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/utils.py
--rw-r--r--   0        0        0     3779 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/http_client.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/__init__.py
--rw-r--r--   0        0        0    11411 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/image2text.py
--rw-r--r--   0        0        0    11777 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/text2image.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/__init__.py
--rw-r--r--   0        0        0    27287 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/base.py
--rw-r--r--   0        0        0    42166 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/chat_completion.py
--rw-r--r--   0        0        0    11545 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/completion.py
--rw-r--r--   0        0        0    10678 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/embedding.py
--rw-r--r--   0        0        0    13139 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/plugin.py
--rw-r--r--   0        0        0    14096 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/__init__.py
--rw-r--r--   0        0        0    12846 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/base.py
--rw-r--r--   0        0        0     3189 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/console_requestor.py
--rw-r--r--   0        0        0    22243 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/openapi_requestor.py
--rw-r--r--   0        0        0    10266 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/token_limiter.py
--rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/__init__.py
--rw-r--r--   0        0        0     4909 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/tokenizer.py
--rw-r--r--   0        0        0     3580 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/utils.py
--rw-r--r--   0        0        0     9199 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/typing.py
--rw-r--r--   0        0        0     1141 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/__init__.py
--rw-r--r--   0        0        0    46962 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/actions.py
--rw-r--r--   0        0        0     6000 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/base.py
--rw-r--r--   0        0        0    38188 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/configs.py
--rw-r--r--   0        0        0     3600 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/consts.py
--rw-r--r--   0        0        0     3403 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/event.py
--rw-r--r--   0        0        0    12166 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/finetune.py
--rw-r--r--   0        0        0    10187 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/pipeline.py
--rw-r--r--   0        0        0     8360 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/post_pretrain.py
--rw-r--r--   0        0        0     1680 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/ppl.yaml
--rw-r--r--   0        0        0     4843 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/trainer.py
--rw-r--r--   0        0        0     1244 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/bos_uploader.py
--rw-r--r--   0        0        0      696 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/cache/__init__.py
--rw-r--r--   0        0        0      787 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/cache/base.py
--rw-r--r--   0        0        0      827 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/__init__.py
--rw-r--r--   0        0        0      946 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/compute.py
--rw-r--r--   0        0        0      812 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/functions.py
--rw-r--r--   0        0        0      869 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/ipc.py
--rw-r--r--   0        0        0      984 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/table.py
--rw-r--r--   0        0        0     1084 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/helper.py
--rw-r--r--   0        0        0     5670 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/logging.py
--rw-r--r--   0        0        0      734 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/pydantic/__init__.py
--rw-r--r--   0        0        0     7230 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/utils.py
--rw-r--r--   0        0        0      900 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/version.py
--rw-r--r--   0        0        0    10489 1970-01-01 00:00:00.000000 qianfan-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     6443 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/README.pypi.md
+-rw-r--r--   0        0        0     3774 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1578 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/__init__.py
+-rw-r--r--   0        0        0     2451 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/context.py
+-rw-r--r--   0        0        0     4502 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/launcher.py
+-rw-r--r--   0        0        0      847 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/runner/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/runner/base.py
+-rw-r--r--   0        0        0     6028 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/runner/infer_runner.py
+-rw-r--r--   0        0        0     6278 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/runner/qianfan_runner.py
+-rw-r--r--   0        0        0     1460 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/space.py
+-rw-r--r--   0        0        0      784 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/suggestor/__init__.py
+-rw-r--r--   0        0        0     3370 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/suggestor/base.py
+-rw-r--r--   0        0        0     3356 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/suggestor/random_suggestor.py
+-rw-r--r--   0        0        0     3973 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/tune.py
+-rw-r--r--   0        0        0     1357 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/autotuner/utils.py
+-rw-r--r--   0        0        0      699 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/__init__.py
+-rw-r--r--   0        0        0    15290 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/chat.py
+-rw-r--r--   0        0        0     7120 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/completion.py
+-rw-r--r--   0        0        0    14564 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/dataset.py
+-rw-r--r--   0        0        0      790 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/embedding.py
+-rw-r--r--   0        0        0     9595 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/evaluation.py
+-rw-r--r--   0        0        0     6437 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/main.py
+-rw-r--r--   0        0        0     4107 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/openai_adapter.py
+-rw-r--r--   0        0        0    17018 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/plugin.py
+-rw-r--r--   0        0        0    24762 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/trainer.py
+-rw-r--r--   0        0        0     3265 2024-04-15 07:07:53.081074 qianfan-0.3.8.1/qianfan/common/client/txt2img.py
+-rw-r--r--   0        0        0     9991 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/client/utils.py
+-rw-r--r--   0        0        0        1 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/hub/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/hub/hub.py
+-rw-r--r--   0        0        0     3512 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/hub/interface.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/persister/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/persister/base.py
+-rw-r--r--   0        0        0     2982 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/persister/persist.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/prompt/__init__.py
+-rw-r--r--   0        0        0    30862 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/prompt/prompt.py
+-rw-r--r--   0        0        0     2215 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/prompt/template.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/runnable/__init__.py
+-rw-r--r--   0        0        0     7049 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/runnable/base.py
+-rw-r--r--   0        0        0     3698 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/tool/baidu_search_tool.py
+-rw-r--r--   0        0        0     7561 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/tool/base_tool.py
+-rw-r--r--   0        0        0     2962 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/tool/duckduckgo_search_tool.py
+-rw-r--r--   0        0        0     3312 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/common/tool/wikipedia_tool.py
+-rw-r--r--   0        0        0     9582 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/config.py
+-rw-r--r--   0        0        0    12267 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/consts.py
+-rw-r--r--   0        0        0     1367 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/consts.py
+-rw-r--r--   0        0        0      600 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_insight/__init__.py
+-rw-r--r--   0        0        0     2369 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_insight/assets/index.html
+-rw-r--r--   0        0        0      841 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_insight/data_insight_utils.py
+-rw-r--r--   0        0        0     8768 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_insight/insight.py
+-rw-r--r--   0        0        0     4363 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_operator.py
+-rw-r--r--   0        0        0     1013 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/__init__.py
+-rw-r--r--   0        0        0    27521 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/baidu_qianfan.py
+-rw-r--r--   0        0        0     2701 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/base.py
+-rw-r--r--   0        0        0    13584 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/bos.py
+-rw-r--r--   0        0        0     9436 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/chunk_reader.py
+-rw-r--r--   0        0        0     9532 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/file.py
+-rw-r--r--   0        0        0    26192 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/data_source/utils.py
+-rw-r--r--   0        0        0    72805 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/dataset.py
+-rw-r--r--   0        0        0    17893 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/dataset_utils.py
+-rw-r--r--   0        0        0     1139 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/__init__.py
+-rw-r--r--   0        0        0     2237 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/base.py
+-rw-r--r--   0        0        0     3942 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
+-rw-r--r--   0        0        0     4482 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_flagged_words.py
+-rw-r--r--   0        0        0     2443 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
+-rw-r--r--   0        0        0     2504 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_special_characters.py
+-rw-r--r--   0        0        0     4313 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_stopwords.py
+-rw-r--r--   0        0        0     3085 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_word_number.py
+-rw-r--r--   0        0        0     3910 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
+-rw-r--r--   0        0        0     4483 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/consts.py
+-rw-r--r--   0        0        0     4693 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/utils.py
+-rw-r--r--   0        0        0   136258 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/local_data_operators/word_list.py
+-rw-r--r--   0        0        0     2832 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/process_interface.py
+-rw-r--r--   0        0        0     4363 2024-04-15 07:07:53.085074 qianfan-0.3.8.1/qianfan/dataset/qianfan_data_operators.py
+-rw-r--r--   0        0        0    10622 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/dataset/schema.py
+-rw-r--r--   0        0        0     2010 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/dataset/summarization_method.py
+-rw-r--r--   0        0        0    51211 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/dataset/table.py
+-rw-r--r--   0        0        0     1302 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/dataset/table_utils.py
+-rw-r--r--   0        0        0     2334 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/errors.py
+-rw-r--r--   0        0        0      878 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/__init__.py
+-rw-r--r--   0        0        0     2748 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/consts.py
+-rw-r--r--   0        0        0    26571 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/evaluation_manager.py
+-rw-r--r--   0        0        0     1325 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/evaluation_result.py
+-rw-r--r--   0        0        0     4484 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/evaluator.py
+-rw-r--r--   0        0        0     4379 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/local_evaluator.py
+-rw-r--r--   0        0        0     2468 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/evaluation/opencompass_evaluator.py
+-rw-r--r--   0        0        0       66 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/langchain/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    13709 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/openai/__init__.py
+-rw-r--r--   0        0        0    18554 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/openai/adapter.py
+-rw-r--r--   0        0        0     1602 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0     7804 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
+-rw-r--r--   0        0        0     1627 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
+-rw-r--r--   0        0        0     5365 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
+-rw-r--r--   0        0        0     4056 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
+-rw-r--r--   0        0        0     2577 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/fake_pyarrow_replacer.py
+-rw-r--r--   0        0        0      742 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/model/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/model/configs.py
+-rw-r--r--   0        0        0      938 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/model/consts.py
+-rw-r--r--   0        0        0    23100 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/py.typed
+-rw-r--r--   0        0        0     1648 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/auth/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/auth/iam.py
+-rw-r--r--   0        0        0    15255 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/auth/oauth.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/__init__.py
+-rw-r--r--   0        0        0     4183 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/charge.py
+-rw-r--r--   0        0        0     7533 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/consts.py
+-rw-r--r--   0        0        0    30894 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/data.py
+-rw-r--r--   0        0        0    16673 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/finetune.py
+-rw-r--r--   0        0        0    23132 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/model.py
+-rw-r--r--   0        0        0    19491 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/prompt.py
+-rw-r--r--   0        0        0     5607 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/service.py
+-rw-r--r--   0        0        0     4941 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/console/utils.py
+-rw-r--r--   0        0        0     3779 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/http_client.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/images/__init__.py
+-rw-r--r--   0        0        0    11411 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/images/image2text.py
+-rw-r--r--   0        0        0    11777 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/images/text2image.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/llm/__init__.py
+-rw-r--r--   0        0        0    27287 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/llm/base.py
+-rw-r--r--   0        0        0    42166 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/llm/chat_completion.py
+-rw-r--r--   0        0        0    11545 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/llm/completion.py
+-rw-r--r--   0        0        0    10678 2024-04-15 07:07:53.089074 qianfan-0.3.8.1/qianfan/resources/llm/embedding.py
+-rw-r--r--   0        0        0    13139 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/llm/plugin.py
+-rw-r--r--   0        0        0    14096 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/requestor/__init__.py
+-rw-r--r--   0        0        0    12846 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/requestor/base.py
+-rw-r--r--   0        0        0     3189 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/requestor/console_requestor.py
+-rw-r--r--   0        0        0    22243 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/requestor/openapi_requestor.py
+-rw-r--r--   0        0        0    10266 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/token_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/tools/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/tools/tokenizer.py
+-rw-r--r--   0        0        0     3580 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/tools/utils.py
+-rw-r--r--   0        0        0     9199 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/resources/typing.py
+-rw-r--r--   0        0        0     1141 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/__init__.py
+-rw-r--r--   0        0        0    46962 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/actions.py
+-rw-r--r--   0        0        0     6000 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/base.py
+-rw-r--r--   0        0        0    38188 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/configs.py
+-rw-r--r--   0        0        0     3600 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/consts.py
+-rw-r--r--   0        0        0     3403 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/event.py
+-rw-r--r--   0        0        0    13824 2024-04-15 07:07:53.093074 qianfan-0.3.8.1/qianfan/trainer/finetune.py
+-rw-r--r--   0        0        0    10187 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/trainer/pipeline.py
+-rw-r--r--   0        0        0     8360 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/trainer/post_pretrain.py
+-rw-r--r--   0        0        0     1680 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/trainer/ppl.yaml
+-rw-r--r--   0        0        0     4843 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/trainer/trainer.py
+-rw-r--r--   0        0        0     1244 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/bos_uploader.py
+-rw-r--r--   0        0        0      696 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/cache/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/cache/base.py
+-rw-r--r--   0        0        0      827 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/compute.py
+-rw-r--r--   0        0        0      812 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/functions.py
+-rw-r--r--   0        0        0      869 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/ipc.py
+-rw-r--r--   0        0        0      984 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/table.py
+-rw-r--r--   0        0        0     1084 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/helper.py
+-rw-r--r--   0        0        0     5670 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/logging.py
+-rw-r--r--   0        0        0      734 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0     7230 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/utils/utils.py
+-rw-r--r--   0        0        0      900 2024-04-15 07:07:53.097074 qianfan-0.3.8.1/qianfan/version.py
+-rw-r--r--   0        0        0    10491 1970-01-01 00:00:00.000000 qianfan-0.3.8.1/PKG-INFO
```

### Comparing `qianfan-0.3.8/README.pypi.md` & `qianfan-0.3.8.1/README.pypi.md`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/pyproject.toml` & `qianfan-0.3.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qianfan"
-version = "0.3.8"
+version = "0.3.8.1"
 description = "文心千帆大模型平台 Python SDK"
 authors = []
 license = "Apache-2.0"
 readme = "README.pypi.md"
 exclude = [
     "qianfan/tests",
     "qianfan/docs",
```

### Comparing `qianfan-0.3.8/qianfan/__init__.py` & `qianfan-0.3.8.1/qianfan/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/__init__.py` & `qianfan-0.3.8.1/qianfan/autotuner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/context.py` & `qianfan-0.3.8.1/qianfan/autotuner/context.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/launcher.py` & `qianfan-0.3.8.1/qianfan/autotuner/launcher.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/runner/__init__.py` & `qianfan-0.3.8.1/qianfan/autotuner/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/runner/base.py` & `qianfan-0.3.8.1/qianfan/autotuner/runner/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/runner/infer_runner.py` & `qianfan-0.3.8.1/qianfan/autotuner/runner/infer_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/runner/qianfan_runner.py` & `qianfan-0.3.8.1/qianfan/autotuner/runner/qianfan_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/space.py` & `qianfan-0.3.8.1/qianfan/autotuner/space.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/suggestor/__init__.py` & `qianfan-0.3.8.1/qianfan/autotuner/suggestor/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/suggestor/base.py` & `qianfan-0.3.8.1/qianfan/autotuner/suggestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/suggestor/random_suggestor.py` & `qianfan-0.3.8.1/qianfan/autotuner/suggestor/random_suggestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/tune.py` & `qianfan-0.3.8.1/qianfan/autotuner/tune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/autotuner/utils.py` & `qianfan-0.3.8.1/qianfan/autotuner/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/__init__.py` & `qianfan-0.3.8.1/qianfan/common/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/chat.py` & `qianfan-0.3.8.1/qianfan/common/client/chat.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/completion.py` & `qianfan-0.3.8.1/qianfan/common/client/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/dataset.py` & `qianfan-0.3.8.1/qianfan/common/client/dataset.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/embedding.py` & `qianfan-0.3.8.1/qianfan/common/client/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/evaluation.py` & `qianfan-0.3.8.1/qianfan/common/client/evaluation.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/main.py` & `qianfan-0.3.8.1/qianfan/common/client/main.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/openai_adapter.py` & `qianfan-0.3.8.1/qianfan/common/client/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/plugin.py` & `qianfan-0.3.8.1/qianfan/common/client/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/trainer.py` & `qianfan-0.3.8.1/qianfan/common/client/trainer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/txt2img.py` & `qianfan-0.3.8.1/qianfan/common/client/txt2img.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/client/utils.py` & `qianfan-0.3.8.1/qianfan/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/hub/hub.py` & `qianfan-0.3.8.1/qianfan/common/hub/hub.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/hub/interface.py` & `qianfan-0.3.8.1/qianfan/common/hub/interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/persister/base.py` & `qianfan-0.3.8.1/qianfan/common/persister/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/persister/persist.py` & `qianfan-0.3.8.1/qianfan/common/persister/persist.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/prompt/prompt.py` & `qianfan-0.3.8.1/qianfan/common/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/prompt/template.py` & `qianfan-0.3.8.1/qianfan/common/prompt/template.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/runnable/base.py` & `qianfan-0.3.8.1/qianfan/common/runnable/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/tool/baidu_search_tool.py` & `qianfan-0.3.8.1/qianfan/common/tool/baidu_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/tool/base_tool.py` & `qianfan-0.3.8.1/qianfan/common/tool/base_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/tool/duckduckgo_search_tool.py` & `qianfan-0.3.8.1/qianfan/common/tool/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/common/tool/wikipedia_tool.py` & `qianfan-0.3.8.1/qianfan/common/tool/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/config.py` & `qianfan-0.3.8.1/qianfan/config.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/consts.py` & `qianfan-0.3.8.1/qianfan/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/__init__.py` & `qianfan-0.3.8.1/qianfan/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/consts.py` & `qianfan-0.3.8.1/qianfan/dataset/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_insight/__init__.py` & `qianfan-0.3.8.1/qianfan/dataset/data_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_insight/assets/index.html` & `qianfan-0.3.8.1/qianfan/dataset/data_insight/assets/index.html`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_insight/data_insight_utils.py` & `qianfan-0.3.8.1/qianfan/dataset/data_insight/data_insight_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_insight/insight.py` & `qianfan-0.3.8.1/qianfan/dataset/data_insight/insight.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_operator.py` & `qianfan-0.3.8.1/qianfan/dataset/data_operator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/__init__.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/baidu_qianfan.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/baidu_qianfan.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/base.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/bos.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/bos.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/chunk_reader.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/chunk_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         **kwargs: Any,
     ):
         super().__init__(chunk_size, **kwargs)
 
         self.file_path = file_path
         self.fd = open(file_path, mode="r", encoding=encoding())
 
-        self.ijson_object = ijson.items(self.fd, element_json_path)
+        self.ijson_object = ijson.items(self.fd, element_json_path, use_float=True)
 
     def _get_an_element(self, index: int) -> Any:
         return next(self.ijson_object)
 
 
 class JsonLineReader(BaseReader):
     def __init__(self, file_path: str, chunk_size: int = 10, **kwargs: Any):
```

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/file.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/file.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/data_source/utils.py` & `qianfan-0.3.8.1/qianfan/dataset/data_source/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/dataset.py` & `qianfan-0.3.8.1/qianfan/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1024,14 +1024,44 @@
             **kwargs (Any):
                 other arguments
         Returns:
             Dataset: a sliced dataset
         """
         return super().take_slice(start, end, should_create_new_obj, **kwargs)
 
+    @_online_except_decorator
+    def sample(
+        self,
+        sample_number: int,
+        start: int = 0,
+        end: int = -1,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        """
+        take random slice in dataset
+
+        Args:
+            sample_number (int):
+                how many entries should be sampled
+            start (int):
+                where the sample part starts
+            end (int):
+                where the sample part ends
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any):
+                other arguments
+        """
+        return super().sample(
+            sample_number, start, end, should_create_new_obj, **kwargs
+        )
+
     def __getitem__(self, key: Any) -> Any:
         if (
             isinstance(key, int)
             or isinstance(key, slice)
             or (isinstance(key, (list, tuple)) and key and isinstance(key[0], int))
         ):
             return self.list(key)
@@ -2016,16 +2046,14 @@
         from tabulate import tabulate
 
         if not methods or len(methods) == 0:
             methods = [
                 MeanMethod(),
                 MinMethod(),
                 MaxMethod(),
-                QuantileMethod(q=0.2),
-                QuantileMethod(q=0.5),
                 QuantileMethod(q=0.8),
                 QuantileMethod(q=0.9),
             ]
 
         columns = [k for k, v in self.list(0).items() if isinstance(v, (int, float))]
         result_data = [method.calculate(self, columns, **kwargs) for method in methods]
         index_names = [method.name for method in methods]
```

### Comparing `qianfan-0.3.8/qianfan/dataset/dataset_utils.py` & `qianfan-0.3.8.1/qianfan/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/__init__.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/base.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_character_repetition_filter.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_flagged_words.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_flagged_words.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_sentence_length_filter.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_special_characters.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_special_characters.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_stopwords.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_stopwords.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_number.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_word_number.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_repetition_filter.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/consts.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/utils.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/local_data_operators/word_list.py` & `qianfan-0.3.8.1/qianfan/dataset/local_data_operators/word_list.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/process_interface.py` & `qianfan-0.3.8.1/qianfan/dataset/process_interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/qianfan_data_operators.py` & `qianfan-0.3.8.1/qianfan/dataset/qianfan_data_operators.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/schema.py` & `qianfan-0.3.8.1/qianfan/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/summarization_method.py` & `qianfan-0.3.8.1/qianfan/dataset/summarization_method.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/dataset/table.py` & `qianfan-0.3.8.1/qianfan/dataset/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 wrapper for pyarrow.Table
 """
+import random
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
     Optional,
@@ -515,14 +516,46 @@
             raise ValueError(err_msg)
 
         if end < 0:
             end = self.table.num_rows - 1
 
         return self.table.slice(start, end - start + 1)
 
+    def sample(
+        self,
+        sample_number: int,
+        start: int = 0,
+        end: int = -1,
+    ) -> PyarrowTable:
+        if start < 0:
+            err_msg = f"start index is smaller than 0: {start}"
+            log_error(err_msg)
+            raise ValueError(err_msg)
+
+        if end >= self.table.num_rows:
+            err_msg = (
+                f"end index {end} is bigger than table size: {self.table.num_rows}"
+            )
+            log_error(err_msg)
+            raise ValueError(err_msg)
+
+        if end < 0:
+            end = self.table.num_rows - 1
+
+        if sample_number < 0:
+            err_msg = f"can't sample {sample_number} entries"
+            log_error(err_msg)
+            raise ValueError(err_msg)
+
+        if sample_number >= self.table.num_rows:
+            return self.table
+
+        numbers = random.sample(range(start, end + 1), sample_number)
+        return self.table.take(numbers)
+
 
 class _PyarrowColumnManipulator(BaseModel, Addable, Listable, Processable):
     """handler for processing of pyarrow table column"""
 
     class Config:
         arbitrary_types_allowed = True
 
@@ -1189,14 +1222,26 @@
         should_create_new_obj: bool = False,
         **kwargs: Any,
     ) -> Self:
         manipulator = self._row_op()
         result_ds = manipulator.take_slice(start, end)
         return self._create_new_obj(result_ds, should_create_new_obj)
 
+    def sample(
+        self,
+        sample_number: int,
+        start: int = 0,
+        end: int = -1,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        manipulator = self._row_op()
+        result_ds = manipulator.sample(sample_number, start, end)
+        return self._create_new_obj(result_ds, should_create_new_obj)
+
     def col_map(
         self,
         op: Callable[[Any], Any],
         should_create_new_obj: bool = False,
         **kwargs: Any,
     ) -> Self:
         """
```

### Comparing `qianfan-0.3.8/qianfan/dataset/table_utils.py` & `qianfan-0.3.8.1/qianfan/dataset/table_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/errors.py` & `qianfan-0.3.8.1/qianfan/errors.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/__init__.py` & `qianfan-0.3.8.1/qianfan/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/consts.py` & `qianfan-0.3.8.1/qianfan/evaluation/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/evaluation_manager.py` & `qianfan-0.3.8.1/qianfan/evaluation/evaluation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,15 +417,28 @@
 
         if not EvaluationSchema().validate(dataset):
             raise ValueError("validate failed before evaluation")
 
         tmp_ds = Dataset.create_from_pyobj(
             self._run_evaluator_locally(dataset, **kwargs)
         )
-        return EvaluationResult(result_dataset=dataset.col_append(tmp_ds.col_list()))
+
+        assert self.local_evaluators
+
+        summarization_dict: Dict[str, Any] = {}
+
+        for evaluator in self.local_evaluators:
+            summarization = evaluator.summarize(tmp_ds)
+            if summarization:
+                summarization_dict.update(summarization)
+
+        return EvaluationResult(
+            metrics=summarization_dict,
+            result_dataset=dataset.col_append(tmp_ds.col_list()),
+        )
 
     def eval(
         self,
         llms: Sequence[Union[Model, Service]],
         dataset: Dataset,
         download_when_doing_online: bool = True,
         **kwargs: Any,
```

### Comparing `qianfan-0.3.8/qianfan/evaluation/evaluation_result.py` & `qianfan-0.3.8.1/qianfan/evaluation/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/evaluator.py` & `qianfan-0.3.8.1/qianfan/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/local_evaluator.py` & `qianfan-0.3.8.1/qianfan/evaluation/local_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/evaluation/opencompass_evaluator.py` & `qianfan-0.3.8.1/qianfan/evaluation/opencompass_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py` & `qianfan-0.3.8.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/openai/adapter.py` & `qianfan-0.3.8.1/qianfan/extensions/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/semantic_kernel/__init__.py` & `qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py` & `qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py` & `qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py` & `qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py` & `qianfan-0.3.8.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/fake_pyarrow_replacer.py` & `qianfan-0.3.8.1/qianfan/fake_pyarrow_replacer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/model/__init__.py` & `qianfan-0.3.8.1/qianfan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/model/configs.py` & `qianfan-0.3.8.1/qianfan/model/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/model/consts.py` & `qianfan-0.3.8.1/qianfan/model/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/model/model.py` & `qianfan-0.3.8.1/qianfan/model/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/__init__.py` & `qianfan-0.3.8.1/qianfan/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/auth/iam.py` & `qianfan-0.3.8.1/qianfan/resources/auth/iam.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/auth/oauth.py` & `qianfan-0.3.8.1/qianfan/resources/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/charge.py` & `qianfan-0.3.8.1/qianfan/resources/console/charge.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/consts.py` & `qianfan-0.3.8.1/qianfan/resources/console/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/data.py` & `qianfan-0.3.8.1/qianfan/resources/console/data.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/finetune.py` & `qianfan-0.3.8.1/qianfan/resources/console/finetune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/model.py` & `qianfan-0.3.8.1/qianfan/resources/console/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/prompt.py` & `qianfan-0.3.8.1/qianfan/resources/console/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/service.py` & `qianfan-0.3.8.1/qianfan/resources/console/service.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/console/utils.py` & `qianfan-0.3.8.1/qianfan/resources/console/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/http_client.py` & `qianfan-0.3.8.1/qianfan/resources/http_client.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/images/image2text.py` & `qianfan-0.3.8.1/qianfan/resources/images/image2text.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/images/text2image.py` & `qianfan-0.3.8.1/qianfan/resources/images/text2image.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/llm/base.py` & `qianfan-0.3.8.1/qianfan/resources/llm/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/llm/chat_completion.py` & `qianfan-0.3.8.1/qianfan/resources/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/llm/completion.py` & `qianfan-0.3.8.1/qianfan/resources/llm/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/llm/embedding.py` & `qianfan-0.3.8.1/qianfan/resources/llm/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/llm/plugin.py` & `qianfan-0.3.8.1/qianfan/resources/llm/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/rate_limiter.py` & `qianfan-0.3.8.1/qianfan/resources/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/requestor/base.py` & `qianfan-0.3.8.1/qianfan/resources/requestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/requestor/console_requestor.py` & `qianfan-0.3.8.1/qianfan/resources/requestor/console_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/requestor/openapi_requestor.py` & `qianfan-0.3.8.1/qianfan/resources/requestor/openapi_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/token_limiter.py` & `qianfan-0.3.8.1/qianfan/resources/token_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/tools/tokenizer.py` & `qianfan-0.3.8.1/qianfan/resources/tools/tokenizer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/tools/utils.py` & `qianfan-0.3.8.1/qianfan/resources/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/resources/typing.py` & `qianfan-0.3.8.1/qianfan/resources/typing.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/__init__.py` & `qianfan-0.3.8.1/qianfan/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/actions.py` & `qianfan-0.3.8.1/qianfan/trainer/actions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/base.py` & `qianfan-0.3.8.1/qianfan/trainer/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/configs.py` & `qianfan-0.3.8.1/qianfan/trainer/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/consts.py` & `qianfan-0.3.8.1/qianfan/trainer/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/event.py` & `qianfan-0.3.8.1/qianfan/trainer/event.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/finetune.py` & `qianfan-0.3.8.1/qianfan/trainer/finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     TrainConfig,
 )
 from qianfan.trainer.consts import (
     TrainStatus,
 )
 from qianfan.trainer.pipeline import Pipeline
 from qianfan.trainer.trainer import Trainer
+from qianfan.utils.logging import log_info
 
 
 class Finetune(Trainer):
     """
     Class implements the SFT training pipeline with several actions.
     Use `run()` to synchronously run the training pipeline until the
     model training is finished.
@@ -274,15 +275,15 @@
         )
 
     @property
     def output(self) -> Any:
         if self.result[0]:
             return self.result[0]
         else:
-            return self.info()["actions"][-1]["output"]
+            return self.info()["actions"][-1].get("output")
 
     @classmethod
     def train_type_list(cls) -> Dict[str, ModelInfo]:
         return ModelInfoMapping
 
     @staticmethod
     def list() -> List["Trainer"]:
@@ -304,14 +305,16 @@
     @staticmethod
     def load(id: Optional[str] = None, file: Optional[str] = None) -> "Trainer":
         if file is not None:
             with open(file=file, mode="rb") as f:
                 task_ppl = Pipeline.load(f.read())
         elif id:
             task_ppl = cast(Pipeline, g_persister.load(id, Pipeline))
+            # load完save到本地
+            g_persister.save(task_ppl)
         else:
             raise InvalidArgumentError("invalid id or file to load")
         assert isinstance(task_ppl, Pipeline)
         if (
             task_ppl._case_init_params is not None
             and task_ppl._case_init_params.get("case_type") == Finetune.__name__
         ):
@@ -331,9 +334,49 @@
         tmp = cast(Pipeline, g_persister.load(self.id, Pipeline))
         return tmp._action_dict()
 
     @property
     def id(self) -> str:
         return self.ppls[0].id
 
+    def show(self) -> None:
+        if self.output and self.output.get("checkpoints"):
+            try:
+                import matplotlib.pyplot as plt
+            except ImportError:
+                raise RuntimeError(
+                    "matplotlib is required to show the training lossing, "
+                    "please install it by `pip install matplotlib`."
+                )
+
+            checkpoints = self.output["checkpoints"]
+            steps = [ckpt["step"] for ckpt in checkpoints]
+            loss = [ckpt["trainingLoss"] for ckpt in checkpoints]
+            perplexity = [ckpt["perplexity"] for ckpt in checkpoints]
+
+            # 创建图形和轴对象
+            _, ax1 = plt.subplots()
+
+            # 绘制 loss 曲线（使用左侧 Y 轴）
+            ax1.plot(steps, loss, color="tab:blue", label="Loss")
+            ax1.set_xlabel("Step")
+            ax1.set_ylabel("Loss", color="tab:blue")
+
+            # 创建第二个 Y 轴
+            ax2 = ax1.twinx()
+            ax2.plot(steps, perplexity, color="tab:red", label="Perplexity")
+            ax2.set_ylabel("Perplexity", color="tab:red")
+
+            # 添加图例
+            lines, labels = ax1.get_legend_handles_labels()
+            lines2, labels2 = ax2.get_legend_handles_labels()
+            ax2.legend(lines + lines2, labels + labels2, loc="upper right")
+
+            # 设置标题
+            plt.title("Loss and Perplexity over Steps")
+
+            plt.show()
+        else:
+            log_info("no checkpoints to show, check if finished")
+
 
 LLMFinetune = Finetune
```

### Comparing `qianfan-0.3.8/qianfan/trainer/pipeline.py` & `qianfan-0.3.8.1/qianfan/trainer/pipeline.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/post_pretrain.py` & `qianfan-0.3.8.1/qianfan/trainer/post_pretrain.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/ppl.yaml` & `qianfan-0.3.8.1/qianfan/trainer/ppl.yaml`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/trainer/trainer.py` & `qianfan-0.3.8.1/qianfan/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/__init__.py` & `qianfan-0.3.8.1/qianfan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/bos_uploader.py` & `qianfan-0.3.8.1/qianfan/utils/bos_uploader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/cache/__init__.py` & `qianfan-0.3.8.1/qianfan/utils/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/cache/base.py` & `qianfan-0.3.8.1/qianfan/utils/cache/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/fake_pyarrow/__init__.py` & `qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/fake_pyarrow/compute.py` & `qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/compute.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/fake_pyarrow/functions.py` & `qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/functions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/fake_pyarrow/ipc.py` & `qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/ipc.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/fake_pyarrow/table.py` & `qianfan-0.3.8.1/qianfan/utils/fake_pyarrow/table.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/helper.py` & `qianfan-0.3.8.1/qianfan/utils/helper.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/logging.py` & `qianfan-0.3.8.1/qianfan/utils/logging.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/pydantic/__init__.py` & `qianfan-0.3.8.1/qianfan/utils/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/utils/utils.py` & `qianfan-0.3.8.1/qianfan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/qianfan/version.py` & `qianfan-0.3.8.1/qianfan/version.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8/PKG-INFO` & `qianfan-0.3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qianfan
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: 文心千帆大模型平台 Python SDK
 Home-page: https://cloud.baidu.com/product/wenxinworkshop
 License: Apache-2.0
 Keywords: baidu,qianfan
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

