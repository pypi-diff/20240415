# Comparing `tmp/ms-swift-1.7.3.tar.gz` & `tmp/ms-swift-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms-swift-1.7.3.tar", last modified: Sun Mar 17 12:21:49 2024, max compression
+gzip compressed data, was "dist/ms-swift-2.0.0.tar", last modified: Mon Apr 15 08:42:44 2024, max compression
```

## Comparing `ms-swift-1.7.3.tar` & `ms-swift-2.0.0.tar`

### file list

```diff
@@ -1,222 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-17 12:21:45.000000 ms-swift-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    45694 2024-03-17 12:21:49.000000 ms-swift-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40731 2024-03-17 12:21:45.000000 ms-swift-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45694 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-17 12:21:49.000000 ms-swift-1.7.3/ms_swift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-17 12:21:45.000000 ms-swift-1.7.3/requirements/aigc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-17 12:21:45.000000 ms-swift-1.7.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-17 12:21:45.000000 ms-swift-1.7.3/requirements/framework.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-17 12:21:45.000000 ms-swift-1.7.3/requirements/llm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-17 12:21:45.000000 ms-swift-1.7.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-17 12:21:49.000000 ms-swift-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-17 12:21:45.000000 ms-swift-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/aigc/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/animatediff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/animatediff_infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/aigc/diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_sdxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/aigc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/aigc/utils/argument.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/app_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/merge_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/cli/web_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/push_to_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/snapshot_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/hub/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/llm/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/agent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/app_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/llm/data/
--rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/data/self_cognition.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/dpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/llm/ds_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/ds_config/zero2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/ds_config/zero3.json
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/llm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47609 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46976 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    96158 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    44987 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    32005 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/llm/utils/vllm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/dpo_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/trainers/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/adafactor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/adamw8bit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/galore_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/optimizers/galore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/trainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    43552 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/llamapro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/tuners/longlora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/longlora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17244 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/longlora/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/longlora/longlora.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    34829 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/module_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/neftune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/restuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/restuning_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/tuners/rome/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/compute_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/compute_v.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/context_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/nethook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/repr_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/rome/rome_hparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/tuners/scetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/scetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/scetuning/scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/scetuning/scetuning_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/side.py
--rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/tuners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/ui/llm_infer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_infer/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18409 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_infer/llm_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_infer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_infer/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/ui/llm_train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/llm_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15535 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/self_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/ui/llm_train/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/swift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/np_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-17 12:21:45.000000 ms-swift-1.7.3/swift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/hub/test_check_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20171 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/llm/test_vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/model_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/tests/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_extra_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_merged_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_neft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_swift_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_swift_device_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/tuners/test_swift_restuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:49.000000 ms-swift-1.7.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-17 12:21:45.000000 ms-swift-1.7.3/tests/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 08:42:39.000000 ms-swift-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    54434 2024-04-15 08:42:44.000000 ms-swift-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49082 2024-04-15 08:42:39.000000 ms-swift-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    54434 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/aigc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/framework.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/llm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:42:44.000000 ms-swift-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-15 08:42:39.000000 ms-swift-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/animatediff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/animatediff_infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_sdxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/utils/argument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/app_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/merge_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/web_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/push_to_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/snapshot_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/agent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/app_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/data/self_cognition.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/dpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/ds_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/ds_config/zero2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/ds_config/zero3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51305 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107400 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51488 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/torchacc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/dpo_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30353 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adafactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw8bit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/galore_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43987 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/llamapro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/longlora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/longlora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40712 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/module_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/neftune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/restuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/restuning_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/rome/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/compute_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/compute_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/context_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/nethook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/repr_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/rome_hparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/scetuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/scetuning_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/llm_infer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18409 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/llm_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/llm_train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/llm_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/self_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/np_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/hub/test_check_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/model_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_extra_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_merged_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_neft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23706 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_device_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_restuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/test_torch_utils.py
```

### Comparing `ms-swift-1.7.3/PKG-INFO` & `ms-swift-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,539 +1,562 @@
-Metadata-Version: 2.1
-Name: ms-swift
-Version: 1.7.3
-Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
-Home-page: https://github.com/modelscope/swift
-Author: DAMO ModelScope teams
-Author-email: contact@modelscope.cn
-License: Apache License 2.0
-Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
-        
-        <p align="center">
-            <br>
-            <img src="https://modelscope.oss-cn-beijing.aliyuncs.com/modelscope.gif" width="400"/>
-            <br>
-        <p>
-        <p align="center">
-        <a href="https://modelscope.cn/home">ModelScope Community</a>
-        <br>
-                <a href="README_CN.md">中文</a>&nbsp ｜ &nbspEnglish&nbsp ｜ &nbsp<a href="https://github.com/modelscope/swift/blob/main/docs/source/GetStarted/%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8.md">Docs</a>
-        </p>
-        
-        
-        <p align="center">
-        <img src="https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg">
-        <img src="https://img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg">
-        <a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
-        <a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
-        <a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
-        <a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
-        <a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
-        </p>
-        
-        ## 📖 Table of Contents
-        - [Introduction](#-introduction)
-        - [News](#-news)
-        - 🔥[LLM Training and Inference](#-llm-training-and-inference)
-        - 🔥[SCEdit Tuner](#-SCEdit)
-        - [Installation](#-installation)
-        - [Getting Started](#-getting-started)
-        - [Learn More](#-learn-more)
-        - [License](#license)
-        - [Contact Us](#-contact-us)
-        
-        ## 📝 Introduction
-        SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning) is an extensible framework designed to facilitate lightweight model fine-tuning and inference. It integrates implementations for various efficient fine-tuning methods,  by embracing approaches that is parameter-efficient, memory-efficient, and time-efficient. SWIFT integrates seamlessly into ModelScope ecosystem and offers the capabilities to finetune various models, with a primary emphasis on LLMs and vision models. Additionally, SWIFT is fully compatible with [PEFT](https://github.com/huggingface/peft), enabling users to  leverage the familiar Peft interface to finetune ModelScope models.
-        
-        Currently supported approaches (and counting):
-        
-        1. 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
-        2. 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf)
-        3. 🔥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf)
-        4. 🔥SCEdit: [SCEdit: Efficient and Controllable Image Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/2312.11392)  < [arXiv](https://arxiv.org/abs/2312.11392)  |  [Project Page](https://scedit.github.io/) >
-        5. 🔥NEFTune: [Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914)
-        6. QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2309.14717).
-        7. LongLoRA: [Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
-        8. ROME: [Rank-One Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317)
-        9. Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/1902.00751)
-        10. Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/2203.12119)
-        11. Side: [Side-Tuning: A Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503)
-        12. Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859)  < [arXiv](https://arxiv.org/abs/2310.19859)  |  [Project Page](https://res-tuning.github.io/)  |  [Usage](docs/source/GetStarted/ResTuning.md) >
-        13. All tuners offered on [PEFT](https://github.com/huggingface/peft), like IA3, AdaLoRA
-        
-        Key features:
-        
-        1. By integrating the ModelScope library, models can be readily obtained via a model-id.
-        2. Tuners provided by SWIFT can be combined to allow exploration of multiple tuners on a model for best result.
-        3. Support calling `activate_adapter` or `deactivate_adapter` or `set_active_adapters`  to activate/deactivate tuners. User can inference with one model and multiple tuners in different threads independently.
-        4. Support training and inference with scripts/CLI，meanwhile support inference with Web-UI.
-        5. Support model deployment(vllm/chatglm.cpp/xinference)，Check [Official documentation](./docs/source/GetStarted/部署指南.md) for details.
-        
-        Users can check the [documentation of SWIFT](docs/source/GetStarted/快速使用.md) to get detail tutorials.
-        
-        
-        ## 🎉 News
-        - 🔥2024.03.12: Supports inference and fine-tuning for the **deepseek-vl** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/deepseek-vl最佳实践.md).
-        - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507), which can efficiently reduce the memory usage(almost half of the original memory) when training the full model.
-        - 🔥2024.03.10: For the end-to-end best practice of fine-tuning to deployment of Qwen1.5-7B-Chat and Qwen1.5-72B-Chat, you can refer to the [Qwen1.5 Full Workflow Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md).
-        - 🔥2024.03.09: Support training and inference of MAMBA series, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to begin.
-        - 2024.03.09: Support training and inference of AQLM quantized models, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to begin.
-        - 2024.03.06: Support training and inference of AWQ quantized models, use [this Qwen1.5-AWQ script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to begin, support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
-        - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to begin.
-        - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to begin.
-        - 2024.02.25: Support `swift export` to export models for **AWQ/GPTQ** quantization and push to ModelScope Hub. For more details, please refer to the document: [LLM Quantization Document](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E9%87%8F%E5%8C%96%E6%96%87%E6%A1%A3.md).
-        - 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
-        - 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
-        - 🔥2024.02.05: Support **Qwen1.5** series, To view all supported Qwen1.5 models please check [Model List](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B). The [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8) fine-tuned scripts are provided.
-        - 2024.02.05: Support the training of **SDXL**, **SD**, **ControlNet**, or techniques like **DreamBooth**, you can check the [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
-        - 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
-        - 🔥2024.02.01: Support dataset mixture to reduce **Catastrophic Forgetting**. Use `--train_dataset_mix_ratio 2.0` to train! We also provide a common knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
-        - 🔥2024.02.01: Support Agent training! Agent training algorithm comes from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also introduce the [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary) dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to begin an agent training!
-        - 🔥2024.02.01: Support SFT loss to DPO training to reduce the repeat generation problem caused by the KL-divergence loss.
-        - 2024.02.01: Support AdaLoRA and IA3 adapter in SFT.
-        - 2024.02.01: Support `--merge_lora` in AnimateDiff training.
-        <details><summary>More</summary>
-        
-        - 2024.01.30: Support [internlm-xcomposer2-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm_xcomposer2_7b_chat).
-        - 🔥2024.01.30: Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), just need to specify `--deepspeed default-zero3`.
-        - 2024.01.29: Support internlm2-math series: internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat.
-        - 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
-        - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
-        - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
-        - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
-        - 🔥2024.01.17: Support **internlm2** series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
-        - 2024.1.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
-        - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
-        - 🔥2024.01.04: Support for **VLLM deployment**, compatible with the **OpenAI API** style. For more details, please refer to [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署)
-        - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) to facilitate viewing the training speed and GPU memory required for different models.
-        - 🔥 2023.12.29: Support web-ui for training and inference, use `swift web-ui` after the installation of ms-swift.
-        - 🔥 2023.12.29: Support DPO RLHF(Reinforcement Learning from Human Feedback) and three datasets: AI-ModelScope/stack-exchange-paired and AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn for this task. Check [this documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
-        - 🔥 2023.12.28: Support SCEdit! This framework can easily reduce memory usage in training and inference, and replace ControlNet for controllable image generating scenarios, view the following chapter for details.
-        - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
-        - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
-        - 2023.12.18: Support for VLLM for inference acceleration.
-        - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-        - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b_instruct).
-        - 2023.12.09: Support the `freeze_parameters` parameter as a compromise between LoRA and full parameter. Corresponding shell scripts can be found at [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, for details please refer to [Command-Line parameters](https://github.com/modelscope/swift/blob/main/docs/source/LLM/命令行参数.md).
-        - 2023.12.08: Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k.
-        - 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E5%BE%AE%E8%B0%83%E6%96%87%E6%A1%A3.md#%E4%BD%BF%E7%94%A8cli).
-        - 2023.12.04: Supported models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat. Supported datasets: hc3-zh, hc3-en.
-        - 🔥 2023.12.02: [Best Practice for Self-cognition Fine-tuning](https://github.com/modelscope/swift/blob/main/docs/source/LLM/自我认知微调最佳实践.md), **10 minutes for self-cognition fine-tuning for LLM**, creating a LLM that is specific to oneself.
-        - 🔥 2023.11.30: Support for training and inference of the **qwen-1_8b**, **qwen-72b**, and **qwen-audio** model series. The corresponding shell scripts can be viewed at [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_audio_chat).
-        - 🔥 2023.11.29: Support the training and inference for **AnimateDiff**
-        - 🔥 2023.11.24: Support for **yi-34b-chat**, **codefuse-codellama-34b-chat**: The corresponding shell script can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codefuse_codellama_34b_chat).
-        - 🔥 2023.11.18: Support for **tongyi-finance-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4. The corresponding shell script can be found in [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4).
-        - 2023.11.16: Added support for more models in **flash attn**: qwen series, qwen-vl series, llama series, openbuddy series, mistral series, yi series, ziya series. Please use the `use_flash_attn` parameter.
-        - 🔥 2023.11.11: **NEFTune** Supported, Use is with `Swift.prepare_model(model, NEFTuneConfig())`
-        - 🔥 2023.11.11: Support training and inference with **CLI**, and inference with **Web-UI**. Check the [Run using Swift CLI](https://github.com/modelscope/swift/tree/main#run-using-swift-cli) chapter for details.
-        - 🔥 2023.11.11: Support model **deployment**(vllm/chatglm.cpp/xinference)，Check [Official documentation](./docs/source/GetStarted/部署指南.md) for details.
-        - 🔥 2023.11.10: Support for **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. The corresponding shell script can be found in [bluelm_7b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/bluelm_7b_chat).
-        - 🔥 2023.11.08: Support the finetuning of **xverse-65b** model, scripts can be found at: [xverse_65b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_65b).
-        - 🔥 2023.11.07: Support the finetuning of **yi-6b**, **yi-34b** model, scripts can be found at: [yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b).
-        - 🔥 2023.10.30: Support **QA-LoRA** and **LongLoRA** to decrease memory usage in training.
-        - 🔥 2023.10.30: Support **ROME**(Rank One Model Editing) to add/modify knowledges, training is not needed!
-        - 2023.10.30: Support for **skywork-13b** series models: skywork-13b, skywork-13b-chat. The corresponding shell script can be found in [skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/skywork_13b).
-        - 🔥 2023.10.27: Support for **chatglm3** series models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. The corresponding shell script can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b).
-        - 🔥 2023.10.17: Supported **int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8.
-        - 2023.10.15: Supported **ziya2-13b** model series: ziya2-13b, ziya2-13b-chat.
-        - 2023.10.12: Supported **mistral-7b** model series: openbuddy-mistral-7b-chat, mistral-7b, mistral-7b-instruct.
-        - 🔥 2023.10.07: Supported **DeepSpeed ZeRO-2**, enabling LoRA (not just QLoRA) to run DDP on 2*A10.
-        - 2023.10.04: Supported datasets in the fields of mathematics, law, SQL, and coding: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en.
-        - 🔥 2023.09.25: Supported **qwen-14b** model series: qwen-14b, qwen-14b-chat.
-        - 2023.09.18: Supported **internlm-20b** model series: internlm-20b, internlm-20b-chat.
-        - 2023.09.12: Supported training with **MP+DDP** to accelerate full-parameter fine-tuning speed.
-        - 2023.09.05: Supported **openbuddy-llama2-70b-chat** model.
-        - 2023.09.03: Supported **baichuan2** model series: baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat.
-        </details>
-        
-        
-        ## ✨ LLM Training and Inference
-        If you want to learn more about **best practices** for LLM or multimodal LLM, or if you are interested in **tutorials** on inference, fine-tuning, quantization, and deployment of LLM, you can refer to the [LLM series documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/index.md).
-        
-        
-        ### WEB UI training and inference
-        
-        After installation, you can use web-ui training/inference like:
-        
-        ```shell
-        SWIFT_UI_LANG=en swift web-ui
-        ```
-        
-        > Supported environment variables:
-        >
-        > WEBUI_SHARE=1 Share the gradio or not
-        > SWIFT_UI_LANG=en/zh The language of radio
-        > WEBUI_SERVER server_name， web-ui host ip，0.0.0.0 means all routes are allowed，127.0.0.1 means only localhost can visit the web
-        > WEBUI_PORT The port of web-ui
-        
-        Here is a simple introduction of web-ui:
-        
-        [![Watch the video](docs/source/cources/resources/20240119160942.jpg)](https://modelscope-open.oss-cn-hangzhou.aliyuncs.com/SWIFT%E8%A7%86%E9%A2%91_%E8%B0%83%E6%95%B4%E5%B0%81%E9%9D%A2.mp4)
-        
-        
-        ### Quick Start
-        You can test if the environment is installed correctly by running the following code.
-        ```python
-        # pip install ms-swift[llm] -U
-        
-        # Experimental environment: A10, 3090, V100, ...
-        # 8GB GPU memory
-        import os
-        os.environ['CUDA_VISIBLE_DEVICES'] = '0'
-        
-        import torch
-        
-        from swift.llm import (
-            DatasetName, InferArguments, ModelType, SftArguments,
-            infer_main, sft_main, app_ui_main, merge_lora
-        )
-        
-        model_type = ModelType.qwen1half_0_5b
-        sft_args = SftArguments(
-            model_type=model_type,
-            train_dataset_sample=2000,
-            dataset=[DatasetName.jd_sentiment_zh],
-            output_dir='output')
-        result = sft_main(sft_args)
-        best_model_checkpoint = result['best_model_checkpoint']
-        print(f'best_model_checkpoint: {best_model_checkpoint}')
-        torch.cuda.empty_cache()
-        
-        infer_args = InferArguments(
-            ckpt_dir=best_model_checkpoint,
-            load_dataset_config=True,
-            val_dataset_sample=10)
-        merge_lora(infer_args, device_map='cpu')
-        result = infer_main(infer_args)
-        torch.cuda.empty_cache()
-        
-        app_ui_main(infer_args)
-        ```
-        
-        ### Training Scripts
-        You can refer to the following scripts to customize your own training script.
-        
-        - full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
-        - full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
-        - full+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3) (4\*A100)
-        - lora: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_mp) (2\*A100)
-        - lora+ddp: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp) (2\*3090)
-        - lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3) (4\*3090), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100)
-        - qlora(gptq-int4): [qwen-7b-chat-int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat_int4/qlora) (3090)
-        - qlora(gptq-int8): [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8/qlora) (3090)
-        - qlora(bnb-int4): [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/qlora) (3090)
-        
-        
-        ### Features
-        - Supported SFT Methods: [lora](https://arxiv.org/abs/2106.09685), [qlora](https://arxiv.org/abs/2305.14314), [longlora](https://arxiv.org/abs/2309.12307), [qalora](https://arxiv.org/abs/2309.14717), full parameter fine-tuning, partial parameter fine-tuning.
-        - Supported Features: quantization, DDP, model parallelism, gradient checkpointing, pushing to modelscope hub, custom datasets, multimodal and agent SFT, mutli-round chat, DPO, self-cognition fine-tuning, ...
-        - Supported Models: [[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
-          - Multi-Modal:
-            - [qwen-vl](https://github.com/QwenLM/Qwen-VL) series: qwen-vl, qwen-vl-chat, qwen-vl-chat-int4.
-            - [qwen-audio](https://github.com/QwenLM/Qwen-Audio) series: qwen-audio, qwen-audio-chat.
-            - [deepseek-vl](https://github.com/deepseek-ai/DeepSeek-VL) series: deepseek-vl-1_3b-chat, deepseek-vl-7b-chat.
-            - [yi-vl](https://github.com/01-ai/Yi) series: yi-vl-6b-chat, yi-vl-34b-chat.
-            - [internlm-xcomposer2](https://github.com/InternLM/InternLM-XComposer) series: internlm-xcomposer2-7b-chat.
-            - [minicpm-v](https://github.com/OpenBMB/MiniCPM) series: minicpm-v-3b-chat.
-            - [cogvlm](https://github.com/THUDM/CogVLM) series: cogvlm-17b-instruct, cogagent-18b-chat, cogagent-18b-instruct.
-          - General:
-            - [qwen](https://github.com/QwenLM/Qwen) series:
-              - qwen-1_8b, qwen-1_8b-chat, qwen-1_8b-chat-int4, qwen-1_8b-chat-int8.
-              - qwen-7b, qwen-7b-chat, qwen-7b-chat-int4, qwen-7b-chat-int8.
-              - qwen-14b, qwen-14b-chat, qwen-14b-chat-int4, qwen-14b-chat-int8.
-              - qwen-72b, qwen-72b-chat, qwen-72b-chat-int4, qwen-72b-chat-int8.
-            - [qwen1.5](https://github.com/QwenLM/Qwen1.5) series:
-              - qwen1half-0_5b, qwen1half-0_5b-chat, qwen1half-0_5b-chat-int4, qwen1half-0_5b-chat-int8, qwen1half-0_5b-chat-awq.
-              - qwen1half-1_8b, qwen1half-1_8b-chat, qwen1half-1_8b-chat-int4, qwen1half-1_8b-chat-int8, qwen1half-1_8b-chat-awq.
-              - qwen1half-4b, qwen1half-4b-chat, qwen1half-4b-chat-int4, qwen1half-4b-chat-int8, qwen1half-4b-chat-awq.
-              - qwen1half-7b, qwen1half-7b-chat, qwen1half-7b-chat-int4, qwen1half-7b-chat-int8, qwen1half-7b-chat-awq.
-              - qwen1half-14b, qwen1half-14b-chat, qwen1half-14b-chat-int4, qwen1half-14b-chat-int8, qwen1half-14b-chat-awq.
-              - qwen1half-72b, qwen1half-72b-chat, qwen1half-72b-chat-int4, qwen1half-72b-chat-int8, qwen1half-72b-chat-awq.
-            - [chatglm](https://github.com/THUDM/ChatGLM-6B) series: chatglm2-6b, chatglm2-6b-32k, chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k.
-            - [llama](https://github.com/facebookresearch/llama) series: llama2-7b, llama2-7b-chat, llama2-13b, llama2-13b-chat, llama2-70b, llama2-70b-chat.
-            - [yi](https://github.com/01-ai/Yi) series: yi-6b, yi-6b-200k, yi-6b-chat, yi-9b, yi-34b, yi-34b-200k, yi-34b-chat.
-            - [internlm](https://github.com/InternLM/InternLM) series:
-              - internlm-7b, internlm-7b-chat, internlm-7b-chat-8k, internlm-20b, internlm-20b-chat.
-              - internlm2-1_8b, internlm2-1_8b-sft-chat, internlm2-1_8b-chat, internlm2-7b-base, internlm2-7b, internlm2-7b-sft-chat, internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
-            - [deepseek](https://github.com/deepseek-ai/deepseek-LLM) series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, deepseek-moe-16b, deepseek-moe-16b-chat.
-            - [gemma](https://github.com/google/gemma_pytorch) series: gemma-2b, gemma-2b-instruct, gemma-7b, gemma-7b-instruct.
-            - [minicpm](https://github.com/OpenBMB/mlc-MiniCPM) series: minicpm-2b-sft-chat, minicpm-2b-chat.
-            - [openbuddy](https://github.com/OpenBuddy/OpenBuddy) series: openbuddy-llama2-13b-chat, openbuddy-llama-65b-chat, openbuddy-llama2-70b-chat, openbuddy-mistral-7b-chat, openbuddy-zephyr-7b-chat, openbuddy-deepseek-67b-chat, openbuddy-mixtral-moe-7b-chat.
-            - [mistral](https://github.com/mistralai/mistral-src) series: mistral-7b, mistral-7b-instruct, mistral-7b-instruct-v2.
-            - [mixtral](https://github.com/mistralai/mistral-src) series: mixtral-moe-7b, mixtral-moe-7b-instruct.
-            - [baichuan](https://github.com/baichuan-inc/Baichuan2) series: baichuan-7b, baichuan-13b, baichuan-13b-chat, baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4.
-            - [yuan](https://github.com/IEIT-Yuan/Yuan-2.0) series: yuan2-2b-instruct, yuan2-2b-janus-instruct, yuan2-51b-instruct, yuan2-102b-instruct.
-            - [xverse](https://github.com/xverse-ai/XVERSE-13B) series: xverse-7b, xverse-7b-chat, xverse-13b, xverse-13b-chat, xverse-65b, xverse-65b-v2, xverse-65b-chat, xverse-13b-256k.
-            - [orion](https://github.com/OrionStarAI/OrionStar-Yi-34B-Chat) series: orion-14b, orion-14b-chat.
-            - [bluelm](https://github.com/vivo-ai-lab/BlueLM) series: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k.
-            - [zephyr](https://github.com/huggingface/alignment-handbook) series: zephyr-7b-beta-chat.
-            - [ziya](https://github.com/IDEA-CCNL/Fengshenbang-LM) series: ziya2-13b, ziya2-13b-chat.
-            - [skywork](https://github.com/SkyworkAI/Skywork) series: skywork-13b, skywork-13b-chat.
-            - other: [polylm-13b](https://github.com/DAMO-NLP-MT/PolyLM), [seqgpt-560m](https://github.com/Alibaba-NLP/SeqGPT), [sus-34b-chat](https://github.com/SUSTech-IDEA/SUS-Chat).
-          - Financial:
-            - [tongyi-finance](https://github.com/QwenLM/Qwen) series: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4.
-          - Coding:
-            - [codefuse](https://github.com/codefuse-ai) series: codefuse-codellama-34b-chat, codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
-            - [deepseek-coder](https://github.com/deepseek-ai/DeepSeek-Coder) series: deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-            - [codegeex2](https://github.com/THUDM/CodeGeeX2) series: codegeex2-6b.
-            - [phi](https://www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-language-models/) series: phi2-3b.
-          - Math:
-            - [internlm2-math](https://github.com/InternLM/InternLM-Math) series: internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat.
-            - [deepseek-math](https://github.com/deepseek-ai/DeepSeek-Math) series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
-        - Supported Datasets: [[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%95%B0%E6%8D%AE%E9%9B%86)
-          - NLP:
-            - General: 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini.
-            - Agent: 🔥ms-agent, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.
-            - RLHF: 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.
-            - Coding: code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.
-            - Medical: medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.
-            - Law: lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.
-            - Math: 🔥blossom-math-zh, school-math-zh, open-platypus-en.
-            - SQL: text2sql-en, 🔥sql-create-context-en.
-            - Text Generation: 🔥advertise-gen-zh, 🔥dureader-robust-zh.
-            - Classification: cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.
-            - AWQ: pileval.
-            - Other: finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.
-          - Multi-Modal:
-            - Vision: coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.
-            - Audio: aishell1-zh, 🔥aishell1-mini-zh.
-          - Custom Dataset
-        - Supported Templates:
-          - Text Generation: default-generation, default-generation-bos, chatglm-generation, qwen-audio-generation.
-          - Chat: default, qwen, qwen-audio, baichuan, chatglm2, chatglm3, llama, openbuddy, internlm, internlm2, internlm-xcomposer2, yi, yi-vl, yuan, xverse, ziya, skywork, bluelm, zephyr, sus, deepseek, deepseek-coder, codefuse-codellama, codefuse, cogvlm-instruct, cogagent-chat, cogagent-instruct, orion, minicpm, minicpm-v, gemma, chatml.
-        
-        
-        ## 🔥SCEdit
-        
-        SCEdit is an efficient generative fine-tuning framework proposed by Alibaba TongYi Vision Intelligence Lab. This framework enhances the fine-tuning capabilities for text-to-image generation downstream tasks and enables quick adaptation to specific generative scenarios, **saving 30%-50% of training memory costs compared to LoRA**. Furthermore, it can be directly extended to controllable image generation tasks, **requiring only 7.9% of the parameters that ControlNet needs for conditional generation and saving 30% of memory usage**. It supports various conditional generation tasks including edge maps, depth maps, segmentation maps, poses, color maps, and image completion.
-        
-        We using 3D style data from the [style transfer dataset](https://modelscope.cn/datasets/damo/style_custom_dataset/dataPeview) for training, and testing with the same `Prompt: A boy in a camouflage jacket with a scarf`. The qualitative and quantitative results are as follows:
-        
-        | Method    | bs   | ep   | Target Module | Param. (M)    | Mem. (MiB) | 3D style                                                     |
-        | --------- | ---- | ---- | ------------- | ------------- | ---------- | ------------------------------------------------------------ |
-        | LoRA/r=64 | 1    | 50   | q/k/v/out/mlp | 23.94 (2.20%) | 8440MiB    | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703665229562-0f33bbb0-c492-41b4-9f37-3ae720dca80d.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 1    | 50   | up_blocks     | 19.68 (1.81%) | 7556MiB    | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703665933913-74b98741-3b57-46a4-9871-539df3a0112c.png" alt="img" style="zoom:20%;" /> |
-        | LoRA/r=64 | 10   | 100  | q/k/v/out/mlp | 23.94 (2.20%) | 26300MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703750608529-de20d0e7-bf9c-4928-8e59-73cc54f2c8d7.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 10   | 100  | up_blocks     | 19.68 (1.81%) | 18634MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703663033092-94492e44-341f-4259-9df4-13c168e3b5d6.png" alt="img" style="zoom:20%;" /> |
-        | LoRA/r=64 | 30   | 200  | q/k/v/out/mlp | 23.94 (2.20%) | 69554MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703750626635-2e368d7b-5e99-4a06-b189-8615f302bcd7.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 30   | 200  | up_blocks     | 19.68 (1.81%) | 43350MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703662246942-1102b1f4-93ab-4653-b943-3302f2a5259e.png" alt="img" style="zoom:20%;" /> |
-        
-        The benchmark listed above can be reproduced by：
-        
-        ```shell
-        # Install swift by the next chapter
-        cd examples/pytorch/multi_modal/notebook
-        python text_to_image_synthesis.py
-        ```
-        
-        
-        ## 🛠️ Installation
-        
-        SWIFT is running in Python environment. Please make sure your python version is higher than 3.8.
-        
-        - Install SWIFT by the `pip` command:
-        
-        ```shell
-        # full ability
-        pip install ms-swift[all] -U
-        # only use llm
-        pip install ms-swift[llm] -U
-        # only use aigc
-        pip install ms-swift[aigc] -U
-        # only use adapters
-        pip install ms-swift -U
-        ```
-        
-        - Install SWIFT by source code(for running sft/infer examples), please run:
-        
-        ```shell
-        git clone https://github.com/modelscope/swift.git
-        cd swift
-        pip install -e .[llm]
-        ```
-        
-        SWIFT requires torch>=1.13.
-        
-        - Use SWIFT in our docker image:
-        
-        ```shell
-        docker pull registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu20.04-cuda11.8.0-py38-torch2.0.1-tf2.13.0-1.9.1
-        ```
-        
-        ## 🚀 Getting Started
-        
-        SWIFT supports multiple tuners, as well as tuners provided by [PEFT](https://github.com/huggingface/peft). To use these tuners, simply call:
-        
-        ```python
-        from swift import Swift, LoRAConfig
-        config = LoRAConfig(...)
-        model = Swift.prepare_model(model, config, extra_state_keys=['...'])
-        ```
-        
-        The code snippet above initialized the tuner randomly. The input model is an instance of `torch.nn.Module`, the config is a subclass instance of `SwiftConfig` or `PeftConfig`. extra_state_keys is
-        the extra module weights(like the linear head) to be trained and stored in the output dir.
-        
-        You may combine multiple tuners by:
-        
-        ```python
-        from swift import Swift, LoRAConfig, PromptConfig
-        model = Swift.prepare_model(model, {'lora': LoRAConfig(...), 'prompt': PromptConfig(...)})
-        ```
-        
-        Call `save_pretrained` and `push_to_hub` after finetuning:
-        
-        ```python
-        from swift import push_to_hub
-        model.save_pretrained('some-output-folder')
-        push_to_hub('my-group/some-repo-id-modelscope', 'some-output-folder', token='some-ms-token')
-        ```
-        Assume `my-group/some-repo-id-modelscope` is the model-id in the hub, and `some-ms-token` is the token for uploading.
-        
-        Using the model-id to do later inference:
-        
-        ```python
-        from swift import Swift
-        model = Swift.from_pretrained(model, 'my-group/some-repo-id-modelscope')
-        ```
-        
-        Here shows a runnable example:
-        
-        ```python
-        import os
-        import tempfile
-        
-        # Please install modelscope by `pip install modelscope`
-        from modelscope import Model
-        
-        from swift import LoRAConfig, SwiftModel, Swift, push_to_hub
-        
-        tmp_dir = tempfile.TemporaryDirectory().name
-        if not os.path.exists(tmp_dir):
-            os.makedirs(tmp_dir)
-        
-        
-        model = Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto')
-        lora_config = LoRAConfig(target_modules=['q_proj', 'k_proj', 'v_proj'])
-        model: SwiftModel = Swift.prepare_model(model, lora_config)
-        # Do some finetuning here
-        model.save_pretrained(tmp_dir)
-        
-        push_to_hub('my-group/swift_llama2', output_dir=tmp_dir)
-        model = Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto')
-        model = SwiftModel.from_pretrained(model, 'my-group/swift_llama2', device_map='auto')
-        ```
-        
-        This is a example that uses transformers for model creation uses SWIFT for efficient tuning.
-        
-        ```python
-        from swift import Swift, LoRAConfig, AdapterConfig, PromptConfig
-        from transformers import AutoModelForImageClassification
-        
-        # init vit model
-        model = AutoModelForImageClassification.from_pretrained("google/vit-base-patch16-224")
-        
-        # init lora tuner config
-        lora_config = LoRAConfig(
-            r=10,  # the rank of the LoRA module
-            target_modules=['query', 'key', 'value'],  # the modules to be replaced with the end of the module name
-            merge_weights=False  # whether to merge weights
-        )
-        
-        # init adapter tuner config
-        adapter_config = AdapterConfig(
-            dim=768,  # the dimension of the hidden states
-            hidden_pos=0,  # the position of the hidden state to passed into the adapter
-            target_modules=r'.*attention.output.dense$',  # the modules to be replaced with regular expression
-            adapter_length=10  # the length of the adapter length
-        )
-        
-        # init prompt tuner config
-        prompt_config = PromptConfig(
-            dim=768,  # the dimension of the hidden states
-            target_modules=r'.*layer\.\d+$',  # the modules to be replaced with regular expression
-            embedding_pos=0,    # the position of the embedding tensor
-            prompt_length=10,   # the length of the prompt tokens
-            attach_front=False  # Whether prompt is attached in front of the embedding
-        )
-        
-        # create model with swift. In practice, you can use any of these tuners or a combination of them.
-        model = Swift.prepare_model(model, {"lora_tuner": lora_config, "adapter_tuner": adapter_config, "prompt_tuner": prompt_config})
-        
-        # get the trainable parameters of model
-        model.get_trainable_parameters()
-        # 'trainable params: 838,776 || all params: 87,406,432 || trainable%: 0.9596273189597764'
-        ```
-        
-        You can use the features offered by Peft in SWIFT:
-        
-        ```python
-        from swift import LoraConfig, Swift
-        from peft import TaskType
-        lora_config = LoraConfig(target_modules=['query', 'key', 'value'], task_type=TaskType.CAUSAL_LM)
-        model_wrapped = Swift.prepare_model(model, lora_config)
-        
-        # or call from_pretrained to load weights in the modelhub
-        model_wrapped = Swift.from_pretrained(model, 'some-id-in-the-modelscope-modelhub')
-        ```
-        
-        
-        The saving strategy between Swift tuners and Peft tuners are slightly different. You can name a tuner by:
-        
-        ```python
-        model = Swift.prepare_model(model, {'default': LoRAConfig(...)})
-        model.save_pretrained('./output')
-        ```
-        
-        In the output dir, you will have a dir structure like this:
-        
-        ```text
-        output
-            |-- default
-                |-- adapter_config.json
-                |-- adapter_model.bin
-            |-- adapter_config.json
-            |-- adapter_model.bin
-        ```
-        
-        The config/weights stored in the output dir is the config of `extra_state_keys` and the weights of it. This is different from PEFT, which stores the weights and config of the `default` tuner.
-        
-        
-        ## 🔍 Learn More
-        
-        - [ModelScope library](https://github.com/modelscope/modelscope/)
-        
-          ModelScope Library is the model library of ModelScope project, which contains a large number of popular models.
-        
-        - [Contribute your own model to ModelScope](https://modelscope.cn/docs/ModelScope%E6%A8%A1%E5%9E%8B%E6%8E%A5%E5%85%A5%E6%B5%81%E7%A8%8B%E6%A6%82%E8%A7%88)
-        
-        
-        ## License
-        
-        This project is licensed under the [Apache License (Version 2.0)](https://github.com/modelscope/modelscope/blob/master/LICENSE).
-        
-        
-        ## ☎ Contact Us
-        You can contact and communicate with us by joining our WeChat Group:
-        
-        <p align="left">
-        <img src="asset/wechat.png" width="250" style="display: inline-block;">
-        </p>
-        
-        
-        ## Star History
-        
-        [![Star History Chart](https://api.star-history.com/svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/swift&Date)
-        
-Keywords: python,petl,efficient tuners
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: llm
-Provides-Extra: aigc
-Provides-Extra: all
+# SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
+
+<p align="center">
+    <br>
+    <img src="resources/banner.png"/>
+    <br>
+<p>
+<p align="center">
+<a href="https://modelscope.cn/home">ModelScope Community Website</a>
+<br>
+        <a href="README_CN.md">中文</a> &nbsp ｜ &nbsp English &nbsp
+</p>
+
+<p align="center">
+<img src="https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg">
+<img src="https://img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg">
+<a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
+<a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
+<a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
+<a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
+<a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
+</p>
+
+## 📖 Table of Contents
+- [Introduction](#-introduction)
+- [News](#-news)
+- [Installation](#%EF%B8%8F-installation)
+- [Getting Started](#-getting-started)
+- [Documentation](#-documentation)
+- [License](#-License)
+- [Citation](#-citation)
+- [Contact Us](#-contact-us)
+
+## 📝 Introduction
+SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
+
+To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
+
+Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
+
+## 🎉 News
+- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
+- 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
+- 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train.
+- 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
+- 🔥2024.04.09: Support ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/Supported-models-datasets.md) to begin training!
+- 2024.04.08: Support the fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/xverse_moe_a4_2b/lora/sft.sh) to start training!
+- 2024.04.04: Support **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_70b_chat/qlora_fsdp/sft.sh) to train.
+- 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
+- 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
+- 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
+- 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
+- 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
+- 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
+- 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/llava最佳实践.md).
+- 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
+- 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
+- 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
+- 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
+- 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
+- 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
+- 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
+- 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start training.
+- 2024.02.25: Support `swift export` to quantize models using **AWQ/GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/source_en/LLM/LLM-quantization.md).
+<details><summary>More</summary>
+
+- 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
+- 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
+- 🔥2024.02.05: Support **Qwen1.5** series models, see [model list](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B) for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8).
+- 2024.02.05: Support training of diffusion models such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training. See corresponding [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
+- 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
+- 🔥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**. Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
+- 🔥2024.02.01: Support Agent training! Agent training algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary), a high-quality agent dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to start Agent training!
+- 🔥2024.02.01: Support adding SFT loss in DPO training to reduce repetitive generation caused by KL divergence loss.
+- 2024.02.01: Support using AdaLoRA and IA3 adapters in training.
+- 2024.02.01: Support `--merge_lora` parameter in AnimateDiff training.
+- 2024.01.30: Support [internlm-xcomposer2-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm_xcomposer2_7b_chat).
+- 🔥2024.01.30: Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), simply specify `--deepspeed default-zero3`.
+- 2024.01.29: Support internlm2-math series: internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat.
+- 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
+- 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
+- 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
+- 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
+- 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
+- 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
+- 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
+- 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署) for details.
+- 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
+- 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
+- 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
+- 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
+- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
+- 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
+- 2023.12.18: Support VLLM for inference acceleration.
+- 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
+- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct).
+- 2023.12.09: Support `freeze_parameters` parameter as a compromise between lora and full-parameter training. Corresponding sh can be found in [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, see [command line arguments](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details.
+- 2023.12.08: Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k.
+- 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E5%BE%AE%E8%B0%83%E6%96%87%E6%A1%A3.md#%E4%BD%BF%E7%94%A8cli).
+- 2023.12.05: Support models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat. Support datasets: hc3-zh, hc3-en.
+- 🔥2023.12.02: [Self-cognition fine-tuning best practices](docs/source_en/LLM/Self-cognition-best-practice.md), **10 minutes to fine-tune a large model for self-cognition**, create your own unique large model.
+- 🔥2023.11.30: Support training and inference of **qwen-1_8b**, **qwen-72b**, **qwen-audio** series models. Corresponding sh scripts can be found in [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_audio_chat)
+- 🔥2023.11.29: Support training and inference of **AnimateDiff**
+- 🔥2023.11.24: Support **yi-34b-chat**, **codefuse-codellama-34b-chat** models. Corresponding sh scripts can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codefuse_codellama_34b_chat).
+- 🔥2023.11.18: Support **tongyi-finance-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4. Corresponding sh scripts can be found in [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4).
+- 2023.11.16: Support **flash attn** for more models: qwen series, qwen-vl series, llama series, openbuddy series, mistral series, yi series, ziya series. Please use `use_flash_attn` parameter.
+- 🔥2023.11.11: Support **NEFTune**, simply use `Swift.prepare_model(model, NEFTuneConfig())` to enable.
+- 🔥2023.11.11: Support training and inference by **command line** and inference by **Web-UI**, see `Usage with Swift CLI` section below for details.
+- 🔥2023.11.10: Support **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. Corresponding sh scripts can be found in [bluelm_7b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/bluelm_7b_chat).
+- 🔥2023.11.08: Support training and inference of **xverse-65b** model, script at [xverse_65b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_65b).
+- 🔥2023.11.07: Support training and inference of **yi-6b**, **yi-34b** models, scripts at [yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b).
+- 🔥2023.10.30: Support two new tuners: **QA-LoRA** and **LongLoRA**.
+- 🔥2023.10.30: Support editing models using **ROME** (Rank One Model Editing) to infuse new knowledge into models without training!
+- 2023.10.30: Support **skywork-13b** series models: skywork-13b, skywork-13b-chat. Corresponding sh scripts can be found in [skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/skywork_13b).
+- 🔥2023.10.27: Support **chatglm3** series models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. Corresponding sh scripts can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b).
+- 🔥2023.10.17: Support SFT of **int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8.
+- 2023.10.15: Support **ziya2-13b** series models: ziya2-13b, ziya2-13b-chat.
+- 2023.10.12: Support **mistral-7b** series models: openbuddy-mistral-7b-chat, mistral-7b, mistral-7b-instruct.
+- 🔥2023.10.07: Support **DeepSpeed ZeRO-2**, enabling lora (not just qlora) to run DDP on dual A10 cards.
+- 2023.10.04: Support more math, law, SQL, code domain datasets: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en.
+- 🔥2023.09.25: Support **qwen-14b** series: qwen-14b, qwen-14b-chat.
+- 2023.09.18: Support **internlm-20b** series: internlm-20b, internlm-20b-chat.
+- 2023.09.12: Support **MP+DDP** to accelerate full-parameter training.
+- 2023.09.05: Support **openbuddy-llama2-70b-chat**.
+- 2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat.
+</details>
+
+## 🛠️ Installation
+
+SWIFT runs in the Python environment. Please ensure your Python version is higher than 3.8.
+
+- Method 1: Install SWIFT using pip command:
+
+```shell
+# Full capabilities
+pip install ms-swift[all] -U
+# LLM only
+pip install ms-swift[llm] -U
+# AIGC only
+pip install ms-swift[aigc] -U
+# Adapters only
+pip install ms-swift -U
+```
+
+- Method 2: Install SWIFT through source code (convenient for running training and inference scripts), please run the following commands:
+
+```shell
+git clone https://github.com/modelscope/swift.git
+cd swift
+pip install -e .[llm]
+```
+
+SWIFT depends on torch>=1.13, recommend torch>=2.0.0.
+
+- Method 3: Use SWIFT in our Docker image
+
+```shell
+# China-Hangzhou image
+docker pull registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1
+# US-west image
+docker pull registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1
+```
+
+## 🚀 Getting Started
+
+This section introduces basic usage, see the [Documentation](#-documentation) section for more ways to use.
+
+### Web-UI
+
+```shell
+swift web-ui
+```
+
+### Training
+
+#### Training Scripts
+You can refer to the following scripts to customize your own training script.
+
+- full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
+- full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
+- full+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3) (4\*A100)
+- lora: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_mp) (2\*A100)
+- lora+ddp: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp) (2\*3090)
+- lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3) (4\*3090), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100)
+- qlora(gptq-int4): [qwen-7b-chat-int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat_int4/qlora) (3090)
+- qlora(gptq-int8): [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8/qlora) (3090)
+- qlora(bnb-int4): [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/qlora) (3090)
+
+
+#### Supported Training Processes
+
+| Training Process | Training Method                                                               |
+|------------------|-------------------------------------------------------------------------------|
+| Pretraining      | Text Generation                                                               |
+| Fine-tuning      | Single-turn/Multi-turn<br>Agent Training/Self-cognition<br>Multi-modal Vision/Multi-modal Speech|
+| Human Alignment  | DPO                                                                           |
+| Text-to-Image    | DreamBooth, etc.                                                              |
+| Text-to-Video    | -                                                                             |
+
+#### Single GPU Training
+
+Start single GPU fine-tuning with the following command:
+
+LoRA:
+```shell
+# Experimental Environment: A100
+# GPU Memory Requirement: 20GB
+# Runtime: 3.1 hours
+CUDA_VISIBLE_DEVICES=0 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+    --eval_steps 200 \
+```
+
+Full-parameter:
+```shell
+# Experimental Environment: A100
+# GPU Memory Requirement: 80GB
+# Runtime: 2.5 hours
+CUDA_VISIBLE_DEVICES=0 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type full \
+    --output_dir output \
+    --eval_steps 500 \
+```
+
+
+#### Model Parallel Training
+
+
+```shell
+# Experimental Environment: 2 * A100
+# GPU Memory Requirement: 10GB + 13GB
+# Runtime: 3.4 hours
+CUDA_VISIBLE_DEVICES=0,1 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+```
+
+#### Data Parallel Training
+
+```shell
+# Experimental Environment: 4 * A100
+# GPU Memory Requirement: 4 * 30GB
+# Runtime: 0.8 hours
+NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+```
+
+Combining Model Parallelism and Data Parallelism:
+```shell
+# Experimental Environment: 4 * A100
+# GPU Memory Requirement: 2*14GB + 2*18GB
+# Runtime: 1.7 hours
+NPROC_PER_NODE=2 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+```
+
+#### Deepspeed Training
+
+ZeRO2:
+```shell
+# Experimental Environment: 4 * A100
+# GPU Memory Requirement: 4 * 21GB
+# Runtime: 0.9 hours
+NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+    --deepspeed default-zero2 \
+```
+
+ZeRO3:
+```shell
+# Experimental Environment: 4 * A100
+# GPU Memory Requirement: 4 * 19GB
+# Runtime: 3.2 hours
+NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \
+    --model_type qwen1half-7b-chat \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+    --deepspeed default-zero3 \
+```
+
+### Inference
+Original model:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
+# use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
+    --infer_backend vllm --max_model_len 8192
+```
+
+LoRA fine-tuned:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true
+# use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer \
+    --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \
+    --merge_lora true --infer_backend vllm --max_model_len 8192
+```
+
+### Evaluation
+
+```shell
+CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset mmlu ceval
+```
+
+### Export
+
+Original model:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift export --model_type qwen1half-7b-chat \
+    --quant_bits 4 --quant_method awq
+```
+
+LoRA fine-tuned:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift export \
+    --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \
+    --quant_method awq --quant_bits 4 \
+    --merge_lora true \
+```
+
+### Deployment
+
+Original model:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat
+# 使用VLLM加速
+CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat \
+    --infer_backend vllm --max_model_len 8192
+```
+
+LoRA fine-tuned:
+```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx
+# 使用VLLM加速
+CUDA_VISIBLE_DEVICES=0 swift deploy \
+    --ckpt_dir xxx/checkpoint-xxx --merge_lora true \
+    --infer_backend vllm --max_model_len 8192
+```
+
+### Supported Models
+
+#### LLMs
+
+| Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
+|------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
+| Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model                      |
+| ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
+| Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
+| Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
+| XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
+| LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
+| Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
+| YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
+| InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
+| DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
+| MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
+| Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
+| MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
+| OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
+| Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
+| BlueLM                                         | [VIVO BlueLM large model](https://github.com/vivo-ai-lab/BlueLM)        | Chinese<br>English    | 7B                                     | base model<br>chat model                       |
+| Ziya2                                          | [Fengshenbang series models](https://github.com/IDEA-CCNL/Fengshenbang-LM) | Chinese<br>English  | 13B                                    | base model<br>chat model                       |
+| Skywork                                        | [Skywork series models](https://github.com/SkyworkAI/Skywork) | Chinese<br>English    | 13B                                    | base model<br>chat model                       |
+| Zephyr                                         | Zephyr series models based on Mistral                                  | English            | 7B                                     | chat model                                 |
+| PolyLM                                         | [Tongyi Lab self-developed PolyLM series models](https://github.com/DAMO-NLP-MT/PolyLM) | Multilingual | 13B                                 | base model                                 |
+| SeqGPT                                         | [Tongyi Lab self-developed text understanding model for information extraction and text classification](https://github.com/Alibaba-NLP/SeqGPT) | Chinese | 560M                               | semantic understanding model                |
+| SUS                                            | [Southern University of Science and Technology model fine-tuned on YI](https://github.com/SUSTech-IDEA/SUS-Chat) | Chinese<br>English | 34B                              | chat model                                 |
+| Tongyi-Finance                                 | [Tongyi finance series models](https://github.com/QwenLM/Qwen)          | Chinese<br>English    | 14B                                    | base model<br>chat model<br>financial model        |
+| CodeFuse-CodeLLaMA<br>CodeFuse-Codegeex2<br>CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai)        | Chinese<br>English    | 6B-34B                                 | chat model<br>code model                      |
+| phi2                                           | Microsoft's PHI2 model                                                 | English            | 3B                                     | base model<br>code model                          |
+| Grok | [X-ai](https://github.com/xai-org/grok-1) | English | 300B | base model |
+| TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat) | Chinese<br>English | 7B-12B | chat model |
+| dbrx | [databricks](https://github.com/databricks/dbrx) | English | 132B | base model<br>chat model  |
+| mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) | Chinese<br>English | 13B | base model  |
+| c4ai-command-r | [c4ai](https://cohere.com/command) | Multilingual | 35B-104B | chat model  |
+
+
+#### MLLMs
+
+| Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
+|------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
+| Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
+| Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
+| YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
+| XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
+| DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
+| MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
+| CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
+| Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B               | chat model |
+
+#### Diffusion Models
+
+| Model Type          | Model Introduction                                                    | Language | Model Type        |
+|---------------------|----------------------------------------------------------------------|----------|------------------ |
+| AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
+| SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
+
+### Supported Open Source Datasets
+
+| Dataset Type | Training Task  | Documentation                                                                                                                                                                                                                                                                                                        |
+|--------------|:---------------|--------------------------------------------------------------- |
+| General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini. |
+| Agent        | Fine-tuning    | 🔥ms-agent, ms-agent-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.                                                                                                                                                                                                                                                |
+| General      | Human Alignment | 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.                            |
+| Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.                                                                                                                                                                                                                          |
+| Medical      | Fine-tuning    | medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.                                                                                                                                                                                                                                                          |
+| Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.                                                                                                                                                                                                                                                                 |
+| Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                                                                                                                                                                                                                                                                 |
+| SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                                                                                                                                                                                                                                                                |
+| Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                                                                                                                                                                                                                                                                            |
+| Classification | Fine-tuning  | cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.                                                                                                                                                                                                                                                    |
+| Quantization Assist | Quantization | pileval.                                                                                                                                                                                                                                                                                                             |
+| Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.                                                                                                                                                                                                                               |
+| Vision       | Fine-tuning    | coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.                                                                                                                                                                                                                                                              |
+| Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-mini-zh.                                                                                                                                                                                                                                                                                     |
+
+### Supported Technologies
+
+| Technology Name                                               |
+|--------------------------------------------------------------- |
+| 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) |
+| 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) |
+| 🔥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf) |
+| 🔥SCEdit: [SCEdit: Efficient and Controllable Image Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/2312.11392)  < [arXiv](https://arxiv.org/abs/2312.11392)  \|  [Project Page](https://scedit.github.io/) > |
+| 🔥NEFTune: [Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914) |
+| QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2309.14717) |
+| LongLoRA: [Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307) |
+| ROME: [Rank-One Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) |
+| Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/1902.00751) |
+| Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/2203.12119) |
+| Side: [Side-Tuning: A Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503) |
+| Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859)  < [arXiv](https://arxiv.org/abs/2310.19859)  \|  [Project Page](https://res-tuning.github.io/)  \|  [Usage](docs/source/GetStarted/ResTuning.md) > |
+| Tuners provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA, etc. |
+
+### Supported Hardware
+
+| Hardware Environment           | Notes                                           |
+|--------------------------------|-------------------------------------------------|
+| CPU                            |                                                 |
+| RTX 20/30/40 series, etc.      | After 30 series, BF16 and FlashAttn can be used |
+| Computing cards T4/V100, etc.  | BF16 and FlashAttn not supported                |
+| Computing cards A10/A100, etc. | Support BF16 and FlashAttn                      |
+| Huawei Ascend NPU              |                                                 |
+
+## 📃 Documentation
+
+### Documentation Compiling
+
+```shell
+make docs
+# Check docs/build/html/index.html in web-browser
+```
+
+### User Guide
+
+| Document Name                                                |
+| ------------------------------------------------------------ |
+| [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
+| [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
+| [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
+| [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
+| [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
+| [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
+| [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
+| [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
+
+### Reference Documentation
+| Document Name                                                |
+| ------------------------------------------------------------ |
+| [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
+| [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
+| [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
+| [Runtime Speed and Memory Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) |
+
+
+### Best Practices
+
+| Best Practices Name                                                |
+| ------------------------------------------------------------ |
+| [Agent Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+| [Self-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+|  [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+|  [Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/Multi-Modal/index.md) |
+
+### Deep Learning Tutorials
+
+| Tutorial Name                                                |
+|-------------------------------------------------------------- |
+| [Introduction to Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md) |
+| [Large Model Basics](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md) |
+| [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-prompt%20engineering.md) |
+| [Transformer Architecture Introduction](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/D.Transformer%E7%BB%93%E6%9E%84.md) |
+| [Training Technique Selection](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/E.%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B.md) |
+| [Data Preprocessing](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/F.%E6%95%B0%E6%8D%AE%E9%A2%84%E5%A4%84%E7%90%86.md) |
+| [Quantization](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/G.%E9%87%8F%E5%8C%96.md) |
+| [Training](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/H.%E8%AE%AD%E7%BB%83.md) |
+| [Inference](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/I.LLM%E5%92%8C%E5%A4%9A%E6%A8%A1%E6%80%81%E6%A8%A1%E5%9E%8B%E9%AB%98%E6%95%88%E6%8E%A8%E7%90%86%E5%AE%9E%E8%B7%B5.md) |
+| [Deployment](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/J.%E9%83%A8%E7%BD%B2.md) |
+| [Evaluation](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98--LLM%20Automatic%20Evaluation.md) |
+
+## 🏛 License
+
+This framework is licensed under the [Apache License (Version 2.0)](https://github.com/modelscope/modelscope/blob/master/LICENSE). For models and datasets, please refer to the original resource page and follow the corresponding License.
+
+## 📎 Citation
+
+```bibtex
+@Misc{swift,
+  title = {SWIFT:Scalable lightWeight Infrastructure for Fine-Tuning},
+  author = {The ModelScope Team},
+  howpublished = {\url{https://github.com/modelscope/swift}},
+  year = {2024}
+}
+```
+
+## ☎ Contact Us
+
+You can contact us and communicate with us by adding our WeChat group:
+
+<p align="left">
+<img src="asset/wechat.png" width="250" style="display: inline-block;">
+</p>
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/swift&Date)
```

#### html2text {}

```diff
@@ -1,525 +1,596 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 1.7.3 Summary: Swift: Scalable
-lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
-modelscope/swift Author: DAMO ModelScope teams Author-email:
-contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
-(Scalable lightWeight Infrastructure for Fine-Tuning)
+# SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
 
-        [https://modelscope.oss-cn-beijing.aliyuncs.com/modelscope.gif]
-                             _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y
-                      _ä_¸_­_æ__  ï½ &nbspEnglish  ï½  _D_o_c_s
+                            [resources/banner.png]
+                         _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
+                           _ä_¸_­_æ__   ï½   English  
       [https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg][https://
   img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_m_o_d_e_l_s_c_o_p_e_-_%_E_2_%_8_9_%_A_5_1_._9_._5_-_5_D_9_1_D_4_._s_v_g_]_[_h_t_t_p_s_:_/_/
      _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_m_s_-_s_w_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
   _m_o_d_e_l_s_c_o_p_e_/_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_s_-_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                          _b_a_d_g_e_/_P_R_-_w_e_l_c_o_m_e_-_5_5_E_B_9_9_._s_v_g_]
 ## ð Table of Contents - [Introduction](#-introduction) - [News](#-news) -
-ð¥[LLM Training and Inference](#-llm-training-and-inference) - ð¥[SCEdit
-Tuner](#-SCEdit) - [Installation](#-installation) - [Getting Started](#-
-getting-started) - [Learn More](#-learn-more) - [License](#license) - [Contact
-Us](#-contact-us) ## ð Introduction SWIFT (Scalable lightWeight
-Infrastructure for Fine-Tuning) is an extensible framework designed to
-facilitate lightweight model fine-tuning and inference. It integrates
-implementations for various efficient fine-tuning methods, by embracing
-approaches that is parameter-efficient, memory-efficient, and time-efficient.
-SWIFT integrates seamlessly into ModelScope ecosystem and offers the
-capabilities to finetune various models, with a primary emphasis on LLMs and
-vision models. Additionally, SWIFT is fully compatible with [PEFT](https://
-github.com/huggingface/peft), enabling users to leverage the familiar Peft
-interface to finetune ModelScope models. Currently supported approaches (and
-counting): 1. ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS]
-(https://arxiv.org/abs/2106.09685) 2. ð¥LoRA+: [LoRA+: Efficient Low Rank
-Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) 3. ð¥LLaMA
-PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/
-2401.02415.pdf) 4. ð¥SCEdit: [SCEdit: Efficient and Controllable Image
-Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/
-2312.11392) < [arXiv](https://arxiv.org/abs/2312.11392) | [Project Page](https:
-//scedit.github.io/) > 5. ð¥NEFTune: [Noisy Embeddings Improve Instruction
-Finetuning](https://arxiv.org/abs/2310.05914) 6. QA-LoRA:[Quantization-Aware
-Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/
-2309.14717). 7. LongLoRA: [Efficient Fine-tuning of Long-Context Large Language
-Models](https://arxiv.org/abs/2309.12307) 8. ROME: [Rank-One Editing of
-Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) 9. Adapter:
-[Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/
-1902.00751) 10. Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/
-2203.12119) 11. Side: [Side-Tuning: A Baseline for Network Adaptation via
-Additive Side Networks](https://arxiv.org/abs/1912.13503) 12. Res-Tuning: [Res-
-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from
-Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://arxiv.org/abs/
-2310.19859) | [Project Page](https://res-tuning.github.io/) | [Usage](docs/
-source/GetStarted/ResTuning.md) > 13. All tuners offered on [PEFT](https://
-github.com/huggingface/peft), like IA3, AdaLoRA Key features: 1. By integrating
-the ModelScope library, models can be readily obtained via a model-id. 2.
-Tuners provided by SWIFT can be combined to allow exploration of multiple
-tuners on a model for best result. 3. Support calling `activate_adapter` or
-`deactivate_adapter` or `set_active_adapters` to activate/deactivate tuners.
-User can inference with one model and multiple tuners in different threads
-independently. 4. Support training and inference with scripts/CLIï¼meanwhile
-support inference with Web-UI. 5. Support model deployment(vllm/chatglm.cpp/
-xinference)ï¼Check [Official documentation](./docs/source/GetStarted/
-é¨ç½²æå.md) for details. Users can check the [documentation of SWIFT]
-(docs/source/GetStarted/å¿«éä½¿ç¨.md) to get detail tutorials. ## ð News
-- ð¥2024.03.12: Supports inference and fine-tuning for the **deepseek-vl**
-series. For best practice, you can refer to [here](https://github.com/
-modelscope/swift/tree/main/docs/source/Multi-Modal/deepseek-vlæä½³å®è·µ.md).
-- ð¥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507), which can
-efficiently reduce the memory usage(almost half of the original memory) when
-training the full model. - ð¥2024.03.10: For the end-to-end best practice of
-fine-tuning to deployment of Qwen1.5-7B-Chat and Qwen1.5-72B-Chat, you can
-refer to the [Qwen1.5 Full Workflow Best Practice](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
-Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md). -
-ð¥2024.03.09: Support training and inference of MAMBA series, use [this
-script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/mamba-1.4b/lora/sft.sh) to begin. - 2024.03.09: Support training and
-inference of AQLM quantized models, use [this script](https://github.com/
-modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to begin. - 2024.03.06: Support training
-and inference of AWQ quantized models, use [this Qwen1.5-AWQ script](https://
+[Installation](#%EF%B8%8F-installation) - [Getting Started](#-getting-started)
+- [Documentation](#-documentation) - [License](#-License) - [Citation](#-
+citation) - [Contact Us](#-contact-us) ## ð Introduction SWIFT supports
+training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs**
+(multimodal large models). Developers can directly apply our framework to their
+own research and production environments to realize the complete workflow from
+model training and evaluation to application. In addition to supporting the
+lightweight training solutions provided by [PEFT](https://github.com/
+huggingface/peft), we also provide a complete **Adapters library** to support
+the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
+adapter library can be used directly in your own custom workflow without our
+training scripts. To facilitate use by users unfamiliar with deep learning, we
+provide a Gradio web-ui for controlling training and inference, as well as
+accompanying deep learning courses and best practices for beginners.
+Additionally, we are expanding capabilities for other modalities. Currently, we
+support full-parameter training and LoRA training for AnimateDiff. ## ð News
+- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1
+model, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start
+training! - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-
+V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
+Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
+with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
+for details. Meanwhile, we support a trick way to do multiple ablation
+experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
+command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train. -
+2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
+function call capabilities, and combine it with [Modelscope-Agent](https://
+github.com/modelscope/modelscope-agent) for best practices, which can be found
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
+best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
+ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
+fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat_awq/lora/sft.sh) to begin, support training and inference of
-[yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/yi_9b/lora_zero3). - ð¥2024.02.29: Support [LLaMA PRO](https://
-arxiv.org/pdf/2401.02415.pdf), use [this script](https://github.com/modelscope/
-swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to
-begin. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf),
-use [this script](https://github.com/modelscope/swift/blob/main/examples/
-pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to begin. - 2024.02.25: Support
-`swift export` to export models for **AWQ/GPTQ** quantization and push to
-ModelScope Hub. For more details, please refer to the document: [LLM
-Quantization Document](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/LLM%E9%87%8F%E5%8C%96%E6%96%87%E6%A1%A3.md). - 2024.02.22: Support
-gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b,
-gemma-7b-instruct. - 2024.02.16: Support deepseek-math series: deepseek-math-
-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support
-**Qwen1.5** series, To view all supported Qwen1.5 models please check [Model
-List](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B).
-The [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat_int8) fine-tuned scripts are provided. - 2024.02.05: Support
-the training of **SDXL**, **SD**, **ControlNet**, or techniques like
-**DreamBooth**, you can check the [training scripts](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details. -
-2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat),
-minicpm-2b-chat. - ð¥2024.02.01: Support dataset mixture to reduce
-**Catastrophic Forgetting**. Use `--train_dataset_mix_ratio 2.0` to train! We
-also provide a common knowledge dataset [ms-bench](https://www.modelscope.cn/
-datasets/iic/ms_bench/summary). - ð¥2024.02.01: Support Agent training! Agent
-training algorithm comes from this [paper](https://arxiv.org/pdf/
-2309.00986.pdf). We also introduce the [ms-agent](https://www.modelscope.cn/
-datasets/iic/ms_agent/summary) dataset. Use [this script](https://github.com/
+xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
+**QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
+**Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-
+Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/
+pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training! -
+ð¥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base
+model, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start
+training! - ð¥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-
+instruct, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training! -
+ð¥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-
+A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4. - ð¥2024.03.29: Support the
+fine-tuning and inference of **Grok-1** 300B MoE, please view details [here]
+(https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
+practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
+7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
+swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
+training! - ð¥2024.03.20: Supports inference and fine-tuning for the
+**llava** series. For best practice, you can refer to [here](https://
+github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/
+llavaæä½³å®è·µ.md). - ð¥2024.03.12: Support inference and fine-tuning for
+**deepseek-vl** series. Best practices can be found [here](docs/source_en/
+Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
+(https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
+2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
+best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
+to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
+Support training and inference of MAMBA model, use [this script](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/
+lora/sft.sh) to start training! - 2024.03.09: Support training and inference of
+AQLM quantized model, use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to
+start training! - 2024.03.06: Support training and inference of AWQ quantized
+model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to
+start training, and support training and inference of [yi-9b](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/
+lora_zero3). - ð¥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/
+2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start
+training. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/
+2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start
+training. - 2024.02.25: Support `swift export` to quantize models using **AWQ/
+GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md). More - 2024.02.22: Support gemma series:
+gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
+2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-
+instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support **Qwen1.5** series
+models, see [model list](https://github.com/modelscope/swift/blob/main/docs/
+source/LLM/
+%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
+for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-
+7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen1half_7b_chat_int8). - 2024.02.05: Support training of diffusion models
+such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training.
+See corresponding [training scripts](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/sdxl/scripts) for details. - 2024.02.01: Support minicpm
+series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat. -
+ð¥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**.
+Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced
+the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/
+iic/ms_bench/summary). - ð¥2024.02.01: Support Agent training! Agent training
+algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf).
+We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/
+summary), a high-quality agent dataset. Use [this script](https://github.com/
 modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/
-sft.sh) to begin an agent training! - ð¥2024.02.01: Support SFT loss to DPO
-training to reduce the repeat generation problem caused by the KL-divergence
-loss. - 2024.02.01: Support AdaLoRA and IA3 adapter in SFT. - 2024.02.01:
-Support `--merge_lora` in AnimateDiff training. More - 2024.01.30: Support
+sft.sh) to start Agent training! - ð¥2024.02.01: Support adding SFT loss in
+DPO training to reduce repetitive generation caused by KL divergence loss. -
+2024.02.01: Support using AdaLoRA and IA3 adapters in training. - 2024.02.01:
+Support `--merge_lora` parameter in AnimateDiff training. - 2024.01.30: Support
 [internlm-xcomposer2-7b-chat](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/internlm_xcomposer2_7b_chat). - ð¥2024.01.30:
 Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), just need to specify `--
-deepspeed default-zero3`. - 2024.01.29: Support internlm2-math series:
-internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-
-20b-chat. - ð¥2024.01.26: Support [yi-vl-6b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-
-34b-chat. - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-
-chat. - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://
+pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), simply specify `--deepspeed
+default-zero3`. - 2024.01.29: Support internlm2-math series: internlm2-math-7b,
+internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat. -
+ð¥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/
+tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat. -
+2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat. -
+2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 orion_14b_chat). - 2024.01.20: Support [xverse-13b-256k](https://github.com/
 modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k),
-xverse-65b-v2, xverse-65b-chat. - ð¥2024.01.17: Support **internlm2** series:
+xverse-65b-v2, xverse-65b-chat. - ð¥2024.01.17: Support internlm2 series:
 internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/
 modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat),
 internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat,
-internlm2-20b-chat. - 2024.1.15: Support yuan series: yuan2-2b-instruct,
+internlm2-20b-chat. - 2024.01.15: Support yuan series: yuan2-2b-instruct,
 [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct,
 yuan2-102b-instruct. - ð¥2024.01.12: Support **deepseek-moe** series:
 deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/
 tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat). -
-ð¥2024.01.04: Support for **VLLM deployment**, compatible with the **OpenAI
-API** style. For more details, please refer to [VLLM Inference Acceleration and
-Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²) - 2024.01.04: Update [Benchmark](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) to
-facilitate viewing the training speed and GPU memory required for different
-models. - ð¥ 2023.12.29: Support web-ui for training and inference, use
-`swift web-ui` after the installation of ms-swift. - ð¥ 2023.12.29: Support
-DPO RLHF(Reinforcement Learning from Human Feedback) and three datasets: AI-
-ModelScope/stack-exchange-paired and AI-ModelScope/hh-rlhf and AI-ModelScope/
-hh_rlhf_cn for this task. Check [this documentation](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
+ð¥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API**
+style, see [VLLM Inference Acceleration and Deployment](https://github.com/
+modelscope/swift/blob/main/docs/source/LLM/VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²)
+for details. - 2024.01.04: Update [Benchmark](https://github.com/modelscope/
+swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of
+training speed and memory usage of different models. - ð¥2023.12.29: Support
+web-ui for sft training and inference, use `swift web-ui` after installing ms-
+swift to start. - ð¥2023.12.29: Support DPO RLHF (Reinforcement Learning from
+Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-
+paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation]
+(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
 LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
-to start training! - ð¥ 2023.12.28: Support SCEdit! This framework can easily
-reduce memory usage in training and inference, and replace ControlNet for
-controllable image generating scenarios, view the following chapter for
-details. - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19:
-Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/phi2_3b). - 2023.12.18: Support for VLLM for inference
-acceleration. - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-
-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-
-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b,
-deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-mixtral_moe_7b), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/
-tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b_instruct). - 2023.12.09:
-Support the `freeze_parameters` parameter as a compromise between LoRA and full
-parameter. Corresponding shell scripts can be found at [full_freeze_ddp](https:
-//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
-`preprocess_num_proc` parameters, for details please refer to [Command-Line
-parameters](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-å½ä»¤è¡åæ°.md). - 2023.12.08: Support [sus-34b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/sus_34b_chat), support
-yi-6b-200k, yi-34b-200k. - 2023.12.07: Support [Multi-Node DDP training](https:
-//github.com/modelscope/swift/blob/main/docs/source/LLM/
+to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
+significantly reduce memory usage in U-Net and support low-memory controllable
+image generation (replacing ControlNet), read the section below to learn more.
+- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
+3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+phi2_3b). - 2023.12.18: Support VLLM for inference acceleration. - 2023.12.15:
+Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat,
+deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-
+1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-
+instruct, deepseek-coder-33b, deepseek-coder-33b-instruct. - 2023.12.13:
+Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/
+swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-
+instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/mixtral_7b_moe_instruct). - 2023.12.09: Support `freeze_parameters`
+parameter as a compromise between lora and full-parameter training.
+Corresponding sh can be found in [full_freeze_ddp](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/
+full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
+`preprocess_num_proc` parameters, see [command line arguments](https://
+github.com/modelscope/swift/blob/main/docs/source/LLM/
+%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details. - 2023.12.08:
+Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k. -
+2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/
+swift/blob/main/docs/source/LLM/
 LLM%E5%BE%AE%E8%B0%83%E6%96%87%E6%A1%A3.md#%E4%BD%BF%E7%94%A8cli). -
-2023.12.04: Supported models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat.
-Supported datasets: hc3-zh, hc3-en. - ð¥ 2023.12.02: [Best Practice for Self-
-cognition Fine-tuning](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/èªæè®¤ç¥å¾®è°æä½³å®è·µ.md), **10 minutes for self-cognition
-fine-tuning for LLM**, creating a LLM that is specific to oneself. - ð¥
-2023.11.30: Support for training and inference of the **qwen-1_8b**, **qwen-
-72b**, and **qwen-audio** model series. The corresponding shell scripts can be
-viewed at [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/
+2023.12.05: Support models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat.
+Support datasets: hc3-zh, hc3-en. - ð¥2023.12.02: [Self-cognition fine-tuning
+best practices](docs/source_en/LLM/Self-cognition-best-practice.md), **10
+minutes to fine-tune a large model for self-cognition**, create your own unique
+large model. - ð¥2023.11.30: Support training and inference of **qwen-1_8b**,
+**qwen-72b**, **qwen-audio** series models. Corresponding sh scripts can be
+found in [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/qwen_audio_chat). - ð¥ 2023.11.29: Support
-the training and inference for **AnimateDiff** - ð¥ 2023.11.24: Support for
-**yi-34b-chat**, **codefuse-codellama-34b-chat**: The corresponding shell
-script can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat]
-(https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-codefuse_codellama_34b_chat). - ð¥ 2023.11.18: Support for **tongyi-finance-
-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-
-finance-14b-chat-int4. The corresponding shell script can be found in
+main/examples/pytorch/llm/scripts/qwen_audio_chat) - ð¥2023.11.29: Support
+training and inference of **AnimateDiff** - ð¥2023.11.24: Support **yi-34b-
+chat**, **codefuse-codellama-34b-chat** models. Corresponding sh scripts can be
+found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+codefuse_codellama_34b_chat). - ð¥2023.11.18: Support **tongyi-finance-14b**
+series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-
+chat-int4. Corresponding sh scripts can be found in
 [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4). - 2023.11.16: Added
-support for more models in **flash attn**: qwen series, qwen-vl series, llama
+examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4). - 2023.11.16:
+Support **flash attn** for more models: qwen series, qwen-vl series, llama
 series, openbuddy series, mistral series, yi series, ziya series. Please use
-the `use_flash_attn` parameter. - ð¥ 2023.11.11: **NEFTune** Supported, Use
-is with `Swift.prepare_model(model, NEFTuneConfig())` - ð¥ 2023.11.11:
-Support training and inference with **CLI**, and inference with **Web-UI**.
-Check the [Run using Swift CLI](https://github.com/modelscope/swift/tree/
-main#run-using-swift-cli) chapter for details. - ð¥ 2023.11.11: Support model
-**deployment**(vllm/chatglm.cpp/xinference)ï¼Check [Official documentation](./
-docs/source/GetStarted/é¨ç½²æå.md) for details. - ð¥ 2023.11.10: Support
-for **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-
-7b-chat-32k. The corresponding shell script can be found in [bluelm_7b_chat]
+`use_flash_attn` parameter. - ð¥2023.11.11: Support **NEFTune**, simply use
+`Swift.prepare_model(model, NEFTuneConfig())` to enable. - ð¥2023.11.11:
+Support training and inference by **command line** and inference by **Web-UI**,
+see `Usage with Swift CLI` section below for details. - ð¥2023.11.10: Support
+**bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-
+chat-32k. Corresponding sh scripts can be found in [bluelm_7b_chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+bluelm_7b_chat). - ð¥2023.11.08: Support training and inference of **xverse-
+65b** model, script at [xverse_65b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/xverse_65b). - ð¥2023.11.07: Support
+training and inference of **yi-6b**, **yi-34b** models, scripts at [yi_6b]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-bluelm_7b_chat). - ð¥ 2023.11.08: Support the finetuning of **xverse-65b**
-model, scripts can be found at: [xverse_65b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/xverse_65b). - ð¥ 2023.11.07:
-Support the finetuning of **yi-6b**, **yi-34b** model, scripts can be found at:
-[yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
-scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/yi_34b). - ð¥ 2023.10.30: Support **QA-LoRA**
-and **LongLoRA** to decrease memory usage in training. - ð¥ 2023.10.30:
-Support **ROME**(Rank One Model Editing) to add/modify knowledges, training is
-not needed! - 2023.10.30: Support for **skywork-13b** series models: skywork-
-13b, skywork-13b-chat. The corresponding shell script can be found in
-[skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
-llm/scripts/skywork_13b). - ð¥ 2023.10.27: Support for **chatglm3** series
-models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. The corresponding shell
-script can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/chatglm3_6b). - ð¥ 2023.10.17: Supported
-**int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-
-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-
-14b-chat-int8. - 2023.10.15: Supported **ziya2-13b** model series: ziya2-13b,
-ziya2-13b-chat. - 2023.10.12: Supported **mistral-7b** model series: openbuddy-
-mistral-7b-chat, mistral-7b, mistral-7b-instruct. - ð¥ 2023.10.07: Supported
-**DeepSpeed ZeRO-2**, enabling LoRA (not just QLoRA) to run DDP on 2*A10. -
-2023.10.04: Supported datasets in the fields of mathematics, law, SQL, and
-coding: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en,
-lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en. - ð¥ 2023.09.25:
-Supported **qwen-14b** model series: qwen-14b, qwen-14b-chat. - 2023.09.18:
-Supported **internlm-20b** model series: internlm-20b, internlm-20b-chat. -
-2023.09.12: Supported training with **MP+DDP** to accelerate full-parameter
-fine-tuning speed. - 2023.09.05: Supported **openbuddy-llama2-70b-chat** model.
-- 2023.09.03: Supported **baichuan2** model series: baichuan2-7b, baichuan2-7b-
-chat, baichuan2-13b, baichuan2-13b-chat. ## â¨ LLM Training and Inference If
-you want to learn more about **best practices** for LLM or multimodal LLM, or
-if you are interested in **tutorials** on inference, fine-tuning, quantization,
-and deployment of LLM, you can refer to the [LLM series documentation](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/index.md). ### WEB UI
-training and inference After installation, you can use web-ui training/
-inference like: ```shell SWIFT_UI_LANG=en swift web-ui ``` > Supported
-environment variables: > > WEBUI_SHARE=1 Share the gradio or not >
-SWIFT_UI_LANG=en/zh The language of radio > WEBUI_SERVER server_nameï¼ web-ui
-host ipï¼0.0.0.0 means all routes are allowedï¼127.0.0.1 means only localhost
-can visit the web > WEBUI_PORT The port of web-ui Here is a simple introduction
-of web-ui: [![Watch the video](docs/source/cources/resources/
-20240119160942.jpg)](https://modelscope-open.oss-cn-hangzhou.aliyuncs.com/
-SWIFT%E8%A7%86%E9%A2%91_%E8%B0%83%E6%95%B4%E5%B0%81%E9%9D%A2.mp4) ### Quick
-Start You can test if the environment is installed correctly by running the
-following code. ```python # pip install ms-swift[llm] -U # Experimental
-environment: A10, 3090, V100, ... # 8GB GPU memory import os os.environ
-['CUDA_VISIBLE_DEVICES'] = '0' import torch from swift.llm import
-( DatasetName, InferArguments, ModelType, SftArguments, infer_main, sft_main,
-app_ui_main, merge_lora ) model_type = ModelType.qwen1half_0_5b sft_args =
-SftArguments( model_type=model_type, train_dataset_sample=2000, dataset=
-[DatasetName.jd_sentiment_zh], output_dir='output') result = sft_main(sft_args)
-best_model_checkpoint = result['best_model_checkpoint'] print
-(f'best_model_checkpoint: {best_model_checkpoint}') torch.cuda.empty_cache()
-infer_args = InferArguments( ckpt_dir=best_model_checkpoint,
-load_dataset_config=True, val_dataset_sample=10) merge_lora(infer_args,
-device_map='cpu') result = infer_main(infer_args) torch.cuda.empty_cache()
-app_ui_main(infer_args) ``` ### Training Scripts You can refer to the following
-scripts to customize your own training script. - full: [qwen1half-7b-chat]
+yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/yi_34b). - ð¥2023.10.30: Support two new tuners: **QA-
+LoRA** and **LongLoRA**. - ð¥2023.10.30: Support editing models using
+**ROME** (Rank One Model Editing) to infuse new knowledge into models without
+training! - 2023.10.30: Support **skywork-13b** series models: skywork-13b,
+skywork-13b-chat. Corresponding sh scripts can be found in [skywork_13b](https:
+//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+skywork_13b). - ð¥2023.10.27: Support **chatglm3** series models: chatglm3-
+6b-base, chatglm3-6b, chatglm3-6b-32k. Corresponding sh scripts can be found in
+[chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
+llm/scripts/chatglm3_6b). - ð¥2023.10.17: Support SFT of **int4**, **int8**
+models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-
+chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8. -
+2023.10.15: Support **ziya2-13b** series models: ziya2-13b, ziya2-13b-chat. -
+2023.10.12: Support **mistral-7b** series models: openbuddy-mistral-7b-chat,
+mistral-7b, mistral-7b-instruct. - ð¥2023.10.07: Support **DeepSpeed ZeRO-
+2**, enabling lora (not just qlora) to run DDP on dual A10 cards. - 2023.10.04:
+Support more math, law, SQL, code domain datasets: blossom-math-zh, school-
+math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh,
+leetcode-python-en. - ð¥2023.09.25: Support **qwen-14b** series: qwen-14b,
+qwen-14b-chat. - 2023.09.18: Support **internlm-20b** series: internlm-20b,
+internlm-20b-chat. - 2023.09.12: Support **MP+DDP** to accelerate full-
+parameter training. - 2023.09.05: Support **openbuddy-llama2-70b-chat**. -
+2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat,
+baichuan2-13b, baichuan2-13b-chat. ## ð ï¸ Installation SWIFT runs in the
+Python environment. Please ensure your Python version is higher than 3.8. -
+Method 1: Install SWIFT using pip command: ```shell # Full capabilities pip
+install ms-swift[all] -U # LLM only pip install ms-swift[llm] -U # AIGC only
+pip install ms-swift[aigc] -U # Adapters only pip install ms-swift -U ``` -
+Method 2: Install SWIFT through source code (convenient for running training
+and inference scripts), please run the following commands: ```shell git clone
+https://github.com/modelscope/swift.git cd swift pip install -e .[llm] ```
+SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3: Use SWIFT in
+our Docker image ```shell # China-Hangzhou image docker pull registry.cn-
+hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
+torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull registry.us-west-
+1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
+torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This section introduces
+basic usage, see the [Documentation](#-documentation) section for more ways to
+use. ### Web-UI ```shell swift web-ui ``` ### Training #### Training Scripts
+You can refer to the following scripts to customize your own training script. -
+full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100) -
-full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100) -
-full+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora:
-[chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
-llm/scripts/chatglm3_6b/lora) (3090), [baichuan2-13b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/baichuan2_13b_chat/
-lora_mp) (2\*3090), [yi-34b-chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat]
+qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
+//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/
+lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-
+34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_mp)
+(2\*A100) - lora+ddp: [chatglm3-6b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp) (2\*3090) -
+lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3) (4\*3090), [qwen-
+72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100) - qlora(gptq-int4): [qwen-7b-
+chat-int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen_7b_chat_int4/qlora) (3090) - qlora(gptq-int8): [qwen1half-7b-chat-
+int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-int4): [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_72b_chat/lora_mp) (2\*A100) - lora+ddp: [chatglm3-6b](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp)
-(2\*3090) - lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3)
-(4\*3090), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100) - qlora
-(gptq-int4): [qwen-7b-chat-int4](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_7b_chat_int4/qlora) (3090) - qlora(gptq-
-int8): [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-
-int4): [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen_7b_chat/qlora) (3090) ### Features - Supported SFT
-Methods: [lora](https://arxiv.org/abs/2106.09685), [qlora](https://arxiv.org/
-abs/2305.14314), [longlora](https://arxiv.org/abs/2309.12307), [qalora](https:/
-/arxiv.org/abs/2309.14717), full parameter fine-tuning, partial parameter fine-
-tuning. - Supported Features: quantization, DDP, model parallelism, gradient
-checkpointing, pushing to modelscope hub, custom datasets, multimodal and agent
-SFT, mutli-round chat, DPO, self-cognition fine-tuning, ... - Supported Models:
-[[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/
-LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
-- Multi-Modal: - [qwen-vl](https://github.com/QwenLM/Qwen-VL) series: qwen-vl,
-qwen-vl-chat, qwen-vl-chat-int4. - [qwen-audio](https://github.com/QwenLM/Qwen-
-Audio) series: qwen-audio, qwen-audio-chat. - [deepseek-vl](https://github.com/
-deepseek-ai/DeepSeek-VL) series: deepseek-vl-1_3b-chat, deepseek-vl-7b-chat. -
-[yi-vl](https://github.com/01-ai/Yi) series: yi-vl-6b-chat, yi-vl-34b-chat. -
-[internlm-xcomposer2](https://github.com/InternLM/InternLM-XComposer) series:
-internlm-xcomposer2-7b-chat. - [minicpm-v](https://github.com/OpenBMB/MiniCPM)
-series: minicpm-v-3b-chat. - [cogvlm](https://github.com/THUDM/CogVLM) series:
-cogvlm-17b-instruct, cogagent-18b-chat, cogagent-18b-instruct. - General: -
-[qwen](https://github.com/QwenLM/Qwen) series: - qwen-1_8b, qwen-1_8b-chat,
-qwen-1_8b-chat-int4, qwen-1_8b-chat-int8. - qwen-7b, qwen-7b-chat, qwen-7b-
-chat-int4, qwen-7b-chat-int8. - qwen-14b, qwen-14b-chat, qwen-14b-chat-int4,
-qwen-14b-chat-int8. - qwen-72b, qwen-72b-chat, qwen-72b-chat-int4, qwen-72b-
-chat-int8. - [qwen1.5](https://github.com/QwenLM/Qwen1.5) series: - qwen1half-
-0_5b, qwen1half-0_5b-chat, qwen1half-0_5b-chat-int4, qwen1half-0_5b-chat-int8,
-qwen1half-0_5b-chat-awq. - qwen1half-1_8b, qwen1half-1_8b-chat, qwen1half-1_8b-
-chat-int4, qwen1half-1_8b-chat-int8, qwen1half-1_8b-chat-awq. - qwen1half-4b,
-qwen1half-4b-chat, qwen1half-4b-chat-int4, qwen1half-4b-chat-int8, qwen1half-
-4b-chat-awq. - qwen1half-7b, qwen1half-7b-chat, qwen1half-7b-chat-int4,
-qwen1half-7b-chat-int8, qwen1half-7b-chat-awq. - qwen1half-14b, qwen1half-14b-
-chat, qwen1half-14b-chat-int4, qwen1half-14b-chat-int8, qwen1half-14b-chat-awq.
-- qwen1half-72b, qwen1half-72b-chat, qwen1half-72b-chat-int4, qwen1half-72b-
-chat-int8, qwen1half-72b-chat-awq. - [chatglm](https://github.com/THUDM/
-ChatGLM-6B) series: chatglm2-6b, chatglm2-6b-32k, chatglm3-6b-base, chatglm3-
-6b, chatglm3-6b-32k. - [llama](https://github.com/facebookresearch/llama)
-series: llama2-7b, llama2-7b-chat, llama2-13b, llama2-13b-chat, llama2-70b,
-llama2-70b-chat. - [yi](https://github.com/01-ai/Yi) series: yi-6b, yi-6b-200k,
-yi-6b-chat, yi-9b, yi-34b, yi-34b-200k, yi-34b-chat. - [internlm](https://
-github.com/InternLM/InternLM) series: - internlm-7b, internlm-7b-chat,
-internlm-7b-chat-8k, internlm-20b, internlm-20b-chat. - internlm2-1_8b,
-internlm2-1_8b-sft-chat, internlm2-1_8b-chat, internlm2-7b-base, internlm2-7b,
-internlm2-7b-sft-chat, internlm2-7b-chat, internlm2-20b-base, internlm2-20b,
-internlm2-20b-sft-chat, internlm2-20b-chat. - [deepseek](https://github.com/
-deepseek-ai/deepseek-LLM) series: deepseek-7b, deepseek-7b-chat, deepseek-67b,
-deepseek-67b-chat, deepseek-moe-16b, deepseek-moe-16b-chat. - [gemma](https://
-github.com/google/gemma_pytorch) series: gemma-2b, gemma-2b-instruct, gemma-7b,
-gemma-7b-instruct. - [minicpm](https://github.com/OpenBMB/mlc-MiniCPM) series:
-minicpm-2b-sft-chat, minicpm-2b-chat. - [openbuddy](https://github.com/
-OpenBuddy/OpenBuddy) series: openbuddy-llama2-13b-chat, openbuddy-llama-65b-
-chat, openbuddy-llama2-70b-chat, openbuddy-mistral-7b-chat, openbuddy-zephyr-
-7b-chat, openbuddy-deepseek-67b-chat, openbuddy-mixtral-moe-7b-chat. -
-[mistral](https://github.com/mistralai/mistral-src) series: mistral-7b,
-mistral-7b-instruct, mistral-7b-instruct-v2. - [mixtral](https://github.com/
-mistralai/mistral-src) series: mixtral-moe-7b, mixtral-moe-7b-instruct. -
-[baichuan](https://github.com/baichuan-inc/Baichuan2) series: baichuan-7b,
-baichuan-13b, baichuan-13b-chat, baichuan2-7b, baichuan2-7b-chat, baichuan2-
-13b, baichuan2-13b-chat, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4. -
-[yuan](https://github.com/IEIT-Yuan/Yuan-2.0) series: yuan2-2b-instruct, yuan2-
-2b-janus-instruct, yuan2-51b-instruct, yuan2-102b-instruct. - [xverse](https://
-github.com/xverse-ai/XVERSE-13B) series: xverse-7b, xverse-7b-chat, xverse-13b,
-xverse-13b-chat, xverse-65b, xverse-65b-v2, xverse-65b-chat, xverse-13b-256k. -
-[orion](https://github.com/OrionStarAI/OrionStar-Yi-34B-Chat) series: orion-
-14b, orion-14b-chat. - [bluelm](https://github.com/vivo-ai-lab/BlueLM) series:
-bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. - [zephyr](https:
-//github.com/huggingface/alignment-handbook) series: zephyr-7b-beta-chat. -
-[ziya](https://github.com/IDEA-CCNL/Fengshenbang-LM) series: ziya2-13b, ziya2-
-13b-chat. - [skywork](https://github.com/SkyworkAI/Skywork) series: skywork-
-13b, skywork-13b-chat. - other: [polylm-13b](https://github.com/DAMO-NLP-MT/
-PolyLM), [seqgpt-560m](https://github.com/Alibaba-NLP/SeqGPT), [sus-34b-chat]
-(https://github.com/SUSTech-IDEA/SUS-Chat). - Financial: - [tongyi-finance]
-(https://github.com/QwenLM/Qwen) series: tongyi-finance-14b, tongyi-finance-
-14b-chat, tongyi-finance-14b-chat-int4. - Coding: - [codefuse](https://
-github.com/codefuse-ai) series: codefuse-codellama-34b-chat, codefuse-
-codegeex2-6b-chat, codefuse-qwen-14b-chat. - [deepseek-coder](https://
-github.com/deepseek-ai/DeepSeek-Coder) series: deepseek-coder-1_3b, deepseek-
-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct,
-deepseek-coder-33b, deepseek-coder-33b-instruct. - [codegeex2](https://
-github.com/THUDM/CodeGeeX2) series: codegeex2-6b. - [phi](https://
-www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-
-language-models/) series: phi2-3b. - Math: - [internlm2-math](https://
-github.com/InternLM/InternLM-Math) series: internlm2-math-7b, internlm2-math-
-7b-chat, internlm2-math-20b, internlm2-math-20b-chat. - [deepseek-math](https:/
-/github.com/deepseek-ai/DeepSeek-Math) series: deepseek-math-7b, deepseek-math-
-7b-instruct, deepseek-math-7b-chat. - Supported Datasets: [[Detailed Info]]
-(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%95%B0%E6%8D%AE%E9%9B%86)
-- NLP: - General: ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4),
-ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en,
-cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh,
-tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4,
-ð¥sharegpt-gpt4-mini. - Agent: ð¥ms-agent, damo-mini-agent-zh, damo-agent-
-zh, agent-instruct-all-en. - RLHF: ð¥hh-rlhf-cn, stack-exchange-paired, hh-
-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-
-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-
-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-
-helpful-base-en. - Coding: code-alpaca-en, ð¥leetcode-python-en,
-ð¥codefuse-python-en, ð¥codefuse-evol-instruction-zh. - Medical: medical-
-en, medical-zh, medical-mini-zh, ð¥disc-med-sft-zh. - Law: lawyer-llama-zh,
-tigerbot-law-zh, ð¥disc-law-sft-zh. - Math: ð¥blossom-math-zh, school-math-
-zh, open-platypus-en. - SQL: text2sql-en, ð¥sql-create-context-en. - Text
-Generation: ð¥advertise-gen-zh, ð¥dureader-robust-zh. - Classification:
-cmnli-zh, ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. -
-AWQ: pileval. - Other: finance-en, poetry-zh, webnovel-zh, generated-chat-zh,
-cls-fudan-news-zh, ner-jave-zh. - Multi-Modal: - Vision: coco-en, ð¥coco-
-mini-en, coco-mini-en-2, capcha-images. - Audio: aishell1-zh, ð¥aishell1-
-mini-zh. - Custom Dataset - Supported Templates: - Text Generation: default-
-generation, default-generation-bos, chatglm-generation, qwen-audio-generation.
-- Chat: default, qwen, qwen-audio, baichuan, chatglm2, chatglm3, llama,
-openbuddy, internlm, internlm2, internlm-xcomposer2, yi, yi-vl, yuan, xverse,
-ziya, skywork, bluelm, zephyr, sus, deepseek, deepseek-coder, codefuse-
-codellama, codefuse, cogvlm-instruct, cogagent-chat, cogagent-instruct, orion,
-minicpm, minicpm-v, gemma, chatml. ## ð¥SCEdit SCEdit is an efficient
-generative fine-tuning framework proposed by Alibaba TongYi Vision Intelligence
-Lab. This framework enhances the fine-tuning capabilities for text-to-image
-generation downstream tasks and enables quick adaptation to specific generative
-scenarios, **saving 30%-50% of training memory costs compared to LoRA**.
-Furthermore, it can be directly extended to controllable image generation
-tasks, **requiring only 7.9% of the parameters that ControlNet needs for
-conditional generation and saving 30% of memory usage**. It supports various
-conditional generation tasks including edge maps, depth maps, segmentation
-maps, poses, color maps, and image completion. We using 3D style data from the
-[style transfer dataset](https://modelscope.cn/datasets/damo/
-style_custom_dataset/dataPeview) for training, and testing with the same
-`Prompt: A boy in a camouflage jacket with a scarf`. The qualitative and
-quantitative results are as follows: | Method | bs | ep | Target Module |
-Param. (M) | Mem. (MiB) | 3D style | | --------- | ---- | ---- | ------------
-- | ------------- | ---------- | ----------------------------------------------
--------------- | | LoRA/r=64 | 1 | 50 | q/k/v/out/mlp | 23.94 (2.20%) | 8440MiB
-| [img]| | SCEdit | 1 | 50 | up_blocks | 19.68 (1.81%) | 7556MiB | [img]| |
-LoRA/r=64 | 10 | 100 | q/k/v/out/mlp | 23.94 (2.20%) | 26300MiB | [img]| |
-SCEdit | 10 | 100 | up_blocks | 19.68 (1.81%) | 18634MiB | [img]| | LoRA/r=64 |
-30 | 200 | q/k/v/out/mlp | 23.94 (2.20%) | 69554MiB | [img]| | SCEdit | 30 |
-200 | up_blocks | 19.68 (1.81%) | 43350MiB | [img]| The benchmark listed above
-can be reproduced byï¼ ```shell # Install swift by the next chapter cd
-examples/pytorch/multi_modal/notebook python text_to_image_synthesis.py ``` ##
-ð ï¸ Installation SWIFT is running in Python environment. Please make sure
-your python version is higher than 3.8. - Install SWIFT by the `pip` command:
-```shell # full ability pip install ms-swift[all] -U # only use llm pip install
-ms-swift[llm] -U # only use aigc pip install ms-swift[aigc] -U # only use
-adapters pip install ms-swift -U ``` - Install SWIFT by source code(for running
-sft/infer examples), please run: ```shell git clone https://github.com/
-modelscope/swift.git cd swift pip install -e .[llm] ``` SWIFT requires
-torch>=1.13. - Use SWIFT in our docker image: ```shell docker pull registry.cn-
-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu20.04-cuda11.8.0-py38-
-torch2.0.1-tf2.13.0-1.9.1 ``` ## ð Getting Started SWIFT supports multiple
-tuners, as well as tuners provided by [PEFT](https://github.com/huggingface/
-peft). To use these tuners, simply call: ```python from swift import Swift,
-LoRAConfig config = LoRAConfig(...) model = Swift.prepare_model(model, config,
-extra_state_keys=['...']) ``` The code snippet above initialized the tuner
-randomly. The input model is an instance of `torch.nn.Module`, the config is a
-subclass instance of `SwiftConfig` or `PeftConfig`. extra_state_keys is the
-extra module weights(like the linear head) to be trained and stored in the
-output dir. You may combine multiple tuners by: ```python from swift import
-Swift, LoRAConfig, PromptConfig model = Swift.prepare_model(model, {'lora':
-LoRAConfig(...), 'prompt': PromptConfig(...)}) ``` Call `save_pretrained` and
-`push_to_hub` after finetuning: ```python from swift import push_to_hub
-model.save_pretrained('some-output-folder') push_to_hub('my-group/some-repo-id-
-modelscope', 'some-output-folder', token='some-ms-token') ``` Assume `my-group/
-some-repo-id-modelscope` is the model-id in the hub, and `some-ms-token` is the
-token for uploading. Using the model-id to do later inference: ```python from
-swift import Swift model = Swift.from_pretrained(model, 'my-group/some-repo-id-
-modelscope') ``` Here shows a runnable example: ```python import os import
-tempfile # Please install modelscope by `pip install modelscope` from
-modelscope import Model from swift import LoRAConfig, SwiftModel, Swift,
-push_to_hub tmp_dir = tempfile.TemporaryDirectory().name if not os.path.exists
-(tmp_dir): os.makedirs(tmp_dir) model = Model.from_pretrained('modelscope/
-Llama-2-7b-ms', device_map='auto') lora_config = LoRAConfig(target_modules=
-['q_proj', 'k_proj', 'v_proj']) model: SwiftModel = Swift.prepare_model(model,
-lora_config) # Do some finetuning here model.save_pretrained(tmp_dir)
-push_to_hub('my-group/swift_llama2', output_dir=tmp_dir) model =
-Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto') model =
-SwiftModel.from_pretrained(model, 'my-group/swift_llama2', device_map='auto')
-``` This is a example that uses transformers for model creation uses SWIFT for
-efficient tuning. ```python from swift import Swift, LoRAConfig, AdapterConfig,
-PromptConfig from transformers import AutoModelForImageClassification # init
-vit model model = AutoModelForImageClassification.from_pretrained("google/vit-
-base-patch16-224") # init lora tuner config lora_config = LoRAConfig( r=10, #
-the rank of the LoRA module target_modules=['query', 'key', 'value'], # the
-modules to be replaced with the end of the module name merge_weights=False #
-whether to merge weights ) # init adapter tuner config adapter_config =
-AdapterConfig( dim=768, # the dimension of the hidden states hidden_pos=0, #
-the position of the hidden state to passed into the adapter
-target_modules=r'.*attention.output.dense$', # the modules to be replaced with
-regular expression adapter_length=10 # the length of the adapter length ) #
-init prompt tuner config prompt_config = PromptConfig( dim=768, # the dimension
-of the hidden states target_modules=r'.*layer\.\d+$', # the modules to be
-replaced with regular expression embedding_pos=0, # the position of the
-embedding tensor prompt_length=10, # the length of the prompt tokens
-attach_front=False # Whether prompt is attached in front of the embedding ) #
-create model with swift. In practice, you can use any of these tuners or a
-combination of them. model = Swift.prepare_model(model, {"lora_tuner":
-lora_config, "adapter_tuner": adapter_config, "prompt_tuner": prompt_config}) #
-get the trainable parameters of model model.get_trainable_parameters() #
-'trainable params: 838,776 || all params: 87,406,432 || trainable%:
-0.9596273189597764' ``` You can use the features offered by Peft in SWIFT:
-```python from swift import LoraConfig, Swift from peft import TaskType
-lora_config = LoraConfig(target_modules=['query', 'key', 'value'],
-task_type=TaskType.CAUSAL_LM) model_wrapped = Swift.prepare_model(model,
-lora_config) # or call from_pretrained to load weights in the modelhub
-model_wrapped = Swift.from_pretrained(model, 'some-id-in-the-modelscope-
-modelhub') ``` The saving strategy between Swift tuners and Peft tuners are
-slightly different. You can name a tuner by: ```python model =
-Swift.prepare_model(model, {'default': LoRAConfig(...)}) model.save_pretrained
-('./output') ``` In the output dir, you will have a dir structure like this:
-```text output |-- default |-- adapter_config.json |-- adapter_model.bin |-
-- adapter_config.json |-- adapter_model.bin ``` The config/weights stored in
-the output dir is the config of `extra_state_keys` and the weights of it. This
-is different from PEFT, which stores the weights and config of the `default`
-tuner. ## ð Learn More - [ModelScope library](https://github.com/modelscope/
-modelscope/) ModelScope Library is the model library of ModelScope project,
-which contains a large number of popular models. - [Contribute your own model
-to ModelScope](https://modelscope.cn/docs/
-ModelScope%E6%A8%A1%E5%9E%8B%E6%8E%A5%E5%85%A5%E6%B5%81%E7%A8%8B%E6%A6%82%E8%A7%88)
-## License This project is licensed under the [Apache License (Version 2.0)]
-(https://github.com/modelscope/modelscope/blob/master/LICENSE). ## â Contact
-Us You can contact and communicate with us by joining our WeChat Group:
+qwen_7b_chat/qlora) (3090) #### Supported Training Processes | Training Process
+| Training Method | |------------------|---------------------------------------
+----------------------------------------| | Pretraining | Text Generation | |
+Fine-tuning | Single-turn/Multi-turn
+Agent Training/Self-cognition
+Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO | | Text-to-
+Image | DreamBooth, etc. | | Text-to-Video | - | #### Single GPU Training Start
+single GPU fine-tuning with the following command: LoRA: ```shell #
+Experimental Environment: A100 # GPU Memory Requirement: 20GB # Runtime: 3.1
+hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ --eval_steps 200 \ ``` Full-parameter: ```shell # Experimental
+Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5 hours
+CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --dataset
+blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir output
+\ --eval_steps 500 \ ``` #### Model Parallel Training ```shell # Experimental
+Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB # Runtime: 3.4
+hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type qwen1half-7b-chat \ -
+-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --
+output_dir output \ ``` #### Data Parallel Training ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB # Runtime: 0.8 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
+Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
+Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ ``` #### Deepspeed Training ZeRO2: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB # Runtime: 0.9 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ --deepspeed default-zero2 \ ``` ZeRO3:
+```shell # Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 *
+19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+default-zero3 \ ``` ### Inference Original model: ```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
+infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
+ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
+infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
+CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset
+mmlu ceval ``` ### Export Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
+export --model_type qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ```
+LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/
+checkpoint-xxx --load_dataset_config true \ --quant_method awq --quant_bits 4 \
+--merge_lora true \ ``` ### Deployment Original model: ```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
+ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
+chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
+ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
+checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
+``` ### Supported Models #### LLMs | Model Type | Model Introduction | Language
+| Model Size | Model Type | |------------------------------------------------|-
+-----------------------------------------------------------------------|-------
+-------------|----------------------------------------|------------------------
+------------------- | | Qwen
+Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
+Chinese
+English | 0.5B-72B
+including quantized versions | base model
+chat model
+MoE model | | ChatGLM2
+ChatGLM3
+Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
+English | 6B | base model
+chat model
+code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
+github.com/baichuan-inc) | Chinese
+English | 7B-13B
+including quantized versions | base model
+chat model | | Yuan2 | [Langchao Yuan series models](https://github.com/IEIT-
+Yuan) | Chinese
+English | 2B-102B | instruct model | | XVerse | [XVerse series models](https://
+github.com/xverse-ai) | Chinese
+English | 7B-65B | base model
+chat model
+long text model
+MoE model | | LLaMA2 | [LLaMA2 series models](https://github.com/
+facebookresearch/llama) | English | 7B-70B
+including quantized versions | base model
+chat model | | Mistral
+Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
+English | 7B-22B | base model
+instruct model
+MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
+Chinese
+English | 6B-34B | base model
+chat model
+long text model | | InternLM
+InternLM2
+InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
+InternLM/InternLM) | Chinese
+English | 1.8B-20B | base model
+chat model
+math model | | DeepSeek
+DeepSeek-MoE
+DeepSeek-Coder
+DeepSeek-Math | [DeepSeek series models](https://github.com/deepseek-ai) |
+Chinese
+English | 1.3B-67B | base model
+chat model
+MoE model
+code model
+math model | | MAMBA | [MAMBA temporal convolution model](https://github.com/
+state-spaces/mamba) | English | 130M-2.8B | base model | | Gemma | [Google
+Gemma series models](https://github.com/google/gemma_pytorch) | English | 2B-7B
+| base model
+instruct model | | MiniCPM | [OpenBmB MiniCPM series models](https://
+github.com/OpenBMB/MiniCPM) | Chinese
+English | 2B-3B | chat model
+MoE model | | OpenBuddy | [OpenBuddy series models](https://github.com/
+OpenBuddy/OpenBuddy) | Chinese
+English | 7B-67B | base model
+chat model | | Orion | [OrionStar AI series models](https://github.com/
+OrionStarAI) | Chinese
+English | 14B | base model
+chat model | | BlueLM | [VIVO BlueLM large model](https://github.com/vivo-ai-
+lab/BlueLM) | Chinese
+English | 7B | base model
+chat model | | Ziya2 | [Fengshenbang series models](https://github.com/IDEA-
+CCNL/Fengshenbang-LM) | Chinese
+English | 13B | base model
+chat model | | Skywork | [Skywork series models](https://github.com/SkyworkAI/
+Skywork) | Chinese
+English | 13B | base model
+chat model | | Zephyr | Zephyr series models based on Mistral | English | 7B |
+chat model | | PolyLM | [Tongyi Lab self-developed PolyLM series models](https:
+//github.com/DAMO-NLP-MT/PolyLM) | Multilingual | 13B | base model | | SeqGPT |
+[Tongyi Lab self-developed text understanding model for information extraction
+and text classification](https://github.com/Alibaba-NLP/SeqGPT) | Chinese |
+560M | semantic understanding model | | SUS | [Southern University of Science
+and Technology model fine-tuned on YI](https://github.com/SUSTech-IDEA/SUS-
+Chat) | Chinese
+English | 34B | chat model | | Tongyi-Finance | [Tongyi finance series models]
+(https://github.com/QwenLM/Qwen) | Chinese
+English | 14B | base model
+chat model
+financial model | | CodeFuse-CodeLLaMA
+CodeFuse-Codegeex2
+CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai) |
+Chinese
+English | 6B-34B | chat model
+code model | | phi2 | Microsoft's PHI2 model | English | 3B | base model
+code model | | Grok | [X-ai](https://github.com/xai-org/grok-1) | English |
+300B | base model | | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat)
+| Chinese
+English | 7B-12B | chat model | | dbrx | [databricks](https://github.com/
+databricks/dbrx) | English | 132B | base model
+chat model | | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) |
+Chinese
+English | 13B | base model | | c4ai-command-r | [c4ai](https://cohere.com/
+command) | Multilingual | 35B-104B | chat model | #### MLLMs | Model Type |
+Model Introduction | Language | Model Size | Model Type | |------------------|-
+-----------------------------------------------------------------------|-------
+-------------|-------------------|------------------- | | Qwen-VL | [Tongyi
+Qwen vision model](https://github.com/QwenLM) | Chinese
+English | 7B
+including quantized versions | base model
+chat model | | Qwen-Audio | [Tongyi Qwen speech model](https://github.com/
+QwenLM) | Chinese
+English | 7B | base model
+chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
+ai) | Chinese
+English | 6B-34B | chat model | | XComposer2 | [Pujiang AI Lab InternLM vision
+model](https://github.com/InternLM/InternLM) | Chinese
+English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
+(https://github.com/deepseek-ai) | Chinese
+English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
+(https://github.com/OpenBMB/MiniCPM) | Chinese
+English | 3B | chat model | | CogVLM
+CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
+) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
+github.com/haotian-liu/LLaVA) | English | 7B | chat model | #### Diffusion
+Models | Model Type | Model Introduction | Language | Model Type | |-----------
+----------|--------------------------------------------------------------------
+--|----------|------------------ | | AnimateDiff | [AnimateDiff animation
+model](https://github.com/guoyww/AnimateDiff) | English | text-to-video | |
+SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models](https://github.com/
+Stability-AI) | English | text-to-image | ### Supported Open Source Datasets |
+Dataset Type | Training Task | Documentation | |--------------|:---------------
+|--------------------------------------------------------------- | | General |
+Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en
+(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh,
+cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-
+zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-
+gpt4, ð¥sharegpt-gpt4-mini. | | Agent | Fine-tuning | ð¥ms-agent, ms-agent-
+for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh,
+damo-agent-zh, agent-instruct-all-en. | | General | Human Alignment | ð¥hh-
+rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base,
+hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-
+attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-
+harmless-base-en, hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-
+alpaca-en, ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-
+instruction-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-
+mini-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh,
+tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-
+math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en,
+ð¥sql-create-context-en. | | Text Generation | Fine-tuning | ð¥advertise-
+gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh,
+ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | |
+Quantization Assist | Quantization | pileval. | | Other | Fine-tuning |
+finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-
+jave-zh. | | Vision | Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2,
+capcha-images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. |
+### Supported Technologies | Technology Name | |-------------------------------
+-------------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF
+LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
+Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
+2402.12354.pdf) | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
+Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
+Efficient and Controllable Image Diffusion Generation via Skip Connection
+Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
+2312.11392) \| [Project Page](https://scedit.github.io/) > | | ð¥NEFTune:
+[Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/
+2310.05914) | | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large
+Language Models](https://arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient
+Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/
+2309.12307) | | ROME: [Rank-One Editing of Encoder-Decoder Models](https://
+arxiv.org/abs/2211.13317) | | Adapter: [Parameter-Efficient Transfer Learning
+for NLP](http://arxiv.org/abs/1902.00751) | | Prompt Tuning: [Visual Prompt
+Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline
+for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/
+1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
+Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
+[arXiv](https://arxiv.org/abs/2310.19859) \| [Project Page](https://res-
+tuning.github.io/) \| [Usage](docs/source/GetStarted/ResTuning.md) > | | Tuners
+provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA,
+etc. | ### Supported Hardware | Hardware Environment | Notes | |---------------
+-----------------|-------------------------------------------------| | CPU | |
+| RTX 20/30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used |
+| Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | |
+Computing cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend
+NPU | | ## ð Documentation ### Documentation Compiling ```shell make docs #
+Check docs/build/html/index.html in web-browser ``` ### User Guide | Document
+Name | | ------------------------------------------------------------ | |
+[Using Web-UI](docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/
+source_en/GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-
+fine-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | |
+[LLM Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
+(docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
+Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
+Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
+Documentation | Document Name | | ---------------------------------------------
+--------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
+parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
+Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
+Supported-models-datasets.md) | | [Runtime Speed and Memory Benchmark](https://
+github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) | ### Best
+Practices | Best Practices Name | | -------------------------------------------
+----------------- | | [Agent Fine-Tuning Best Practice](https://github.com/
+modelscope/swift/blob/main/docs/source/LLM/
+Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | | [Self-
+Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/
+main/docs/source/LLM/
+%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md)
+| | [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/
+source/LLM/
+Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | |
+[Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/
+blob/main/docs/source/Multi-Modal/index.md) | ### Deep Learning Tutorials |
+Tutorial Name | |-------------------------------------------------------------
+- | | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-
+classroom/blob/main/LLM-tutorial/
+A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
+| | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
+blob/main/LLM-tutorial/
+B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
+| | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
+blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
+prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+D.Transformer%E7%BB%93%E6%9E%84.md) | | [Training Technique Selection](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+E.%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B.md) | | [Data Preprocessing](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+F.%E6%95%B0%E6%8D%AE%E9%A2%84%E5%A4%84%E7%90%86.md) | | [Quantization](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+G.%E9%87%8F%E5%8C%96.md) | | [Training](https://github.com/modelscope/
+modelscope-classroom/blob/main/LLM-tutorial/H.%E8%AE%AD%E7%BB%83.md) | |
+[Inference](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-
+tutorial/
+I.LLM%E5%92%8C%E5%A4%9A%E6%A8%A1%E6%80%81%E6%A8%A1%E5%9E%8B%E9%AB%98%E6%95%88%E6%8E%A8%E7%90%86%E5%AE%9E%E8%B7%B5.md)
+| | [Deployment](https://github.com/modelscope/modelscope-classroom/blob/main/
+LLM-tutorial/J.%E9%83%A8%E7%BD%B2.md) | | [Evaluation](https://github.com/
+modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98-
+-LLM%20Automatic%20Evaluation.md) | ## ð License This framework is licensed
+under the [Apache License (Version 2.0)](https://github.com/modelscope/
+modelscope/blob/master/LICENSE). For models and datasets, please refer to the
+original resource page and follow the corresponding License. ## ð Citation
+```bibtex @Misc{swift, title = {SWIFT:Scalable lightWeight Infrastructure for
+Fine-Tuning}, author = {The ModelScope Team}, howpublished = {\url{https://
+github.com/modelscope/swift}}, year = {2024} } ``` ## â Contact Us You can
+contact us and communicate with us by adding our WeChat group:
 [asset/wechat.png]
 ## Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/
-swift&Date) Keywords: python,petl,efficient tuners Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: llm Provides-Extra: aigc Provides-Extra: all
+swift&Date)
```

### Comparing `ms-swift-1.7.3/ms_swift.egg-info/PKG-INFO` & `ms-swift-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,528 +1,574 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 1.7.3
+Version: 2.0.0
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
         <p align="center">
             <br>
-            <img src="https://modelscope.oss-cn-beijing.aliyuncs.com/modelscope.gif" width="400"/>
+            <img src="resources/banner.png"/>
             <br>
         <p>
         <p align="center">
-        <a href="https://modelscope.cn/home">ModelScope Community</a>
+        <a href="https://modelscope.cn/home">ModelScope Community Website</a>
         <br>
-                <a href="README_CN.md">中文</a>&nbsp ｜ &nbspEnglish&nbsp ｜ &nbsp<a href="https://github.com/modelscope/swift/blob/main/docs/source/GetStarted/%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8.md">Docs</a>
+                <a href="README_CN.md">中文</a> &nbsp ｜ &nbsp English &nbsp
         </p>
         
-        
         <p align="center">
         <img src="https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg">
         <img src="https://img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg">
         <a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
         <a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
         <a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
         <a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
         <a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
         </p>
         
         ## 📖 Table of Contents
         - [Introduction](#-introduction)
         - [News](#-news)
-        - 🔥[LLM Training and Inference](#-llm-training-and-inference)
-        - 🔥[SCEdit Tuner](#-SCEdit)
-        - [Installation](#-installation)
+        - [Installation](#%EF%B8%8F-installation)
         - [Getting Started](#-getting-started)
-        - [Learn More](#-learn-more)
-        - [License](#license)
+        - [Documentation](#-documentation)
+        - [License](#-License)
+        - [Citation](#-citation)
         - [Contact Us](#-contact-us)
         
         ## 📝 Introduction
-        SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning) is an extensible framework designed to facilitate lightweight model fine-tuning and inference. It integrates implementations for various efficient fine-tuning methods,  by embracing approaches that is parameter-efficient, memory-efficient, and time-efficient. SWIFT integrates seamlessly into ModelScope ecosystem and offers the capabilities to finetune various models, with a primary emphasis on LLMs and vision models. Additionally, SWIFT is fully compatible with [PEFT](https://github.com/huggingface/peft), enabling users to  leverage the familiar Peft interface to finetune ModelScope models.
-        
-        Currently supported approaches (and counting):
-        
-        1. 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
-        2. 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf)
-        3. 🔥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf)
-        4. 🔥SCEdit: [SCEdit: Efficient and Controllable Image Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/2312.11392)  < [arXiv](https://arxiv.org/abs/2312.11392)  |  [Project Page](https://scedit.github.io/) >
-        5. 🔥NEFTune: [Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914)
-        6. QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2309.14717).
-        7. LongLoRA: [Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
-        8. ROME: [Rank-One Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317)
-        9. Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/1902.00751)
-        10. Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/2203.12119)
-        11. Side: [Side-Tuning: A Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503)
-        12. Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859)  < [arXiv](https://arxiv.org/abs/2310.19859)  |  [Project Page](https://res-tuning.github.io/)  |  [Usage](docs/source/GetStarted/ResTuning.md) >
-        13. All tuners offered on [PEFT](https://github.com/huggingface/peft), like IA3, AdaLoRA
-        
-        Key features:
-        
-        1. By integrating the ModelScope library, models can be readily obtained via a model-id.
-        2. Tuners provided by SWIFT can be combined to allow exploration of multiple tuners on a model for best result.
-        3. Support calling `activate_adapter` or `deactivate_adapter` or `set_active_adapters`  to activate/deactivate tuners. User can inference with one model and multiple tuners in different threads independently.
-        4. Support training and inference with scripts/CLI，meanwhile support inference with Web-UI.
-        5. Support model deployment(vllm/chatglm.cpp/xinference)，Check [Official documentation](./docs/source/GetStarted/部署指南.md) for details.
+        SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
-        Users can check the [documentation of SWIFT](docs/source/GetStarted/快速使用.md) to get detail tutorials.
+        To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
+        Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
         ## 🎉 News
-        - 🔥2024.03.12: Supports inference and fine-tuning for the **deepseek-vl** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/deepseek-vl最佳实践.md).
-        - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507), which can efficiently reduce the memory usage(almost half of the original memory) when training the full model.
-        - 🔥2024.03.10: For the end-to-end best practice of fine-tuning to deployment of Qwen1.5-7B-Chat and Qwen1.5-72B-Chat, you can refer to the [Qwen1.5 Full Workflow Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md).
-        - 🔥2024.03.09: Support training and inference of MAMBA series, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to begin.
-        - 2024.03.09: Support training and inference of AQLM quantized models, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to begin.
-        - 2024.03.06: Support training and inference of AWQ quantized models, use [this Qwen1.5-AWQ script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to begin, support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
-        - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to begin.
-        - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to begin.
-        - 2024.02.25: Support `swift export` to export models for **AWQ/GPTQ** quantization and push to ModelScope Hub. For more details, please refer to the document: [LLM Quantization Document](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E9%87%8F%E5%8C%96%E6%96%87%E6%A1%A3.md).
+        - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
+        - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
+        - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+        - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train.
+        - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
+        - 🔥2024.04.09: Support ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/Supported-models-datasets.md) to begin training!
+        - 2024.04.08: Support the fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/xverse_moe_a4_2b/lora/sft.sh) to start training!
+        - 2024.04.04: Support **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_70b_chat/qlora_fsdp/sft.sh) to train.
+        - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
+        - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
+        - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
+        - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
+        - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
+        - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
+        - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/llava最佳实践.md).
+        - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
+        - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
+        - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
+        - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
+        - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
+        - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
+        - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
+        - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start training.
+        - 2024.02.25: Support `swift export` to quantize models using **AWQ/GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/source_en/LLM/LLM-quantization.md).
+        <details><summary>More</summary>
+        
         - 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
         - 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
-        - 🔥2024.02.05: Support **Qwen1.5** series, To view all supported Qwen1.5 models please check [Model List](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B). The [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8) fine-tuned scripts are provided.
-        - 2024.02.05: Support the training of **SDXL**, **SD**, **ControlNet**, or techniques like **DreamBooth**, you can check the [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
+        - 🔥2024.02.05: Support **Qwen1.5** series models, see [model list](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B) for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8).
+        - 2024.02.05: Support training of diffusion models such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training. See corresponding [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
         - 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
-        - 🔥2024.02.01: Support dataset mixture to reduce **Catastrophic Forgetting**. Use `--train_dataset_mix_ratio 2.0` to train! We also provide a common knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
-        - 🔥2024.02.01: Support Agent training! Agent training algorithm comes from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also introduce the [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary) dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to begin an agent training!
-        - 🔥2024.02.01: Support SFT loss to DPO training to reduce the repeat generation problem caused by the KL-divergence loss.
-        - 2024.02.01: Support AdaLoRA and IA3 adapter in SFT.
-        - 2024.02.01: Support `--merge_lora` in AnimateDiff training.
-        <details><summary>More</summary>
-        
+        - 🔥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**. Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
+        - 🔥2024.02.01: Support Agent training! Agent training algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary), a high-quality agent dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to start Agent training!
+        - 🔥2024.02.01: Support adding SFT loss in DPO training to reduce repetitive generation caused by KL divergence loss.
+        - 2024.02.01: Support using AdaLoRA and IA3 adapters in training.
+        - 2024.02.01: Support `--merge_lora` parameter in AnimateDiff training.
         - 2024.01.30: Support [internlm-xcomposer2-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm_xcomposer2_7b_chat).
-        - 🔥2024.01.30: Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), just need to specify `--deepspeed default-zero3`.
+        - 🔥2024.01.30: Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), simply specify `--deepspeed default-zero3`.
         - 2024.01.29: Support internlm2-math series: internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat.
         - 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
         - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
         - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
         - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
-        - 🔥2024.01.17: Support **internlm2** series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
-        - 2024.1.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
+        - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
+        - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
         - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
-        - 🔥2024.01.04: Support for **VLLM deployment**, compatible with the **OpenAI API** style. For more details, please refer to [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署)
-        - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) to facilitate viewing the training speed and GPU memory required for different models.
-        - 🔥 2023.12.29: Support web-ui for training and inference, use `swift web-ui` after the installation of ms-swift.
-        - 🔥 2023.12.29: Support DPO RLHF(Reinforcement Learning from Human Feedback) and three datasets: AI-ModelScope/stack-exchange-paired and AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn for this task. Check [this documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
-        - 🔥 2023.12.28: Support SCEdit! This framework can easily reduce memory usage in training and inference, and replace ControlNet for controllable image generating scenarios, view the following chapter for details.
+        - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署) for details.
+        - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
+        - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
+        - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
+        - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
         - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
         - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
-        - 2023.12.18: Support for VLLM for inference acceleration.
+        - 2023.12.18: Support VLLM for inference acceleration.
         - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-        - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b_instruct).
-        - 2023.12.09: Support the `freeze_parameters` parameter as a compromise between LoRA and full parameter. Corresponding shell scripts can be found at [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, for details please refer to [Command-Line parameters](https://github.com/modelscope/swift/blob/main/docs/source/LLM/命令行参数.md).
+        - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct).
+        - 2023.12.09: Support `freeze_parameters` parameter as a compromise between lora and full-parameter training. Corresponding sh can be found in [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, see [command line arguments](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details.
         - 2023.12.08: Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k.
         - 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E5%BE%AE%E8%B0%83%E6%96%87%E6%A1%A3.md#%E4%BD%BF%E7%94%A8cli).
-        - 2023.12.04: Supported models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat. Supported datasets: hc3-zh, hc3-en.
-        - 🔥 2023.12.02: [Best Practice for Self-cognition Fine-tuning](https://github.com/modelscope/swift/blob/main/docs/source/LLM/自我认知微调最佳实践.md), **10 minutes for self-cognition fine-tuning for LLM**, creating a LLM that is specific to oneself.
-        - 🔥 2023.11.30: Support for training and inference of the **qwen-1_8b**, **qwen-72b**, and **qwen-audio** model series. The corresponding shell scripts can be viewed at [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_audio_chat).
-        - 🔥 2023.11.29: Support the training and inference for **AnimateDiff**
-        - 🔥 2023.11.24: Support for **yi-34b-chat**, **codefuse-codellama-34b-chat**: The corresponding shell script can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codefuse_codellama_34b_chat).
-        - 🔥 2023.11.18: Support for **tongyi-finance-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4. The corresponding shell script can be found in [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4).
-        - 2023.11.16: Added support for more models in **flash attn**: qwen series, qwen-vl series, llama series, openbuddy series, mistral series, yi series, ziya series. Please use the `use_flash_attn` parameter.
-        - 🔥 2023.11.11: **NEFTune** Supported, Use is with `Swift.prepare_model(model, NEFTuneConfig())`
-        - 🔥 2023.11.11: Support training and inference with **CLI**, and inference with **Web-UI**. Check the [Run using Swift CLI](https://github.com/modelscope/swift/tree/main#run-using-swift-cli) chapter for details.
-        - 🔥 2023.11.11: Support model **deployment**(vllm/chatglm.cpp/xinference)，Check [Official documentation](./docs/source/GetStarted/部署指南.md) for details.
-        - 🔥 2023.11.10: Support for **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. The corresponding shell script can be found in [bluelm_7b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/bluelm_7b_chat).
-        - 🔥 2023.11.08: Support the finetuning of **xverse-65b** model, scripts can be found at: [xverse_65b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_65b).
-        - 🔥 2023.11.07: Support the finetuning of **yi-6b**, **yi-34b** model, scripts can be found at: [yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b).
-        - 🔥 2023.10.30: Support **QA-LoRA** and **LongLoRA** to decrease memory usage in training.
-        - 🔥 2023.10.30: Support **ROME**(Rank One Model Editing) to add/modify knowledges, training is not needed!
-        - 2023.10.30: Support for **skywork-13b** series models: skywork-13b, skywork-13b-chat. The corresponding shell script can be found in [skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/skywork_13b).
-        - 🔥 2023.10.27: Support for **chatglm3** series models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. The corresponding shell script can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b).
-        - 🔥 2023.10.17: Supported **int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8.
-        - 2023.10.15: Supported **ziya2-13b** model series: ziya2-13b, ziya2-13b-chat.
-        - 2023.10.12: Supported **mistral-7b** model series: openbuddy-mistral-7b-chat, mistral-7b, mistral-7b-instruct.
-        - 🔥 2023.10.07: Supported **DeepSpeed ZeRO-2**, enabling LoRA (not just QLoRA) to run DDP on 2*A10.
-        - 2023.10.04: Supported datasets in the fields of mathematics, law, SQL, and coding: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en.
-        - 🔥 2023.09.25: Supported **qwen-14b** model series: qwen-14b, qwen-14b-chat.
-        - 2023.09.18: Supported **internlm-20b** model series: internlm-20b, internlm-20b-chat.
-        - 2023.09.12: Supported training with **MP+DDP** to accelerate full-parameter fine-tuning speed.
-        - 2023.09.05: Supported **openbuddy-llama2-70b-chat** model.
-        - 2023.09.03: Supported **baichuan2** model series: baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat.
+        - 2023.12.05: Support models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat. Support datasets: hc3-zh, hc3-en.
+        - 🔥2023.12.02: [Self-cognition fine-tuning best practices](docs/source_en/LLM/Self-cognition-best-practice.md), **10 minutes to fine-tune a large model for self-cognition**, create your own unique large model.
+        - 🔥2023.11.30: Support training and inference of **qwen-1_8b**, **qwen-72b**, **qwen-audio** series models. Corresponding sh scripts can be found in [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_audio_chat)
+        - 🔥2023.11.29: Support training and inference of **AnimateDiff**
+        - 🔥2023.11.24: Support **yi-34b-chat**, **codefuse-codellama-34b-chat** models. Corresponding sh scripts can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codefuse_codellama_34b_chat).
+        - 🔥2023.11.18: Support **tongyi-finance-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4. Corresponding sh scripts can be found in [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4).
+        - 2023.11.16: Support **flash attn** for more models: qwen series, qwen-vl series, llama series, openbuddy series, mistral series, yi series, ziya series. Please use `use_flash_attn` parameter.
+        - 🔥2023.11.11: Support **NEFTune**, simply use `Swift.prepare_model(model, NEFTuneConfig())` to enable.
+        - 🔥2023.11.11: Support training and inference by **command line** and inference by **Web-UI**, see `Usage with Swift CLI` section below for details.
+        - 🔥2023.11.10: Support **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. Corresponding sh scripts can be found in [bluelm_7b_chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/bluelm_7b_chat).
+        - 🔥2023.11.08: Support training and inference of **xverse-65b** model, script at [xverse_65b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_65b).
+        - 🔥2023.11.07: Support training and inference of **yi-6b**, **yi-34b** models, scripts at [yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b).
+        - 🔥2023.10.30: Support two new tuners: **QA-LoRA** and **LongLoRA**.
+        - 🔥2023.10.30: Support editing models using **ROME** (Rank One Model Editing) to infuse new knowledge into models without training!
+        - 2023.10.30: Support **skywork-13b** series models: skywork-13b, skywork-13b-chat. Corresponding sh scripts can be found in [skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/skywork_13b).
+        - 🔥2023.10.27: Support **chatglm3** series models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. Corresponding sh scripts can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b).
+        - 🔥2023.10.17: Support SFT of **int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8.
+        - 2023.10.15: Support **ziya2-13b** series models: ziya2-13b, ziya2-13b-chat.
+        - 2023.10.12: Support **mistral-7b** series models: openbuddy-mistral-7b-chat, mistral-7b, mistral-7b-instruct.
+        - 🔥2023.10.07: Support **DeepSpeed ZeRO-2**, enabling lora (not just qlora) to run DDP on dual A10 cards.
+        - 2023.10.04: Support more math, law, SQL, code domain datasets: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en.
+        - 🔥2023.09.25: Support **qwen-14b** series: qwen-14b, qwen-14b-chat.
+        - 2023.09.18: Support **internlm-20b** series: internlm-20b, internlm-20b-chat.
+        - 2023.09.12: Support **MP+DDP** to accelerate full-parameter training.
+        - 2023.09.05: Support **openbuddy-llama2-70b-chat**.
+        - 2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat.
         </details>
         
+        ## 🛠️ Installation
         
-        ## ✨ LLM Training and Inference
-        If you want to learn more about **best practices** for LLM or multimodal LLM, or if you are interested in **tutorials** on inference, fine-tuning, quantization, and deployment of LLM, you can refer to the [LLM series documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/index.md).
-        
-        
-        ### WEB UI training and inference
+        SWIFT runs in the Python environment. Please ensure your Python version is higher than 3.8.
         
-        After installation, you can use web-ui training/inference like:
+        - Method 1: Install SWIFT using pip command:
         
         ```shell
-        SWIFT_UI_LANG=en swift web-ui
+        # Full capabilities
+        pip install ms-swift[all] -U
+        # LLM only
+        pip install ms-swift[llm] -U
+        # AIGC only
+        pip install ms-swift[aigc] -U
+        # Adapters only
+        pip install ms-swift -U
         ```
         
-        > Supported environment variables:
-        >
-        > WEBUI_SHARE=1 Share the gradio or not
-        > SWIFT_UI_LANG=en/zh The language of radio
-        > WEBUI_SERVER server_name， web-ui host ip，0.0.0.0 means all routes are allowed，127.0.0.1 means only localhost can visit the web
-        > WEBUI_PORT The port of web-ui
-        
-        Here is a simple introduction of web-ui:
-        
-        [![Watch the video](docs/source/cources/resources/20240119160942.jpg)](https://modelscope-open.oss-cn-hangzhou.aliyuncs.com/SWIFT%E8%A7%86%E9%A2%91_%E8%B0%83%E6%95%B4%E5%B0%81%E9%9D%A2.mp4)
+        - Method 2: Install SWIFT through source code (convenient for running training and inference scripts), please run the following commands:
         
+        ```shell
+        git clone https://github.com/modelscope/swift.git
+        cd swift
+        pip install -e .[llm]
+        ```
         
-        ### Quick Start
-        You can test if the environment is installed correctly by running the following code.
-        ```python
-        # pip install ms-swift[llm] -U
+        SWIFT depends on torch>=1.13, recommend torch>=2.0.0.
         
-        # Experimental environment: A10, 3090, V100, ...
-        # 8GB GPU memory
-        import os
-        os.environ['CUDA_VISIBLE_DEVICES'] = '0'
+        - Method 3: Use SWIFT in our Docker image
         
-        import torch
+        ```shell
+        # China-Hangzhou image
+        docker pull registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1
+        # US-west image
+        docker pull registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1
+        ```
         
-        from swift.llm import (
-            DatasetName, InferArguments, ModelType, SftArguments,
-            infer_main, sft_main, app_ui_main, merge_lora
-        )
+        ## 🚀 Getting Started
         
-        model_type = ModelType.qwen1half_0_5b
-        sft_args = SftArguments(
-            model_type=model_type,
-            train_dataset_sample=2000,
-            dataset=[DatasetName.jd_sentiment_zh],
-            output_dir='output')
-        result = sft_main(sft_args)
-        best_model_checkpoint = result['best_model_checkpoint']
-        print(f'best_model_checkpoint: {best_model_checkpoint}')
-        torch.cuda.empty_cache()
+        This section introduces basic usage, see the [Documentation](#-documentation) section for more ways to use.
         
-        infer_args = InferArguments(
-            ckpt_dir=best_model_checkpoint,
-            load_dataset_config=True,
-            val_dataset_sample=10)
-        merge_lora(infer_args, device_map='cpu')
-        result = infer_main(infer_args)
-        torch.cuda.empty_cache()
+        ### Web-UI
         
-        app_ui_main(infer_args)
+        ```shell
+        swift web-ui
         ```
         
-        ### Training Scripts
+        ### Training
+        
+        #### Training Scripts
         You can refer to the following scripts to customize your own training script.
         
         - full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
         - full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
         - full+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3) (4\*A100)
         - lora: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_mp) (2\*A100)
         - lora+ddp: [chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp) (2\*3090)
         - lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3) (4\*3090), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100)
         - qlora(gptq-int4): [qwen-7b-chat-int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat_int4/qlora) (3090)
         - qlora(gptq-int8): [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8/qlora) (3090)
         - qlora(bnb-int4): [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/qlora) (3090)
         
         
-        ### Features
-        - Supported SFT Methods: [lora](https://arxiv.org/abs/2106.09685), [qlora](https://arxiv.org/abs/2305.14314), [longlora](https://arxiv.org/abs/2309.12307), [qalora](https://arxiv.org/abs/2309.14717), full parameter fine-tuning, partial parameter fine-tuning.
-        - Supported Features: quantization, DDP, model parallelism, gradient checkpointing, pushing to modelscope hub, custom datasets, multimodal and agent SFT, mutli-round chat, DPO, self-cognition fine-tuning, ...
-        - Supported Models: [[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
-          - Multi-Modal:
-            - [qwen-vl](https://github.com/QwenLM/Qwen-VL) series: qwen-vl, qwen-vl-chat, qwen-vl-chat-int4.
-            - [qwen-audio](https://github.com/QwenLM/Qwen-Audio) series: qwen-audio, qwen-audio-chat.
-            - [deepseek-vl](https://github.com/deepseek-ai/DeepSeek-VL) series: deepseek-vl-1_3b-chat, deepseek-vl-7b-chat.
-            - [yi-vl](https://github.com/01-ai/Yi) series: yi-vl-6b-chat, yi-vl-34b-chat.
-            - [internlm-xcomposer2](https://github.com/InternLM/InternLM-XComposer) series: internlm-xcomposer2-7b-chat.
-            - [minicpm-v](https://github.com/OpenBMB/MiniCPM) series: minicpm-v-3b-chat.
-            - [cogvlm](https://github.com/THUDM/CogVLM) series: cogvlm-17b-instruct, cogagent-18b-chat, cogagent-18b-instruct.
-          - General:
-            - [qwen](https://github.com/QwenLM/Qwen) series:
-              - qwen-1_8b, qwen-1_8b-chat, qwen-1_8b-chat-int4, qwen-1_8b-chat-int8.
-              - qwen-7b, qwen-7b-chat, qwen-7b-chat-int4, qwen-7b-chat-int8.
-              - qwen-14b, qwen-14b-chat, qwen-14b-chat-int4, qwen-14b-chat-int8.
-              - qwen-72b, qwen-72b-chat, qwen-72b-chat-int4, qwen-72b-chat-int8.
-            - [qwen1.5](https://github.com/QwenLM/Qwen1.5) series:
-              - qwen1half-0_5b, qwen1half-0_5b-chat, qwen1half-0_5b-chat-int4, qwen1half-0_5b-chat-int8, qwen1half-0_5b-chat-awq.
-              - qwen1half-1_8b, qwen1half-1_8b-chat, qwen1half-1_8b-chat-int4, qwen1half-1_8b-chat-int8, qwen1half-1_8b-chat-awq.
-              - qwen1half-4b, qwen1half-4b-chat, qwen1half-4b-chat-int4, qwen1half-4b-chat-int8, qwen1half-4b-chat-awq.
-              - qwen1half-7b, qwen1half-7b-chat, qwen1half-7b-chat-int4, qwen1half-7b-chat-int8, qwen1half-7b-chat-awq.
-              - qwen1half-14b, qwen1half-14b-chat, qwen1half-14b-chat-int4, qwen1half-14b-chat-int8, qwen1half-14b-chat-awq.
-              - qwen1half-72b, qwen1half-72b-chat, qwen1half-72b-chat-int4, qwen1half-72b-chat-int8, qwen1half-72b-chat-awq.
-            - [chatglm](https://github.com/THUDM/ChatGLM-6B) series: chatglm2-6b, chatglm2-6b-32k, chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k.
-            - [llama](https://github.com/facebookresearch/llama) series: llama2-7b, llama2-7b-chat, llama2-13b, llama2-13b-chat, llama2-70b, llama2-70b-chat.
-            - [yi](https://github.com/01-ai/Yi) series: yi-6b, yi-6b-200k, yi-6b-chat, yi-9b, yi-34b, yi-34b-200k, yi-34b-chat.
-            - [internlm](https://github.com/InternLM/InternLM) series:
-              - internlm-7b, internlm-7b-chat, internlm-7b-chat-8k, internlm-20b, internlm-20b-chat.
-              - internlm2-1_8b, internlm2-1_8b-sft-chat, internlm2-1_8b-chat, internlm2-7b-base, internlm2-7b, internlm2-7b-sft-chat, internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
-            - [deepseek](https://github.com/deepseek-ai/deepseek-LLM) series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, deepseek-moe-16b, deepseek-moe-16b-chat.
-            - [gemma](https://github.com/google/gemma_pytorch) series: gemma-2b, gemma-2b-instruct, gemma-7b, gemma-7b-instruct.
-            - [minicpm](https://github.com/OpenBMB/mlc-MiniCPM) series: minicpm-2b-sft-chat, minicpm-2b-chat.
-            - [openbuddy](https://github.com/OpenBuddy/OpenBuddy) series: openbuddy-llama2-13b-chat, openbuddy-llama-65b-chat, openbuddy-llama2-70b-chat, openbuddy-mistral-7b-chat, openbuddy-zephyr-7b-chat, openbuddy-deepseek-67b-chat, openbuddy-mixtral-moe-7b-chat.
-            - [mistral](https://github.com/mistralai/mistral-src) series: mistral-7b, mistral-7b-instruct, mistral-7b-instruct-v2.
-            - [mixtral](https://github.com/mistralai/mistral-src) series: mixtral-moe-7b, mixtral-moe-7b-instruct.
-            - [baichuan](https://github.com/baichuan-inc/Baichuan2) series: baichuan-7b, baichuan-13b, baichuan-13b-chat, baichuan2-7b, baichuan2-7b-chat, baichuan2-13b, baichuan2-13b-chat, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4.
-            - [yuan](https://github.com/IEIT-Yuan/Yuan-2.0) series: yuan2-2b-instruct, yuan2-2b-janus-instruct, yuan2-51b-instruct, yuan2-102b-instruct.
-            - [xverse](https://github.com/xverse-ai/XVERSE-13B) series: xverse-7b, xverse-7b-chat, xverse-13b, xverse-13b-chat, xverse-65b, xverse-65b-v2, xverse-65b-chat, xverse-13b-256k.
-            - [orion](https://github.com/OrionStarAI/OrionStar-Yi-34B-Chat) series: orion-14b, orion-14b-chat.
-            - [bluelm](https://github.com/vivo-ai-lab/BlueLM) series: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k.
-            - [zephyr](https://github.com/huggingface/alignment-handbook) series: zephyr-7b-beta-chat.
-            - [ziya](https://github.com/IDEA-CCNL/Fengshenbang-LM) series: ziya2-13b, ziya2-13b-chat.
-            - [skywork](https://github.com/SkyworkAI/Skywork) series: skywork-13b, skywork-13b-chat.
-            - other: [polylm-13b](https://github.com/DAMO-NLP-MT/PolyLM), [seqgpt-560m](https://github.com/Alibaba-NLP/SeqGPT), [sus-34b-chat](https://github.com/SUSTech-IDEA/SUS-Chat).
-          - Financial:
-            - [tongyi-finance](https://github.com/QwenLM/Qwen) series: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-chat-int4.
-          - Coding:
-            - [codefuse](https://github.com/codefuse-ai) series: codefuse-codellama-34b-chat, codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
-            - [deepseek-coder](https://github.com/deepseek-ai/DeepSeek-Coder) series: deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-            - [codegeex2](https://github.com/THUDM/CodeGeeX2) series: codegeex2-6b.
-            - [phi](https://www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-language-models/) series: phi2-3b.
-          - Math:
-            - [internlm2-math](https://github.com/InternLM/InternLM-Math) series: internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat.
-            - [deepseek-math](https://github.com/deepseek-ai/DeepSeek-Math) series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
-        - Supported Datasets: [[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%95%B0%E6%8D%AE%E9%9B%86)
-          - NLP:
-            - General: 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini.
-            - Agent: 🔥ms-agent, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.
-            - RLHF: 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.
-            - Coding: code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.
-            - Medical: medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.
-            - Law: lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.
-            - Math: 🔥blossom-math-zh, school-math-zh, open-platypus-en.
-            - SQL: text2sql-en, 🔥sql-create-context-en.
-            - Text Generation: 🔥advertise-gen-zh, 🔥dureader-robust-zh.
-            - Classification: cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.
-            - AWQ: pileval.
-            - Other: finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.
-          - Multi-Modal:
-            - Vision: coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.
-            - Audio: aishell1-zh, 🔥aishell1-mini-zh.
-          - Custom Dataset
-        - Supported Templates:
-          - Text Generation: default-generation, default-generation-bos, chatglm-generation, qwen-audio-generation.
-          - Chat: default, qwen, qwen-audio, baichuan, chatglm2, chatglm3, llama, openbuddy, internlm, internlm2, internlm-xcomposer2, yi, yi-vl, yuan, xverse, ziya, skywork, bluelm, zephyr, sus, deepseek, deepseek-coder, codefuse-codellama, codefuse, cogvlm-instruct, cogagent-chat, cogagent-instruct, orion, minicpm, minicpm-v, gemma, chatml.
-        
-        
-        ## 🔥SCEdit
-        
-        SCEdit is an efficient generative fine-tuning framework proposed by Alibaba TongYi Vision Intelligence Lab. This framework enhances the fine-tuning capabilities for text-to-image generation downstream tasks and enables quick adaptation to specific generative scenarios, **saving 30%-50% of training memory costs compared to LoRA**. Furthermore, it can be directly extended to controllable image generation tasks, **requiring only 7.9% of the parameters that ControlNet needs for conditional generation and saving 30% of memory usage**. It supports various conditional generation tasks including edge maps, depth maps, segmentation maps, poses, color maps, and image completion.
-        
-        We using 3D style data from the [style transfer dataset](https://modelscope.cn/datasets/damo/style_custom_dataset/dataPeview) for training, and testing with the same `Prompt: A boy in a camouflage jacket with a scarf`. The qualitative and quantitative results are as follows:
-        
-        | Method    | bs   | ep   | Target Module | Param. (M)    | Mem. (MiB) | 3D style                                                     |
-        | --------- | ---- | ---- | ------------- | ------------- | ---------- | ------------------------------------------------------------ |
-        | LoRA/r=64 | 1    | 50   | q/k/v/out/mlp | 23.94 (2.20%) | 8440MiB    | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703665229562-0f33bbb0-c492-41b4-9f37-3ae720dca80d.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 1    | 50   | up_blocks     | 19.68 (1.81%) | 7556MiB    | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703665933913-74b98741-3b57-46a4-9871-539df3a0112c.png" alt="img" style="zoom:20%;" /> |
-        | LoRA/r=64 | 10   | 100  | q/k/v/out/mlp | 23.94 (2.20%) | 26300MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703750608529-de20d0e7-bf9c-4928-8e59-73cc54f2c8d7.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 10   | 100  | up_blocks     | 19.68 (1.81%) | 18634MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703663033092-94492e44-341f-4259-9df4-13c168e3b5d6.png" alt="img" style="zoom:20%;" /> |
-        | LoRA/r=64 | 30   | 200  | q/k/v/out/mlp | 23.94 (2.20%) | 69554MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703750626635-2e368d7b-5e99-4a06-b189-8615f302bcd7.png" alt="img" style="zoom:20%;" /> |
-        | SCEdit    | 30   | 200  | up_blocks     | 19.68 (1.81%) | 43350MiB   | <img src="https://intranetproxy.alipay.com/skylark/lark/0/2023/png/167218/1703662246942-1102b1f4-93ab-4653-b943-3302f2a5259e.png" alt="img" style="zoom:20%;" /> |
-        
-        The benchmark listed above can be reproduced by：
-        
-        ```shell
-        # Install swift by the next chapter
-        cd examples/pytorch/multi_modal/notebook
-        python text_to_image_synthesis.py
-        ```
+        #### Supported Training Processes
         
+        | Training Process | Training Method                                                               |
+        |------------------|-------------------------------------------------------------------------------|
+        | Pretraining      | Text Generation                                                               |
+        | Fine-tuning      | Single-turn/Multi-turn<br>Agent Training/Self-cognition<br>Multi-modal Vision/Multi-modal Speech|
+        | Human Alignment  | DPO                                                                           |
+        | Text-to-Image    | DreamBooth, etc.                                                              |
+        | Text-to-Video    | -                                                                             |
         
-        ## 🛠️ Installation
+        #### Single GPU Training
         
-        SWIFT is running in Python environment. Please make sure your python version is higher than 3.8.
-        
-        - Install SWIFT by the `pip` command:
+        Start single GPU fine-tuning with the following command:
         
+        LoRA:
         ```shell
-        # full ability
-        pip install ms-swift[all] -U
-        # only use llm
-        pip install ms-swift[llm] -U
-        # only use aigc
-        pip install ms-swift[aigc] -U
-        # only use adapters
-        pip install ms-swift -U
+        # Experimental Environment: A100
+        # GPU Memory Requirement: 20GB
+        # Runtime: 3.1 hours
+        CUDA_VISIBLE_DEVICES=0 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
+            --eval_steps 200 \
         ```
         
-        - Install SWIFT by source code(for running sft/infer examples), please run:
-        
+        Full-parameter:
         ```shell
-        git clone https://github.com/modelscope/swift.git
-        cd swift
-        pip install -e .[llm]
+        # Experimental Environment: A100
+        # GPU Memory Requirement: 80GB
+        # Runtime: 2.5 hours
+        CUDA_VISIBLE_DEVICES=0 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type full \
+            --output_dir output \
+            --eval_steps 500 \
         ```
         
-        SWIFT requires torch>=1.13.
         
-        - Use SWIFT in our docker image:
+        #### Model Parallel Training
+        
         
         ```shell
-        docker pull registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu20.04-cuda11.8.0-py38-torch2.0.1-tf2.13.0-1.9.1
+        # Experimental Environment: 2 * A100
+        # GPU Memory Requirement: 10GB + 13GB
+        # Runtime: 3.4 hours
+        CUDA_VISIBLE_DEVICES=0,1 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
         ```
         
-        ## 🚀 Getting Started
-        
-        SWIFT supports multiple tuners, as well as tuners provided by [PEFT](https://github.com/huggingface/peft). To use these tuners, simply call:
+        #### Data Parallel Training
         
-        ```python
-        from swift import Swift, LoRAConfig
-        config = LoRAConfig(...)
-        model = Swift.prepare_model(model, config, extra_state_keys=['...'])
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 4 * 30GB
+        # Runtime: 0.8 hours
+        NPROC_PER_NODE=4 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
         ```
         
-        The code snippet above initialized the tuner randomly. The input model is an instance of `torch.nn.Module`, the config is a subclass instance of `SwiftConfig` or `PeftConfig`. extra_state_keys is
-        the extra module weights(like the linear head) to be trained and stored in the output dir.
-        
-        You may combine multiple tuners by:
-        
-        ```python
-        from swift import Swift, LoRAConfig, PromptConfig
-        model = Swift.prepare_model(model, {'lora': LoRAConfig(...), 'prompt': PromptConfig(...)})
+        Combining Model Parallelism and Data Parallelism:
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 2*14GB + 2*18GB
+        # Runtime: 1.7 hours
+        NPROC_PER_NODE=2 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
         ```
         
-        Call `save_pretrained` and `push_to_hub` after finetuning:
+        #### Deepspeed Training
         
-        ```python
-        from swift import push_to_hub
-        model.save_pretrained('some-output-folder')
-        push_to_hub('my-group/some-repo-id-modelscope', 'some-output-folder', token='some-ms-token')
+        ZeRO2:
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 4 * 21GB
+        # Runtime: 0.9 hours
+        NPROC_PER_NODE=4 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
+            --deepspeed default-zero2 \
         ```
-        Assume `my-group/some-repo-id-modelscope` is the model-id in the hub, and `some-ms-token` is the token for uploading.
         
-        Using the model-id to do later inference:
-        
-        ```python
-        from swift import Swift
-        model = Swift.from_pretrained(model, 'my-group/some-repo-id-modelscope')
+        ZeRO3:
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 4 * 19GB
+        # Runtime: 3.2 hours
+        NPROC_PER_NODE=4 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_type qwen1half-7b-chat \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
+            --deepspeed default-zero3 \
         ```
         
-        Here shows a runnable example:
-        
-        ```python
-        import os
-        import tempfile
-        
-        # Please install modelscope by `pip install modelscope`
-        from modelscope import Model
-        
-        from swift import LoRAConfig, SwiftModel, Swift, push_to_hub
-        
-        tmp_dir = tempfile.TemporaryDirectory().name
-        if not os.path.exists(tmp_dir):
-            os.makedirs(tmp_dir)
-        
-        
-        model = Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto')
-        lora_config = LoRAConfig(target_modules=['q_proj', 'k_proj', 'v_proj'])
-        model: SwiftModel = Swift.prepare_model(model, lora_config)
-        # Do some finetuning here
-        model.save_pretrained(tmp_dir)
-        
-        push_to_hub('my-group/swift_llama2', output_dir=tmp_dir)
-        model = Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto')
-        model = SwiftModel.from_pretrained(model, 'my-group/swift_llama2', device_map='auto')
+        ### Inference
+        Original model:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
+        # use VLLM
+        CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
+            --infer_backend vllm --max_model_len 8192
         ```
         
-        This is a example that uses transformers for model creation uses SWIFT for efficient tuning.
-        
-        ```python
-        from swift import Swift, LoRAConfig, AdapterConfig, PromptConfig
-        from transformers import AutoModelForImageClassification
-        
-        # init vit model
-        model = AutoModelForImageClassification.from_pretrained("google/vit-base-patch16-224")
-        
-        # init lora tuner config
-        lora_config = LoRAConfig(
-            r=10,  # the rank of the LoRA module
-            target_modules=['query', 'key', 'value'],  # the modules to be replaced with the end of the module name
-            merge_weights=False  # whether to merge weights
-        )
-        
-        # init adapter tuner config
-        adapter_config = AdapterConfig(
-            dim=768,  # the dimension of the hidden states
-            hidden_pos=0,  # the position of the hidden state to passed into the adapter
-            target_modules=r'.*attention.output.dense$',  # the modules to be replaced with regular expression
-            adapter_length=10  # the length of the adapter length
-        )
-        
-        # init prompt tuner config
-        prompt_config = PromptConfig(
-            dim=768,  # the dimension of the hidden states
-            target_modules=r'.*layer\.\d+$',  # the modules to be replaced with regular expression
-            embedding_pos=0,    # the position of the embedding tensor
-            prompt_length=10,   # the length of the prompt tokens
-            attach_front=False  # Whether prompt is attached in front of the embedding
-        )
-        
-        # create model with swift. In practice, you can use any of these tuners or a combination of them.
-        model = Swift.prepare_model(model, {"lora_tuner": lora_config, "adapter_tuner": adapter_config, "prompt_tuner": prompt_config})
-        
-        # get the trainable parameters of model
-        model.get_trainable_parameters()
-        # 'trainable params: 838,776 || all params: 87,406,432 || trainable%: 0.9596273189597764'
+        LoRA fine-tuned:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true
+        # use VLLM
+        CUDA_VISIBLE_DEVICES=0 swift infer \
+            --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \
+            --merge_lora true --infer_backend vllm --max_model_len 8192
         ```
         
-        You can use the features offered by Peft in SWIFT:
+        ### Evaluation
         
-        ```python
-        from swift import LoraConfig, Swift
-        from peft import TaskType
-        lora_config = LoraConfig(target_modules=['query', 'key', 'value'], task_type=TaskType.CAUSAL_LM)
-        model_wrapped = Swift.prepare_model(model, lora_config)
-        
-        # or call from_pretrained to load weights in the modelhub
-        model_wrapped = Swift.from_pretrained(model, 'some-id-in-the-modelscope-modelhub')
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset mmlu ceval
         ```
         
+        ### Export
         
-        The saving strategy between Swift tuners and Peft tuners are slightly different. You can name a tuner by:
-        
-        ```python
-        model = Swift.prepare_model(model, {'default': LoRAConfig(...)})
-        model.save_pretrained('./output')
+        Original model:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift export --model_type qwen1half-7b-chat \
+            --quant_bits 4 --quant_method awq
         ```
         
-        In the output dir, you will have a dir structure like this:
-        
-        ```text
-        output
-            |-- default
-                |-- adapter_config.json
-                |-- adapter_model.bin
-            |-- adapter_config.json
-            |-- adapter_model.bin
+        LoRA fine-tuned:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift export \
+            --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \
+            --quant_method awq --quant_bits 4 \
+            --merge_lora true \
         ```
         
-        The config/weights stored in the output dir is the config of `extra_state_keys` and the weights of it. This is different from PEFT, which stores the weights and config of the `default` tuner.
-        
+        ### Deployment
         
-        ## 🔍 Learn More
-        
-        - [ModelScope library](https://github.com/modelscope/modelscope/)
+        Original model:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat
+        # 使用VLLM加速
+        CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat \
+            --infer_backend vllm --max_model_len 8192
+        ```
         
-          ModelScope Library is the model library of ModelScope project, which contains a large number of popular models.
+        LoRA fine-tuned:
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx
+        # 使用VLLM加速
+        CUDA_VISIBLE_DEVICES=0 swift deploy \
+            --ckpt_dir xxx/checkpoint-xxx --merge_lora true \
+            --infer_backend vllm --max_model_len 8192
+        ```
+        
+        ### Supported Models
+        
+        #### LLMs
+        
+        | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
+        |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
+        | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model                      |
+        | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
+        | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
+        | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
+        | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
+        | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
+        | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
+        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
+        | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
+        | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
+        | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
+        | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
+        | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
+        | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
+        | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
+        | BlueLM                                         | [VIVO BlueLM large model](https://github.com/vivo-ai-lab/BlueLM)        | Chinese<br>English    | 7B                                     | base model<br>chat model                       |
+        | Ziya2                                          | [Fengshenbang series models](https://github.com/IDEA-CCNL/Fengshenbang-LM) | Chinese<br>English  | 13B                                    | base model<br>chat model                       |
+        | Skywork                                        | [Skywork series models](https://github.com/SkyworkAI/Skywork) | Chinese<br>English    | 13B                                    | base model<br>chat model                       |
+        | Zephyr                                         | Zephyr series models based on Mistral                                  | English            | 7B                                     | chat model                                 |
+        | PolyLM                                         | [Tongyi Lab self-developed PolyLM series models](https://github.com/DAMO-NLP-MT/PolyLM) | Multilingual | 13B                                 | base model                                 |
+        | SeqGPT                                         | [Tongyi Lab self-developed text understanding model for information extraction and text classification](https://github.com/Alibaba-NLP/SeqGPT) | Chinese | 560M                               | semantic understanding model                |
+        | SUS                                            | [Southern University of Science and Technology model fine-tuned on YI](https://github.com/SUSTech-IDEA/SUS-Chat) | Chinese<br>English | 34B                              | chat model                                 |
+        | Tongyi-Finance                                 | [Tongyi finance series models](https://github.com/QwenLM/Qwen)          | Chinese<br>English    | 14B                                    | base model<br>chat model<br>financial model        |
+        | CodeFuse-CodeLLaMA<br>CodeFuse-Codegeex2<br>CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai)        | Chinese<br>English    | 6B-34B                                 | chat model<br>code model                      |
+        | phi2                                           | Microsoft's PHI2 model                                                 | English            | 3B                                     | base model<br>code model                          |
+        | Grok | [X-ai](https://github.com/xai-org/grok-1) | English | 300B | base model |
+        | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat) | Chinese<br>English | 7B-12B | chat model |
+        | dbrx | [databricks](https://github.com/databricks/dbrx) | English | 132B | base model<br>chat model  |
+        | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) | Chinese<br>English | 13B | base model  |
+        | c4ai-command-r | [c4ai](https://cohere.com/command) | Multilingual | 35B-104B | chat model  |
+        
+        
+        #### MLLMs
+        
+        | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
+        |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
+        | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
+        | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
+        | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
+        | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
+        | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
+        | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
+        | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
+        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B               | chat model |
+        
+        #### Diffusion Models
+        
+        | Model Type          | Model Introduction                                                    | Language | Model Type        |
+        |---------------------|----------------------------------------------------------------------|----------|------------------ |
+        | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
+        | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
+        
+        ### Supported Open Source Datasets
+        
+        | Dataset Type | Training Task  | Documentation                                                                                                                                                                                                                                                                                                        |
+        |--------------|:---------------|--------------------------------------------------------------- |
+        | General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini. |
+        | Agent        | Fine-tuning    | 🔥ms-agent, ms-agent-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.                                                                                                                                                                                                                                                |
+        | General      | Human Alignment | 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.                            |
+        | Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.                                                                                                                                                                                                                          |
+        | Medical      | Fine-tuning    | medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.                                                                                                                                                                                                                                                          |
+        | Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.                                                                                                                                                                                                                                                                 |
+        | Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                                                                                                                                                                                                                                                                 |
+        | SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                                                                                                                                                                                                                                                                |
+        | Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                                                                                                                                                                                                                                                                            |
+        | Classification | Fine-tuning  | cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.                                                                                                                                                                                                                                                    |
+        | Quantization Assist | Quantization | pileval.                                                                                                                                                                                                                                                                                                             |
+        | Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.                                                                                                                                                                                                                               |
+        | Vision       | Fine-tuning    | coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.                                                                                                                                                                                                                                                              |
+        | Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-mini-zh.                                                                                                                                                                                                                                                                                     |
+        
+        ### Supported Technologies
+        
+        | Technology Name                                               |
+        |--------------------------------------------------------------- |
+        | 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) |
+        | 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) |
+        | 🔥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf) |
+        | 🔥SCEdit: [SCEdit: Efficient and Controllable Image Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/2312.11392)  < [arXiv](https://arxiv.org/abs/2312.11392)  \|  [Project Page](https://scedit.github.io/) > |
+        | 🔥NEFTune: [Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914) |
+        | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2309.14717) |
+        | LongLoRA: [Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307) |
+        | ROME: [Rank-One Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) |
+        | Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/1902.00751) |
+        | Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/2203.12119) |
+        | Side: [Side-Tuning: A Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503) |
+        | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859)  < [arXiv](https://arxiv.org/abs/2310.19859)  \|  [Project Page](https://res-tuning.github.io/)  \|  [Usage](docs/source/GetStarted/ResTuning.md) > |
+        | Tuners provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA, etc. |
+        
+        ### Supported Hardware
+        
+        | Hardware Environment           | Notes                                           |
+        |--------------------------------|-------------------------------------------------|
+        | CPU                            |                                                 |
+        | RTX 20/30/40 series, etc.      | After 30 series, BF16 and FlashAttn can be used |
+        | Computing cards T4/V100, etc.  | BF16 and FlashAttn not supported                |
+        | Computing cards A10/A100, etc. | Support BF16 and FlashAttn                      |
+        | Huawei Ascend NPU              |                                                 |
         
-        - [Contribute your own model to ModelScope](https://modelscope.cn/docs/ModelScope%E6%A8%A1%E5%9E%8B%E6%8E%A5%E5%85%A5%E6%B5%81%E7%A8%8B%E6%A6%82%E8%A7%88)
+        ## 📃 Documentation
         
+        ### Documentation Compiling
         
-        ## License
+        ```shell
+        make docs
+        # Check docs/build/html/index.html in web-browser
+        ```
         
-        This project is licensed under the [Apache License (Version 2.0)](https://github.com/modelscope/modelscope/blob/master/LICENSE).
+        ### User Guide
         
+        | Document Name                                                |
+        | ------------------------------------------------------------ |
+        | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
+        | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
+        | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
+        | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
+        | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
+        | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
+        | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
+        | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
+        
+        ### Reference Documentation
+        | Document Name                                                |
+        | ------------------------------------------------------------ |
+        | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
+        | [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
+        | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
+        | [Runtime Speed and Memory Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) |
+        
+        
+        ### Best Practices
+        
+        | Best Practices Name                                                |
+        | ------------------------------------------------------------ |
+        | [Agent Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+        | [Self-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+        |  [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
+        |  [Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/Multi-Modal/index.md) |
+        
+        ### Deep Learning Tutorials
+        
+        | Tutorial Name                                                |
+        |-------------------------------------------------------------- |
+        | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md) |
+        | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md) |
+        | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-prompt%20engineering.md) |
+        | [Transformer Architecture Introduction](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/D.Transformer%E7%BB%93%E6%9E%84.md) |
+        | [Training Technique Selection](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/E.%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B.md) |
+        | [Data Preprocessing](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/F.%E6%95%B0%E6%8D%AE%E9%A2%84%E5%A4%84%E7%90%86.md) |
+        | [Quantization](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/G.%E9%87%8F%E5%8C%96.md) |
+        | [Training](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/H.%E8%AE%AD%E7%BB%83.md) |
+        | [Inference](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/I.LLM%E5%92%8C%E5%A4%9A%E6%A8%A1%E6%80%81%E6%A8%A1%E5%9E%8B%E9%AB%98%E6%95%88%E6%8E%A8%E7%90%86%E5%AE%9E%E8%B7%B5.md) |
+        | [Deployment](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/J.%E9%83%A8%E7%BD%B2.md) |
+        | [Evaluation](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98--LLM%20Automatic%20Evaluation.md) |
+        
+        ## 🏛 License
+        
+        This framework is licensed under the [Apache License (Version 2.0)](https://github.com/modelscope/modelscope/blob/master/LICENSE). For models and datasets, please refer to the original resource page and follow the corresponding License.
+        
+        ## 📎 Citation
+        
+        ```bibtex
+        @Misc{swift,
+          title = {SWIFT:Scalable lightWeight Infrastructure for Fine-Tuning},
+          author = {The ModelScope Team},
+          howpublished = {\url{https://github.com/modelscope/swift}},
+          year = {2024}
+        }
+        ```
         
         ## ☎ Contact Us
-        You can contact and communicate with us by joining our WeChat Group:
+        
+        You can contact us and communicate with us by adding our WeChat group:
         
         <p align="left">
         <img src="asset/wechat.png" width="250" style="display: inline-block;">
         </p>
         
-        
         ## Star History
         
         [![Star History Chart](https://api.star-history.com/svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/swift&Date)
         
 Keywords: python,petl,efficient tuners
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -532,8 +578,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: llm
 Provides-Extra: aigc
+Provides-Extra: eval
 Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,525 +1,607 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 1.7.3 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.0 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
-        [https://modelscope.oss-cn-beijing.aliyuncs.com/modelscope.gif]
-                             _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y
-                      _ä_¸_­_æ__  ï½ &nbspEnglish  ï½  _D_o_c_s
+                            [resources/banner.png]
+                         _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
+                           _ä_¸_­_æ__   ï½   English  
       [https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg][https://
   img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_m_o_d_e_l_s_c_o_p_e_-_%_E_2_%_8_9_%_A_5_1_._9_._5_-_5_D_9_1_D_4_._s_v_g_]_[_h_t_t_p_s_:_/_/
      _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_m_s_-_s_w_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
   _m_o_d_e_l_s_c_o_p_e_/_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_s_-_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                          _b_a_d_g_e_/_P_R_-_w_e_l_c_o_m_e_-_5_5_E_B_9_9_._s_v_g_]
 ## ð Table of Contents - [Introduction](#-introduction) - [News](#-news) -
-ð¥[LLM Training and Inference](#-llm-training-and-inference) - ð¥[SCEdit
-Tuner](#-SCEdit) - [Installation](#-installation) - [Getting Started](#-
-getting-started) - [Learn More](#-learn-more) - [License](#license) - [Contact
-Us](#-contact-us) ## ð Introduction SWIFT (Scalable lightWeight
-Infrastructure for Fine-Tuning) is an extensible framework designed to
-facilitate lightweight model fine-tuning and inference. It integrates
-implementations for various efficient fine-tuning methods, by embracing
-approaches that is parameter-efficient, memory-efficient, and time-efficient.
-SWIFT integrates seamlessly into ModelScope ecosystem and offers the
-capabilities to finetune various models, with a primary emphasis on LLMs and
-vision models. Additionally, SWIFT is fully compatible with [PEFT](https://
-github.com/huggingface/peft), enabling users to leverage the familiar Peft
-interface to finetune ModelScope models. Currently supported approaches (and
-counting): 1. ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS]
-(https://arxiv.org/abs/2106.09685) 2. ð¥LoRA+: [LoRA+: Efficient Low Rank
-Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) 3. ð¥LLaMA
-PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://arxiv.org/pdf/
-2401.02415.pdf) 4. ð¥SCEdit: [SCEdit: Efficient and Controllable Image
-Diffusion Generation via Skip Connection Editing](https://arxiv.org/abs/
-2312.11392) < [arXiv](https://arxiv.org/abs/2312.11392) | [Project Page](https:
-//scedit.github.io/) > 5. ð¥NEFTune: [Noisy Embeddings Improve Instruction
-Finetuning](https://arxiv.org/abs/2310.05914) 6. QA-LoRA:[Quantization-Aware
-Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/
-2309.14717). 7. LongLoRA: [Efficient Fine-tuning of Long-Context Large Language
-Models](https://arxiv.org/abs/2309.12307) 8. ROME: [Rank-One Editing of
-Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) 9. Adapter:
-[Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/
-1902.00751) 10. Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/
-2203.12119) 11. Side: [Side-Tuning: A Baseline for Network Adaptation via
-Additive Side Networks](https://arxiv.org/abs/1912.13503) 12. Res-Tuning: [Res-
-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from
-Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://arxiv.org/abs/
-2310.19859) | [Project Page](https://res-tuning.github.io/) | [Usage](docs/
-source/GetStarted/ResTuning.md) > 13. All tuners offered on [PEFT](https://
-github.com/huggingface/peft), like IA3, AdaLoRA Key features: 1. By integrating
-the ModelScope library, models can be readily obtained via a model-id. 2.
-Tuners provided by SWIFT can be combined to allow exploration of multiple
-tuners on a model for best result. 3. Support calling `activate_adapter` or
-`deactivate_adapter` or `set_active_adapters` to activate/deactivate tuners.
-User can inference with one model and multiple tuners in different threads
-independently. 4. Support training and inference with scripts/CLIï¼meanwhile
-support inference with Web-UI. 5. Support model deployment(vllm/chatglm.cpp/
-xinference)ï¼Check [Official documentation](./docs/source/GetStarted/
-é¨ç½²æå.md) for details. Users can check the [documentation of SWIFT]
-(docs/source/GetStarted/å¿«éä½¿ç¨.md) to get detail tutorials. ## ð News
-- ð¥2024.03.12: Supports inference and fine-tuning for the **deepseek-vl**
-series. For best practice, you can refer to [here](https://github.com/
-modelscope/swift/tree/main/docs/source/Multi-Modal/deepseek-vlæä½³å®è·µ.md).
-- ð¥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507), which can
-efficiently reduce the memory usage(almost half of the original memory) when
-training the full model. - ð¥2024.03.10: For the end-to-end best practice of
-fine-tuning to deployment of Qwen1.5-7B-Chat and Qwen1.5-72B-Chat, you can
-refer to the [Qwen1.5 Full Workflow Best Practice](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
-Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md). -
-ð¥2024.03.09: Support training and inference of MAMBA series, use [this
-script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/mamba-1.4b/lora/sft.sh) to begin. - 2024.03.09: Support training and
-inference of AQLM quantized models, use [this script](https://github.com/
-modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to begin. - 2024.03.06: Support training
-and inference of AWQ quantized models, use [this Qwen1.5-AWQ script](https://
+[Installation](#%EF%B8%8F-installation) - [Getting Started](#-getting-started)
+- [Documentation](#-documentation) - [License](#-License) - [Citation](#-
+citation) - [Contact Us](#-contact-us) ## ð Introduction SWIFT supports
+training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs**
+(multimodal large models). Developers can directly apply our framework to their
+own research and production environments to realize the complete workflow from
+model training and evaluation to application. In addition to supporting the
+lightweight training solutions provided by [PEFT](https://github.com/
+huggingface/peft), we also provide a complete **Adapters library** to support
+the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
+adapter library can be used directly in your own custom workflow without our
+training scripts. To facilitate use by users unfamiliar with deep learning, we
+provide a Gradio web-ui for controlling training and inference, as well as
+accompanying deep learning courses and best practices for beginners.
+Additionally, we are expanding capabilities for other modalities. Currently, we
+support full-parameter training and LoRA training for AnimateDiff. ## ð News
+- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1
+model, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start
+training! - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-
+V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
+Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
+with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
+for details. Meanwhile, we support a trick way to do multiple ablation
+experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
+command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train. -
+2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
+function call capabilities, and combine it with [Modelscope-Agent](https://
+github.com/modelscope/modelscope-agent) for best practices, which can be found
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
+best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
+ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
+fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat_awq/lora/sft.sh) to begin, support training and inference of
-[yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/yi_9b/lora_zero3). - ð¥2024.02.29: Support [LLaMA PRO](https://
-arxiv.org/pdf/2401.02415.pdf), use [this script](https://github.com/modelscope/
-swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to
-begin. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf),
-use [this script](https://github.com/modelscope/swift/blob/main/examples/
-pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to begin. - 2024.02.25: Support
-`swift export` to export models for **AWQ/GPTQ** quantization and push to
-ModelScope Hub. For more details, please refer to the document: [LLM
-Quantization Document](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/LLM%E9%87%8F%E5%8C%96%E6%96%87%E6%A1%A3.md). - 2024.02.22: Support
-gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b,
-gemma-7b-instruct. - 2024.02.16: Support deepseek-math series: deepseek-math-
-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support
-**Qwen1.5** series, To view all supported Qwen1.5 models please check [Model
-List](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B).
-The [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat_int8) fine-tuned scripts are provided. - 2024.02.05: Support
-the training of **SDXL**, **SD**, **ControlNet**, or techniques like
-**DreamBooth**, you can check the [training scripts](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details. -
-2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat),
-minicpm-2b-chat. - ð¥2024.02.01: Support dataset mixture to reduce
-**Catastrophic Forgetting**. Use `--train_dataset_mix_ratio 2.0` to train! We
-also provide a common knowledge dataset [ms-bench](https://www.modelscope.cn/
-datasets/iic/ms_bench/summary). - ð¥2024.02.01: Support Agent training! Agent
-training algorithm comes from this [paper](https://arxiv.org/pdf/
-2309.00986.pdf). We also introduce the [ms-agent](https://www.modelscope.cn/
-datasets/iic/ms_agent/summary) dataset. Use [this script](https://github.com/
+xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
+**QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
+**Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-
+Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/
+pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training! -
+ð¥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base
+model, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start
+training! - ð¥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-
+instruct, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training! -
+ð¥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-
+A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4. - ð¥2024.03.29: Support the
+fine-tuning and inference of **Grok-1** 300B MoE, please view details [here]
+(https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
+practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
+7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
+swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
+training! - ð¥2024.03.20: Supports inference and fine-tuning for the
+**llava** series. For best practice, you can refer to [here](https://
+github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/
+llavaæä½³å®è·µ.md). - ð¥2024.03.12: Support inference and fine-tuning for
+**deepseek-vl** series. Best practices can be found [here](docs/source_en/
+Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
+(https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
+2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
+best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
+to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
+Support training and inference of MAMBA model, use [this script](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/
+lora/sft.sh) to start training! - 2024.03.09: Support training and inference of
+AQLM quantized model, use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to
+start training! - 2024.03.06: Support training and inference of AWQ quantized
+model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to
+start training, and support training and inference of [yi-9b](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/
+lora_zero3). - ð¥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/
+2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start
+training. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/
+2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/
+blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start
+training. - 2024.02.25: Support `swift export` to quantize models using **AWQ/
+GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md). More - 2024.02.22: Support gemma series:
+gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
+2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-
+instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support **Qwen1.5** series
+models, see [model list](https://github.com/modelscope/swift/blob/main/docs/
+source/LLM/
+%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
+for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-
+7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen1half_7b_chat_int8). - 2024.02.05: Support training of diffusion models
+such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training.
+See corresponding [training scripts](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/sdxl/scripts) for details. - 2024.02.01: Support minicpm
+series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat. -
+ð¥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**.
+Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced
+the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/
+iic/ms_bench/summary). - ð¥2024.02.01: Support Agent training! Agent training
+algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf).
+We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/
+summary), a high-quality agent dataset. Use [this script](https://github.com/
 modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/
-sft.sh) to begin an agent training! - ð¥2024.02.01: Support SFT loss to DPO
-training to reduce the repeat generation problem caused by the KL-divergence
-loss. - 2024.02.01: Support AdaLoRA and IA3 adapter in SFT. - 2024.02.01:
-Support `--merge_lora` in AnimateDiff training. More - 2024.01.30: Support
+sft.sh) to start Agent training! - ð¥2024.02.01: Support adding SFT loss in
+DPO training to reduce repetitive generation caused by KL divergence loss. -
+2024.02.01: Support using AdaLoRA and IA3 adapters in training. - 2024.02.01:
+Support `--merge_lora` parameter in AnimateDiff training. - 2024.01.30: Support
 [internlm-xcomposer2-7b-chat](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/internlm_xcomposer2_7b_chat). - ð¥2024.01.30:
 Support [ZeRO-3](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), just need to specify `--
-deepspeed default-zero3`. - 2024.01.29: Support internlm2-math series:
-internlm2-math-7b, internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-
-20b-chat. - ð¥2024.01.26: Support [yi-vl-6b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-
-34b-chat. - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-
-chat. - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://
+pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3/), simply specify `--deepspeed
+default-zero3`. - 2024.01.29: Support internlm2-math series: internlm2-math-7b,
+internlm2-math-7b-chat, internlm2-math-20b, internlm2-math-20b-chat. -
+ð¥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/
+tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat. -
+2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat. -
+2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 orion_14b_chat). - 2024.01.20: Support [xverse-13b-256k](https://github.com/
 modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k),
-xverse-65b-v2, xverse-65b-chat. - ð¥2024.01.17: Support **internlm2** series:
+xverse-65b-v2, xverse-65b-chat. - ð¥2024.01.17: Support internlm2 series:
 internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/
 modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat),
 internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat,
-internlm2-20b-chat. - 2024.1.15: Support yuan series: yuan2-2b-instruct,
+internlm2-20b-chat. - 2024.01.15: Support yuan series: yuan2-2b-instruct,
 [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct,
 yuan2-102b-instruct. - ð¥2024.01.12: Support **deepseek-moe** series:
 deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/
 tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat). -
-ð¥2024.01.04: Support for **VLLM deployment**, compatible with the **OpenAI
-API** style. For more details, please refer to [VLLM Inference Acceleration and
-Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²) - 2024.01.04: Update [Benchmark](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) to
-facilitate viewing the training speed and GPU memory required for different
-models. - ð¥ 2023.12.29: Support web-ui for training and inference, use
-`swift web-ui` after the installation of ms-swift. - ð¥ 2023.12.29: Support
-DPO RLHF(Reinforcement Learning from Human Feedback) and three datasets: AI-
-ModelScope/stack-exchange-paired and AI-ModelScope/hh-rlhf and AI-ModelScope/
-hh_rlhf_cn for this task. Check [this documentation](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
+ð¥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API**
+style, see [VLLM Inference Acceleration and Deployment](https://github.com/
+modelscope/swift/blob/main/docs/source/LLM/VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²)
+for details. - 2024.01.04: Update [Benchmark](https://github.com/modelscope/
+swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of
+training speed and memory usage of different models. - ð¥2023.12.29: Support
+web-ui for sft training and inference, use `swift web-ui` after installing ms-
+swift to start. - ð¥2023.12.29: Support DPO RLHF (Reinforcement Learning from
+Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-
+paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation]
+(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
 LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
-to start training! - ð¥ 2023.12.28: Support SCEdit! This framework can easily
-reduce memory usage in training and inference, and replace ControlNet for
-controllable image generating scenarios, view the following chapter for
-details. - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19:
-Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/phi2_3b). - 2023.12.18: Support for VLLM for inference
-acceleration. - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-
-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-
-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b,
-deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
-- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-mixtral_moe_7b), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/
-tree/main/examples/pytorch/llm/scripts/mixtral_moe_7b_instruct). - 2023.12.09:
-Support the `freeze_parameters` parameter as a compromise between LoRA and full
-parameter. Corresponding shell scripts can be found at [full_freeze_ddp](https:
-//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
-`preprocess_num_proc` parameters, for details please refer to [Command-Line
-parameters](https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-å½ä»¤è¡åæ°.md). - 2023.12.08: Support [sus-34b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/sus_34b_chat), support
-yi-6b-200k, yi-34b-200k. - 2023.12.07: Support [Multi-Node DDP training](https:
-//github.com/modelscope/swift/blob/main/docs/source/LLM/
+to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
+significantly reduce memory usage in U-Net and support low-memory controllable
+image generation (replacing ControlNet), read the section below to learn more.
+- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
+3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+phi2_3b). - 2023.12.18: Support VLLM for inference acceleration. - 2023.12.15:
+Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat,
+deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-
+1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-
+instruct, deepseek-coder-33b, deepseek-coder-33b-instruct. - 2023.12.13:
+Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/
+swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-
+instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/mixtral_7b_moe_instruct). - 2023.12.09: Support `freeze_parameters`
+parameter as a compromise between lora and full-parameter training.
+Corresponding sh can be found in [full_freeze_ddp](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/
+full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
+`preprocess_num_proc` parameters, see [command line arguments](https://
+github.com/modelscope/swift/blob/main/docs/source/LLM/
+%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details. - 2023.12.08:
+Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k. -
+2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/
+swift/blob/main/docs/source/LLM/
 LLM%E5%BE%AE%E8%B0%83%E6%96%87%E6%A1%A3.md#%E4%BD%BF%E7%94%A8cli). -
-2023.12.04: Supported models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat.
-Supported datasets: hc3-zh, hc3-en. - ð¥ 2023.12.02: [Best Practice for Self-
-cognition Fine-tuning](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/èªæè®¤ç¥å¾®è°æä½³å®è·µ.md), **10 minutes for self-cognition
-fine-tuning for LLM**, creating a LLM that is specific to oneself. - ð¥
-2023.11.30: Support for training and inference of the **qwen-1_8b**, **qwen-
-72b**, and **qwen-audio** model series. The corresponding shell scripts can be
-viewed at [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/
+2023.12.05: Support models: zephyr-7b-beta-chat, openbuddy-zephyr-7b-chat.
+Support datasets: hc3-zh, hc3-en. - ð¥2023.12.02: [Self-cognition fine-tuning
+best practices](docs/source_en/LLM/Self-cognition-best-practice.md), **10
+minutes to fine-tune a large model for self-cognition**, create your own unique
+large model. - ð¥2023.11.30: Support training and inference of **qwen-1_8b**,
+**qwen-72b**, **qwen-audio** series models. Corresponding sh scripts can be
+found in [qwen_1_8b_chat](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/qwen_1_8b_chat), [qwen_72b_chat](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_72b_chat), [qwen_audio_chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/qwen_audio_chat). - ð¥ 2023.11.29: Support
-the training and inference for **AnimateDiff** - ð¥ 2023.11.24: Support for
-**yi-34b-chat**, **codefuse-codellama-34b-chat**: The corresponding shell
-script can be found in [yi_34b_chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat]
-(https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-codefuse_codellama_34b_chat). - ð¥ 2023.11.18: Support for **tongyi-finance-
-14b** series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-
-finance-14b-chat-int4. The corresponding shell script can be found in
+main/examples/pytorch/llm/scripts/qwen_audio_chat) - ð¥2023.11.29: Support
+training and inference of **AnimateDiff** - ð¥2023.11.24: Support **yi-34b-
+chat**, **codefuse-codellama-34b-chat** models. Corresponding sh scripts can be
+found in [yi_34b_chat](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/yi_34b_chat), [codefuse_codellama_34b_chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+codefuse_codellama_34b_chat). - ð¥2023.11.18: Support **tongyi-finance-14b**
+series models: tongyi-finance-14b, tongyi-finance-14b-chat, tongyi-finance-14b-
+chat-int4. Corresponding sh scripts can be found in
 [tongyi_finance_14b_chat_int4](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4). - 2023.11.16: Added
-support for more models in **flash attn**: qwen series, qwen-vl series, llama
+examples/pytorch/llm/scripts/tongyi_finance_14b_chat_int4). - 2023.11.16:
+Support **flash attn** for more models: qwen series, qwen-vl series, llama
 series, openbuddy series, mistral series, yi series, ziya series. Please use
-the `use_flash_attn` parameter. - ð¥ 2023.11.11: **NEFTune** Supported, Use
-is with `Swift.prepare_model(model, NEFTuneConfig())` - ð¥ 2023.11.11:
-Support training and inference with **CLI**, and inference with **Web-UI**.
-Check the [Run using Swift CLI](https://github.com/modelscope/swift/tree/
-main#run-using-swift-cli) chapter for details. - ð¥ 2023.11.11: Support model
-**deployment**(vllm/chatglm.cpp/xinference)ï¼Check [Official documentation](./
-docs/source/GetStarted/é¨ç½²æå.md) for details. - ð¥ 2023.11.10: Support
-for **bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-
-7b-chat-32k. The corresponding shell script can be found in [bluelm_7b_chat]
+`use_flash_attn` parameter. - ð¥2023.11.11: Support **NEFTune**, simply use
+`Swift.prepare_model(model, NEFTuneConfig())` to enable. - ð¥2023.11.11:
+Support training and inference by **command line** and inference by **Web-UI**,
+see `Usage with Swift CLI` section below for details. - ð¥2023.11.10: Support
+**bluelm** series models: bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-
+chat-32k. Corresponding sh scripts can be found in [bluelm_7b_chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+bluelm_7b_chat). - ð¥2023.11.08: Support training and inference of **xverse-
+65b** model, script at [xverse_65b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/xverse_65b). - ð¥2023.11.07: Support
+training and inference of **yi-6b**, **yi-34b** models, scripts at [yi_6b]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-bluelm_7b_chat). - ð¥ 2023.11.08: Support the finetuning of **xverse-65b**
-model, scripts can be found at: [xverse_65b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/xverse_65b). - ð¥ 2023.11.07:
-Support the finetuning of **yi-6b**, **yi-34b** model, scripts can be found at:
-[yi_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
-scripts/yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/yi_34b). - ð¥ 2023.10.30: Support **QA-LoRA**
-and **LongLoRA** to decrease memory usage in training. - ð¥ 2023.10.30:
-Support **ROME**(Rank One Model Editing) to add/modify knowledges, training is
-not needed! - 2023.10.30: Support for **skywork-13b** series models: skywork-
-13b, skywork-13b-chat. The corresponding shell script can be found in
-[skywork_13b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
-llm/scripts/skywork_13b). - ð¥ 2023.10.27: Support for **chatglm3** series
-models: chatglm3-6b-base, chatglm3-6b, chatglm3-6b-32k. The corresponding shell
-script can be found in [chatglm3_6b](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/chatglm3_6b). - ð¥ 2023.10.17: Supported
-**int4**, **int8** models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-
-int4, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-
-14b-chat-int8. - 2023.10.15: Supported **ziya2-13b** model series: ziya2-13b,
-ziya2-13b-chat. - 2023.10.12: Supported **mistral-7b** model series: openbuddy-
-mistral-7b-chat, mistral-7b, mistral-7b-instruct. - ð¥ 2023.10.07: Supported
-**DeepSpeed ZeRO-2**, enabling LoRA (not just QLoRA) to run DDP on 2*A10. -
-2023.10.04: Supported datasets in the fields of mathematics, law, SQL, and
-coding: blossom-math-zh, school-math-zh, text2sql-en, sql-create-context-en,
-lawyer-llama-zh, tigerbot-law-zh, leetcode-python-en. - ð¥ 2023.09.25:
-Supported **qwen-14b** model series: qwen-14b, qwen-14b-chat. - 2023.09.18:
-Supported **internlm-20b** model series: internlm-20b, internlm-20b-chat. -
-2023.09.12: Supported training with **MP+DDP** to accelerate full-parameter
-fine-tuning speed. - 2023.09.05: Supported **openbuddy-llama2-70b-chat** model.
-- 2023.09.03: Supported **baichuan2** model series: baichuan2-7b, baichuan2-7b-
-chat, baichuan2-13b, baichuan2-13b-chat. ## â¨ LLM Training and Inference If
-you want to learn more about **best practices** for LLM or multimodal LLM, or
-if you are interested in **tutorials** on inference, fine-tuning, quantization,
-and deployment of LLM, you can refer to the [LLM series documentation](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/index.md). ### WEB UI
-training and inference After installation, you can use web-ui training/
-inference like: ```shell SWIFT_UI_LANG=en swift web-ui ``` > Supported
-environment variables: > > WEBUI_SHARE=1 Share the gradio or not >
-SWIFT_UI_LANG=en/zh The language of radio > WEBUI_SERVER server_nameï¼ web-ui
-host ipï¼0.0.0.0 means all routes are allowedï¼127.0.0.1 means only localhost
-can visit the web > WEBUI_PORT The port of web-ui Here is a simple introduction
-of web-ui: [![Watch the video](docs/source/cources/resources/
-20240119160942.jpg)](https://modelscope-open.oss-cn-hangzhou.aliyuncs.com/
-SWIFT%E8%A7%86%E9%A2%91_%E8%B0%83%E6%95%B4%E5%B0%81%E9%9D%A2.mp4) ### Quick
-Start You can test if the environment is installed correctly by running the
-following code. ```python # pip install ms-swift[llm] -U # Experimental
-environment: A10, 3090, V100, ... # 8GB GPU memory import os os.environ
-['CUDA_VISIBLE_DEVICES'] = '0' import torch from swift.llm import
-( DatasetName, InferArguments, ModelType, SftArguments, infer_main, sft_main,
-app_ui_main, merge_lora ) model_type = ModelType.qwen1half_0_5b sft_args =
-SftArguments( model_type=model_type, train_dataset_sample=2000, dataset=
-[DatasetName.jd_sentiment_zh], output_dir='output') result = sft_main(sft_args)
-best_model_checkpoint = result['best_model_checkpoint'] print
-(f'best_model_checkpoint: {best_model_checkpoint}') torch.cuda.empty_cache()
-infer_args = InferArguments( ckpt_dir=best_model_checkpoint,
-load_dataset_config=True, val_dataset_sample=10) merge_lora(infer_args,
-device_map='cpu') result = infer_main(infer_args) torch.cuda.empty_cache()
-app_ui_main(infer_args) ``` ### Training Scripts You can refer to the following
-scripts to customize your own training script. - full: [qwen1half-7b-chat]
+yi_6b), [yi_34b](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/yi_34b). - ð¥2023.10.30: Support two new tuners: **QA-
+LoRA** and **LongLoRA**. - ð¥2023.10.30: Support editing models using
+**ROME** (Rank One Model Editing) to infuse new knowledge into models without
+training! - 2023.10.30: Support **skywork-13b** series models: skywork-13b,
+skywork-13b-chat. Corresponding sh scripts can be found in [skywork_13b](https:
+//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+skywork_13b). - ð¥2023.10.27: Support **chatglm3** series models: chatglm3-
+6b-base, chatglm3-6b, chatglm3-6b-32k. Corresponding sh scripts can be found in
+[chatglm3_6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
+llm/scripts/chatglm3_6b). - ð¥2023.10.17: Support SFT of **int4**, **int8**
+models: qwen-7b-chat-int4, qwen-14b-chat-int4, qwen-vl-chat-int4, baichuan2-7b-
+chat-int4, baichuan2-13b-chat-int4, qwen-7b-chat-int8, qwen-14b-chat-int8. -
+2023.10.15: Support **ziya2-13b** series models: ziya2-13b, ziya2-13b-chat. -
+2023.10.12: Support **mistral-7b** series models: openbuddy-mistral-7b-chat,
+mistral-7b, mistral-7b-instruct. - ð¥2023.10.07: Support **DeepSpeed ZeRO-
+2**, enabling lora (not just qlora) to run DDP on dual A10 cards. - 2023.10.04:
+Support more math, law, SQL, code domain datasets: blossom-math-zh, school-
+math-zh, text2sql-en, sql-create-context-en, lawyer-llama-zh, tigerbot-law-zh,
+leetcode-python-en. - ð¥2023.09.25: Support **qwen-14b** series: qwen-14b,
+qwen-14b-chat. - 2023.09.18: Support **internlm-20b** series: internlm-20b,
+internlm-20b-chat. - 2023.09.12: Support **MP+DDP** to accelerate full-
+parameter training. - 2023.09.05: Support **openbuddy-llama2-70b-chat**. -
+2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat,
+baichuan2-13b, baichuan2-13b-chat. ## ð ï¸ Installation SWIFT runs in the
+Python environment. Please ensure your Python version is higher than 3.8. -
+Method 1: Install SWIFT using pip command: ```shell # Full capabilities pip
+install ms-swift[all] -U # LLM only pip install ms-swift[llm] -U # AIGC only
+pip install ms-swift[aigc] -U # Adapters only pip install ms-swift -U ``` -
+Method 2: Install SWIFT through source code (convenient for running training
+and inference scripts), please run the following commands: ```shell git clone
+https://github.com/modelscope/swift.git cd swift pip install -e .[llm] ```
+SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3: Use SWIFT in
+our Docker image ```shell # China-Hangzhou image docker pull registry.cn-
+hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
+torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull registry.us-west-
+1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
+torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This section introduces
+basic usage, see the [Documentation](#-documentation) section for more ways to
+use. ### Web-UI ```shell swift web-ui ``` ### Training #### Training Scripts
+You can refer to the following scripts to customize your own training script. -
+full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100) -
-full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100) -
-full+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora:
-[chatglm3-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/
-llm/scripts/chatglm3_6b/lora) (3090), [baichuan2-13b-chat](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/baichuan2_13b_chat/
-lora_mp) (2\*3090), [yi-34b-chat](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat]
+qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
+//github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/
+lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-
+34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/yi_34b_chat/lora) (A100), [qwen-72b-chat](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_72b_chat/lora_mp)
+(2\*A100) - lora+ddp: [chatglm3-6b](https://github.com/modelscope/swift/tree/
+main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp) (2\*3090) -
+lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3) (4\*3090), [qwen-
+72b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100) - qlora(gptq-int4): [qwen-7b-
+chat-int4](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen_7b_chat_int4/qlora) (3090) - qlora(gptq-int8): [qwen1half-7b-chat-
+int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
+scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-int4): [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_72b_chat/lora_mp) (2\*A100) - lora+ddp: [chatglm3-6b](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/lora_ddp)
-(2\*3090) - lora+ddp+zero3: [qwen-14b-chat](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/qwen_14b_chat/lora_ddp_zero3)
-(4\*3090), [qwen-72b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_72b_chat/lora_ddp_zero3) (4\*A100) - qlora
-(gptq-int4): [qwen-7b-chat-int4](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen_7b_chat_int4/qlora) (3090) - qlora(gptq-
-int8): [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-
-int4): [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/
-pytorch/llm/scripts/qwen_7b_chat/qlora) (3090) ### Features - Supported SFT
-Methods: [lora](https://arxiv.org/abs/2106.09685), [qlora](https://arxiv.org/
-abs/2305.14314), [longlora](https://arxiv.org/abs/2309.12307), [qalora](https:/
-/arxiv.org/abs/2309.14717), full parameter fine-tuning, partial parameter fine-
-tuning. - Supported Features: quantization, DDP, model parallelism, gradient
-checkpointing, pushing to modelscope hub, custom datasets, multimodal and agent
-SFT, mutli-round chat, DPO, self-cognition fine-tuning, ... - Supported Models:
-[[Detailed Info]](https://github.com/modelscope/swift/blob/main/docs/source/
-LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
-- Multi-Modal: - [qwen-vl](https://github.com/QwenLM/Qwen-VL) series: qwen-vl,
-qwen-vl-chat, qwen-vl-chat-int4. - [qwen-audio](https://github.com/QwenLM/Qwen-
-Audio) series: qwen-audio, qwen-audio-chat. - [deepseek-vl](https://github.com/
-deepseek-ai/DeepSeek-VL) series: deepseek-vl-1_3b-chat, deepseek-vl-7b-chat. -
-[yi-vl](https://github.com/01-ai/Yi) series: yi-vl-6b-chat, yi-vl-34b-chat. -
-[internlm-xcomposer2](https://github.com/InternLM/InternLM-XComposer) series:
-internlm-xcomposer2-7b-chat. - [minicpm-v](https://github.com/OpenBMB/MiniCPM)
-series: minicpm-v-3b-chat. - [cogvlm](https://github.com/THUDM/CogVLM) series:
-cogvlm-17b-instruct, cogagent-18b-chat, cogagent-18b-instruct. - General: -
-[qwen](https://github.com/QwenLM/Qwen) series: - qwen-1_8b, qwen-1_8b-chat,
-qwen-1_8b-chat-int4, qwen-1_8b-chat-int8. - qwen-7b, qwen-7b-chat, qwen-7b-
-chat-int4, qwen-7b-chat-int8. - qwen-14b, qwen-14b-chat, qwen-14b-chat-int4,
-qwen-14b-chat-int8. - qwen-72b, qwen-72b-chat, qwen-72b-chat-int4, qwen-72b-
-chat-int8. - [qwen1.5](https://github.com/QwenLM/Qwen1.5) series: - qwen1half-
-0_5b, qwen1half-0_5b-chat, qwen1half-0_5b-chat-int4, qwen1half-0_5b-chat-int8,
-qwen1half-0_5b-chat-awq. - qwen1half-1_8b, qwen1half-1_8b-chat, qwen1half-1_8b-
-chat-int4, qwen1half-1_8b-chat-int8, qwen1half-1_8b-chat-awq. - qwen1half-4b,
-qwen1half-4b-chat, qwen1half-4b-chat-int4, qwen1half-4b-chat-int8, qwen1half-
-4b-chat-awq. - qwen1half-7b, qwen1half-7b-chat, qwen1half-7b-chat-int4,
-qwen1half-7b-chat-int8, qwen1half-7b-chat-awq. - qwen1half-14b, qwen1half-14b-
-chat, qwen1half-14b-chat-int4, qwen1half-14b-chat-int8, qwen1half-14b-chat-awq.
-- qwen1half-72b, qwen1half-72b-chat, qwen1half-72b-chat-int4, qwen1half-72b-
-chat-int8, qwen1half-72b-chat-awq. - [chatglm](https://github.com/THUDM/
-ChatGLM-6B) series: chatglm2-6b, chatglm2-6b-32k, chatglm3-6b-base, chatglm3-
-6b, chatglm3-6b-32k. - [llama](https://github.com/facebookresearch/llama)
-series: llama2-7b, llama2-7b-chat, llama2-13b, llama2-13b-chat, llama2-70b,
-llama2-70b-chat. - [yi](https://github.com/01-ai/Yi) series: yi-6b, yi-6b-200k,
-yi-6b-chat, yi-9b, yi-34b, yi-34b-200k, yi-34b-chat. - [internlm](https://
-github.com/InternLM/InternLM) series: - internlm-7b, internlm-7b-chat,
-internlm-7b-chat-8k, internlm-20b, internlm-20b-chat. - internlm2-1_8b,
-internlm2-1_8b-sft-chat, internlm2-1_8b-chat, internlm2-7b-base, internlm2-7b,
-internlm2-7b-sft-chat, internlm2-7b-chat, internlm2-20b-base, internlm2-20b,
-internlm2-20b-sft-chat, internlm2-20b-chat. - [deepseek](https://github.com/
-deepseek-ai/deepseek-LLM) series: deepseek-7b, deepseek-7b-chat, deepseek-67b,
-deepseek-67b-chat, deepseek-moe-16b, deepseek-moe-16b-chat. - [gemma](https://
-github.com/google/gemma_pytorch) series: gemma-2b, gemma-2b-instruct, gemma-7b,
-gemma-7b-instruct. - [minicpm](https://github.com/OpenBMB/mlc-MiniCPM) series:
-minicpm-2b-sft-chat, minicpm-2b-chat. - [openbuddy](https://github.com/
-OpenBuddy/OpenBuddy) series: openbuddy-llama2-13b-chat, openbuddy-llama-65b-
-chat, openbuddy-llama2-70b-chat, openbuddy-mistral-7b-chat, openbuddy-zephyr-
-7b-chat, openbuddy-deepseek-67b-chat, openbuddy-mixtral-moe-7b-chat. -
-[mistral](https://github.com/mistralai/mistral-src) series: mistral-7b,
-mistral-7b-instruct, mistral-7b-instruct-v2. - [mixtral](https://github.com/
-mistralai/mistral-src) series: mixtral-moe-7b, mixtral-moe-7b-instruct. -
-[baichuan](https://github.com/baichuan-inc/Baichuan2) series: baichuan-7b,
-baichuan-13b, baichuan-13b-chat, baichuan2-7b, baichuan2-7b-chat, baichuan2-
-13b, baichuan2-13b-chat, baichuan2-7b-chat-int4, baichuan2-13b-chat-int4. -
-[yuan](https://github.com/IEIT-Yuan/Yuan-2.0) series: yuan2-2b-instruct, yuan2-
-2b-janus-instruct, yuan2-51b-instruct, yuan2-102b-instruct. - [xverse](https://
-github.com/xverse-ai/XVERSE-13B) series: xverse-7b, xverse-7b-chat, xverse-13b,
-xverse-13b-chat, xverse-65b, xverse-65b-v2, xverse-65b-chat, xverse-13b-256k. -
-[orion](https://github.com/OrionStarAI/OrionStar-Yi-34B-Chat) series: orion-
-14b, orion-14b-chat. - [bluelm](https://github.com/vivo-ai-lab/BlueLM) series:
-bluelm-7b, bluelm-7b-chat, bluelm-7b-32k, bluelm-7b-chat-32k. - [zephyr](https:
-//github.com/huggingface/alignment-handbook) series: zephyr-7b-beta-chat. -
-[ziya](https://github.com/IDEA-CCNL/Fengshenbang-LM) series: ziya2-13b, ziya2-
-13b-chat. - [skywork](https://github.com/SkyworkAI/Skywork) series: skywork-
-13b, skywork-13b-chat. - other: [polylm-13b](https://github.com/DAMO-NLP-MT/
-PolyLM), [seqgpt-560m](https://github.com/Alibaba-NLP/SeqGPT), [sus-34b-chat]
-(https://github.com/SUSTech-IDEA/SUS-Chat). - Financial: - [tongyi-finance]
-(https://github.com/QwenLM/Qwen) series: tongyi-finance-14b, tongyi-finance-
-14b-chat, tongyi-finance-14b-chat-int4. - Coding: - [codefuse](https://
-github.com/codefuse-ai) series: codefuse-codellama-34b-chat, codefuse-
-codegeex2-6b-chat, codefuse-qwen-14b-chat. - [deepseek-coder](https://
-github.com/deepseek-ai/DeepSeek-Coder) series: deepseek-coder-1_3b, deepseek-
-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct,
-deepseek-coder-33b, deepseek-coder-33b-instruct. - [codegeex2](https://
-github.com/THUDM/CodeGeeX2) series: codegeex2-6b. - [phi](https://
-www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-
-language-models/) series: phi2-3b. - Math: - [internlm2-math](https://
-github.com/InternLM/InternLM-Math) series: internlm2-math-7b, internlm2-math-
-7b-chat, internlm2-math-20b, internlm2-math-20b-chat. - [deepseek-math](https:/
-/github.com/deepseek-ai/DeepSeek-Math) series: deepseek-math-7b, deepseek-math-
-7b-instruct, deepseek-math-7b-chat. - Supported Datasets: [[Detailed Info]]
-(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
-%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%95%B0%E6%8D%AE%E9%9B%86)
-- NLP: - General: ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4),
-ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en,
-cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh,
-tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4,
-ð¥sharegpt-gpt4-mini. - Agent: ð¥ms-agent, damo-mini-agent-zh, damo-agent-
-zh, agent-instruct-all-en. - RLHF: ð¥hh-rlhf-cn, stack-exchange-paired, hh-
-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-
-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-
-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-
-helpful-base-en. - Coding: code-alpaca-en, ð¥leetcode-python-en,
-ð¥codefuse-python-en, ð¥codefuse-evol-instruction-zh. - Medical: medical-
-en, medical-zh, medical-mini-zh, ð¥disc-med-sft-zh. - Law: lawyer-llama-zh,
-tigerbot-law-zh, ð¥disc-law-sft-zh. - Math: ð¥blossom-math-zh, school-math-
-zh, open-platypus-en. - SQL: text2sql-en, ð¥sql-create-context-en. - Text
-Generation: ð¥advertise-gen-zh, ð¥dureader-robust-zh. - Classification:
-cmnli-zh, ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. -
-AWQ: pileval. - Other: finance-en, poetry-zh, webnovel-zh, generated-chat-zh,
-cls-fudan-news-zh, ner-jave-zh. - Multi-Modal: - Vision: coco-en, ð¥coco-
-mini-en, coco-mini-en-2, capcha-images. - Audio: aishell1-zh, ð¥aishell1-
-mini-zh. - Custom Dataset - Supported Templates: - Text Generation: default-
-generation, default-generation-bos, chatglm-generation, qwen-audio-generation.
-- Chat: default, qwen, qwen-audio, baichuan, chatglm2, chatglm3, llama,
-openbuddy, internlm, internlm2, internlm-xcomposer2, yi, yi-vl, yuan, xverse,
-ziya, skywork, bluelm, zephyr, sus, deepseek, deepseek-coder, codefuse-
-codellama, codefuse, cogvlm-instruct, cogagent-chat, cogagent-instruct, orion,
-minicpm, minicpm-v, gemma, chatml. ## ð¥SCEdit SCEdit is an efficient
-generative fine-tuning framework proposed by Alibaba TongYi Vision Intelligence
-Lab. This framework enhances the fine-tuning capabilities for text-to-image
-generation downstream tasks and enables quick adaptation to specific generative
-scenarios, **saving 30%-50% of training memory costs compared to LoRA**.
-Furthermore, it can be directly extended to controllable image generation
-tasks, **requiring only 7.9% of the parameters that ControlNet needs for
-conditional generation and saving 30% of memory usage**. It supports various
-conditional generation tasks including edge maps, depth maps, segmentation
-maps, poses, color maps, and image completion. We using 3D style data from the
-[style transfer dataset](https://modelscope.cn/datasets/damo/
-style_custom_dataset/dataPeview) for training, and testing with the same
-`Prompt: A boy in a camouflage jacket with a scarf`. The qualitative and
-quantitative results are as follows: | Method | bs | ep | Target Module |
-Param. (M) | Mem. (MiB) | 3D style | | --------- | ---- | ---- | ------------
-- | ------------- | ---------- | ----------------------------------------------
--------------- | | LoRA/r=64 | 1 | 50 | q/k/v/out/mlp | 23.94 (2.20%) | 8440MiB
-| [img]| | SCEdit | 1 | 50 | up_blocks | 19.68 (1.81%) | 7556MiB | [img]| |
-LoRA/r=64 | 10 | 100 | q/k/v/out/mlp | 23.94 (2.20%) | 26300MiB | [img]| |
-SCEdit | 10 | 100 | up_blocks | 19.68 (1.81%) | 18634MiB | [img]| | LoRA/r=64 |
-30 | 200 | q/k/v/out/mlp | 23.94 (2.20%) | 69554MiB | [img]| | SCEdit | 30 |
-200 | up_blocks | 19.68 (1.81%) | 43350MiB | [img]| The benchmark listed above
-can be reproduced byï¼ ```shell # Install swift by the next chapter cd
-examples/pytorch/multi_modal/notebook python text_to_image_synthesis.py ``` ##
-ð ï¸ Installation SWIFT is running in Python environment. Please make sure
-your python version is higher than 3.8. - Install SWIFT by the `pip` command:
-```shell # full ability pip install ms-swift[all] -U # only use llm pip install
-ms-swift[llm] -U # only use aigc pip install ms-swift[aigc] -U # only use
-adapters pip install ms-swift -U ``` - Install SWIFT by source code(for running
-sft/infer examples), please run: ```shell git clone https://github.com/
-modelscope/swift.git cd swift pip install -e .[llm] ``` SWIFT requires
-torch>=1.13. - Use SWIFT in our docker image: ```shell docker pull registry.cn-
-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu20.04-cuda11.8.0-py38-
-torch2.0.1-tf2.13.0-1.9.1 ``` ## ð Getting Started SWIFT supports multiple
-tuners, as well as tuners provided by [PEFT](https://github.com/huggingface/
-peft). To use these tuners, simply call: ```python from swift import Swift,
-LoRAConfig config = LoRAConfig(...) model = Swift.prepare_model(model, config,
-extra_state_keys=['...']) ``` The code snippet above initialized the tuner
-randomly. The input model is an instance of `torch.nn.Module`, the config is a
-subclass instance of `SwiftConfig` or `PeftConfig`. extra_state_keys is the
-extra module weights(like the linear head) to be trained and stored in the
-output dir. You may combine multiple tuners by: ```python from swift import
-Swift, LoRAConfig, PromptConfig model = Swift.prepare_model(model, {'lora':
-LoRAConfig(...), 'prompt': PromptConfig(...)}) ``` Call `save_pretrained` and
-`push_to_hub` after finetuning: ```python from swift import push_to_hub
-model.save_pretrained('some-output-folder') push_to_hub('my-group/some-repo-id-
-modelscope', 'some-output-folder', token='some-ms-token') ``` Assume `my-group/
-some-repo-id-modelscope` is the model-id in the hub, and `some-ms-token` is the
-token for uploading. Using the model-id to do later inference: ```python from
-swift import Swift model = Swift.from_pretrained(model, 'my-group/some-repo-id-
-modelscope') ``` Here shows a runnable example: ```python import os import
-tempfile # Please install modelscope by `pip install modelscope` from
-modelscope import Model from swift import LoRAConfig, SwiftModel, Swift,
-push_to_hub tmp_dir = tempfile.TemporaryDirectory().name if not os.path.exists
-(tmp_dir): os.makedirs(tmp_dir) model = Model.from_pretrained('modelscope/
-Llama-2-7b-ms', device_map='auto') lora_config = LoRAConfig(target_modules=
-['q_proj', 'k_proj', 'v_proj']) model: SwiftModel = Swift.prepare_model(model,
-lora_config) # Do some finetuning here model.save_pretrained(tmp_dir)
-push_to_hub('my-group/swift_llama2', output_dir=tmp_dir) model =
-Model.from_pretrained('modelscope/Llama-2-7b-ms', device_map='auto') model =
-SwiftModel.from_pretrained(model, 'my-group/swift_llama2', device_map='auto')
-``` This is a example that uses transformers for model creation uses SWIFT for
-efficient tuning. ```python from swift import Swift, LoRAConfig, AdapterConfig,
-PromptConfig from transformers import AutoModelForImageClassification # init
-vit model model = AutoModelForImageClassification.from_pretrained("google/vit-
-base-patch16-224") # init lora tuner config lora_config = LoRAConfig( r=10, #
-the rank of the LoRA module target_modules=['query', 'key', 'value'], # the
-modules to be replaced with the end of the module name merge_weights=False #
-whether to merge weights ) # init adapter tuner config adapter_config =
-AdapterConfig( dim=768, # the dimension of the hidden states hidden_pos=0, #
-the position of the hidden state to passed into the adapter
-target_modules=r'.*attention.output.dense$', # the modules to be replaced with
-regular expression adapter_length=10 # the length of the adapter length ) #
-init prompt tuner config prompt_config = PromptConfig( dim=768, # the dimension
-of the hidden states target_modules=r'.*layer\.\d+$', # the modules to be
-replaced with regular expression embedding_pos=0, # the position of the
-embedding tensor prompt_length=10, # the length of the prompt tokens
-attach_front=False # Whether prompt is attached in front of the embedding ) #
-create model with swift. In practice, you can use any of these tuners or a
-combination of them. model = Swift.prepare_model(model, {"lora_tuner":
-lora_config, "adapter_tuner": adapter_config, "prompt_tuner": prompt_config}) #
-get the trainable parameters of model model.get_trainable_parameters() #
-'trainable params: 838,776 || all params: 87,406,432 || trainable%:
-0.9596273189597764' ``` You can use the features offered by Peft in SWIFT:
-```python from swift import LoraConfig, Swift from peft import TaskType
-lora_config = LoraConfig(target_modules=['query', 'key', 'value'],
-task_type=TaskType.CAUSAL_LM) model_wrapped = Swift.prepare_model(model,
-lora_config) # or call from_pretrained to load weights in the modelhub
-model_wrapped = Swift.from_pretrained(model, 'some-id-in-the-modelscope-
-modelhub') ``` The saving strategy between Swift tuners and Peft tuners are
-slightly different. You can name a tuner by: ```python model =
-Swift.prepare_model(model, {'default': LoRAConfig(...)}) model.save_pretrained
-('./output') ``` In the output dir, you will have a dir structure like this:
-```text output |-- default |-- adapter_config.json |-- adapter_model.bin |-
-- adapter_config.json |-- adapter_model.bin ``` The config/weights stored in
-the output dir is the config of `extra_state_keys` and the weights of it. This
-is different from PEFT, which stores the weights and config of the `default`
-tuner. ## ð Learn More - [ModelScope library](https://github.com/modelscope/
-modelscope/) ModelScope Library is the model library of ModelScope project,
-which contains a large number of popular models. - [Contribute your own model
-to ModelScope](https://modelscope.cn/docs/
-ModelScope%E6%A8%A1%E5%9E%8B%E6%8E%A5%E5%85%A5%E6%B5%81%E7%A8%8B%E6%A6%82%E8%A7%88)
-## License This project is licensed under the [Apache License (Version 2.0)]
-(https://github.com/modelscope/modelscope/blob/master/LICENSE). ## â Contact
-Us You can contact and communicate with us by joining our WeChat Group:
+qwen_7b_chat/qlora) (3090) #### Supported Training Processes | Training Process
+| Training Method | |------------------|---------------------------------------
+----------------------------------------| | Pretraining | Text Generation | |
+Fine-tuning | Single-turn/Multi-turn
+Agent Training/Self-cognition
+Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO | | Text-to-
+Image | DreamBooth, etc. | | Text-to-Video | - | #### Single GPU Training Start
+single GPU fine-tuning with the following command: LoRA: ```shell #
+Experimental Environment: A100 # GPU Memory Requirement: 20GB # Runtime: 3.1
+hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ --eval_steps 200 \ ``` Full-parameter: ```shell # Experimental
+Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5 hours
+CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --dataset
+blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir output
+\ --eval_steps 500 \ ``` #### Model Parallel Training ```shell # Experimental
+Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB # Runtime: 3.4
+hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type qwen1half-7b-chat \ -
+-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --
+output_dir output \ ``` #### Data Parallel Training ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB # Runtime: 0.8 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
+Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
+Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ ``` #### Deepspeed Training ZeRO2: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB # Runtime: 0.9 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ --deepspeed default-zero2 \ ``` ZeRO3:
+```shell # Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 *
+19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+default-zero3 \ ``` ### Inference Original model: ```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
+infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
+CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
+ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
+infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
+CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset
+mmlu ceval ``` ### Export Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
+export --model_type qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ```
+LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/
+checkpoint-xxx --load_dataset_config true \ --quant_method awq --quant_bits 4 \
+--merge_lora true \ ``` ### Deployment Original model: ```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
+ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
+chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
+CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
+ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
+checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
+``` ### Supported Models #### LLMs | Model Type | Model Introduction | Language
+| Model Size | Model Type | |------------------------------------------------|-
+-----------------------------------------------------------------------|-------
+-------------|----------------------------------------|------------------------
+------------------- | | Qwen
+Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
+Chinese
+English | 0.5B-72B
+including quantized versions | base model
+chat model
+MoE model | | ChatGLM2
+ChatGLM3
+Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
+English | 6B | base model
+chat model
+code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
+github.com/baichuan-inc) | Chinese
+English | 7B-13B
+including quantized versions | base model
+chat model | | Yuan2 | [Langchao Yuan series models](https://github.com/IEIT-
+Yuan) | Chinese
+English | 2B-102B | instruct model | | XVerse | [XVerse series models](https://
+github.com/xverse-ai) | Chinese
+English | 7B-65B | base model
+chat model
+long text model
+MoE model | | LLaMA2 | [LLaMA2 series models](https://github.com/
+facebookresearch/llama) | English | 7B-70B
+including quantized versions | base model
+chat model | | Mistral
+Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
+English | 7B-22B | base model
+instruct model
+MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
+Chinese
+English | 6B-34B | base model
+chat model
+long text model | | InternLM
+InternLM2
+InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
+InternLM/InternLM) | Chinese
+English | 1.8B-20B | base model
+chat model
+math model | | DeepSeek
+DeepSeek-MoE
+DeepSeek-Coder
+DeepSeek-Math | [DeepSeek series models](https://github.com/deepseek-ai) |
+Chinese
+English | 1.3B-67B | base model
+chat model
+MoE model
+code model
+math model | | MAMBA | [MAMBA temporal convolution model](https://github.com/
+state-spaces/mamba) | English | 130M-2.8B | base model | | Gemma | [Google
+Gemma series models](https://github.com/google/gemma_pytorch) | English | 2B-7B
+| base model
+instruct model | | MiniCPM | [OpenBmB MiniCPM series models](https://
+github.com/OpenBMB/MiniCPM) | Chinese
+English | 2B-3B | chat model
+MoE model | | OpenBuddy | [OpenBuddy series models](https://github.com/
+OpenBuddy/OpenBuddy) | Chinese
+English | 7B-67B | base model
+chat model | | Orion | [OrionStar AI series models](https://github.com/
+OrionStarAI) | Chinese
+English | 14B | base model
+chat model | | BlueLM | [VIVO BlueLM large model](https://github.com/vivo-ai-
+lab/BlueLM) | Chinese
+English | 7B | base model
+chat model | | Ziya2 | [Fengshenbang series models](https://github.com/IDEA-
+CCNL/Fengshenbang-LM) | Chinese
+English | 13B | base model
+chat model | | Skywork | [Skywork series models](https://github.com/SkyworkAI/
+Skywork) | Chinese
+English | 13B | base model
+chat model | | Zephyr | Zephyr series models based on Mistral | English | 7B |
+chat model | | PolyLM | [Tongyi Lab self-developed PolyLM series models](https:
+//github.com/DAMO-NLP-MT/PolyLM) | Multilingual | 13B | base model | | SeqGPT |
+[Tongyi Lab self-developed text understanding model for information extraction
+and text classification](https://github.com/Alibaba-NLP/SeqGPT) | Chinese |
+560M | semantic understanding model | | SUS | [Southern University of Science
+and Technology model fine-tuned on YI](https://github.com/SUSTech-IDEA/SUS-
+Chat) | Chinese
+English | 34B | chat model | | Tongyi-Finance | [Tongyi finance series models]
+(https://github.com/QwenLM/Qwen) | Chinese
+English | 14B | base model
+chat model
+financial model | | CodeFuse-CodeLLaMA
+CodeFuse-Codegeex2
+CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai) |
+Chinese
+English | 6B-34B | chat model
+code model | | phi2 | Microsoft's PHI2 model | English | 3B | base model
+code model | | Grok | [X-ai](https://github.com/xai-org/grok-1) | English |
+300B | base model | | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat)
+| Chinese
+English | 7B-12B | chat model | | dbrx | [databricks](https://github.com/
+databricks/dbrx) | English | 132B | base model
+chat model | | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) |
+Chinese
+English | 13B | base model | | c4ai-command-r | [c4ai](https://cohere.com/
+command) | Multilingual | 35B-104B | chat model | #### MLLMs | Model Type |
+Model Introduction | Language | Model Size | Model Type | |------------------|-
+-----------------------------------------------------------------------|-------
+-------------|-------------------|------------------- | | Qwen-VL | [Tongyi
+Qwen vision model](https://github.com/QwenLM) | Chinese
+English | 7B
+including quantized versions | base model
+chat model | | Qwen-Audio | [Tongyi Qwen speech model](https://github.com/
+QwenLM) | Chinese
+English | 7B | base model
+chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
+ai) | Chinese
+English | 6B-34B | chat model | | XComposer2 | [Pujiang AI Lab InternLM vision
+model](https://github.com/InternLM/InternLM) | Chinese
+English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
+(https://github.com/deepseek-ai) | Chinese
+English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
+(https://github.com/OpenBMB/MiniCPM) | Chinese
+English | 3B | chat model | | CogVLM
+CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
+) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
+github.com/haotian-liu/LLaVA) | English | 7B | chat model | #### Diffusion
+Models | Model Type | Model Introduction | Language | Model Type | |-----------
+----------|--------------------------------------------------------------------
+--|----------|------------------ | | AnimateDiff | [AnimateDiff animation
+model](https://github.com/guoyww/AnimateDiff) | English | text-to-video | |
+SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models](https://github.com/
+Stability-AI) | English | text-to-image | ### Supported Open Source Datasets |
+Dataset Type | Training Task | Documentation | |--------------|:---------------
+|--------------------------------------------------------------- | | General |
+Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en
+(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh,
+cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-
+zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-
+gpt4, ð¥sharegpt-gpt4-mini. | | Agent | Fine-tuning | ð¥ms-agent, ms-agent-
+for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh,
+damo-agent-zh, agent-instruct-all-en. | | General | Human Alignment | ð¥hh-
+rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base,
+hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-
+attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-
+harmless-base-en, hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-
+alpaca-en, ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-
+instruction-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-
+mini-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh,
+tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-
+math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en,
+ð¥sql-create-context-en. | | Text Generation | Fine-tuning | ð¥advertise-
+gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh,
+ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | |
+Quantization Assist | Quantization | pileval. | | Other | Fine-tuning |
+finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-
+jave-zh. | | Vision | Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2,
+capcha-images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. |
+### Supported Technologies | Technology Name | |-------------------------------
+-------------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF
+LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
+Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
+2402.12354.pdf) | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
+Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
+Efficient and Controllable Image Diffusion Generation via Skip Connection
+Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
+2312.11392) \| [Project Page](https://scedit.github.io/) > | | ð¥NEFTune:
+[Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/
+2310.05914) | | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large
+Language Models](https://arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient
+Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/
+2309.12307) | | ROME: [Rank-One Editing of Encoder-Decoder Models](https://
+arxiv.org/abs/2211.13317) | | Adapter: [Parameter-Efficient Transfer Learning
+for NLP](http://arxiv.org/abs/1902.00751) | | Prompt Tuning: [Visual Prompt
+Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline
+for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/
+1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
+Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
+[arXiv](https://arxiv.org/abs/2310.19859) \| [Project Page](https://res-
+tuning.github.io/) \| [Usage](docs/source/GetStarted/ResTuning.md) > | | Tuners
+provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA,
+etc. | ### Supported Hardware | Hardware Environment | Notes | |---------------
+-----------------|-------------------------------------------------| | CPU | |
+| RTX 20/30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used |
+| Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | |
+Computing cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend
+NPU | | ## ð Documentation ### Documentation Compiling ```shell make docs #
+Check docs/build/html/index.html in web-browser ``` ### User Guide | Document
+Name | | ------------------------------------------------------------ | |
+[Using Web-UI](docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/
+source_en/GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-
+fine-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | |
+[LLM Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
+(docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
+Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
+Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
+Documentation | Document Name | | ---------------------------------------------
+--------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
+parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
+Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
+Supported-models-datasets.md) | | [Runtime Speed and Memory Benchmark](https://
+github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) | ### Best
+Practices | Best Practices Name | | -------------------------------------------
+----------------- | | [Agent Fine-Tuning Best Practice](https://github.com/
+modelscope/swift/blob/main/docs/source/LLM/
+Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | | [Self-
+Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/
+main/docs/source/LLM/
+%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md)
+| | [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/
+source/LLM/
+Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | |
+[Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/
+blob/main/docs/source/Multi-Modal/index.md) | ### Deep Learning Tutorials |
+Tutorial Name | |-------------------------------------------------------------
+- | | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-
+classroom/blob/main/LLM-tutorial/
+A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
+| | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
+blob/main/LLM-tutorial/
+B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
+| | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
+blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
+prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+D.Transformer%E7%BB%93%E6%9E%84.md) | | [Training Technique Selection](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+E.%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B.md) | | [Data Preprocessing](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+F.%E6%95%B0%E6%8D%AE%E9%A2%84%E5%A4%84%E7%90%86.md) | | [Quantization](https://
+github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+G.%E9%87%8F%E5%8C%96.md) | | [Training](https://github.com/modelscope/
+modelscope-classroom/blob/main/LLM-tutorial/H.%E8%AE%AD%E7%BB%83.md) | |
+[Inference](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-
+tutorial/
+I.LLM%E5%92%8C%E5%A4%9A%E6%A8%A1%E6%80%81%E6%A8%A1%E5%9E%8B%E9%AB%98%E6%95%88%E6%8E%A8%E7%90%86%E5%AE%9E%E8%B7%B5.md)
+| | [Deployment](https://github.com/modelscope/modelscope-classroom/blob/main/
+LLM-tutorial/J.%E9%83%A8%E7%BD%B2.md) | | [Evaluation](https://github.com/
+modelscope/modelscope-classroom/blob/main/LLM-tutorial/
+K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98-
+-LLM%20Automatic%20Evaluation.md) | ## ð License This framework is licensed
+under the [Apache License (Version 2.0)](https://github.com/modelscope/
+modelscope/blob/master/LICENSE). For models and datasets, please refer to the
+original resource page and follow the corresponding License. ## ð Citation
+```bibtex @Misc{swift, title = {SWIFT:Scalable lightWeight Infrastructure for
+Fine-Tuning}, author = {The ModelScope Team}, howpublished = {\url{https://
+github.com/modelscope/swift}}, year = {2024} } ``` ## â Contact Us You can
+contact us and communicate with us by adding our WeChat group:
 [asset/wechat.png]
 ## Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/
 swift&Date) Keywords: python,petl,efficient tuners Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: llm Provides-Extra: aigc Provides-Extra: all
+Extra: llm Provides-Extra: aigc Provides-Extra: eval Provides-Extra: all
```

### Comparing `ms-swift-1.7.3/ms_swift.egg-info/SOURCES.txt` & `ms-swift-2.0.0/ms_swift.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 ms_swift.egg-info/dependency_links.txt
 ms_swift.egg-info/entry_points.txt
 ms_swift.egg-info/not-zip-safe
 ms_swift.egg-info/requires.txt
 ms_swift.egg-info/top_level.txt
 requirements/aigc.txt
 requirements/docs.txt
+requirements/eval.txt
 requirements/framework.txt
 requirements/llm.txt
 requirements/tests.txt
 swift/__init__.py
+swift/torchacc_utils.py
 swift/version.py
 swift/aigc/__init__.py
 swift/aigc/animatediff.py
 swift/aigc/animatediff_infer.py
 swift/aigc/diffusers/__init__.py
 swift/aigc/diffusers/infer_controlnet.py
 swift/aigc/diffusers/infer_controlnet_sdxl.py
@@ -40,14 +42,15 @@
 swift/aigc/diffusers/train_text_to_image_sdxl.py
 swift/aigc/utils/__init__.py
 swift/aigc/utils/argument.py
 swift/cli/__init__.py
 swift/cli/app_ui.py
 swift/cli/deploy.py
 swift/cli/dpo.py
+swift/cli/eval.py
 swift/cli/export.py
 swift/cli/infer.py
 swift/cli/main.py
 swift/cli/merge_lora.py
 swift/cli/sft.py
 swift/cli/web_ui.py
 swift/hub/__init__.py
@@ -60,17 +63,19 @@
 swift/hub/push_to_hub.py
 swift/hub/repository.py
 swift/hub/snapshot_download.py
 swift/hub/utils/__init__.py
 swift/hub/utils/caching.py
 swift/hub/utils/utils.py
 swift/llm/__init__.py
+swift/llm/accelerator.py
 swift/llm/app_ui.py
 swift/llm/deploy.py
 swift/llm/dpo.py
+swift/llm/eval.py
 swift/llm/export.py
 swift/llm/infer.py
 swift/llm/rome.py
 swift/llm/sft.py
 swift/llm/tuner.py
 swift/llm/agent/__init__.py
 swift/llm/agent/utils.py
```

### Comparing `ms-swift-1.7.3/ms_swift.egg-info/requires.txt` & `ms-swift-2.0.0/ms_swift.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 accelerate
 dacite
 datasets
 jieba
 matplotlib
-modelscope>=1.9.3
+modelscope>=1.13.3
 nltk
 numpy
 optimum>=1.17.0
 pandas
-peft<0.10.0,>=0.9.0
+peft<0.11.0,>=0.9.0
 requests
 rouge
 safetensors
 tensorboard
 tqdm
-transformers<4.39,>=4.33
+transformers<4.41,>=4.33
 transformers_stream_generator
 trl>=0.7.7
 
 [aigc]
 decord
 diffusers==0.25.0
 einops
@@ -26,39 +26,43 @@
 
 [all]
 accelerate
 dacite
 datasets
 jieba
 matplotlib
-modelscope>=1.9.3
+modelscope>=1.13.3
 nltk
 numpy
 optimum>=1.17.0
 pandas
-peft<0.10.0,>=0.9.0
+peft<0.11.0,>=0.9.0
 requests
 rouge
 safetensors
 tensorboard
 tqdm
-transformers<4.39,>=4.33
+transformers<4.41,>=4.33
 transformers_stream_generator
 trl>=0.7.7
 charset_normalizer
 cpm_kernels
 fastapi
 gradio>=3.40.0
 sentencepiece
 tiktoken
 uvicorn
 decord
 diffusers==0.25.0
 einops
 torchvision
+llmuses>=0.3.0
+
+[eval]
+llmuses>=0.3.0
 
 [llm]
 charset_normalizer
 cpm_kernels
 fastapi
 gradio>=3.40.0
 sentencepiece
```

### Comparing `ms-swift-1.7.3/setup.cfg` & `ms-swift-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 quiet-level = 3
 ignore-words-list = patten,nd,ty,mot,hist,formating,winn,gool,datas,wan,confids
 
 [flake8]
 max-line-length = 120
 select = B,C,E,F,P,T4,W,B9
 ignore = F401,F403,F405,F821,W503,E251,W504
-exclude = docs/src,*.pyi,.git
+exclude = docs/src,*.pyi,.git,peft.py
 
 [darglint]
 ignore = DAR101
 
 [easy_install]
 index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```

### Comparing `ms-swift-1.7.3/setup.py` & `ms-swift-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,19 @@
 
 if __name__ == '__main__':
     install_requires, deps_link = parse_requirements('requirements.txt')
     extra_requires = {}
     all_requires = []
     extra_requires['llm'], _ = parse_requirements('requirements/llm.txt')
     extra_requires['aigc'], _ = parse_requirements('requirements/aigc.txt')
+    extra_requires['eval'], _ = parse_requirements('requirements/eval.txt')
     all_requires.extend(install_requires)
     all_requires.extend(extra_requires['llm'])
     all_requires.extend(extra_requires['aigc'])
+    all_requires.extend(extra_requires['eval'])
     extra_requires['all'] = all_requires
 
     setup(
         name='ms-swift',
         version=get_version(),
         description=
         'Swift: Scalable lightWeight Infrastructure for Fine-Tuning',
```

### Comparing `ms-swift-1.7.3/swift/__init__.py` & `ms-swift-2.0.0/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/__init__.py` & `ms-swift-2.0.0/swift/aigc/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/animatediff.py` & `ms-swift-2.0.0/swift/aigc/animatediff.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/animatediff_infer.py` & `ms-swift-2.0.0/swift/aigc/animatediff_infer.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/__init__.py` & `ms-swift-2.0.0/swift/aigc/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_controlnet.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_controlnet_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth_lora.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_lora.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/infer_text_to_image_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_controlnet.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_controlnet_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth_lora.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_lora.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/diffusers/train_text_to_image_sdxl.py` & `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/aigc/utils/argument.py` & `ms-swift-2.0.0/swift/aigc/utils/argument.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/cli/main.py` & `ms-swift-2.0.0/swift/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     'sft': 'swift.cli.sft',
     'infer': 'swift.cli.infer',
     'app-ui': 'swift.cli.app_ui',
     'merge-lora': 'swift.cli.merge_lora',
     'web-ui': 'swift.cli.web_ui',
     'deploy': 'swift.cli.deploy',
     'dpo': 'swift.cli.dpo',
-    'export': 'swift.cli.export'
+    'export': 'swift.cli.export',
+    'eval': 'swift.cli.eval'
 }
 
 ROUTE_MAPPING.update(
     {k.replace('-', '_'): v
      for k, v in ROUTE_MAPPING.items()})
```

### Comparing `ms-swift-1.7.3/swift/hub/api.py` & `ms-swift-2.0.0/swift/hub/api.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/check_model.py` & `ms-swift-2.0.0/swift/hub/check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/constants.py` & `ms-swift-2.0.0/swift/hub/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/errors.py` & `ms-swift-2.0.0/swift/hub/errors.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/file_download.py` & `ms-swift-2.0.0/swift/hub/file_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/git.py` & `ms-swift-2.0.0/swift/hub/git.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/push_to_hub.py` & `ms-swift-2.0.0/swift/hub/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/repository.py` & `ms-swift-2.0.0/swift/hub/repository.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/snapshot_download.py` & `ms-swift-2.0.0/swift/hub/snapshot_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/utils/caching.py` & `ms-swift-2.0.0/swift/hub/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/hub/utils/utils.py` & `ms-swift-2.0.0/swift/hub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/__init__.py` & `ms-swift-2.0.0/swift/llm/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from .app_ui import gradio_chat_demo, gradio_generation_demo, app_ui_main
     from .deploy import deploy_main
     from .dpo import dpo_main
     from .infer import merge_lora, prepare_model_template, infer_main, merge_lora_main
     from .rome import rome_main
     from .sft import sft_main
     from .export import export_main
+    from .eval import eval_main
 else:
     _extra_objects = {
         k: v
         for k, v in globals().items() if not k.startswith('_')
     }
     _import_structure = {
         'app_ui':
@@ -26,14 +27,15 @@
         'infer': [
             'merge_lora', 'prepare_model_template', 'infer_main',
             'merge_lora_main'
         ],
         'rome': ['rome_main'],
         'sft': ['sft_main'],
         'export': ['export_main'],
+        'eval': ['eval_main'],
     }
 
     import sys
 
     sys.modules[__name__] = _LazyModule(
         __name__,
         globals()['__file__'],
```

### Comparing `ms-swift-1.7.3/swift/llm/app_ui.py` & `ms-swift-2.0.0/swift/llm/app_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
-from typing import Tuple
+from typing import Iterator, Tuple
 
 from swift.utils import get_logger, get_main
 from .infer import merge_lora, prepare_model_template
 from .utils import (AppUIArguments, History, inference_stream,
                     limit_history_length)
 
 logger = get_logger()
@@ -17,15 +17,15 @@
     import gradio as gr
     if args.infer_backend == 'vllm':
         from swift.llm import prepare_vllm_engine_template, inference_stream_vllm, inference_vllm
         llm_engine, template = prepare_vllm_engine_template(args)
     else:
         model, template = prepare_model_template(args)
 
-    def model_generation(query: str) -> str:
+    def model_generation(query: str) -> Iterator[str]:
         if args.infer_backend == 'vllm':
             gen = inference_stream_vllm(llm_engine, template, [{
                 'query': query
             }])
             for resp_list in gen:
                 response = resp_list[0]['response']
                 yield response
@@ -60,15 +60,16 @@
     import gradio as gr
     if args.infer_backend == 'vllm':
         from swift.llm import prepare_vllm_engine_template, inference_stream_vllm
         llm_engine, template = prepare_vllm_engine_template(args)
     else:
         model, template = prepare_model_template(args)
 
-    def model_chat(query: str, history: History) -> Tuple[str, History]:
+    def model_chat(query: str,
+                   history: History) -> Iterator[Tuple[str, History]]:
         old_history, history = limit_history_length(template, query, history,
                                                     args.max_length)
         if args.infer_backend == 'vllm':
             gen = inference_stream_vllm(llm_engine, template,
                                         [{
                                             'query': query,
                                             'history': history
```

### Comparing `ms-swift-1.7.3/swift/llm/data/self_cognition.jsonl` & `ms-swift-2.0.0/swift/llm/data/self_cognition.jsonl`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/deploy.py` & `ms-swift-2.0.0/swift/llm/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                     ChatCompletionResponseStreamChoice,
                     ChatCompletionStreamResponse, ChatMessage,
                     CompletionRequest, CompletionResponse,
                     CompletionResponseChoice, CompletionResponseStreamChoice,
                     CompletionStreamResponse, DeltaMessage, DeployArguments,
                     Model, ModelList, UsageInfo, inference, inference_stream,
                     messages_to_history, random_uuid)
+from .utils.utils import _get_safe_print_idx
 
 logger = get_logger()
 
 app = FastAPI()
 _args = None
 model = None
 llm_engine = None
@@ -37,15 +38,22 @@
     status_code = int(status_code)
     return JSONResponse({'message': message, 'object': 'error'}, status_code)
 
 
 @app.get('/v1/models')
 async def get_available_models():
     global _args
-    return ModelList(data=[Model(id=_args.model_type)])
+    model_list = [_args.model_type]
+    if _args.vllm_lora_request_list is not None:
+        model_list += [
+            lora_request.lora_name
+            for lora_request in _args.vllm_lora_request_list
+        ]
+    data = [Model(id=model_id) for model_id in model_list]
+    return ModelList(data=data)
 
 
 async def check_length(request: Union[ChatCompletionRequest,
                                       CompletionRequest],
                        input_ids: List[int]) -> Optional[str]:
     global llm_engine, model, _args
     if _args.infer_backend == 'vllm':
@@ -83,15 +91,15 @@
     else:
         return False
 
 
 async def inference_vllm_async(request: Union[ChatCompletionRequest,
                                               CompletionRequest],
                                raw_request: Request):
-    global llm_engine, template
+    global llm_engine, template, _args
     from .utils import VllmGenerationConfig
     error_msg = await check_model(request)
     if error_msg is not None:
         return create_error_response(HTTPStatus.BAD_REQUEST, error_msg)
 
     if request.seed is not None:
         seed_everything(request.seed, verbose=False)
@@ -150,16 +158,27 @@
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
     request_info['generation_config'] = generation_config
     request_info.update({'seed': request.seed, 'stream': request.stream})
     logger.info(request_info)
 
     created_time = int(time.time())
+    generate_kwargs = {}
+    if _args.vllm_enable_lora and request.model != _args.model_type:
+        lora_request = None
+        for lora_req in _args.vllm_lora_request_list:
+            if lora_req.lora_name == request.model:
+                lora_request = lora_req
+                break
+        assert lora_request is not None, (
+            f"request.model: '{request.model}', "
+            f'available_models: {await get_available_models()}')
+        generate_kwargs['lora_request'] = lora_request
     result_generator = llm_engine.generate(None, generation_config, request_id,
-                                           input_ids)
+                                           input_ids, **generate_kwargs)
 
     async def _generate_full():
         result = None
         async for result in result_generator:
             if await raw_request.is_disconnected():
                 await llm_engine.abort(request_id)
                 return create_error_response(HTTPStatus.BAD_REQUEST,
@@ -219,16 +238,19 @@
                 completion_tokens=num_generated_tokens,
                 total_tokens=num_prompt_tokens + num_generated_tokens,
             )
             if isinstance(request, ChatCompletionRequest):
                 choices = []
                 for output in result.outputs:
                     text = template.tokenizer.decode(output.token_ids, True)
-                    delta_text = text[print_idx_list[output.index]:]
-                    print_idx_list[output.index] += len(delta_text)
+                    new_print_idx = _get_safe_print_idx(
+                        text, print_idx_list[output.index], output.finished())
+                    delta_text = text[print_idx_list[output.
+                                                     index]:new_print_idx]
+                    print_idx_list[output.index] = new_print_idx
                     choice = ChatCompletionResponseStreamChoice(
                         index=output.index,
                         delta=DeltaMessage(
                             role='assistant', content=delta_text),
                         finish_reason=output.finish_reason)
                     choices.append(choice)
                 response = ChatCompletionStreamResponse(
@@ -237,16 +259,19 @@
                     usage=usage_info,
                     id=request_id,
                     created=created_time)
             else:
                 choices = []
                 for output in result.outputs:
                     text = template.tokenizer.decode(output.token_ids, True)
-                    delta_text = text[print_idx_list[output.index]:]
-                    print_idx_list[output.index] += len(delta_text)
+                    new_print_idx = _get_safe_print_idx(
+                        text, print_idx_list[output.index], output.finished())
+                    delta_text = text[print_idx_list[output.
+                                                     index]:new_print_idx]
+                    print_idx_list[output.index] = new_print_idx
                     choice = CompletionResponseStreamChoice(
                         index=output.index,
                         text=delta_text,
                         finish_reason=output.finish_reason)
                     choices.append(choice)
                 response = CompletionStreamResponse(
                     model=request.model,
```

### Comparing `ms-swift-1.7.3/swift/llm/dpo.py` & `ms-swift-2.0.0/swift/llm/dpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from transformers import IntervalStrategy
 from transformers.integrations import is_deepspeed_zero3_enabled
 
 from swift.trainers.dpo_trainers import DPOTrainer
 from swift.utils import (check_json_format, get_dist_setting, get_logger,
                          get_main, get_model_info, is_ddp_plus_mp, is_dist,
                          is_master, plot_images, seed_everything, show_layers)
+from . import get_time_info
 from .tuner import prepare_model
 from .utils import (DPOArguments, Template, get_dataset, get_model_tokenizer,
                     get_template, set_generation_config)
 
 logger = get_logger()
 
 
@@ -53,17 +54,20 @@
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=args.model_id_or_path,
         **kwargs)
     if args.ref_model_type is not None:
-        ref_model, _ = get_model_tokenizer(args.ref_model_type,
-                                           args.torch_dtype, model_kwargs,
-                                           **kwargs)
+        ref_model, _ = get_model_tokenizer(
+            args.ref_model_type,
+            args.torch_dtype,
+            model_kwargs,
+            model_id_or_path=args.ref_model_id_or_path,
+            **kwargs)
     else:
         ref_model = None
 
     logger.info(f'model_config: {model.config}')
     if hasattr(model, 'hf_device_map'):
         logger.info(f'model device_map {model.hf_device_map}')
     generation_config = GenerationConfig(
@@ -173,26 +177,34 @@
     logger.info(f'The logging file will be saved in: {logging_path}')
     trainer.train(training_args.resume_from_checkpoint)
     last_model_checkpoint = getattr(trainer.state, 'last_model_checkpoint',
                                     None)
     logger.info(f'last_model_checkpoint: {last_model_checkpoint}')
     logger.info(
         f'best_model_checkpoint: {trainer.state.best_model_checkpoint}')
+    train_time = get_time_info(trainer.state.log_history, len(train_dataset))
     # Visualization
     if is_master():
         images_dir = os.path.join(args.output_dir, 'images')
         logger.info(f'images_dir: {images_dir}')
         plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
         if args.push_to_hub:
             trainer._add_patterns_to_gitignore(['images/'])
             trainer.push_to_hub()
-    return {
+    run_info = {
+        'memory': trainer.perf['memory'],
+        'train_time': train_time,
         'last_model_checkpoint': last_model_checkpoint,
         'best_model_checkpoint': trainer.state.best_model_checkpoint,
         'best_metric': trainer.state.best_metric,
         'global_step': trainer.state.global_step,
         'log_history': trainer.state.log_history,
         'model_info': model_info,
+        'dataset_info': trainer.dataset_info,
     }
+    jsonl_path = os.path.join(args.output_dir, 'logging.jsonl')
+    with open(jsonl_path, 'a', encoding='utf-8') as f:
+        f.write(json.dumps(run_info) + '\n')
+    return run_info
 
 
 dpo_main = get_main(DPOArguments, llm_dpo)
```

### Comparing `ms-swift-1.7.3/swift/llm/ds_config/zero2.json` & `ms-swift-2.0.0/swift/llm/ds_config/zero2.json`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/ds_config/zero3.json` & `ms-swift-2.0.0/swift/llm/ds_config/zero3.json`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/export.py` & `ms-swift-2.0.0/swift/llm/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from modelscope import GenerationConfig
 from transformers import AwqConfig, PreTrainedModel
 
 from swift.utils import (get_logger, get_main, get_model_info, push_to_ms_hub,
                          seed_everything, show_layers)
 from .infer import merge_lora, prepare_model_template, save_checkpoint
 from .utils import (ExportArguments, Template, get_dataset,
-                    get_model_tokenizer, get_template, set_generation_config)
+                    get_model_tokenizer, get_template, set_generation_config,
+                    swift_to_peft_format)
 
 logger = get_logger()
 
 
 def prepare_awq_model_template(
         args: ExportArguments) -> Tuple[PreTrainedModel, Template]:
     from awq import AutoAWQForCausalLM
@@ -154,14 +155,17 @@
     quantizer.get_dataset = _origin_get_dataset  # recover
     return gptq_quantizer
 
 
 def llm_export(args: ExportArguments) -> None:
     global _args, template
     logger.info(f'args: {args}')
+    if args.to_peft_format:
+        assert args.sft_type == 'lora'
+        args.ckpt_dir = swift_to_peft_format(args.ckpt_dir)
     if args.merge_lora:
         merge_lora(args, device_map=args.merge_device_map)
     if args.quant_bits > 0:
         _args = args
         assert args.quantization_bit == 0
         assert args.sft_type == 'full', 'you need to merge lora'
         if args.dtype == 'AUTO' and args.torch_dtype is None:
```

### Comparing `ms-swift-1.7.3/swift/llm/infer.py` & `ms-swift-2.0.0/swift/llm/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,20 @@
 
     for fname in fname_list:
         tgt_path = os.path.join(target_dir, fname)
         for model_dir in [ckpt_dir, model_cache_dir]:
             if model_dir is None:
                 continue
             src_path = os.path.join(model_dir, fname)
-            if os.path.exists(src_path):
+            if os.path.isfile(src_path):
                 shutil.copy(src_path, tgt_path)
                 break
+            elif os.path.isdir(src_path):
+                shutil.copytree(src_path, tgt_path)
+                break
     # configuration.json
     configuration_fname = 'configuration.json'
     new_configuration_path = os.path.join(target_dir, configuration_fname)
     for model_dir in [ckpt_dir, model_cache_dir]:
         if model_dir is None:
             continue
         old_configuration_path = os.path.join(model_dir, configuration_fname)
@@ -250,14 +253,18 @@
         from .utils import prepare_vllm_engine_template, inference_stream_vllm, inference_vllm
         llm_engine, template = prepare_vllm_engine_template(args)
     else:
         model, template = prepare_model_template(args)
         if args.overwrite_generation_config:
             assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
             model.generation_config.save_pretrained(args.ckpt_dir)
+    lora_request = None
+    if args.vllm_enable_lora:
+        assert len(args.vllm_lora_request_list) == 1
+        lora_request = args.vllm_lora_request_list[0]
     # Inference
     result = []
     jsonl_path = None
     if args.save_result and args.ckpt_dir is not None:
         time = dt.datetime.now().strftime('%Y%m%d-%H%M%S')
         jsonl_path = os.path.join(args.ckpt_dir, f'infer_result_{time}.jsonl')
     if args.eval_human:
@@ -321,27 +328,33 @@
             if args.infer_backend == 'vllm':
                 request_list = [{
                     'query': query,
                     'history': history,
                     'system': system
                 }]
                 if args.stream:
-                    gen = inference_stream_vllm(llm_engine, template,
-                                                request_list)
+                    gen = inference_stream_vllm(
+                        llm_engine,
+                        template,
+                        request_list,
+                        lora_request=lora_request)
                     print_idx = 0
                     for resp_list in gen:
                         response = resp_list[0]['response']
                         new_history = resp_list[0]['history']
                         if len(response) > print_idx:
                             print(response[print_idx:], end='', flush=True)
                             print_idx = len(response)
                     print()
                 else:
-                    resp_list = inference_vllm(llm_engine, template,
-                                               request_list)
+                    resp_list = inference_vllm(
+                        llm_engine,
+                        template,
+                        request_list,
+                        lora_request=lora_request)
                     response = resp_list[0]['response']
                     new_history = resp_list[0]['history']
                     print(response)
             else:
                 if args.stop_words:
                     infer_kwargs['stop_words'] = args.stop_words
                 if args.stream:
@@ -428,15 +441,18 @@
                     kwargs['system'] = system
                 if images is not None:
                     kwargs['images'] = images
                 if args.infer_backend == 'vllm':
                     assert args.stream is True
                     if args.verbose:
                         print(f"[QUERY]{data['query']}\n[RESPONSE]", end='')
-                    gen = inference_stream_vllm(llm_engine, template, [kwargs])
+                    gen = inference_stream_vllm(
+                        llm_engine,
+                        template, [kwargs],
+                        lora_request=lora_request)
                     print_idx = 0
                     for resp_list in gen:
                         response = resp_list[0]['response']
                         if args.verbose and len(response) > print_idx:
                             print(response[print_idx:], end='', flush=True)
                             print_idx = len(response)
                     print()
@@ -458,12 +474,16 @@
                     print()
                     print(f'[LABELS]{label}')
                     if images is not None:
                         print(f'[IMAGES]{images}')
                     print('-' * 50)
     if args.save_result and args.ckpt_dir is not None:
         logger.info(f'save_result_path: {jsonl_path}')
+    if args.val_dataset_sample == 10:  # is default
+        logger.info(
+            'You can set `--val_dataset_sample -1` to perform inference on the entire dataset.'
+        )
     return {'result': result}
 
 
 infer_main = get_main(InferArguments, llm_infer)
 merge_lora_main = get_main(InferArguments, merge_lora)
```

### Comparing `ms-swift-1.7.3/swift/llm/rome.py` & `ms-swift-2.0.0/swift/llm/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/sft.py` & `ms-swift-2.0.0/swift/llm/sft.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 import torch
 from modelscope import BitsAndBytesConfig, GenerationConfig
 from transformers import IntervalStrategy
 from transformers.integrations import is_deepspeed_zero3_enabled
 from transformers.utils import is_torch_npu_available
 
 from swift.trainers import Seq2SeqTrainer
+from swift.trainers.utils import can_return_loss, find_labels
 from swift.utils import (check_json_format, compute_acc_metrics,
                          compute_nlg_metrics, get_dist_setting, get_logger,
                          get_main, get_model_info, is_ddp_plus_mp, is_dist,
                          is_master, plot_images, preprocess_logits_for_metrics,
-                         seed_everything, show_layers)
+                         seed_everything, show_layers, use_torchacc)
+from .accelerator import ta_accelerate
 from .tuner import prepare_model
 from .utils import (TEMPLATE_MAPPING, LazyLLMDataset, SftArguments, Template,
                     add_self_cognition_dataset, dataset_map, get_dataset,
                     get_model_tokenizer, get_template, get_time_info,
                     print_example, set_generation_config, sort_by_max_length,
                     stat_dataset)
 from .utils.argument import handle_dataset_mixture
@@ -36,31 +38,32 @@
     else:
         print(f'device_count: {torch.cuda.device_count()}')
     rank, local_rank, world_size, local_world_size = get_dist_setting()
     print(f'rank: {rank}, local_rank: {local_rank}, '
           f'world_size: {world_size}, local_world_size: {local_world_size}')
     seed_everything(args.seed)
 
-    if args.gpu_memory_fraction:
+    if args.gpu_memory_fraction is not None:
         for device_id in range(torch.cuda.device_count()):
             torch.cuda.set_per_process_memory_fraction(
                 max(min(args.gpu_memory_fraction, 1.0), 0.01),
                 device=device_id)
 
     # Loading Model and Tokenizer
     if is_torch_npu_available():
         model_kwargs = {'device_map': local_rank if local_rank >= 0 else 0}
     elif is_deepspeed_zero3_enabled():
         model_kwargs = {'device_map': None}
     else:
         model_kwargs = {'low_cpu_mem_usage': True}
         if is_dist() and not is_ddp_plus_mp():
             model_kwargs['device_map'] = {'': local_rank}
-        else:
+        elif not use_torchacc():
             model_kwargs['device_map'] = 'auto'
+
     if args.load_in_8bit or args.load_in_4bit:
         quantization_config = BitsAndBytesConfig(
             args.load_in_8bit,
             args.load_in_4bit,
             bnb_4bit_compute_dtype=args.bnb_4bit_compute_dtype,
             bnb_4bit_quant_type=args.bnb_4bit_quant_type,
             bnb_4bit_use_double_quant=args.bnb_4bit_use_double_quant)
@@ -73,15 +76,14 @@
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=args.model_id_or_path,
         is_training=True,
         **kwargs)
-    # logger.info(f'device_map: {dict(model.hf_device_map)}')
     logger.info(f'model_config: {model.config}')
     generation_config = GenerationConfig(
         max_new_tokens=args.max_new_tokens,
         temperature=args.temperature,
         top_k=args.top_k,
         top_p=args.top_p,
         do_sample=args.do_sample,
@@ -89,14 +91,21 @@
         num_beams=args.num_beams,
         pad_token_id=tokenizer.pad_token_id,
         eos_token_id=tokenizer.eos_token_id)
     logger.info(f'generation_config: {generation_config}')
     set_generation_config(model, generation_config)
     training_args.generation_config = generation_config
 
+    if use_torchacc():
+        import torchacc as ta
+        # Get `label` and `return_loss` before 'ta_accelerate' because it will
+        # wrapper the model and make these properties wrong.
+        label_names = find_labels(model)
+        return_loss = can_return_loss(model)
+        model = ta.patch_qwen_model(model)
     # Preparing LoRA
     model, callbacks = prepare_model(model, args)
 
     show_layers(model)
     model_info = None
     if not is_deepspeed_zero3_enabled():
         model_info = get_model_info(model)
@@ -104,47 +113,51 @@
     logger.info(model)
 
     if args.gradient_checkpointing:
         model.config.use_cache = False  # fix transformers==4.36
         logger.info('Setting model.config.use_cache: False')
         model.enable_input_require_grads()
 
+    if use_torchacc():
+        model.config.use_cache = False
+        logger.info('Setting model.config.use_cache: False')
+        model = ta_accelerate(
+            model,
+            world_size,
+            args.model_layer_cls_name,
+            args.bf16,
+            args.fp16,
+            gradient_checkpointing=True,
+            fsdp_flatten_parameters=False)
+
     # Loading Dataset
     random_state = np.random.RandomState(args.dataset_seed)
     train_dataset, val_dataset = get_dataset(
         args.dataset,
         args.dataset_test_ratio,
         random_state,
         check_dataset_strategy=args.check_dataset_strategy)
     val_dataset_sample = args.val_dataset_sample
-    mix_dataset_sample = 0 if not args.train_dataset_mix_ratio else round(
-        len(train_dataset) * args.train_dataset_mix_ratio)
     if train_dataset is not None and args.train_dataset_sample >= 0:
-        total_dataset_sample = min(args.train_dataset_sample,
+        train_dataset_sample = min(args.train_dataset_sample,
                                    train_dataset.shape[0])
-        train_dataset_sample = total_dataset_sample
-        if args.train_dataset_mix_ratio:
-            train_dataset_sample = round(
-                1. / (1 + args.train_dataset_mix_ratio) * total_dataset_sample)
-            mix_dataset_sample = total_dataset_sample - train_dataset_sample
         if train_dataset.shape[0] > train_dataset_sample:
             logger.info(f'train_dataset_sample: {train_dataset_sample}')
             train_idxs = random_state.permutation(train_dataset_sample)
             train_dataset = train_dataset.select(train_idxs)
         if val_dataset_sample is None:
             val_dataset_sample = max(
                 int(train_dataset_sample * args.dataset_test_ratio), 1)
     if val_dataset is not None and val_dataset_sample is not None and val_dataset_sample >= 0:
         if val_dataset.shape[0] > val_dataset_sample:
             logger.info(f'val_dataset_sample: {val_dataset_sample}')
             val_idxs = random_state.permutation(val_dataset_sample)
             val_dataset = val_dataset.select(val_idxs)
 
-    train_dataset = handle_dataset_mixture(args, train_dataset,
-                                           mix_dataset_sample)
+    train_dataset = handle_dataset_mixture(args, train_dataset)
 
     # add self-cognition dataset
     if args.self_cognition_sample > 0:
         train_dataset = add_self_cognition_dataset(train_dataset,
                                                    args.self_cognition_sample,
                                                    args.model_name,
                                                    args.model_author)
@@ -189,14 +202,23 @@
         train_dataset = LazyLLMDataset(train_dataset, template)
         if val_dataset is not None:
             val_dataset = LazyLLMDataset(val_dataset, template)
 
     padding_to = args.max_length if args.sft_type == 'longlora' else None
     data_collator = partial(template.data_collator, padding_to=padding_to)
 
+    trian_batch_size = args.batch_size
+    eval_batch_size = args.eval_batch_size
+    if use_torchacc():
+        trian_batch_size *= world_size
+        eval_batch_size *= world_size
+    training_args.per_device_train_batch_size = trian_batch_size
+    training_args.per_device_eval_batch_size = eval_batch_size
+    training_args.group_by_length = use_torchacc()
+
     # Trainer
     logger.info(f'training_args: {training_args}')
 
     trainer_kwargs = {}
     if args.predict_with_generate:
         trainer_kwargs['compute_metrics'] = partial(
             compute_nlg_metrics, tokenizer=tokenizer)
@@ -215,14 +237,17 @@
         data_collator=data_collator,
         train_dataset=train_dataset,
         eval_dataset=val_dataset,
         tokenizer=tokenizer,
         callbacks=callbacks,
         **trainer_kwargs)
     trainer.sft_args = args
+    if use_torchacc():
+        trainer.label_names = label_names
+        trainer.can_return_loss = return_loss
     if is_master():
         for args_obj, fname in zip([args, training_args],
                                    ['sft_args.json', 'training_args.json']):
             fpath = os.path.join(args.output_dir, fname)
             logger.info(
                 f'The {args_obj.__class__.__name__} will be saved in: {fpath}')
             with open(fpath, 'w', encoding='utf-8') as f:
@@ -237,28 +262,44 @@
     last_model_checkpoint = getattr(trainer.state, 'last_model_checkpoint',
                                     None)
     logger.info(f'last_model_checkpoint: {last_model_checkpoint}')
     logger.info(
         f'best_model_checkpoint: {trainer.state.best_model_checkpoint}')
     train_time = get_time_info(trainer.state.log_history, len(train_dataset))
     # Visualization
-    if is_master():
+    if is_master() and not use_torchacc():
         images_dir = os.path.join(args.output_dir, 'images')
         logger.info(f'images_dir: {images_dir}')
         plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
         if args.push_to_hub:
             trainer._add_patterns_to_gitignore(['images/'])
             trainer.push_to_hub()
-    return {
+    run_info = {
         'memory': trainer.perf['memory'],
+        'gen_time': trainer.perf['gen_time'],
+        'gen_len': trainer.perf['gen_len'],
         'train_time': train_time,
         'last_model_checkpoint': last_model_checkpoint,
         'best_model_checkpoint': trainer.state.best_model_checkpoint,
         'best_metric': trainer.state.best_metric,
         'global_step': trainer.state.global_step,
         'log_history': trainer.state.log_history,
         'model_info': model_info,
         'dataset_info': dataset_info,
     }
+    jsonl_path = os.path.join(args.output_dir, 'logging.jsonl')
+    with open(jsonl_path, 'a', encoding='utf-8') as f:
+        f.write(json.dumps(run_info) + '\n')
+    return run_info
+
+
+def get_sft_main(args, llm):
+    if use_torchacc():
+        logger.warning('TorchAcc is currently only available internally '
+                       'within Alibaba Cloud.')
+        import torchacc as ta
+        # This patch should be called before `llm_sft`.
+        ta.accelerate_hf_trainer()
+    return get_main(args, llm)
 
 
-sft_main = get_main(SftArguments, llm_sft)
+sft_main = get_sft_main(SftArguments, llm_sft)
```

### Comparing `ms-swift-1.7.3/swift/llm/tuner.py` & `ms-swift-2.0.0/swift/llm/tuner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
+import os
 import types
 
 import torch
 import transformers
 from packaging import version
 
+from swift.torchacc_utils import consolidate_checkpoint
 from swift.trainers import TrainerCallback
-from swift.tuners import (AdaLoraConfig, IA3Config, LongLoRAConfig,
-                          LongLoRAModelType, LoraConfig, LoRAConfig,
-                          NEFTuneConfig, Swift)
+from swift.tuners import (AdaLoraConfig, AdapterConfig, IA3Config,
+                          LongLoRAConfig, LongLoRAModelType, LoraConfig,
+                          LoRAConfig, NEFTuneConfig, Swift)
 from swift.tuners.llamapro import LLaMAProConfig
 from swift.tuners.module_mapping import MODEL_KEYS_MAPPING
 from swift.utils import (activate_model_parameters, freeze_model_parameters,
-                         get_logger)
+                         get_logger, use_torchacc)
 from .utils import (SftArguments, find_all_linears, find_embedding, find_ln,
                     is_adapter)
 
 logger = get_logger()
 
 
 def handle_target_modules(model, args: SftArguments) -> None:
@@ -67,53 +69,40 @@
             lora_kwargs = {
                 'r': args.lora_rank,
                 'target_modules': args.lora_target_modules,
                 'lora_alpha': args.lora_alpha,
                 'lora_dropout': args.lora_dropout_p,
                 'bias': args.lora_bias_trainable,
                 'modules_to_save': args.lora_modules_to_save,
-                'layers_to_transform': args.lora_layers_to_transform,
-                'layers_pattern': args.lora_layers_pattern,
-                'rank_pattern': args.lora_rank_pattern,
-                'alpha_pattern': args.lora_alpha_pattern,
-                'loftq_config': args.lora_loftq_config,
+                'use_rslora': args.use_rslora,
                 'use_dora': args.use_dora,
+                'lorap_lr_ratio': args.lora_lr_ratio,
             }
             if args.sft_type == 'lora':
                 if args.tuner_backend == 'swift':
-                    lora_kwargs['lr_ratio'] = args.lora_lr_ratio
                     lora_config = LoRAConfig(
                         lora_dtype=args.lora_dtype, **lora_kwargs)
                 elif args.tuner_backend == 'peft':
                     lora_config = LoraConfig(
-                        task_type='CAUSAL_LM', **lora_kwargs)
+                        task_type='CAUSAL_LM',
+                        lora_dtype=args.lora_dtype,
+                        **lora_kwargs)
                 model = Swift.prepare_model(model, lora_config)
                 logger.info(f'lora_config: {lora_config}')
             elif args.sft_type == 'longlora':
                 assert args.tuner_backend == 'swift'
                 assert LongLoRAModelType.LLAMA in args.model_type
                 longlora_config = LongLoRAConfig(
                     lora_dtype=args.lora_dtype,
                     model_type=LongLoRAModelType.LLAMA,
-                    use_flash_attn=args.use_flash_attn,
                     **lora_kwargs)
                 model = Swift.prepare_model(model, longlora_config)
                 logger.info(f'longlora_config: {longlora_config}')
-            elif args.sft_type == 'qalora':
-                assert args.tuner_backend == 'swift'
-                assert getattr(
-                    model, 'quantization_method',
-                    None) == 'gptq', 'qalora must be used with auto_gptq'
-                qalora_config = LoRAConfig(
-                    lora_dtype=args.lora_dtype,
-                    use_qa_lora=True,
-                    **lora_kwargs)
-                model = Swift.prepare_model(model, qalora_config)
-                logger.info(f'qalora_config: {qalora_config}')
             elif args.sft_type == 'adalora':
+                lora_kwargs.pop('lorap_lr_ratio', None)
                 lora_kwargs['rank_pattern'] = None
                 adalora_config = AdaLoraConfig(
                     task_type='CAUSAL_LM',
                     **lora_kwargs,
                     target_r=args.adalora_target_r,
                     init_r=args.adalora_init_r,
                     tinit=args.adalora_tinit,
@@ -143,15 +132,36 @@
 
                 llamapro_config = LLaMAProConfig(
                     model_type=model_type,
                     num_new_blocks=args.llamapro_num_new_blocks,
                     num_groups=args.llamapro_num_groups)
                 model = Swift.prepare_model(model, llamapro_config)
                 logger.info(f'llamapro_config: {llamapro_config}')
+            elif args.sft_type == 'adapter':
+                model_type = args.model_type or args.model_id_or_path
+                for key in MODEL_KEYS_MAPPING.keys():
+                    if key in model_type.lower():
+                        model_type = key
+                        break
+
+                assert model_type in MODEL_KEYS_MAPPING
+                mlp_key = MODEL_KEYS_MAPPING[model_type].mlp
+                mlp_key = mlp_key.split('.{}.')[1]
+                adapter_config = AdapterConfig(
+                    dim=model.config.hidden_size,
+                    target_modules=[mlp_key],
+                    hidden_pos=0,
+                    adapter_length=args.adapter_length,
+                    act_layer=args.adapter_act)
+                model = Swift.prepare_model(model, adapter_config)
+                logger.info(f'adapter_config: {adapter_config}')
         else:
+            if use_torchacc():
+                consolidate_checkpoint(args.resume_from_checkpoint,
+                                       'adapter_model')
             model = Swift.from_pretrained(
                 model, args.resume_from_checkpoint, is_trainable=True)
         # fix bug: Attempting to unscale FP16 gradients.
         #   peft: https://github.com/huggingface/peft/issues/1249
         #   modules_to_save + fp16
         is_logging = False
         for p in model.parameters():
@@ -163,14 +173,22 @@
                 p.data = p.data.to(dtype=torch.float32)
     elif args.sft_type == 'full':
         if args.freeze_parameters > 0:
             freeze_model_parameters(model, args.freeze_parameters)
         if len(args.additional_trainable_parameters) > 0:
             activate_model_parameters(model,
                                       args.additional_trainable_parameters)
+        if use_torchacc() and args.resume_from_checkpoint is not None:
+            consolidate_checkpoint(args.resume_from_checkpoint, 'model')
+            weights_file = os.path.join(args.resume_from_checkpoint,
+                                        'model.bin')
+            state_dict = torch.load(weights_file, map_location='cpu')
+            model.load_state_dict(state_dict, False)
+            # release memory
+            del state_dict
     else:
         raise ValueError(f'args.sft_type: {args.sft_type}')
 
     if args.neftune_backend == 'swift' and args.neftune_noise_alpha not in {
             None, 0.
     }:
         neftune_config = NEFTuneConfig(noise_alpha=args.neftune_noise_alpha)
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/__init__.py` & `ms-swift-2.0.0/swift/llm/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from .argument import (AppUIArguments, DeployArguments, DPOArguments,
-                       ExportArguments, InferArguments, RomeArguments,
-                       SftArguments, is_adapter)
+                       EvalArguments, ExportArguments, InferArguments,
+                       RomeArguments, SftArguments, is_adapter,
+                       swift_to_peft_format)
 from .client_utils import get_model_list_client, inference_client
 from .dataset import (DATASET_MAPPING, DatasetName, GetDatasetFunction,
                       HfDataset, add_self_cognition_dataset, get_dataset,
                       get_dataset_from_repo, load_dataset_from_local,
                       load_ms_dataset, register_dataset)
 from .model import (MODEL_MAPPING, GetModelTokenizerFunction, LoRATM,
                     ModelType, get_additional_saved_files,
@@ -38,11 +39,15 @@
                     sort_by_max_length, stat_dataset, to_device)
 
 try:
     if is_vllm_available():
         from .vllm_utils import (VllmGenerationConfig, get_vllm_engine,
                                  inference_stream_vllm, inference_vllm,
                                  prepare_vllm_engine_template)
+        try:
+            from .vllm_utils import LoRARequest
+        except ImportError:
+            pass
 except Exception as e:
     from swift.utils import get_logger
     logger = get_logger()
     logger.warning(f'import vllm_utils error: {e}')
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/argument.py` & `ms-swift-2.0.0/swift/llm/utils/argument.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
-import inspect
 import math
 import os
 from dataclasses import dataclass, field
-from typing import Dict, List, Literal, Optional, Set, Tuple, Union
+from typing import List, Literal, Optional, Set, Tuple, Union
 
 import json
 import numpy as np
 import torch
-import torch.distributed as dist
 import transformers
+from datasets import Dataset as HfDataset
 from datasets import concatenate_datasets
 from packaging import version
 from torch import dtype as Dtype
 from transformers.utils import (is_torch_bf16_gpu_available,
                                 is_torch_cuda_available,
                                 is_torch_npu_available)
 from transformers.utils.versions import require_version
 
-from swift import get_logger
 from swift.hub import HubApi, ModelScopeConfig
 from swift.trainers import Seq2SeqTrainingArguments
-from swift.utils import (add_version_to_work_dir, broadcast_string,
-                         get_dist_setting, get_pai_tensorboard_dir, is_dist,
-                         is_mp, is_pai_training_job)
+from swift.tuners import Swift
+from swift.utils import (add_version_to_work_dir, get_dist_setting, get_logger,
+                         get_pai_tensorboard_dir, is_dist, is_mp,
+                         is_pai_training_job)
 from .dataset import (DATASET_MAPPING, get_custom_dataset, get_dataset,
                       register_dataset)
 from .model import (MODEL_MAPPING, dtype_mapping, get_additional_saved_files,
                     get_default_lora_target_modules, get_default_template_type)
-from .template import TEMPLATE_MAPPING, TemplateType
+from .template import TEMPLATE_MAPPING
 from .utils import is_vllm_available
 
 logger = get_logger()
 
 
 def is_adapter(sft_type: str) -> bool:
     return sft_type in {
-        'lora', 'longlora', 'qalora', 'adalora', 'ia3', 'llamapro'
+        'lora', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter'
     }
 
 
 @dataclass
 class SftArguments:
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None,
         metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
+    model_layer_cls_name: Optional[str] = field(
+        default=None,
+        metadata={
+            'help':
+            "Decoder Class name of model, e.g. 'QWenBlock' for QWen, 'LlamaDecoderLayer' for LLama"
+        })
 
-    sft_type: Literal['lora', 'full', 'longlora', 'qalora', 'adalora', 'ia3',
-                      'llamapro'] = 'lora'
+    sft_type: Literal['lora', 'full', 'longlora', 'adalora', 'ia3', 'llamapro',
+                      'adapter'] = 'lora'
     freeze_parameters: float = 0.  # 0 ~ 1
     additional_trainable_parameters: List[str] = field(default_factory=list)
-    tuner_backend: Literal['swift', 'peft'] = 'swift'
+    tuner_backend: Literal['swift', 'peft'] = 'peft'
     template_type: str = field(
         default='AUTO',
         metadata={
             'help':
             f"template_type choices: {list(TEMPLATE_MAPPING.keys()) + ['AUTO']}"
         })
     output_dir: str = 'output'
     add_output_dir_suffix: Optional[bool] = None
-    ddp_backend: Literal['nccl', 'gloo', 'mpi', 'ccl'] = 'nccl'
+    ddp_backend: Literal['nccl', 'gloo', 'mpi', 'ccl'] = None
     ddp_find_unused_parameters: Optional[bool] = None
     ddp_broadcast_buffers: Optional[bool] = None
 
     seed: int = 42
     resume_from_checkpoint: Optional[str] = None
     dtype: Literal['bf16', 'fp16', 'fp32', 'AUTO'] = 'AUTO'
 
     dataset: List[str] = field(
         default_factory=list,
         metadata={'help': f'dataset choices: {list(DATASET_MAPPING.keys())}'})
     dataset_seed: int = 42
     dataset_test_ratio: float = 0.01
-    train_dataset_sample: int = 20000  # -1: all dataset
-    train_dataset_mix_ratio: Optional[float] = None
+    train_dataset_sample: int = -1  # -1: all dataset
+    train_dataset_mix_ratio: float = 0.
     train_dataset_mix_ds: List[str] = field(
         default_factory=lambda: ['ms-bench'])
     val_dataset_sample: Optional[int] = None  # -1: all dataset
     use_loss_scale: bool = False
     system: Optional[str] = None
     max_length: int = 2048  # -1: no limit
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete'
@@ -99,33 +104,32 @@
     # If you want to use qlora, set the quantization_bit to 8 or 4.
     # And you need to install bitsandbytes: `pip install bitsandbytes -U`
     # note: bf16 and quantization have requirements for gpu architecture
     quantization_bit: Literal[0, 4, 8] = 0
     bnb_4bit_comp_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'AUTO'
     bnb_4bit_quant_type: Literal['fp4', 'nf4'] = 'nf4'
     bnb_4bit_use_double_quant: bool = True
+    bnb_4bit_quant_storage: Optional[str] = None
     # lora
     lora_target_modules: List[str] = field(default_factory=lambda: ['DEFAULT'])
     lora_rank: int = 8
     lora_alpha: int = 32
     lora_dropout_p: float = 0.05
     lora_bias_trainable: Literal['none', 'all'] = 'none'
     # e.g. ['wte', 'ln_1', 'ln_2', 'ln_f', 'lm_head']
     lora_modules_to_save: List[str] = field(default_factory=list)
-    lora_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'fp32'
+    lora_dtype: Literal['fp16', 'bf16', 'fp32'] = 'fp32'
     lora_lr_ratio: float = None
-
     use_rslora: bool = False
-    lora_layers_to_transform: Optional[List[int]] = None
-    lora_layers_pattern: Optional[List[str]] = None
-    lora_rank_pattern: Dict = field(default_factory=dict)
-    lora_alpha_pattern: Dict = field(default_factory=dict)
-    lora_loftq_config: Dict = field(default_factory=dict)
     use_dora: bool = False
 
+    # adapter
+    adapter_act: str = 'gelu'
+    adapter_length: int = 128
+
     # galore
     use_galore: bool = False
     galore_rank: int = 128
     galore_target_modules: Optional[List[str]] = None
     galore_update_proj_gap: int = 50
     galore_scale: float = 1.0
     galore_proj_type: str = 'std'
@@ -161,15 +165,15 @@
     num_train_epochs: int = 1
     # if max_steps >= 0, override num_train_epochs
     max_steps: int = -1
     optim: str = 'adamw_torch'
     adam_beta1: float = 0.9
     adam_beta2: float = 0.999
     learning_rate: Optional[float] = None
-    weight_decay: float = 0.01
+    weight_decay: float = 0.1
     gradient_accumulation_steps: Optional[int] = None
     max_grad_norm: float = 0.5
     predict_with_generate: bool = False
     lr_scheduler_type: str = 'linear'
     warmup_ratio: float = 0.05
 
     eval_steps: int = 50
@@ -232,14 +236,19 @@
     per_device_eval_batch_size: Optional[int] = None
     # compatibility. (Deprecated)
     only_save_model: Optional[bool] = None
     neftune_alpha: Optional[float] = None
     deepspeed_config_path: Optional[str] = None
     model_cache_dir: Optional[str] = None
 
+    # fsdp option
+    fsdp: Optional[str] = ''
+    # fsdp config file
+    fsdp_config: Optional[str] = None
+
     def _prepare_target_modules(self, target_modules) -> List[str]:
         if isinstance(target_modules, str):
             target_modules = [target_modules]
         if len(target_modules) == 0:
             return target_modules
         elif len(target_modules) == 1:
             if ',' in target_modules[0]:
@@ -278,18 +287,21 @@
         ds_config_folder = os.path.join(__file__, '..', '..', 'ds_config')
         if self.deepspeed == 'default-zero2':
             self.deepspeed = os.path.abspath(
                 os.path.join(ds_config_folder, 'zero2.json'))
         elif self.deepspeed == 'default-zero3':
             self.deepspeed = os.path.abspath(
                 os.path.join(ds_config_folder, 'zero3.json'))
+
         handle_path(self)
         set_model_type(self)
         if isinstance(self.dataset, str):
             self.dataset = [self.dataset]
+        if isinstance(self.train_dataset_mix_ds, str):
+            self.train_dataset_mix_ds = [self.train_dataset_mix_ds]
         register_custom_dataset(self)
         check_flash_attn(self)
         handle_generation_config(self)
 
         self.lora_use_embedding = False
         self.lora_use_all = False
         self.lora_m2s_use_embedding = False
@@ -403,15 +415,18 @@
                 self.eval_batch_size = self.batch_size
         if self.save_total_limit == -1:
             self.save_total_limit = None
         if self.max_length == -1:
             self.max_length = None
 
         if self.deepspeed is not None:
-            assert not is_mp(), 'DeepSpeed is not compatible with MP.'
+            if is_mp():
+                raise ValueError('DeepSpeed is not compatible with MP. '
+                                 f'n_gpu: {torch.cuda.device_count()}, '
+                                 f'local_world_size: {get_dist_setting()[3]}.')
             require_version('deepspeed')
             if self.deepspeed.endswith('.json') or os.path.isfile(
                     self.deepspeed):
                 with open(self.deepspeed, 'r', encoding='utf-8') as f:
                     self.deepspeed = json.load(f)
             logger.info(f'Using deepspeed: {self.deepspeed}')
 
@@ -517,14 +532,16 @@
             deepspeed=self.deepspeed,
             additional_saved_files=additional_saved_files,
             disable_tqdm=self.disable_tqdm,
             save_on_each_node=self.save_on_each_node,
             acc_strategy=self.acc_strategy,
             save_safetensors=self.save_safetensors,
             logging_first_step=True,
+            fsdp=self.fsdp,
+            fsdp_config=self.fsdp_config,
             **kwargs)
 
         training_args.ddp_find_unused_parameters = self.ddp_find_unused_parameters
         training_args.ddp_broadcast_buffers = self.ddp_broadcast_buffers
         if is_dist() and training_args.ddp_find_unused_parameters is None:
             if self.gradient_checkpointing:
                 training_args.ddp_find_unused_parameters = False
@@ -558,15 +575,15 @@
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None,
         metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
 
-    sft_type: Literal['lora', 'longlora', 'qalora', 'full', 'adalora', 'ia3',
+    sft_type: Literal['lora', 'longlora', 'full', 'adalora', 'ia3',
                       'llamapro'] = 'lora'
     template_type: str = field(
         default='AUTO',
         metadata={
             'help':
             f"template_type choices: {list(TEMPLATE_MAPPING.keys()) + ['AUTO']}"
         })
@@ -618,14 +635,17 @@
     save_safetensors: bool = True
     overwrite_generation_config: Optional[bool] = None
     verbose: Optional[bool] = None
     # vllm
     gpu_memory_utilization: float = 0.9
     tensor_parallel_size: int = 1
     max_model_len: Optional[int] = None
+    vllm_enable_lora: bool = False
+    vllm_max_lora_rank: int = 16
+    vllm_lora_modules: List[str] = field(default_factory=list)
     # compatibility. (Deprecated)
     show_dataset_sample: int = 10
     safe_serialization: Optional[bool] = None
     model_cache_dir: Optional[str] = None
     merge_lora_and_save: Optional[bool] = None
 
     def __post_init__(self) -> None:
@@ -643,24 +663,24 @@
                 'Due to `ckpt_dir` being `None`, `load_args_from_ckpt_dir` is set to `False`.'
             )
         if self.load_args_from_ckpt_dir:
             load_from_ckpt_dir(self)
         else:
             assert self.load_dataset_config is False, 'You need to first set `--load_args_from_ckpt_dir true`.'
         set_model_type(self)
+        if isinstance(self.dataset, str):
+            self.dataset = [self.dataset]
         register_custom_dataset(self)
         check_flash_attn(self)
         handle_generation_config(self)
 
         self.torch_dtype, _, _ = select_dtype(self)
         if self.template_type == 'AUTO':
             self.template_type = get_default_template_type(self.model_type)
             logger.info(f'Setting template_type: {self.template_type}')
-        if isinstance(self.dataset, str):
-            self.dataset = [self.dataset]
         has_dataset = (
             len(self.dataset) > 0 or len(self.custom_train_dataset_path) > 0
             or len(self.custom_val_dataset_path) > 0)
         if self.eval_human is None:
             if not has_dataset:
                 self.eval_human = True
             else:
@@ -683,30 +703,40 @@
             logger.info(
                 f'Setting overwrite_generation_config: {self.overwrite_generation_config}'
             )
         if self.ckpt_dir is None:
             self.sft_type = 'full'
         model_info = MODEL_MAPPING[self.model_type]
         support_vllm = model_info.get('support_vllm', False)
+        self.vllm_lora_request_list = None
         if self.infer_backend == 'AUTO':
             self.infer_backend = 'pt'
             if is_vllm_available() and support_vllm:
                 if ((self.sft_type == 'full'
                      or self.sft_type == 'lora' and self.merge_lora)
                         and self.quantization_bit == 0):
                     self.infer_backend = 'vllm'
+                if self.vllm_enable_lora:
+                    self.infer_backend = 'vllm'
         if self.infer_backend == 'vllm':
             require_version('vllm')
             assert self.quantization_bit == 0, 'VLLM does not support bnb.'
             if not support_vllm:
                 logger.warning(f'vllm not support `{self.model_type}`')
-            if self.sft_type == 'lora':
+            if self.sft_type == 'lora' and not self.vllm_enable_lora:
                 assert self.merge_lora is True, (
                     'To use VLLM, you need to provide the complete weight parameters. '
                     'Please set `--merge_lora true`.')
+            if self.vllm_enable_lora:
+                self.vllm_lora_modules.append(f'default-lora={self.ckpt_dir}')
+                self.vllm_lora_request_list = _parse_vllm_lora_modules(
+                    self.vllm_lora_modules)
+                logger.info(
+                    f'args.vllm_lora_request_list: {self.vllm_lora_request_list}'
+                )
         template_info = TEMPLATE_MAPPING[self.template_type]
         if self.num_beams != 1:
             self.stream = False
             logger.info('Setting self.stream: False')
         self.infer_media_type = template_info.get('infer_media_type', 'none')
         if self.merge_device_map is None:
             self.merge_device_map = 'cpu'
@@ -744,15 +774,31 @@
         tags = model_info.get('tags', [])
         if 'multi-modal' in tags:
             raise ValueError(
                 'Deployment of multimodal models is currently not supported.')
 
 
 @dataclass
+class EvalArguments(InferArguments):
+
+    name: Optional[str] = None
+
+    eval_dataset: List[str] = field(
+        default_factory=lambda: ['ceval', 'gsm8k', 'arc'])
+
+    eval_few_shot: Optional[int] = None
+
+    eval_limit: Optional[int] = None
+
+    custom_eval_config: Optional[str] = None
+
+
+@dataclass
 class ExportArguments(InferArguments):
+    to_peft_format: bool = False
     # The parameter has been defined in InferArguments.
     # merge_lora: bool = False
 
     # awq: 4; gptq: 2, 3, 4, 8
     quant_bits: int = 0  # e.g. 4
     quant_method: Literal['awq', 'gptq'] = 'awq'
     quant_n_samples: Optional[int] = None
@@ -793,14 +839,16 @@
 @dataclass
 class DPOArguments(SftArguments):
 
     ref_model_type: Optional[str] = field(
         default=None,
         metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
 
+    ref_model_id_or_path: Optional[str] = None
+
     max_prompt_length: int = 1024
     beta: float = 0.1
     label_smoothing: float = 0.0
     loss_type: Literal['sigmoid', 'hinge', 'ipo', 'kto_pair'] = 'sigmoid'
     sft_beta: float = 0.1
 
 
@@ -1057,33 +1105,46 @@
         value = getattr(args, k, None)
         if value is None:
             continue
         value = _check_path(k, value, check_exist_path_set)
         setattr(args, k, value)
 
 
+def _register_local_dataset(dataset_name: str, train_dataset_path: List[str],
+                            val_dataset_path: List[str]) -> None:
+    register_dataset(
+        dataset_name,
+        '_',
+        train_dataset_path,
+        val_dataset_path,
+        get_function=get_custom_dataset,
+        exists_ok=True)
+
+
 def register_custom_dataset(args: Union[SftArguments, InferArguments]) -> None:
+    dataset = []
+    for d in args.dataset:
+        if os.path.exists(d):
+            args.custom_train_dataset_path.append(d)
+        else:
+            dataset.append(d)
+    args.dataset = dataset
+
     for key in ['custom_train_dataset_path', 'custom_val_dataset_path']:
         value = getattr(args, key)
         if isinstance(value, str):
             setattr(args, key, [value])
     if len(args.custom_train_dataset_path) == 0 and len(
             args.custom_val_dataset_path) == 0:
         return
-    register_dataset(
-        '_custom_dataset',
-        '_custom_dataset',
-        args.custom_train_dataset_path,
-        args.custom_val_dataset_path,
-        get_function=get_custom_dataset,
-        exists_ok=True)
-    if args.dataset is None:
-        args.dataset = ['_custom_dataset']
-    elif '_custom_dataset' not in args.dataset:
-        args.dataset.append('_custom_dataset')
+
+    dataset_name = '_custom_dataset'
+    _register_local_dataset(dataset_name, args.custom_train_dataset_path,
+                            args.custom_val_dataset_path)
+    args.dataset.append(dataset_name)
 
 
 def load_from_ckpt_dir(args: InferArguments) -> None:
     sft_args_path = os.path.join(args.ckpt_dir, 'sft_args.json')
     if not os.path.exists(sft_args_path):
         logger.info(f'{sft_args_path} not found')
         return
@@ -1104,14 +1165,17 @@
         if (key in {
                 'dataset', 'custom_train_dataset_path',
                 'custom_val_dataset_path'
         } and len(getattr(args, key)) > 0):
             continue
         setattr(args, key, sft_args.get(key))
 
+    if args.model_id_or_path is None:
+        args.model_id_or_path = sft_args.get('model_id_or_path')
+
 
 def check_flash_attn(args: Union[SftArguments, InferArguments]) -> None:
     model_info = MODEL_MAPPING[args.model_type]
     support_flash_attn = model_info.get('support_flash_attn', False)
     if args.use_flash_attn and not support_flash_attn:
         logger.warning(f'use_flash_attn: {args.use_flash_attn}, '
                        f'but support_flash_attn: {support_flash_attn}')
@@ -1126,35 +1190,80 @@
         args.top_k = 50
         logger.info(
             'Due to do_sample=False, the following settings are applied: args.temperature: '
             f'{args.temperature}, args.top_p: {args.top_p}, args.top_k: {args.top_k}.'
         )
 
 
-def handle_dataset_mixture(args: SftArguments, train_dataset,
-                           mix_dataset_sample) -> None:
+def handle_dataset_mixture(args: SftArguments,
+                           train_dataset: HfDataset) -> None:
     if train_dataset is None:
         return train_dataset
-    train_length = len(train_dataset)
+    if args.train_dataset_mix_ratio <= 0 or len(
+            args.train_dataset_mix_ds) == 0:
+        return train_dataset
+
     random_state = np.random.RandomState(args.dataset_seed)
-    if mix_dataset_sample:
-        assert args.train_dataset_mix_ds is not None
-        train_dataset_mix_ds = [args.train_dataset_mix_ds] if isinstance(
-            args.train_dataset_mix_ds, str) else args.train_dataset_mix_ds
-        mixed_dataset = get_dataset(
-            train_dataset_mix_ds,
-            0.0,
-            random_state,
-            check_dataset_strategy=args.check_dataset_strategy)[0]
-        if len(mixed_dataset) < mix_dataset_sample:
-            logger.warn(
-                f'The length of dataset used for mixin: {train_dataset_mix_ds} are '
-                'lesser than the ratio required by the `train_dataset_mix_ratio` '
-                f'argument:{args.train_dataset_mix_ratio}'
-                f'the actual ratio is : {len(mixed_dataset)/float(train_length)}'
-            )
+    train_dataset_mix_ds = []
+    custom_mix_ds = []
+    for mix_ds in args.train_dataset_mix_ds:
+        if os.path.exists(mix_ds):
+            custom_mix_ds.append(mix_ds)
         else:
-            train_idxs = random_state.permutation(mix_dataset_sample)
-            mixed_dataset = mixed_dataset.select(train_idxs)
-        return concatenate_datasets([train_dataset, mixed_dataset])
+            train_dataset_mix_ds.append(mix_ds)
+
+    if len(custom_mix_ds) > 0:
+        dataset_name = '_custom_mixture'
+        _register_local_dataset(dataset_name, custom_mix_ds, [])
+        train_dataset_mix_ds.append(dataset_name)
+    mix_dataset_sample = int(len(train_dataset) * args.train_dataset_mix_ratio)
+    logger.info(f'train_dataset_mix_ds: {train_dataset_mix_ds}')
+    logger.info(
+        f'len(train_dataset): {len(train_dataset)}, mix_dataset_sample: {mix_dataset_sample}'
+    )
+    mixed_dataset = get_dataset(
+        train_dataset_mix_ds,
+        0.0,
+        random_state,
+        check_dataset_strategy=args.check_dataset_strategy)[0]
+    if len(mixed_dataset) < mix_dataset_sample:
+        logger.warn(
+            f'The length of dataset used for mixin: {train_dataset_mix_ds} are '
+            'lesser than the ratio required by the `train_dataset_mix_ratio` '
+            f'argument: {args.train_dataset_mix_ratio}. '
+            f'the actual ratio is: {len(mixed_dataset)/len(train_dataset):.6}.'
+        )
     else:
-        return train_dataset
+        train_idxs = random_state.permutation(mix_dataset_sample)
+        mixed_dataset = mixed_dataset.select(train_idxs)
+    return concatenate_datasets([train_dataset, mixed_dataset])
+
+
+def swift_to_peft_format(lora_checkpoint_path: str) -> str:
+    if 'default' in os.listdir(lora_checkpoint_path):  # swift_backend
+        new_lora_checkpoint_path = f'{lora_checkpoint_path}-peft'
+        Swift.save_to_peft_format(lora_checkpoint_path,
+                                  new_lora_checkpoint_path)
+        lora_checkpoint_path = new_lora_checkpoint_path
+        logger.info('Converting the swift format checkpoint to peft format, '
+                    f"and saving it to: '{new_lora_checkpoint_path}'")
+    else:
+        logger.info('The format of the checkpoint is already in peft format.')
+    return lora_checkpoint_path
+
+
+def _parse_vllm_lora_modules(
+        vllm_lora_modules: List[str]) -> List['LoRARequest']:
+    try:
+        from .vllm_utils import LoRARequest
+    except ImportError:
+        logger.warning(
+            'The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.'
+        )
+        raise
+    lora_request_list = []
+    for i, vllm_lora_module in enumerate(vllm_lora_modules):
+        lora_name, lora_local_path = vllm_lora_module.split('=')
+        lora_local_path = swift_to_peft_format(lora_local_path)
+        lora_request_list.append(
+            LoRARequest(lora_name, i + 1, lora_local_path))
+    return lora_request_list
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/client_utils.py` & `ms-swift-2.0.0/swift/llm/utils/client_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/utils/dataset.py` & `ms-swift-2.0.0/swift/llm/utils/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     wikipedia_zh = 'wikipedia-zh'
     open_orca = 'open-orca'
     open_orca_gpt4 = 'open-orca-gpt4'
     sharegpt_gpt4 = 'sharegpt-gpt4'
     sharegpt_gpt4_mini = 'sharegpt-gpt4-mini'
     # agent
     ms_agent = 'ms-agent'
+    ms_agent_for_agentfabric_default = 'ms-agent-for-agentfabric-default'
+    ms_agent_for_agentfabric_addition = 'ms-agent-for-agentfabric-addition'
     damo_agent_zh = 'damo-agent-zh'
     damo_agent_mini_zh = 'damo-agent-mini-zh'
     agent_instruct_all_en = 'agent-instruct-all-en'
     # coding
     code_alpaca_en = 'code-alpaca-en'
     leetcode_python_en = 'leetcode-python-en'
     codefuse_python_en = 'codefuse-python-en'
@@ -106,14 +108,15 @@
     finance_en = 'finance-en'
     poetry_zh = 'poetry-zh'
     webnovel_zh = 'webnovel-zh'
     generated_chat_zh = 'generated-chat-zh'
     # example dataset for specific model
     cls_fudan_news_zh = 'cls-fudan-news-zh'  # seqgpt-560m
     ner_java_zh = 'ner-jave-zh'  # seqgpt-560m
+    long_alpaca_12k = 'long-alpaca-12k'
 
     # multi-modal
     # for qwen-vl
     coco_en = 'coco-en'
     coco_mini_en = 'coco-mini-en'
     # for yi-vl, cogagnet
     coco_mini_en_2 = 'coco-mini-en-2'
@@ -134,14 +137,34 @@
     hh_rlhf_cn_harmless_base_en = 'hh-rlhf-cn-harmless-base-en'
     hh_rlhf_cn_helpful_base_en = 'hh-rlhf-cn-helpful-base-en'
     stack_exchange_paired = 'stack-exchange-paired'
 
     # for awq
     pileval = 'pileval'
 
+    # COIG-CQIA
+    coig_cqia_chinese_traditional = 'coig-cqia-chinese-traditional'
+    coig_cqia_coig_pc = 'coig-cqia-coig-pc'
+    coig_cqia_exam = 'coig-cqia-exam'
+    coig_cqia_finance = 'coig-cqia-finance'
+    coig_cqia_douban = 'coig-cqia-douban'
+    coig_cqia_human_value = 'coig-cqia-human-value'
+    coig_cqia_logi_qa = 'coig-cqia-logi-qa'
+    coig_cqia_ruozhiba = 'coig-cqia-ruozhiba'
+    coig_cqia_segmentfault = 'coig-cqia-segmentfault'
+    coig_cqia_wiki = 'coig-cqia-wiki'
+    coig_cqia_wikihow = 'coig-cqia-wikihow'
+    coig_cqia_xhs = 'coig-cqia-xhs'
+    coig_cqia_zhihu = 'coig-cqia-zhihu'
+
+    # ruozhiba
+    ruozhiba_post_annual = 'ruozhiba-post-annual'
+    ruozhiba_title_good = 'ruozhiba-title-good'
+    ruozhiba_title_norm = 'ruozhiba-title-norm'
+
     @classmethod
     def get_dataset_name_list(cls) -> List[str]:
         res = []
         for k in cls.__dict__.keys():
             if k.startswith('__') or k == 'get_dataset_name_list':
                 continue
             res.append(cls.__dict__[k])
@@ -207,15 +230,17 @@
     dataset_list = []
     for subset_split in subset_split_list:
         if isinstance(subset_split, str):
             subset_split = ('default', subset_split)
         assert len(subset_split) == 2
         subset_name, split = subset_split
         dataset = MsDataset.load(
-            dataset_id, subset_name=subset_name, split=split).to_hf_dataset()
+            dataset_id, subset_name=subset_name, split=split)
+        if hasattr(dataset, 'to_hf_dataset'):
+            dataset = dataset.to_hf_dataset()
         dataset_list.append(dataset)
     return concatenate_datasets(dataset_list)
 
 
 @register_dataset(
     DatasetName.text2sql_en,
     'AI-ModelScope/texttosqlv2_25000_v2', ['train'],
@@ -248,14 +273,74 @@
     DatasetName.finance_en,
     'wyj123456/finance_en', ['train'],
     tags=['chat', 'financial'])
 @register_dataset(
     DatasetName.alpaca_en,
     'AI-ModelScope/alpaca-gpt4-data-en', ['train'],
     tags=['chat', 'general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_chinese_traditional,
+    'AI-ModelScope/COIG-CQIA', [('chinese_traditional', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_coig_pc,
+    'AI-ModelScope/COIG-CQIA', [('coig_pc', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_exam,
+    'AI-ModelScope/COIG-CQIA', [('exam', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_finance,
+    'AI-ModelScope/COIG-CQIA', [('finance', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_douban,
+    'AI-ModelScope/COIG-CQIA', [('douban', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_human_value,
+    'AI-ModelScope/COIG-CQIA', [('human_value', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_logi_qa,
+    'AI-ModelScope/COIG-CQIA', [('logi_qa', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_ruozhiba,
+    'AI-ModelScope/COIG-CQIA', [('ruozhiba', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_segmentfault,
+    'AI-ModelScope/COIG-CQIA', [('segmentfault', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_wiki,
+    'AI-ModelScope/COIG-CQIA', [('wiki', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_wikihow,
+    'AI-ModelScope/COIG-CQIA', [('wikihow', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_xhs,
+    'AI-ModelScope/COIG-CQIA', [('xhs', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.coig_cqia_zhihu,
+    'AI-ModelScope/COIG-CQIA', [('zhihu', 'train')],
+    tags=['general', '🔥'])
+@register_dataset(
+    DatasetName.ms_agent_for_agentfabric_default,
+    'AI-ModelScope/ms_agent_for_agentfabric', [('default', 'train')],
+    tags=['chat', 'agent', 'multi-round'])
+@register_dataset(
+    DatasetName.ms_agent_for_agentfabric_addition,
+    'AI-ModelScope/ms_agent_for_agentfabric', [('addition', 'train')],
+    tags=['chat', 'agent', 'multi-round'])
 def get_dataset_from_repo(
         dataset_id: str,
         train_subset_split_list: List[SubsetSplit],
         val_subset_split_list: Optional[List[SubsetSplit]],
         preprocess_func: PreprocessFunc,
         remove_useless_columns: bool = True,
         train_dataset_sample: int = -1,
@@ -453,14 +538,70 @@
     for c in conversations:
         value = c['value'].lower()
         if 'moss' in value or 'human:' in value or 'assistant:' in value:
             return
     return conversations
 
 
+def long_alpaca_preprocessor(dataset: HfDataset):
+
+    def map_row(row):
+        response = row['response']
+        if response and response.startswith('Answer:'):
+            response = response[len('Answer:') + 1:].strip()
+        return {'query': row['query'], 'response': response}
+
+    return dataset.rename_columns({'instruction': 'query', 'output': 'response'}) \
+        .remove_columns(['input', 'file']).map(map_row).filter(lambda row: row['response'] is not None)
+
+
+register_dataset(
+    DatasetName.long_alpaca_12k,
+    'AI-ModelScope/LongAlpaca-12k', ['train'], [],
+    long_alpaca_preprocessor,
+    get_dataset_from_repo,
+    tags=['longlora', 'QA'])
+
+
+def _preprocess_ruozhiba(dataset: HfDataset):
+
+    def map_row(row):
+        title = row['title'] if 'title' in row else row['content']
+        abs = row['abs'] if 'abs' in row else None
+        if abs and abs != title:
+            title = title + '，' + abs
+
+        pattern = r'\d+[\.,\s,\、](.+)'
+        match = re.search(pattern, title)
+        if match:
+            title = match.group(1)
+        return {'response': title}
+
+    return dataset.map(map_row).filter(lambda row: row['response'])
+
+
+register_dataset(
+    DatasetName.ruozhiba_post_annual,
+    'AI-ModelScope/ruozhiba', [('post-annual', 'train')], [],
+    _preprocess_ruozhiba,
+    get_dataset_from_repo,
+    tags=['pretrain', '🔥'])
+register_dataset(
+    DatasetName.ruozhiba_title_good,
+    'AI-ModelScope/ruozhiba', [('title-good', 'train')], [],
+    _preprocess_ruozhiba,
+    get_dataset_from_repo,
+    tags=['pretrain', '🔥'])
+register_dataset(
+    DatasetName.ruozhiba_title_norm,
+    'AI-ModelScope/ruozhiba', [('title-norm', 'train')], [],
+    _preprocess_ruozhiba,
+    get_dataset_from_repo,
+    tags=['pretrain', '🔥'])
+
 register_dataset(
     DatasetName.ms_bench,
     'iic/ms_bench', ['train'], [],
     ConversationsPreprocessor(
         repair_conversations=_repair_ms_bench, error_strategy='delete'),
     get_dataset_from_repo,
     tags=['chat', 'general', 'multi-round', '🔥'])
@@ -753,44 +894,64 @@
     tags=['rlhf', 'dpo', 'pairwise'])
 
 
 def process_hh_rlhf_cn(dataset):
 
     def reorganize_row(row):
         history = []
-        if isinstance(row['context'], str):
-            row['context'] = ast.literal_eval(row['context'])
-        if isinstance(row['chosen'], str):
-            row['chosen'] = ast.literal_eval(row['chosen'])
-        if isinstance(row['rejected'], str):
-            row['rejected'] = ast.literal_eval(row['rejected'])
-        for idx, h in enumerate(row['context']):
-            if idx % 2 == 0 and h['role'] != 'human':
-                return {'query': None}
-            if idx % 2 != 0 and h['role'] != 'assistant':
-                return {'query': None}
-            if idx % 2 == 0:
-                history.append([h['text'], None])
-            else:
-                history[-1][-1] = h['text']
-        if history[-1][-1] is not None:
-            return {'query': None}
-        query = history[-1][0]
-        history = history[:-1]
-        response = row['chosen']['text']
-        rejected_response = row['rejected']['text']
+        try:
+            if isinstance(row['context'], str):
+                row['context'] = ast.literal_eval(row['context'])
+            if isinstance(row['chosen'], str):
+                row['chosen'] = ast.literal_eval(row['chosen'])
+            if isinstance(row['rejected'], str):
+                row['rejected'] = ast.literal_eval(row['rejected'])
+            for idx, h in enumerate(row['context']):
+                if idx % 2 == 0 and h['role'] != 'human':
+                    raise ValueError()
+                if idx % 2 != 0 and h['role'] != 'assistant':
+                    raise ValueError()
+                if idx % 2 == 0:
+                    history.append([h['text'], None])
+                else:
+                    history[-1][-1] = h['text']
+            if history[-1][-1] is not None:
+                raise ValueError()
+            query = history[-1][0]
+            history = history[:-1]
+            response = row['chosen']['text']
+            rejected_response = row['rejected']['text']
+        except:  # noqa
+            return {
+                'query': '',
+                'response': '',
+                'rejected_response': '',
+                'history': [],
+            }
         return {
             'query': query,
             'response': response,
             'rejected_response': rejected_response,
             'history': history,
         }
 
-    return dataset.map(reorganize_row).filter(
-        lambda row: row['query'] is not None)
+    def row_can_be_parsed(row):
+        try:
+            if isinstance(row['context'], str):
+                row['context'] = ast.literal_eval(row['context'])
+            if isinstance(row['chosen'], str):
+                row['chosen'] = ast.literal_eval(row['chosen'])
+            if isinstance(row['rejected'], str):
+                row['rejected'] = ast.literal_eval(row['rejected'])
+            return True
+        except:  # noqa
+            return False
+
+    return dataset.filter(row_can_be_parsed).map(reorganize_row).filter(
+        lambda row: row['query'])
 
 
 register_dataset(
     DatasetName.hh_rlhf_cn,
     'AI-ModelScope/hh_rlhf_cn', [('hh_rlhf', 'train')], [('hh_rlhf', 'test')],
     process_hh_rlhf_cn,
     get_dataset_from_repo,
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/model.py` & `ms-swift-2.0.0/swift/llm/utils/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from transformers import (PretrainedConfig, PreTrainedModel,
                           PreTrainedTokenizerBase)
 from transformers.dynamic_module_utils import get_class_from_dynamic_module
 from transformers.models.auto.tokenization_auto import get_tokenizer_config
 from transformers.utils.versions import require_version
 
 from swift import get_logger
-from swift.utils import is_dist, is_local_master
+from swift.utils import (get_dist_setting, is_dist, is_local_master,
+                         use_torchacc)
 from .template import TemplateType
 from .utils import get_max_model_len
 
 logger = get_logger()
 
 # Model Home: 'https://modelscope.cn/models/{model_id_or_path}/summary'
 MODEL_MAPPING: Dict[str, Dict[str, Any]] = {}
@@ -56,35 +57,41 @@
     qwen_72b_chat_int8 = 'qwen-72b-chat-int8'
     # qwen1.5
     qwen1half_0_5b = 'qwen1half-0_5b'
     qwen1half_1_8b = 'qwen1half-1_8b'
     qwen1half_4b = 'qwen1half-4b'
     qwen1half_7b = 'qwen1half-7b'
     qwen1half_14b = 'qwen1half-14b'
+    qwen1half_32b = 'qwen1half-32b'
     qwen1half_72b = 'qwen1half-72b'
+    qwen1half_moe_a2_7b = 'qwen1half-moe-a2_7b'
     qwen1half_0_5b_chat = 'qwen1half-0_5b-chat'
     qwen1half_1_8b_chat = 'qwen1half-1_8b-chat'
     qwen1half_4b_chat = 'qwen1half-4b-chat'
     qwen1half_7b_chat = 'qwen1half-7b-chat'
     qwen1half_14b_chat = 'qwen1half-14b-chat'
+    qwen1half_32b_chat = 'qwen1half-32b-chat'
     qwen1half_72b_chat = 'qwen1half-72b-chat'
+    qwen1half_moe_a2_7b_chat = 'qwen1half-moe-a2_7b-chat'
 
     # qwen1.5 gptq
     qwen1half_0_5b_chat_int4 = 'qwen1half-0_5b-chat-int4'
     qwen1half_1_8b_chat_int4 = 'qwen1half-1_8b-chat-int4'
     qwen1half_4b_chat_int4 = 'qwen1half-4b-chat-int4'
     qwen1half_7b_chat_int4 = 'qwen1half-7b-chat-int4'
     qwen1half_14b_chat_int4 = 'qwen1half-14b-chat-int4'
+    qwen1half_32b_chat_int4 = 'qwen1half-32b-chat-int4'
     qwen1half_72b_chat_int4 = 'qwen1half-72b-chat-int4'
     qwen1half_0_5b_chat_int8 = 'qwen1half-0_5b-chat-int8'
     qwen1half_1_8b_chat_int8 = 'qwen1half-1_8b-chat-int8'
     qwen1half_4b_chat_int8 = 'qwen1half-4b-chat-int8'
     qwen1half_7b_chat_int8 = 'qwen1half-7b-chat-int8'
     qwen1half_14b_chat_int8 = 'qwen1half-14b-chat-int8'
     qwen1half_72b_chat_int8 = 'qwen1half-72b-chat-int8'
+    qwen1half_moe_a2_7b_chat_int4 = 'qwen1half-moe-a2_7b-chat-int4'
 
     # qwen1.5 awq
     qwen1half_0_5b_chat_awq = 'qwen1half-0_5b-chat-awq'
     qwen1half_1_8b_chat_awq = 'qwen1half-1_8b-chat-awq'
     qwen1half_4b_chat_awq = 'qwen1half-4b-chat-awq'
     qwen1half_7b_chat_awq = 'qwen1half-7b-chat-awq'
     qwen1half_14b_chat_awq = 'qwen1half-14b-chat-awq'
@@ -108,14 +115,16 @@
     llama2_7b = 'llama2-7b'
     llama2_7b_chat = 'llama2-7b-chat'
     llama2_13b = 'llama2-13b'
     llama2_13b_chat = 'llama2-13b-chat'
     llama2_70b = 'llama2-70b'
     llama2_70b_chat = 'llama2-70b-chat'
     llama2_7b_aqlm_2bit_1x16 = 'llama2-7b-aqlm-2bit-1x16'  # aqlm
+    # llava
+    llava1d6_mistral_7b_instruct = 'llava1d6-mistral-7b-instruct'
     # yi
     yi_6b = 'yi-6b'
     yi_6b_200k = 'yi-6b-200k'
     yi_6b_chat = 'yi-6b-chat'
     yi_9b = 'yi-9b'
     yi_34b = 'yi-34b'
     yi_34b_200k = 'yi-34b-200k'
@@ -171,33 +180,39 @@
     deepseek_vl_7b_chat = 'deepseek-vl-7b-chat'
     # gemma
     gemma_2b = 'gemma-2b'
     gemma_7b = 'gemma-7b'
     gemma_2b_instruct = 'gemma-2b-instruct'
     gemma_7b_instruct = 'gemma-7b-instruct'
     # minicpm
+    minicpm_1b_sft_chat = 'minicpm-1b-sft-chat'
     minicpm_2b_sft_chat = 'minicpm-2b-sft-chat'
     minicpm_2b_chat = 'minicpm-2b-chat'
+    minicpm_2b_128k = 'minicpm-2b-128k'
+    minicpm_moe_8x2b = 'minicpm-moe-8x2b'
     # minicpm-v
     minicpm_v_3b_chat = 'minicpm-v-3b-chat'
+    minicpm_v_v2 = 'minicpm-v-v2'
     # openbuddy
     openbuddy_llama2_13b_chat = 'openbuddy-llama2-13b-chat'
     openbuddy_llama2_65b_chat = 'openbuddy-llama-65b-chat'
     openbuddy_llama2_70b_chat = 'openbuddy-llama2-70b-chat'
     openbuddy_mistral_7b_chat = 'openbuddy-mistral-7b-chat'
     openbuddy_zephyr_7b_chat = 'openbuddy-zephyr-7b-chat'
     openbuddy_deepseek_67b_chat = 'openbuddy-deepseek-67b-chat'
     openbuddy_mixtral_moe_7b_chat = 'openbuddy-mixtral-moe-7b-chat'
     # mistral
     mistral_7b = 'mistral-7b'
+    mistral_7b_v2 = 'mistral-7b-v2'
     mistral_7b_instruct = 'mistral-7b-instruct'
     mistral_7b_instruct_v2 = 'mistral-7b-instruct-v2'
     mixtral_moe_7b = 'mixtral-moe-7b'
     mixtral_moe_7b_instruct = 'mixtral-moe-7b-instruct'
     mixtral_moe_7b_aqlm_2bit_1x16 = 'mixtral-moe-7b-aqlm-2bit-1x16'  # aqlm
+    mixtral_moe_8x22b_v1 = 'mixtral-moe-8x22b-v1'
     # baichuan
     baichuan_7b = 'baichuan-7b'
     baichuan_13b = 'baichuan-13b'
     baichuan_13b_chat = 'baichuan-13b-chat'
     # baichuan2
     baichuan2_7b = 'baichuan2-7b'
     baichuan2_7b_chat = 'baichuan2-7b-chat'
@@ -215,14 +230,15 @@
     xverse_7b_chat = 'xverse-7b-chat'
     xverse_13b = 'xverse-13b'
     xverse_13b_chat = 'xverse-13b-chat'
     xverse_65b = 'xverse-65b'
     xverse_65b_v2 = 'xverse-65b-v2'
     xverse_65b_chat = 'xverse-65b-chat'
     xverse_13b_256k = 'xverse-13b-256k'
+    xverse_moe_a4_2b = 'xverse-moe-a4_2b'
     # orion
     orion_14b = 'orion-14b'
     orion_14b_chat = 'orion-14b-chat'
     # vivo
     bluelm_7b = 'bluelm-7b'
     bluelm_7b_32k = 'bluelm-7b-32k'
     bluelm_7b_chat = 'bluelm-7b-chat'
@@ -257,14 +273,27 @@
     # mamba
     mamba_130m = 'mamba-130m'
     mamba_370m = 'mamba-370m'
     mamba_390m = 'mamba-390m'
     mamba_790m = 'mamba-790m'
     mamba_1_4b = 'mamba-1.4b'
     mamba_2_8b = 'mamba-2.8b'
+    # teleAI
+    telechat_7b = 'telechat-7b'
+    telechat_12b = 'telechat-12b'
+    # grok-1
+    grok_1 = 'grok-1'
+    # dbrx
+    dbrx_instruct = 'dbrx-instruct'
+    dbrx_base = 'dbrx-base'
+    # mengzi
+    mengzi3_13b_base = 'mengzi3-13b-base'
+    # c4ai
+    c4ai_command_r_v01 = 'c4ai-command-r-v01'
+    c4ai_command_r_plus = 'c4ai-command-r-plus'
 
     @classmethod
     def get_model_name_list(cls) -> List[str]:
         res = []
         for k in cls.__dict__.keys():
             if k.startswith('__') or k == 'get_model_name_list':
                 continue
@@ -289,14 +318,17 @@
     cogvlm = [
         'vision_expert_query_key_value', 'vision_expert_dense',
         'language_expert_query_key_value', 'language_expert_dense'
     ]
     phi = ['Wqkv']
     internlm2 = ['wqkv']
     mamba = ['in_proj', 'x_proj', 'embeddings', 'out_proj']
+    telechat = ['key_value', 'query']
+    grok_1 = ['q_proj', 'k_proj', 'v_proj']
+    dbrx = ['attn.Wqkv']
 
 
 GetModelTokenizerFunction = Callable[..., Tuple[Optional[PreTrainedModel],
                                                 PreTrainedTokenizerBase]]
 
 
 def register_model(
@@ -402,28 +434,53 @@
     LoRATM.llama2,
     TemplateType.default_generation,
     revision='v1.0.0')
 @register_model(ModelType.xverse_7b_chat, 'xverse/XVERSE-7B-Chat',
                 LoRATM.llama2, TemplateType.xverse)
 @register_model(ModelType.xverse_7b, 'xverse/XVERSE-7B', LoRATM.llama2,
                 TemplateType.default_generation)
+@register_model(ModelType.xverse_moe_a4_2b, 'xverse/XVERSE-MoE-A4.2B',
+                LoRATM.llama2, TemplateType.default_generation)
 @register_model(
     ModelType.baichuan_13b_chat,
     'baichuan-inc/Baichuan-13B-Chat',
     LoRATM.baichuan,
     TemplateType.baichuan,
     requires=['transformers<4.34'],
     support_vllm=True)
 @register_model(
     ModelType.baichuan_7b,
     'baichuan-inc/baichuan-7B',
     LoRATM.baichuan,
     TemplateType.default_generation,
     requires=['transformers<4.34'],
     support_vllm=True)
+@register_model(
+    ModelType.mengzi3_13b_base,
+    'langboat/Mengzi3-13B-Base',
+    LoRATM.llama2,
+    TemplateType.mengzi,
+    support_vllm=True,
+    support_flash_attn=True)
+@register_model(
+    ModelType.c4ai_command_r_v01,
+    'AI-ModelScope/c4ai-command-r-v01',
+    LoRATM.llama2,
+    TemplateType.c4ai,
+    requires=['transformers>=4.39.1'],
+    support_vllm=False,
+    support_flash_attn=True)
+@register_model(
+    ModelType.c4ai_command_r_plus,
+    'AI-ModelScope/c4ai-command-r-plus',
+    LoRATM.llama2,
+    TemplateType.c4ai,
+    requires=['transformers>4.39'],
+    support_vllm=False,
+    support_flash_attn=True)
 def get_model_tokenizer_from_repo(model_dir: str,
                                   torch_dtype: Optional[Dtype],
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   model_config=None,
                                   tokenizer=None,
                                   automodel_class=AutoModelForCausalLM,
@@ -450,54 +507,91 @@
                 torch_dtype=torch_dtype,
                 trust_remote_code=True,
                 **model_kwargs)
     return model, tokenizer
 
 
 @register_model(
+    ModelType.grok_1,
+    'colossalai/grok-1-pytorch',
+    LoRATM.grok_1,
+    TemplateType.default_generation,
+    support_vllm=False,
+    support_flash_attn=False)
+def get_model_tokenizer_grok(model_dir: str,
+                             torch_dtype: Optional[Dtype],
+                             model_kwargs: Dict[str, Any],
+                             load_model: bool = True,
+                             model_config=None,
+                             tokenizer=None,
+                             automodel_class=AutoModelForCausalLM,
+                             **kwargs):
+    if model_config is None:
+        model_config = AutoConfig.from_pretrained(
+            model_dir, trust_remote_code=True)
+    if torch_dtype is not None:
+        model_config.torch_dtype = torch_dtype
+    if tokenizer is None:
+        tokenizer = AutoTokenizer.from_pretrained(
+            'AI-ModelScope/grok-1-tokenizer', trust_remote_code=True)
+    eos_token = kwargs.get('eos_token')
+    if eos_token is not None:
+        tokenizer.eos_token = eos_token
+    model = None
+    if load_model:
+        model = automodel_class.from_pretrained(
+            model_dir,
+            config=model_config,
+            torch_dtype=torch_dtype,
+            trust_remote_code=True,
+            **model_kwargs)
+    return model, tokenizer
+
+
+@register_model(
     ModelType.mamba_130m,
     'AI-ModelScope/mamba-130m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 @register_model(
     ModelType.mamba_370m,
     'AI-ModelScope/mamba-370m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 @register_model(
     ModelType.mamba_390m,
     'AI-ModelScope/mamba-390m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 @register_model(
     ModelType.mamba_790m,
     'AI-ModelScope/mamba-790m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 @register_model(
     ModelType.mamba_1_4b,
     'AI-ModelScope/mamba-1.4b-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 @register_model(
     ModelType.mamba_2_8b,
     'AI-ModelScope/mamba-2.8b-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
-    requires=['transformers>=4.39.0.dev0'],
+    requires=['transformers>=4.39.0'],
     support_vllm=False)
 def get_model_tokenizer_mamba(model_dir: str,
                               torch_dtype: Optional[Dtype],
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     logger.info(
@@ -925,22 +1019,38 @@
     'qwen/Qwen1.5-14B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
 @register_model(
+    ModelType.qwen1half_32b,
+    'qwen/Qwen1.5-32B',
+    LoRATM.qwen1half,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
+@register_model(
     ModelType.qwen1half_72b,
     'qwen/Qwen1.5-72B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
 @register_model(
+    ModelType.qwen1half_moe_a2_7b,
+    'qwen/Qwen1.5-MoE-A2.7B',
+    LoRATM.qwen1half,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
+@register_model(
     ModelType.deepseek_coder_1_3b,
     'deepseek-ai/deepseek-coder-1.3b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True,
     tags=['coding'])
@@ -1169,14 +1279,22 @@
     'AI-ModelScope/Mistral-7B-v0.1',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
     support_vllm=True)
 @register_model(
+    ModelType.mistral_7b_v2,
+    'AI-ModelScope/Mistral-7B-v0.2-hf',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    requires=['transformers>=4.34'],
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
     ModelType.mixtral_moe_7b,
     'AI-ModelScope/Mixtral-8x7B-v0.1',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
     support_vllm=True,
@@ -1186,14 +1304,40 @@
     'AI-ModelScope/Mixtral-8x7B-Instruct-v0.1',
     LoRATM.llama2,
     TemplateType.llama,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
     support_vllm=True,
     support_gradient_checkpointing=False)
+@register_model(
+    ModelType.mixtral_moe_8x22b_v1,
+    'AI-ModelScope/Mixtral-8x22B-v0.1',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    requires=['transformers>=4.36'],
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.dbrx_base,
+    'AI-ModelScope/dbrx-base',
+    LoRATM.dbrx,
+    TemplateType.dbrx,
+    requires=['transformers>=4.36'],
+    support_flash_attn=True,
+    support_vllm=True,
+    support_gradient_checkpointing=False)
+@register_model(
+    ModelType.dbrx_instruct,
+    'AI-ModelScope/dbrx-instruct',
+    LoRATM.dbrx,
+    TemplateType.dbrx,
+    requires=['transformers>=4.36'],
+    support_flash_attn=True,
+    support_vllm=True,
+    support_gradient_checkpointing=False)
 def get_model_tokenizer_with_flash_attn(model_dir: str,
                                         torch_dtype: Dtype,
                                         model_kwargs: Dict[str, Any],
                                         load_model: bool = True,
                                         model_config=None,
                                         **kwargs):
     if model_config is None:
@@ -1339,21 +1483,37 @@
     'qwen/Qwen1.5-14B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
 @register_model(
+    ModelType.qwen1half_32b_chat,
+    'qwen/Qwen1.5-32B-Chat',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
+@register_model(
     ModelType.qwen1half_72b_chat,
     'qwen/Qwen1.5-72B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
+@register_model(
+    ModelType.qwen1half_moe_a2_7b_chat,
+    'qwen/Qwen1.5-MoE-A2.7B-Chat',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
 def get_model_tokenizer_qwen1half(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     is_awq = kwargs.pop('is_awq', False)
     is_training = kwargs.pop('is_training', False)
@@ -1464,14 +1624,24 @@
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'bits': 8},
     support_flash_attn=True)
 @register_model(
+    ModelType.qwen1half_32b_chat_int4,
+    'qwen/Qwen1.5-32B-Chat-GPTQ-Int4',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    requires=['auto_gptq>=0.5', 'transformers>=4.37'],
+    torch_dtype=torch.float16,
+    function_kwargs={'bits': 4},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
     ModelType.qwen1half_72b_chat_int4,
     'qwen/Qwen1.5-72B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'bits': 4},
@@ -1482,14 +1652,23 @@
     'qwen/Qwen1.5-72B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'bits': 8},
     support_flash_attn=True)
+@register_model(
+    ModelType.qwen1half_moe_a2_7b_chat_int4,
+    'qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    requires=['auto_gptq>=0.5', 'transformers>=4.37'],
+    torch_dtype=torch.float16,
+    function_kwargs={'bits': 4},
+    support_flash_attn=True)
 def get_model_tokenizer_qwen1half_intx(model_dir: str,
                                        torch_dtype: Dtype,
                                        model_kwargs: Dict[str, Any],
                                        load_model: bool = True,
                                        **kwargs):
     kwargs['get_qwen_function'] = get_model_tokenizer_qwen1half
     return get_model_tokenizer_qwen_intx(model_dir, torch_dtype, model_kwargs,
@@ -2024,15 +2203,35 @@
     support_vllm=True)
 def get_model_tokenizer_qwen_chat(*args, **kwargs):
     model, tokenizer = get_model_tokenizer_qwen(*args, **kwargs)
     tokenizer.eos_token_id = tokenizer.im_end_id
     return model, tokenizer
 
 
+def _qwen_vl_visual_block_forward(
+    self,
+    q_x: torch.Tensor,
+    k_x: Optional[torch.Tensor] = None,
+    v_x: Optional[torch.Tensor] = None,
+    attn_mask: Optional[torch.Tensor] = None,
+):
+    k_x = self.ln_1_kv(k_x) if hasattr(self,
+                                       'ln_1_kv') and k_x is not None else None
+    v_x = self.ln_1_kv(v_x) if hasattr(self,
+                                       'ln_1_kv') and v_x is not None else None
+
+    x = q_x + self.attention(
+        q_x=self.ln_1(q_x), k_x=k_x, v_x=v_x, attn_mask=attn_mask)
+    z = self.mlp(self.ln_2(x))
+    x = x.to(z.device) + z  # FIX
+    return x
+
+
 def fix_qwen_inplace_bug(model) -> None:
+    # qwen-vl, qwen-audio
     first_drop = model.transformer.drop
     if first_drop.p == 0.:
         # fix in-place operation bug
         if not hasattr(first_drop, '__old_forward'):  # Avoid double patching
             if hasattr(first_drop, '_old_forward'):  # device_map
                 __old_forward = first_drop._old_forward
                 first_drop._old_forward = lambda *args, **kwargs: __old_forward(
@@ -2089,20 +2288,35 @@
     class_ref = tokenizer_config['auto_map']['AutoTokenizer'][0]
     tokenizer_cls = get_class_from_dynamic_module(class_ref, model_dir)
     tokenizer_cls._auto_class = 'AutoTokenizer'
     tokenizer_cls.IMAGE_ST = ()  # fix no attr `self.IMAGE_ST` bug
     if not hasattr(tokenizer_cls, '_old_decode'):  # avoid double patching
         tokenizer_cls._old_decode = tokenizer_cls._decode
         tokenizer_cls._decode = _qwen_vl_audio_decode
+    # fix device_map is 4
+    n_gpu = torch.cuda.device_count()
+    local_world_size = get_dist_setting()[3]
+    if n_gpu // local_world_size >= 4:
+        visual_block_cls = get_class_from_dynamic_module(
+            'visual.VisualAttentionBlock', model_dir)
+        if not hasattr(visual_block_cls,
+                       '__old_forward'):  # avoid double patching
+            visual_block_cls.__old_forward = visual_block_cls.forward
+            visual_block_cls.forward = _qwen_vl_visual_block_forward
+
     kwargs['tokenizer'] = tokenizer_cls.from_pretrained(
         model_dir, trust_remote_code=True)
     model, tokenizer = get_qwen_function(model_dir, torch_dtype, model_kwargs,
                                          load_model, **kwargs)
     if model is not None:
         fix_qwen_inplace_bug(model)
+        # fix device_map is 4
+        if n_gpu // local_world_size >= 4:
+            model.transformer.visual.proj.data = model.transformer.visual.proj.to(
+                model.transformer.visual.ln_post.bias.device)
 
     return model, tokenizer
 
 
 @register_model(
     ModelType.qwen_audio_chat,
     'qwen/Qwen-Audio-Chat',
@@ -2244,15 +2458,14 @@
     support_flash_attn=True,
     support_vllm=True)
 def get_model_tokenizer_qwen_intx(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
-
     logger.info('use gptq, ignore bnb arguments')
     bits = kwargs.pop('bits')
     if version.parse(transformers.__version__) >= version.parse('4.35'):
         model_kwargs['quantization_config'] = GPTQConfig(
             bits=bits, use_exllama=False)
     else:
         model_kwargs['quantization_config'] = GPTQConfig(
@@ -2331,14 +2544,20 @@
     'AI-ModelScope/phi-2',
     LoRATM.phi,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     support_gradient_checkpointing=False,
     tags=['coding'])
+@register_model(
+    ModelType.telechat_12b,
+    'TeleAI/TeleChat-12B',
+    LoRATM.telechat,
+    TemplateType.telechat,
+    support_flash_attn=True)
 def get_model_tokenizer_phi(model_dir: str,
                             torch_dtype: Dtype,
                             model_kwargs: Dict[str, Any],
                             load_model: bool = True,
                             **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2350,27 +2569,64 @@
         model_kwargs,
         load_model,
         model_config=model_config,
         **kwargs)
 
 
 @register_model(
+    ModelType.telechat_7b,
+    'TeleAI/TeleChat-7B',
+    LoRATM.telechat,
+    TemplateType.telechat,
+    support_flash_attn=True)
+def get_model_tokenizer_telechat(model_dir: str,
+                                 torch_dtype: Dtype,
+                                 model_kwargs: Dict[str, Any],
+                                 load_model: bool = True,
+                                 **kwargs):
+    if torch_dtype == torch.bfloat16:
+        logger.info(
+            'telechat-7b does not support the bfl16 dtype; the dtype is converted to fp16.'
+        )
+        torch_dtype = torch.float16
+    model_config = AutoConfig.from_pretrained(
+        model_dir, trust_remote_code=True)
+    use_flash_attn = kwargs.pop('use_flash_attn', False)
+    model_config.flash_attn = use_flash_attn
+    return get_model_tokenizer_from_repo(
+        model_dir,
+        torch_dtype,
+        model_kwargs,
+        load_model,
+        model_config=model_config,
+        **kwargs)
+
+
+@register_model(
     ModelType.deepseek_moe_16b_chat,
     'deepseek-ai/deepseek-moe-16b-chat',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
     support_vllm=True)
 @register_model(
     ModelType.deepseek_moe_16b,
     'deepseek-ai/deepseek-moe-16b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True)
+@register_model(
+    ModelType.minicpm_moe_8x2b,
+    'OpenBMB/MiniCPM-MoE-8x2B',
+    LoRATM.llama2,
+    TemplateType.minicpm,
+    requires=['transformers>=4.36.0'],
+    support_flash_attn=True,
+    support_vllm=True)
 def get_model_tokenizer_deepseek_moe(model_dir: str,
                                      torch_dtype: Dtype,
                                      model_kwargs: Dict[str, Any],
                                      load_model: bool = True,
                                      **kwargs):
     model, tokenizer = get_model_tokenizer_with_flash_attn(
         model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
@@ -2495,36 +2751,40 @@
 
 
 @register_model(
     ModelType.yi_vl_34b_chat,
     '01ai/Yi-VL-34B',
     LoRATM.llama2,
     TemplateType.yi_vl,
+    support_flash_attn=True,
     requires=['transformers>=4.34'],
     tags=['multi-modal', 'vision'])
 @register_model(
     ModelType.yi_vl_6b_chat,
     '01ai/Yi-VL-6B',
     LoRATM.llama2,
     TemplateType.yi_vl,
+    support_flash_attn=True,
     requires=['transformers>=4.34'],
     tags=['multi-modal', 'vision'])
 def get_model_tokenizer_yi_vl(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     local_repo_path = _git_clone_github('https://github.com/01-ai/Yi')
     sys.path.append(os.path.join(local_repo_path, 'VL'))
     from llava.model import LlavaLlamaForCausalLM, LlavaConfig
     from llava.model.constants import key_info
 
     model_config = LlavaConfig.from_pretrained(model_dir)
-    model_config.mm_vision_tower = os.path.join(model_dir,
-                                                model_config.mm_vision_tower)
+    mm_vision_tower = model_config.mm_vision_tower
+    model_config.mm_vision_tower = os.path.join(
+        model_dir,
+        *mm_vision_tower.rsplit('/', maxsplit=2)[-2:])
     model_config.attention_dropout = 0.
     key_info['model_path'] = model_dir
     model, tokenizer = get_model_tokenizer_with_flash_attn(
         model_dir,
         torch_dtype,
         model_kwargs,
         load_model,
@@ -2543,21 +2803,39 @@
 
 
 @register_model(
     ModelType.minicpm_2b_sft_chat,
     'OpenBMB/MiniCPM-2B-sft-fp32',
     LoRATM.llama2,
     TemplateType.minicpm,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    support_vllm=True)
 @register_model(
     ModelType.minicpm_2b_chat,
     'OpenBMB/MiniCPM-2B-dpo-fp32',
     LoRATM.llama2,
     TemplateType.minicpm,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.minicpm_1b_sft_chat,
+    'OpenBMB/MiniCPM-1B-sft-bf16',
+    LoRATM.llama2,
+    TemplateType.minicpm,
+    requires=['transformers>=4.36.0'],
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.minicpm_2b_128k,
+    'OpenBMB/MiniCPM-2B-128k',
+    LoRATM.llama2,
+    TemplateType.chatml,
+    requires=['transformers>=4.36.0'],
+    support_flash_attn=True,
+    support_vllm=True)
 def get_model_tokenizer_minicpm(model_dir: str,
                                 torch_dtype: Dtype,
                                 model_kwargs: Dict[str, Any],
                                 load_model: bool = True,
                                 **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2575,14 +2853,20 @@
 
 @register_model(
     ModelType.minicpm_v_3b_chat,
     'OpenBMB/MiniCPM-V',
     LoRATM.llama2,
     TemplateType.minicpm_v,
     support_flash_attn=True)
+@register_model(
+    ModelType.minicpm_v_v2,
+    'OpenBMB/MiniCPM-V-2',
+    LoRATM.llama2,
+    TemplateType.minicpm_v,
+    support_flash_attn=True)
 def get_model_tokenizer_minicpm_v(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     model, tokenizer = get_model_tokenizer_minicpm(model_dir, torch_dtype,
                                                    model_kwargs, load_model,
@@ -2590,14 +2874,71 @@
     if load_model:
         model.resampler.to(torch_dtype)  # fix float32
         func_list = ['generate', 'get_input_embeddings', 'forward']
         _use_submodel_func(model, 'llm', func_list)
     return model, tokenizer
 
 
+def _patch_llava(model):
+    if hasattr(model, '__old_generate'):
+        return
+    generate = model.generate
+    model.__old_generate = generate
+
+    @wraps(generate)
+    def _new_generate(inputs=None, *args, **kwargs):
+        input_ids = kwargs.pop('input_ids', None)
+        if inputs is None and input_ids is not None:
+            inputs = input_ids
+        return generate(inputs, *args, **kwargs)
+
+    model.generate = _new_generate
+
+
+@register_model(
+    ModelType.llava1d6_mistral_7b_instruct,
+    'AI-ModelScope/llava-v1.6-mistral-7b',
+    LoRATM.llama2,
+    TemplateType.llava_mistral_instruct,
+    requires=['transformers>=4.34'],
+    support_flash_attn=True,
+    tags=['multi-modal', 'vision'])
+def get_model_tokenizer_llava(model_dir: str,
+                              torch_dtype: Dtype,
+                              model_kwargs: Dict[str, Any],
+                              load_model: bool = True,
+                              **kwargs):
+    local_repo_path = _git_clone_github(
+        'https://github.com/haotian-liu/LLaVA.git')
+    sys.path.append(os.path.join(local_repo_path))
+
+    from llava.model import LlavaMistralForCausalLM, LlavaMistralConfig
+    model_config = LlavaMistralConfig.from_pretrained(model_dir)
+    model_config.mm_vision_tower = snapshot_download(
+        'AI-ModelScope/clip-vit-large-patch14-336')
+    model, tokenizer = get_model_tokenizer_with_flash_attn(
+        model_dir,
+        torch_dtype,
+        model_kwargs,
+        load_model,
+        model_config=model_config,
+        automodel_class=LlavaMistralForCausalLM,
+        **kwargs)
+
+    model.resize_token_embeddings(len(tokenizer))
+    vision_tower = model.get_vision_tower()
+    device_map = str(model_kwargs.get('device_map', str(model.device)))
+    if not vision_tower.is_loaded:
+        vision_tower.load_model(device_map=device_map)
+    if not hasattr(model.config, 'max_sequence_length'):
+        model.config.max_sequence_length = 2048
+    _patch_llava(model)
+    return model, tokenizer
+
+
 def fix_transformers_upgrade(module: PreTrainedModel) -> None:
     # from 4.35, transformers changes its arguments of _set_gradient_checkpointing
     if version.parse(transformers.__version__) >= version.parse('4.35'):
         if isinstance(module, PreTrainedModel) and hasattr(module, '_set_gradient_checkpointing') \
                 and 'value' in inspect.signature(module._set_gradient_checkpointing).parameters.keys():
             module._set_gradient_checkpointing = MethodType(
                 PreTrainedModel._set_gradient_checkpointing, module)
@@ -2707,15 +3048,15 @@
     model_info = MODEL_MAPPING[model_type]
     requires = model_info['requires']
     for require in requires:
         require_version(require)
     get_function = model_info['get_function']
     if model_kwargs is None:
         model_kwargs = {}
-    if 'device_map' not in model_kwargs:
+    if 'device_map' not in model_kwargs and not use_torchacc():
         model_kwargs['device_map'] = 'auto'
 
     if model_info.get('torch_dtype') is not None:
         model_torch_dtype = model_info['torch_dtype']
         if torch_dtype is None:
             torch_dtype = model_torch_dtype
             logger.info(f'Setting torch_dtype: {torch_dtype}')
@@ -2767,15 +3108,16 @@
     return model, tokenizer
 
 
 def get_additional_saved_files(model_type: str) -> List[str]:
     files_mapping = {
         'qwen-vl': ['SimSun.ttf'],
         'qwen-audio': ['mel_filters.npz'],
-        'deepseek-vl': ['preprocessor_config.json']
+        'deepseek-vl': ['preprocessor_config.json'],
+        'yi-vl': ['vit']
     }
     for key, files_list in files_mapping.items():
         if key in model_type:
             return files_list
     return []
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/preprocess.py` & `ms-swift-2.0.0/swift/llm/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/utils/protocol.py` & `ms-swift-2.0.0/swift/llm/utils/protocol.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/llm/utils/template.py` & `ms-swift-2.0.0/swift/llm/utils/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
+import numpy as np
 import requests
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn.utils.rnn import pad_sequence
 from transformers import PreTrainedTokenizerBase, StoppingCriteria
 
 from swift.llm.agent.utils import calculate_loss_scale
+from swift.torchacc_utils import pad_and_split_batch
+from swift.utils import get_dist_setting, use_torchacc
 
 DEFAULT_SYSTEM = 'You are a helpful assistant.'
 History = List[Union[Tuple[str, str], List[str]]]
 
 
 class TemplateType:
     # text-generation
@@ -26,14 +29,15 @@
     default = 'default'
     qwen = 'qwen'
     qwen_audio = 'qwen-audio'
     baichuan = 'baichuan'
     chatglm2 = 'chatglm2'
     chatglm3 = 'chatglm3'
     llama = 'llama'
+    llava_mistral_instruct = 'llava-mistral-instruct'
     openbuddy = 'openbuddy'
     internlm = 'internlm'
     internlm2 = 'internlm2'
     internlm_xcomposer2 = 'internlm-xcomposer2'
     yi = 'yi'
     yi_vl = 'yi-vl'
     yuan = 'yuan'
@@ -53,14 +57,18 @@
     cogagent_instruct = 'cogagent-instruct'
     orion = 'orion'
     minicpm = 'minicpm'
     minicpm_v = 'minicpm-v'
     gemma = 'gemma'
     # compatibility. (Deprecated)
     chatml = 'chatml'
+    telechat = 'telechat'
+    dbrx = 'dbrx'
+    mengzi = 'mengzi'
+    c4ai = 'c4ai'
 
     @classmethod
     def get_template_name_list(cls) -> List[str]:
         res = []
         for k in cls.__dict__.keys():
             if k.startswith('__') or k == 'get_template_name_list':
                 continue
@@ -407,34 +415,40 @@
             if padding_len > 0:
                 input_ids[0] = F.pad(input_ids[0], (0, padding_len),
                                      'constant', tokenizer.pad_token_id)
                 attention_mask[0] = F.pad(attention_mask[0], (0, padding_len),
                                           'constant', 0)
                 labels[0] = F.pad(labels[0], (0, padding_len), 'constant',
                                   -100)
-                if loss_scale:
-                    loss_scale[0] = F.pad(
-                        loss_scale[0], (0, padding_to - labels[0].shape[-1]),
-                        'constant', 0.)
+        if loss_scale:
+            loss_scale[0] = F.pad(loss_scale[0],
+                                  (0, padding_to - labels[0].shape[-1]),
+                                  'constant', 0.)
 
         input_ids = pad_sequence(
             input_ids, batch_first=True, padding_value=tokenizer.pad_token_id)
         attention_mask = pad_sequence(
             attention_mask, batch_first=True, padding_value=0)
         if loss_scale:
             loss_scale = pad_sequence(
                 loss_scale, batch_first=True, padding_value=0.)
         labels = pad_sequence(labels, batch_first=True, padding_value=-100)
 
+        if use_torchacc():
+            rank, _, world_size, _ = get_dist_setting()
+            input_ids, attention_mask, labels, loss_scale = pad_and_split_batch(
+                padding_to, input_ids, attention_mask, labels, loss_scale,
+                self.max_length, self.tokenizer, rank, world_size)
+
         res = {
             'input_ids': input_ids,
             'attention_mask': attention_mask,
             'labels': labels,
         }
-        if loss_scale is not None:
+        if loss_scale:
             res['loss_scale'] = loss_scale
         return res
 
     @staticmethod
     def get_generate_ids(generate_ids: Tensor,
                          input_token_len: int) -> List[int]:
         return generate_ids[0, input_token_len:].tolist()
@@ -563,35 +577,32 @@
         if img_path.startswith('http'):
             content = requests.get(img_path).content
             image = Image.open(BytesIO(content))
         else:
             image = Image.open(img_path)
     else:
         image = img_path
-    if image.mode in {'L', 'RGBA'}:
+    if image.mode != 'RGB':
         image = image.convert('RGB')
     return image
 
 
 class YiVLTemplate(Template):
 
     def encode(
             self, example: Dict[str,
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         inputs, _ = super().encode(example)
         inputs.pop('loss_scale', None)
         from llava.mm_utils import expand2square
-        model = self.model
         model = self.model.model
         if not hasattr(model, 'vision_tower'):
             model = model.model
         image_processor = model.vision_tower.image_processor
         images_path = example['images']
-        if not isinstance(images_path, (list, tuple)):
-            images_path = [images_path]
         images = []
         for image_path in images_path:
             image = _read_from_path(image_path)
             background_color = tuple(
                 int(x * 255) for x in image_processor.image_mean)
             image = expand2square(image, background_color)
             images.append(image)
@@ -600,16 +611,15 @@
         inputs['images'] = image_tensor.to(model.dtype)
         return inputs, {}
 
     def data_collator(self,
                       batch: List[Dict[str, Any]],
                       padding_to: Optional[int] = None) -> Dict[str, Any]:
         res = super().data_collator(batch, padding_to)
-        if batch[0].get('images') is not None:
-            res['images'] = torch.concat([b['images'] for b in batch])
+        res['images'] = torch.concat([b['images'] for b in batch])
         return res
 
 
 register_template(
     TemplateType.yi_vl,
     YiVLTemplate([], ['### Human: ', [-200], '\n{{QUERY}}\n### Assistant:'],
                  ['\n'], ['\n###'], yi_vl_default_system, ['{{SYSTEM}}\n\n']),
@@ -877,14 +887,63 @@
     ], ('You are an AI programming assistant, utilizing the Deepseek Coder model, '
         'developed by Deepseek Company, and you only answer questions related to computer science. '
         'For politically sensitive questions, security and privacy issues, '
         'and other non-computer science questions, you will refuse to answer\n'
         )))
 
 
+class LLavaTemplate(Template):
+
+    def __init__(self):
+        super().__init__(['<s>[INST] '], [[-200], '\n{{QUERY}} [/INST]'], None,
+                         ['</s>'])
+
+    def encode(
+            self, example: Dict[str,
+                                Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        inputs, _ = super().encode(example)
+        images_path = example['images']
+        images = []
+        for image_path in images_path:
+            image = _read_from_path(image_path)
+            images.append(image)
+        image_sizes = [x.size for x in images]
+        from llava.mm_utils import process_images
+        model = self.model.model
+        if not hasattr(model, 'vision_tower'):
+            model = model.model
+        image_processor = model.vision_tower.image_processor
+        images_tensor = process_images(images, image_processor,
+                                       self.model.config)
+        inputs['images'] = images_tensor.to(model.dtype)
+        inputs['image_sizes'] = image_sizes
+        return inputs, {}
+
+    def data_collator(self,
+                      batch: List[Dict[str, Any]],
+                      padding_to: Optional[int] = None) -> Dict[str, Any]:
+        res = super().data_collator(batch, padding_to)
+        res['images'] = torch.concat([b['images'] for b in batch])
+        res['image_sizes'] = sum([b['image_sizes'] for b in batch], start=[])
+        return res
+
+    @staticmethod
+    def get_generate_ids(generate_ids: Tensor,
+                         input_token_len: int) -> List[int]:
+        return generate_ids[0].tolist()
+
+
+register_template(
+    TemplateType.llava_mistral_instruct,
+    LLavaTemplate(),
+    use_model=True,
+    infer_media_type='round',
+    lazy_tokenize=True)
+
+
 def _findall(token_list: List[int], token: int) -> List[int]:
     """Find the index of a token in the token_list."""
     res = []
     idx = -1
     try:
         while True:
             idx = token_list.index(token, idx + 1)
@@ -908,16 +967,14 @@
             self.DEEPSEEK_VL_SYSTEM)
 
     def encode(
             self, example: Dict[str,
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         inputs, _ = super().encode(example)
         images_path = example['images']
-        if not isinstance(images_path, (list, tuple)):
-            images_path = [images_path]
         images = []
         for image_path in images_path:
             image = _read_from_path(image_path)
             images.append(image)
 
         vl_chat_processor = self.tokenizer.vl_chat_processor
         input_ids, labels = inputs['input_ids'], inputs['labels']
@@ -1099,25 +1156,80 @@
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         images_path = example['images']
         assert len(images_path) == 1
         image = _read_from_path(images_path[0])
         inputs, _ = super().encode(example)
         input_ids = inputs['input_ids']
         labels = inputs['labels']
-        idx = input_ids.index(0)
+
+        img_start_idxs = np.where(
+            np.array(input_ids) == self.tokenizer.im_start_id)[0]
+        if len(
+                img_start_idxs
+        ) > 1:  # if mutli-round, input_ids have mutli <image><unk></image>\n
+            start = 0
+            new_input_ids = []
+            for idx in img_start_idxs[1:]:
+                new_input_ids = new_input_ids + input_ids[start:idx]
+                start = idx + 4  # skip <image><unk></image>\n
+            new_input_ids = new_input_ids + input_ids[start:]
+            input_ids = new_input_ids
+
+        idx = img_start_idxs[0] + 1  # first <unk>
         config = self.model.config
-        input_ids = (
-            input_ids[:idx] + [self.tokenizer.unk_token_id] * config.query_num
-            + input_ids[idx + 1:])
-        if labels is not None:
-            labels = (
-                labels[:idx] + [-100] * config.query_num + labels[idx + 1:])
-        image_bound = [torch.tensor([[idx, idx + config.query_num]])]
-        pixel_values = self.model.transform(image)[None].to(
-            device=self.model.device)
+        if hasattr(config, 'slice_mode') and config.slice_mode:
+            slice_mode = True
+            assert hasattr(config, 'patch_size')
+            assert hasattr(config, 'max_slice_nums')
+            assert hasattr(config, 'scale_resolution')
+        else:
+            slice_mode = False
+
+        if slice_mode:
+            images, placeholder = self.model.get_slice_image_placeholder(
+                image, self.tokenizer)
+            placeholder_id = self.tokenizer.encode(
+                placeholder, add_special_tokens=False)
+            input_ids = (
+                input_ids[:idx - 1] + placeholder_id + input_ids[idx + 2:])
+            if labels is not None:
+                labels = (
+                    labels[:idx - 1] + [-100] * len(placeholder_id)
+                    + labels[idx + 2])
+            input_tensor_ids = torch.tensor(input_ids)
+            image_start_idx = torch.where(
+                input_tensor_ids == self.tokenizer.im_start_id)[0]
+            image_start_idx += 1
+            image_end_idx = torch.where(
+                input_tensor_ids == self.tokenizer.im_end_id)[0]
+            valid_image_nums = max(len(image_start_idx), len(image_end_idx))
+            image_bound = [
+                torch.hstack([
+                    image_start_idx[:valid_image_nums].unsqueeze(-1),
+                    image_end_idx[:valid_image_nums].unsqueeze(-1)
+                ])
+            ]
+            pixel_values = [
+                self.model.transform(img).to(device=self.model.device)
+                for img in images
+            ]
+
+        else:
+            input_ids = (
+                input_ids[:idx]
+                + [self.tokenizer.unk_token_id] * config.query_num
+                + input_ids[idx + 1:])
+            if labels is not None:
+                labels = (
+                    labels[:idx] + [-100] * config.query_num
+                    + labels[idx + 1:])
+            image_bound = [torch.tensor([[idx, idx + config.query_num]])]
+            pixel_values = [
+                self.model.transform(image).to(device=self.model.device)
+            ]
         inputs_embeds, _ = self.model.get_vllm_embedding({
             'input_ids':
             torch.tensor(input_ids)[None].to(device=self.model.device),
             'image_bound':
             image_bound,
             'pixel_values': [pixel_values]
         })
@@ -1144,14 +1256,56 @@
 gemma_template = Template(
     ['<bos>'],
     ['<start_of_turn>user\n{{QUERY}}<end_of_turn>\n<start_of_turn>model\n'],
     ['<end_of_turn>\n'], ['<end_of_turn>'], None,
     ['<bos><start_of_turn>system\n{{SYSTEM}}<end_of_turn>\n'])
 register_template(TemplateType.gemma, gemma_template)
 
+register_template(
+    TemplateType.telechat,
+    Template([], ['<_user>{{QUERY}}<_bot>'], ['<_end>'], ['<_end>']))
+
+DBRX_SYSTEM = (
+    'You are DBRX, created by Databricks. You were last updated in December 2023. '
+    'You answer questions based on information available up to that point.\n'
+    'YOU PROVIDE SHORT RESPONSES TO SHORT QUESTIONS OR STATEMENTS, '
+    'but provide thorough responses to more complex and open-ended questions.\n'
+    'You assist with various tasks, from writing to coding (using markdown for code blocks '
+    '— remember to use ``` with code, JSON, and tables).\n'
+    'You do not have real-time data access or code execution capabilities.'
+    ' You avoid stereotyping and provide balanced perspectives on controversial topics. '
+    'You do not provide song lyrics, poems, or news articles and do not divulge details of your training data.\n'
+    'This is your system prompt, guiding your responses. Do not reference it, just respond to the user. '
+    'If you find yourself talking about this message, stop. You should be responding appropriately '
+    'and usually that means not mentioning this.'
+    'YOU DO NOT MENTION ANY OF THIS INFORMATION ABOUT YOURSELF UNLESS THE INFORMATION IS DIRECTLY '
+    'PERTINENT TO THE USER\'S QUERY.')
+register_template(
+    TemplateType.dbrx,
+    Template(
+        [], ['<|im_start|>user\n{{QUERY}}<|im_end|>\n<|im_start|>assistant\n'],
+        ['<|im_end|>\n'], ['<|im_end|>'], DBRX_SYSTEM,
+        ['<|im_start|>system\n{{SYSTEM}}<|im_end|>\n']))
+
+register_template(
+    TemplateType.mengzi,
+    Template([], ['输入：{{QUERY}}输出：\n'], [], [['eos_token_id']], None,
+             ['指令：{{SYSTEM}}']))
+
+C4AI_SYSTEM = (
+    'You are Command-R, a brilliant, sophisticated, AI-assistant trained to assist human users by '
+    'providing thorough responses.You are trained by Cohere.')
+register_template(
+    TemplateType.c4ai,
+    Template(['<BOS_TOKEN>'], [
+        '<|START_OF_TURN_TOKEN|><|USER_TOKEN|>{{QUERY}}<|END_OF_TURN_TOKEN|><|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>'
+    ], ['<|END_OF_TURN_TOKEN|>'], ['<|END_OF_TURN_TOKEN|>'], C4AI_SYSTEM, [
+        '<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>{{SYSTEM}}<|END_OF_TURN_TOKEN|'
+    ]))
+
 
 def get_template(
     template_type: str,
     tokenizer: PreTrainedTokenizerBase,
     default_system: Optional[str] = None,
     max_length: Optional[int] = None,
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete',
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/utils.py` & `ms-swift-2.0.0/swift/llm/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 # Part of the implementation is borrowed from huggingface/transformers.
 import heapq
 import importlib.util
 import logging
 import os
 import shutil
+import sys
 from copy import deepcopy
 from functools import partial, wraps
 from queue import Empty, Queue
 from tempfile import TemporaryDirectory
 from threading import Thread
 from typing import (Any, Callable, Dict, Iterator, List, Mapping, Optional,
                     Sequence, Tuple, Union)
@@ -34,17 +35,18 @@
 from tqdm.auto import tqdm
 from transformers import (GenerationConfig, PretrainedConfig, PreTrainedModel,
                           PreTrainedTokenizerBase, StoppingCriteriaList,
                           TextStreamer, trainer)
 from transformers.generation.streamers import BaseStreamer
 
 from swift.hub import ModelScopeConfig
-from swift.tuners.module_mapping import MODEL_KEYS_MAPPING, ModelKeys
+from swift.tuners.module_mapping import MODEL_KEYS_MAPPING
 from swift.utils import (get_dist_setting, get_logger, is_ddp_plus_mp, is_dist,
-                         is_local_master, is_master, stat_array, upper_bound)
+                         is_local_master, is_master, stat_array, upper_bound,
+                         use_torchacc)
 from .template import History, StopWords, StopWordsCriteria, Template
 
 logger = get_logger()
 ms_logger = get_ms_logger()
 
 logger_format = logging.Formatter('[%(levelname)s:%(name)s] %(message)s')
 
@@ -393,20 +395,31 @@
             linear_cls.append(AutoGPTQQuantLinear)
     if 'awq' in model_type:
         from awq.modules.linear import WQLinear_GEMM
         linear_cls.append(WQLinear_GEMM)
     if 'aqlm' in model_type:
         from aqlm import QuantizedLinear
         linear_cls.append(QuantizedLinear)
+
+    # The content of target_module_names cannot exist in inner_nodes.
+    # O(n^2logn), n represents the number of nodes, n<1000.
+    inner_nodes = set()
+    for name, module in model.named_modules():
+        if not isinstance(module, tuple(linear_cls)):
+            inner_nodes.add(name)
     target_module_names = set()
     for name, module in model.named_modules():
-        if isinstance(module, tuple(linear_cls)):
-            module_name = '.'.join(name.split('.')[-2:])
-            if head_module_name not in module_name:
-                target_module_names.add(module_name)
+        if isinstance(module,
+                      tuple(linear_cls)) and head_module_name not in name:
+            module_name_list = name.split('.')
+            module_name = module_name_list.pop()
+            for inner_node in inner_nodes:
+                while inner_node.endswith(module_name):
+                    module_name = f'{module_name_list.pop()}.{module_name}'
+            target_module_names.add(module_name)
     return list(target_module_names)
 
 
 def sort_by_max_length(llm_dataset: LLMDataset, num_dataset: int) -> HfDataset:
     logger.info('sort by max length...')
     dataset_len = [len(d['input_ids']) for d in llm_dataset]
     idx = heapq.nlargest(
@@ -425,14 +438,27 @@
             or (cp >= 0xF900 and cp <= 0xFAFF)
             or (cp >= 0x2F800 and cp <= 0x2FA1F)):
         return True
 
     return False
 
 
+def _get_safe_print_idx(response: str,
+                        print_idx: int,
+                        is_finished: bool = False) -> int:
+    if is_finished:
+        return len(response)
+    if response.endswith('\n') or len(response) > 0 and _is_chinese_char(
+            ord(response[-1])):
+        print_idx = len(response)
+    else:
+        print_idx = max(response.rfind(' ') + 1, print_idx)
+    return print_idx
+
+
 def to_device(inputs: Any, device: Device) -> Any:
     if callable(getattr(inputs, 'to', None)):
         return inputs.to(device=device)
     #
     if isinstance(inputs, Mapping):
         res = {}
         for k, v in inputs.items():
@@ -543,14 +569,20 @@
         generation_config.eos_token_id = tokenizer.eos_token_id
     if tokenizer.pad_token_id is not None:
         generation_config.pad_token_id = tokenizer.pad_token_id
     if tokenizer.bos_token_id is not None:
         generation_config.bos_token_id = tokenizer.bos_token_id
     if generation_config.max_new_tokens is not None:
         generation_config.max_length = 20  # fix max_length, max_new_tokens warning
+        max_length = get_max_model_len(model.config)
+        if max_length and token_len + generation_config.max_new_tokens > max_length:
+            generation_config.max_new_tokens = max_length - token_len
+            if generation_config.max_new_tokens <= 0:
+                raise AssertionError('Current sentence length exceeds'
+                                     f'the model max_length: {max_length}')
     if template.suffix[-1] not in stop_words:
         stop_words.append(template.suffix[-1])
     stopping_criteria = StoppingCriteriaList(
         [StopWordsCriteria(tokenizer, stop_words, **tokenizer_kwargs)])
     inputs = to_device(inputs, device)
     if generation_info is not None:
         generation_info['num_prompt_tokens'] = token_len
@@ -566,44 +598,55 @@
     thread = Thread(target=model.generate, kwargs=generation_kwargs)
     thread.start()
     raw_generate_ids, generate_ids = [], []
     response, safe_response = '', ''
     print_idx = 0
     if not is_observation:
         history.append(None)  # dummy
+    # Avoid the occurrence of repeated words in sentence.
+    first_num_space = -1
     for token in streamer:
         raw_generate_ids.append(token)
         generate_ids = template.get_generate_ids(
             torch.tensor(raw_generate_ids)[None], token_len)
         if generation_info is not None:
             generation_info['num_generated_tokens'] = len(generate_ids)
         # avoid printing template.suffix[-1])
         if isinstance(template.suffix[-1], list):
             generate_ids = generate_ids[:-len(template.suffix[-1])]
         response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
+        cur_num_space = len(response) - len(response.lstrip(' '))
+        if first_num_space == -1:
+            first_num_space = cur_num_space
+        if cur_num_space < first_num_space:
+            response = ' ' * (first_num_space - cur_num_space) + response
+        elif cur_num_space > first_num_space:
+            response = response[cur_num_space - first_num_space:]
         if isinstance(template.suffix[-1], str):
             response = response[:-len(template.suffix[-1])]
-        if response.endswith('\n') or len(response) > 0 and _is_chinese_char(
-                ord(response[-1])):
-            print_idx = len(response)
-        else:
-            print_idx = max(response.rfind(' ') + 1, print_idx)
+        print_idx = _get_safe_print_idx(response, print_idx)
         # avoid printing incomplete words
         if safe_response != response[:print_idx]:
             safe_response = response[:print_idx]
             if not is_observation:
                 history[-1] = [query, safe_response]
             else:
                 history[-1][-1] = history[-1][-1][:act_length] + safe_response
             yield safe_response, history
     # avoid printing template.suffix[-1])
     if (isinstance(template.suffix[-1], list) and
             generate_ids[-len(template.suffix[-1]):] == template.suffix[-1]):
         generate_ids = generate_ids[:-len(template.suffix[-1])]
     response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
+    if first_num_space > -1:
+        cur_num_space = len(response) - len(response.lstrip(' '))
+        if cur_num_space < first_num_space:
+            response = ' ' * (first_num_space - cur_num_space) + response
+        elif cur_num_space > first_num_space:
+            response = response[cur_num_space - first_num_space:]
     if isinstance(
             template.suffix[-1], str
     ) and response[-len(template.suffix[-1]):] == template.suffix[-1]:
         response = response[:-len(template.suffix[-1])]
     if not is_observation:
         history[-1] = [query, response]
     else:
@@ -693,14 +736,20 @@
         generation_config.eos_token_id = tokenizer.eos_token_id
     if tokenizer.pad_token_id is not None:
         generation_config.pad_token_id = tokenizer.pad_token_id
     if tokenizer.bos_token_id is not None:
         generation_config.bos_token_id = tokenizer.bos_token_id
     if generation_config.max_new_tokens is not None:
         generation_config.max_length = 20  # fix max_length, max_new_tokens warning
+        max_length = get_max_model_len(model.config)
+        if max_length and token_len + generation_config.max_new_tokens > max_length:
+            generation_config.max_new_tokens = max_length - token_len
+            if generation_config.max_new_tokens <= 0:
+                raise AssertionError('Current sentence length exceeds'
+                                     f'the model max_length: {max_length}')
     if template.suffix[-1] not in stop_words:
         stop_words.append(template.suffix[-1])
     stopping_criteria = StoppingCriteriaList(
         [StopWordsCriteria(tokenizer, stop_words, **tokenizer_kwargs)])
     inputs = to_device(inputs, device)
     if generation_info is not None:
         generation_info['num_prompt_tokens'] = token_len
@@ -734,18 +783,20 @@
     else:
         history[-1][-1] = history[-1][-1] + response
     return response, history
 
 
 def limit_history_length(template: Template, query: str,
                          history: Optional[History],
-                         max_length: int) -> Tuple[History, History]:
+                         max_length: Optional[int]) -> Tuple[History, History]:
     """binary search"""
     if history is None:
         history = []
+    if max_length is None:
+        return [], history
 
     def compute_token_length(history_length: int) -> int:
         assert history_length != 0
         example = {'query': query, 'history': history[-history_length:]}
         input_ids = template.encode(example)[0]['input_ids']
         return len(input_ids)
 
@@ -853,13 +904,15 @@
 if is_ddp_plus_mp():
     _old_ddp_init = DDP.__init__
     accelerate.accelerator.torch.nn.parallel.DistributedDataParallel.__init__ = (
         lambda self, model, device_ids, output_device, *args, **kwargs:
         _old_ddp_init(self, model, *args, **kwargs))
     transformers.modeling_utils.get_balanced_memory = lambda *args, **kwargs: None
     transformers.modeling_utils.infer_auto_device_map = _infer_auto_device_map_patch
+
+if is_ddp_plus_mp() or use_torchacc():
     _old_accelerator_init = trainer.Accelerator.__init__
     trainer.Accelerator.__init__ = (
         lambda self, device_placement=False, *args, **kwargs:
         _old_accelerator_init(
             self, device_placement=device_placement, *args, **kwargs))
     trainer.Accelerator.verify_device_map = lambda *args, **kwargs: False
```

### Comparing `ms-swift-1.7.3/swift/llm/utils/vllm_utils.py` & `ms-swift-2.0.0/swift/llm/utils/vllm_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,32 +10,41 @@
 from packaging import version
 from torch import dtype as Dtype
 from tqdm import tqdm
 from transformers import PreTrainedTokenizerBase
 from vllm import (AsyncEngineArgs, AsyncLLMEngine, EngineArgs, LLMEngine,
                   SamplingParams)
 
+from swift.tuners import Swift
 from swift.utils import get_logger, seed_everything
 from .argument import InferArguments
 from .model import get_model_tokenizer
 from .template import Template, get_template
-from .utils import _is_chinese_char
+from .utils import _get_safe_print_idx
+
+try:
+    from vllm.lora.request import LoRARequest
+except ImportError:
+    pass
 
 logger = get_logger()
 
 
 def get_vllm_engine(model_type: str,
                     torch_dtype: Optional[Dtype] = None,
                     *,
                     model_id_or_path: Optional[str] = None,
                     gpu_memory_utilization: float = 0.9,
                     tensor_parallel_size: int = 1,
                     max_model_len: Optional[int] = None,
                     engine_kwargs: Optional[Dict[str, Any]] = None,
                     use_async: bool = False,
+                    enable_lora: bool = False,
+                    max_loras: int = 1,
+                    max_lora_rank: int = 16,
                     **kwargs) -> LLMEngine:
     model_dir = kwargs.pop('model_dir', None)  # compat with swift<1.7
     tokenizer = get_model_tokenizer(
         model_type,
         load_model=False,
         model_id_or_path=model_id_or_path,
         model_dir=model_dir)[1]
@@ -55,14 +64,25 @@
     if use_async:
         engine_args_cls = AsyncEngineArgs
         llm_engine_cls = AsyncLLMEngine
         engine_kwargs['disable_log_requests'] = True
     else:
         engine_args_cls = EngineArgs
         llm_engine_cls = LLMEngine
+
+    parameters = inspect.signature(engine_args_cls.__init__).parameters
+    if 'enable_lora' in parameters:
+        engine_kwargs['enable_lora'] = enable_lora
+        engine_kwargs['max_loras'] = max_loras
+        engine_kwargs['max_lora_rank'] = max_lora_rank
+    else:
+        assert not enable_lora, (
+            'The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.'
+        )
+
     engine_args = engine_args_cls(
         model=model_dir,
         trust_remote_code=True,
         dtype=dtype,
         gpu_memory_utilization=gpu_memory_utilization,
         tensor_parallel_size=tensor_parallel_size,
         max_model_len=max_model_len,
@@ -180,14 +200,15 @@
 
 def inference_stream_vllm(
         llm_engine: LLMEngine,
         template: Template,
         request_list: List[Dict[str, Any]],
         *,
         generation_config: Optional[VllmGenerationConfig] = None,
+        lora_request: Optional['LoRARequest'] = None,
         use_tqdm: bool = False,
         **kwargs) -> Iterator[List[Dict[str, Any]]]:
     """
     request_list: e.g. [{'query': 'hello!'}].
         The keys that can be included are: 'query', 'history', 'system'.
     generation_config: Priority: generation_config > model.generation_config.
     return: e.g. [{'response': 'hi!', 'history': [('hello!', 'hi!')]}].
@@ -206,14 +227,22 @@
     tokenizer = template.tokenizer
     if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
         generation_config.stop.append(tokenizer.eos_token)
     if isinstance(template.suffix[-1],
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
 
+    parameters = inspect.signature(llm_engine.add_request).parameters
+    add_request_kwargs = {}
+    if 'lora_request' in parameters:
+        add_request_kwargs['lora_request'] = lora_request
+    else:
+        assert lora_request is None, (
+            'The current version of VLLM does not support `lora_request`. Please upgrade VLLM.'
+        )
     request_temp = []
     for i, request in enumerate(request_list):
         history = request.get('history', None)
         if history is None:
             history = []
 
         # agent support
@@ -224,34 +253,35 @@
             history[-1][-1] = history[-1][-1] + request['query']
             act_length = len(history[-1][-1])
             request['query'] = None
         request_temp.append((is_observation, act_length))
 
         request['history'] = history
         inputs = template.encode(request)[0]
+        if len(inputs) == 0:
+            raise ValueError(
+                'input_ids exceeds `max_length`. Please increase the value of `max_length`.'
+            )
         input_ids = inputs['input_ids']
-        llm_engine.add_request(str(i), None, generation_config, input_ids)
+        llm_engine.add_request(
+            str(i), None, generation_config, input_ids, **add_request_kwargs)
 
     batch_size = len(request_list)
     resp_list = [None] * batch_size
     print_idx_list = [0] * batch_size
     prog_bar = tqdm(total=batch_size, dynamic_ncols=True, disable=not use_tqdm)
     while llm_engine.has_unfinished_requests():
         step_outputs = llm_engine.step()
         for output in step_outputs:
             i = int(output.request_id)
             request = request_list[i]
             response = tokenizer.decode(output.outputs[0].token_ids, True)
-            if output.finished or response.endswith(
-                    '\n') or len(response) > 0 and _is_chinese_char(
-                        ord(response[-1])):
-                print_idx_list[i] = len(response)
-            else:
-                print_idx_list[i] = max(
-                    response.rfind(' ') + 1, print_idx_list[i])
+            print_idx_list[i] = _get_safe_print_idx(response,
+                                                    print_idx_list[i],
+                                                    output.finished)
             # avoid printing incomplete words
             safe_response = response[:print_idx_list[i]]
             query = request['query']
             history = request['history']
             if resp_list[i] is None and not request_temp[i][0]:
                 history.append(None)
             if not request_temp[i][0]:
@@ -266,14 +296,15 @@
 
 
 def inference_vllm(llm_engine: LLMEngine,
                    template: Template,
                    request_list: List[Dict[str, Any]],
                    *,
                    generation_config: Optional[VllmGenerationConfig] = None,
+                   lora_request: Optional['LoRARequest'] = None,
                    use_tqdm: bool = False,
                    verbose: bool = False,
                    prompt_prefix: str = '[PROMPT]',
                    output_prefix: str = '[OUTPUT]',
                    **kwargs) -> List[Dict[str, Any]]:
     """
     request_list: e.g. [{'query': 'hello!'}].
@@ -292,28 +323,42 @@
     tokenizer = template.tokenizer
     if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
         generation_config.stop.append(tokenizer.eos_token)
     if isinstance(template.suffix[-1],
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
 
+    parameters = inspect.signature(llm_engine.add_request).parameters
+    add_request_kwargs = {}
+    if 'lora_request' in parameters:
+        add_request_kwargs['lora_request'] = lora_request
+    else:
+        assert lora_request is None, (
+            'The current version of VLLM does not support `lora_request`. Please upgrade VLLM.'
+        )
+
     for i, request in enumerate(request_list):
         history = request.get('history', None)
         if history is None:
             history = []
 
         is_observation = history[-1][-1].endswith(
             'Observation:') if history and history[-1][-1] else False
         if is_observation:
             history[-1][-1] = history[-1][-1] + request['query']
             request['query'] = None
         request['history'] = history
         inputs = template.encode(request)[0]
+        if len(inputs) == 0:
+            raise ValueError(
+                'input_ids exceeds `max_length`. Please increase the value of `max_length`.'
+            )
         input_ids = inputs['input_ids']
-        llm_engine.add_request(str(i), None, generation_config, input_ids)
+        llm_engine.add_request(
+            str(i), None, generation_config, input_ids, **add_request_kwargs)
 
     batch_size = len(request_list)
     if use_tqdm is True:
         assert verbose is False
     prog_bar = tqdm(total=batch_size, dynamic_ncols=True, disable=not use_tqdm)
     outputs = []
     while llm_engine.has_unfinished_requests():
@@ -346,29 +391,33 @@
 def prepare_vllm_engine_template(
         args: InferArguments,
         use_async: bool = False) -> Tuple[LLMEngine, Template]:
     logger.info(f'device_count: {torch.cuda.device_count()}')
     seed_everything(args.seed)
 
     assert args.quantization_bit == 0, 'not support bnb'
-    assert args.sft_type == 'full', 'you need to merge lora'
+    assert not (args.sft_type == 'lora'
+                and not args.vllm_enable_lora), 'you need to merge lora'
     # Loading Model and Tokenizer
     model_id_or_path = None
     if args.sft_type == 'full' and args.ckpt_dir is not None:
         model_id_or_path = args.ckpt_dir
     elif args.model_id_or_path is not None:
         model_id_or_path = args.model_id_or_path
     llm_engine = get_vllm_engine(
         args.model_type,
         args.torch_dtype,
         gpu_memory_utilization=args.gpu_memory_utilization,
         tensor_parallel_size=args.tensor_parallel_size,
         max_model_len=args.max_model_len,
         use_async=use_async,
-        model_id_or_path=model_id_or_path)
+        model_id_or_path=model_id_or_path,
+        enable_lora=args.vllm_enable_lora,
+        max_loras=len(args.vllm_lora_modules),
+        max_lora_rank=args.vllm_max_lora_rank)
     tokenizer = llm_engine.hf_tokenizer
     if use_async:
         model_config = asyncio.run(llm_engine.get_model_config())
         llm_engine.model_config = model_config
     else:
         model_config = llm_engine.model_config
     logger.info(f'model_config: {model_config.hf_config}')
```

### Comparing `ms-swift-1.7.3/swift/trainers/__init__.py` & `ms-swift-2.0.0/swift/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/arguments.py` & `ms-swift-2.0.0/swift/trainers/arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import torch
 from transformers.training_args import TrainingArguments as HfTrainingArguments
 from transformers.training_args_seq2seq import \
     Seq2SeqTrainingArguments as HfSeq2SeqTrainingArguments
 from transformers.utils import is_accelerate_available
 
-from swift.utils import is_dist
+from swift.utils import is_dist, use_torchacc
 
 
 @dataclass
 class SwiftArgumentsMixin:
     # ckpt only save model
     save_only_model: bool = False
     train_sampler_random: bool = True
@@ -48,8 +48,11 @@
 class TrainingArguments(SwiftArgumentsMixin, HfTrainingArguments):
     pass
 
 
 @dataclass
 class Seq2SeqTrainingArguments(SwiftArgumentsMixin,
                                HfSeq2SeqTrainingArguments):
-    pass
+
+    @property
+    def place_model_on_device(self):
+        return False if use_torchacc() else super().place_model_on_device
```

### Comparing `ms-swift-1.7.3/swift/trainers/callback.py` & `ms-swift-2.0.0/swift/trainers/callback.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/dpo_trainers.py` & `ms-swift-2.0.0/swift/trainers/dpo_trainers.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,40 @@
                  template: Template,
                  sft_beta=0.,
                  test_oom_error=False,
                  **kwargs):
         self.template = template
         self.sft_beta = sft_beta
         super().__init__(*args, **kwargs)
-        self.stat_dataset(self.train_dataset)
-        self.stat_dataset(self.eval_dataset)
+        train_ds_info = self.stat_dataset(self.train_dataset)
+        val_ds_info = self.stat_dataset(self.eval_dataset)
+        self.dataset_info = {
+            'train_dataset': train_ds_info,
+            'val_dataset': val_ds_info
+        }
         if test_oom_error:
             self.train_dataset = sort_by_max_length(self.train_dataset, 20000)
+        # performance
+        self.perf: Dict[str, Any] = {
+            'gen_time':
+            0.,
+            'gen_len':
+            0,
+            'memory': {},
+            'model':
+            self.model.get_trainable_parameters() if hasattr(
+                self.model, 'get_trainable_parameters') else None,
+        }
+
+    def train(self, *args, **kwargs) -> torch.Tensor:
+        res = super().train(*args, **kwargs)
+        for i in range(torch.cuda.device_count()):
+            self.perf['memory'][
+                f'cuda:{i}'] = f'{torch.cuda.max_memory_reserved(i)/1024/1024/1024:.2f}GiB'
+        return res
 
     def concat_template(self, feature):
         query: Optional[str] = feature.get('query', None)
         system: Optional[str] = feature.get('system', None)
         history: List = feature.get('history', [])
         if system is None:
             if self.template.use_default_system:
@@ -183,15 +205,15 @@
         else:
             # encoder-decoder
             batch = super().tokenize_row(feature, model)
 
         return batch
 
     @staticmethod
-    def stat_dataset(llm_dataset) -> None:
+    def stat_dataset(llm_dataset) -> Any:
         _token_len = []
         from datasets import Dataset as HfDataset
         from swift.utils.np_utils import stat_array
         if isinstance(llm_dataset, HfDataset):
             chosen = llm_dataset['chosen_input_ids']
             rejected = llm_dataset['rejected_input_ids']
             for cc, rr in zip(chosen, rejected):
@@ -200,14 +222,15 @@
             for d in llm_dataset:
                 _token_len.append(
                     max(
                         len(d['chosen_input_ids']),
                         len(d['rejected_input_ids'])))
         _, stat_str = stat_array(_token_len)
         logger.info(f'Dataset Token Length: {stat_str}')
+        return stat_str
 
     def get_batch_loss_metrics(
         self,
         model,
         batch: Dict[str, Union[List, torch.LongTensor]],
         train_eval: Literal['train', 'eval'] = 'train',
     ):
```

### Comparing `ms-swift-1.7.3/swift/trainers/mixin.py` & `ms-swift-2.0.0/swift/trainers/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,36 @@
 import numpy as np
 import safetensors
 import torch
 import transformers
 from datasets import Dataset as HfDataset
 from packaging import version
 from peft import PeftModel
-from torch import nn
 from torch.nn import Module
-from transformers import (PreTrainedModel, PreTrainedTokenizerBase,
-                          is_bitsandbytes_available)
+from transformers import PreTrainedModel, PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollator
 from transformers.modeling_utils import unwrap_model
 from transformers.trainer import ADAPTER_CONFIG_NAME  # noqa
 from transformers.trainer import (ADAPTER_SAFE_WEIGHTS_NAME,
                                   ADAPTER_WEIGHTS_NAME, CONFIG_NAME,
                                   PREFIX_CHECKPOINT_DIR, SAFE_WEIGHTS_NAME,
                                   TRAINER_STATE_NAME, TRAINING_ARGS_NAME,
                                   WEIGHTS_NAME, IntervalStrategy, Trainer,
                                   TrainerCallback, is_peft_available)
 from transformers.trainer_utils import EvalPrediction
 from transformers.training_args import TrainingArguments
 
 from swift.hub import Repository
 from swift.hub.check_model import check_local_model_is_latest
+from swift.torchacc_utils import (save_ta_checkpoint,
+                                  ta_load_optimizer_and_scheduler,
+                                  ta_save_optimizer_and_scheduler)
 from swift.tuners import SwiftModel
-from swift.utils import check_json_format, create_ms_repo, get_logger
+from swift.utils import (check_json_format, create_ms_repo, get_logger,
+                         use_torchacc)
 from swift.utils.constants import Invoke
 from .optimizers.galore import create_optimizer_and_scheduler
 from .utils import (can_return_loss, find_labels, get_function,
                     is_instance_of_ms_model)
 
 logger = get_logger()
 
@@ -355,14 +357,39 @@
             json.dump(
                 check_json_format(self.sft_args.__dict__),
                 f,
                 ensure_ascii=False,
                 indent=2)
         return
 
+    def _save_optimizer_and_scheduler(self, output_dir):
+        if not use_torchacc():
+            return super()._save_optimizer_and_scheduler(output_dir)
+
+        ta_save_optimizer_and_scheduler(self.optimizer, self.lr_scheduler,
+                                        output_dir)
+
+    def _load_optimizer_and_scheduler(self, checkpoint):
+        if not use_torchacc():
+            return super()._load_optimizer_and_scheduler(checkpoint)
+
+        if checkpoint is None or self.args.save_only_model:
+            return
+
+        self.optimizer, self.lr_scheduler = ta_load_optimizer_and_scheduler(
+            self.optimizer, self.lr_scheduler, checkpoint, self.args.device)
+
+    def _save_tpu(self, output_dir: Optional[str] = None):
+        if not use_torchacc():
+            return super()._save_tpu(output_dir)
+
+        output_dir = output_dir if output_dir is not None else self.args.output_dir
+        logger.info(f'Saving model checkpoint to {output_dir}')
+        save_ta_checkpoint(self.model, self.tokenizer, self.args, output_dir)
+
     def _save(self, output_dir: Optional[str] = None, state_dict=None):
         """Compatible with swift and peft"""
         # If we are executing this function, we are the process zero, so we don't check for that.
         output_dir = output_dir if output_dir is not None else self.args.output_dir
         os.makedirs(output_dir, exist_ok=True)
         # configuration.json
         model_dir = getattr(self.model, 'model_dir', None)
@@ -421,16 +448,18 @@
         torch.save(self.args, os.path.join(output_dir, 'training_args.bin'))
         # additional files
         additional_files = getattr(self.args, 'additional_saved_files', [])
         if model_dir is not None:
             for file in additional_files:
                 src_path = os.path.join(model_dir, file)
                 dst_path = os.path.join(output_dir, file)
-                if os.path.exists(src_path):
+                if os.path.isfile(src_path):
                     shutil.copy(src_path, dst_path)
+                elif os.path.isdir(src_path):
+                    shutil.copytree(src_path, dst_path)
 
     def _save_checkpoint(self, model, trial, metrics=None):
         self.state.last_model_checkpoint = os.path.join(
             self.args.output_dir, f'checkpoint-{self.state.global_step}')
         logger.info(
             f'Saving model checkpoint to {self.state.last_model_checkpoint}')
         if version.parse(transformers.__version__) >= version.parse(
@@ -485,15 +514,22 @@
             return self._get_eval_sampler(self.train_dataset)
 
     def _load_from_checkpoint(self,
                               resume_from_checkpoint: str,
                               model=None) -> None:
         if model is None:
             model = self.model
-        if not isinstance(model, SwiftModel):
+        supported_classes = (SwiftModel, PeftModel)
+        if use_torchacc():
+            # Loading checkpoint of TorchAcc has been done in tuner.py when
+            # sft_type if 'full'.
+            model = model._get_underlay_model().module.module
+            if isinstance(model, PreTrainedModel):
+                return
+        if not isinstance(model, supported_classes):
             # Avoid throwing exceptions
             return super()._load_from_checkpoint(resume_from_checkpoint, model)
 
     def _sorted_checkpoints(self,
                             output_dir=None,
                             checkpoint_prefix=PREFIX_CHECKPOINT_DIR,
                             use_mtime=False) -> List[str]:
@@ -613,22 +649,24 @@
             if version.parse(
                     transformers.__version__) < version.parse('4.34.0'):
                 logger.warning(
                     f'If you are using lora+, please remember using transformers>=4.34.0, '
                     f'but now is {transformers.__version__}')
                 return super().create_optimizer()
 
-            decay_parameters = self.get_decay_parameter_names(opt_model)
-            if isinstance(self.model, SwiftModel):
-                # Lora+ parameter groups (or a default one)
+            optimizer_grouped_parameters = None
+            if hasattr(self.model, 'create_optimizer_param_groups'):
+                # Lora+ parameter groups
                 optimizer_grouped_parameters = self.model.create_optimizer_param_groups(
                     lr=self.args.learning_rate,
                     weight_decay=self.args.weight_decay)
-            else:
+
+            if optimizer_grouped_parameters is None:
                 # Default parameter groups
+                decay_parameters = self.get_decay_parameter_names(opt_model)
                 optimizer_grouped_parameters = [
                     {
                         'params': [
                             p for n, p in opt_model.named_parameters()
                             if (n in decay_parameters and p.requires_grad)
                         ],
                         'weight_decay':
```

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/__init__.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/adafactor.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/adafactor.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/adamw.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/adamw8bit.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw8bit.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/galore_projector.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/galore_projector.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/trainers/optimizers/galore/utils.py` & `ms-swift-2.0.0/swift/trainers/optimizers/galore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from dataclasses import dataclass
 from typing import Any, Dict, List, Tuple, Union
 
 import torch
 from torch import nn
 from torch.optim import Optimizer
-from torch.optim.lr_scheduler import LRScheduler
 from transformers import Trainer, TrainingArguments, get_scheduler
 
 from swift.utils import get_logger
 
+try:
+    from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
+except ImportError:
+    from torch.optim.lr_scheduler import LRScheduler
+
 logger = get_logger()
 
 
 @dataclass
 class GaLoreConfig:
     """
     The configuration class for the Galore module.
```

### Comparing `ms-swift-1.7.3/swift/trainers/trainers.py` & `ms-swift-2.0.0/swift/trainers/trainers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 from peft import PeftModel
 from torch import Tensor, nn
 from torch.nn import CrossEntropyLoss
+from torch.utils.data import DataLoader
 from transformers import Seq2SeqTrainer as HfSeq2SeqTrainer
 from transformers import Trainer as HfTrainer
 from transformers import trainer
 from transformers.modeling_utils import unwrap_model
 from transformers.models.auto.modeling_auto import \
     MODEL_FOR_CAUSAL_LM_MAPPING_NAMES
 from transformers.utils import is_peft_available
 
-from swift.utils import lower_bound
+from swift.torchacc_utils import (ta_eval_dataloader, ta_test_dataloader,
+                                  ta_train_dataloader)
+from swift.utils import use_torchacc
 from .callback import (DefaultFlowCallbackNew, PrinterCallbackNew,
                        ProgressCallbackNew)
 from .mixin import PushToMsHubMixin, SwiftMixin
 
 try:
     from transformers.integrations.deepspeed import is_deepspeed_zero3_enabled
 except ImportError:
@@ -41,14 +44,15 @@
             'gen_len':
             0,
             'memory': {},
             'model':
             self.model.get_trainable_parameters() if hasattr(
                 self.model, 'get_trainable_parameters') else None,
         }
+        self._acc = torch.tensor(0.).to(self.args.device)
 
     def train(self, *args, **kwargs) -> torch.Tensor:
         res = super().train(*args, **kwargs)
         for i in range(torch.cuda.device_count()):
             self.perf['memory'][
                 f'cuda:{i}'] = f'{torch.cuda.max_memory_reserved(i)/1024/1024/1024:.2f}GiB'
         return res
@@ -249,21 +253,94 @@
             acc_list = []
             for i, m in enumerate(masks):
                 acc_list.append(
                     torch.all(preds[i, m] == labels[i,
                                                     m]).to(torch.int64).item())
             acc = torch.tensor(acc_list, device=preds.device).float().mean()
         else:
-            acc = (preds[masks] == labels[masks]).float().mean()
+            acc = (torch.masked_select(preds, masks) == torch.masked_select(
+                labels, masks)).float().mean()
         if model.training and acc is not None:
             if 'acc' not in self._custom_metrics:
-                self._custom_metrics['acc'] = torch.tensor(0.).to(
-                    self.args.device)
-            self._custom_metrics[
-                'acc'] += acc / self.args.gradient_accumulation_steps
+                self._custom_metrics['acc'] = self._acc
+            self._custom_metrics['acc'] = self._custom_metrics[
+                'acc'] + acc / self.args.gradient_accumulation_steps
         return (loss, outputs) if return_outputs else loss
 
+    def get_train_dataloader(self):
+        if not use_torchacc():
+            return super().get_train_dataloader()
+        else:
+            if trainer.is_datasets_available():
+                import datasets
+
+            if self.train_dataset is None:
+                raise ValueError('Trainer: training requires a train_dataset.')
+
+            train_dataset = self.train_dataset
+            data_collator = self.data_collator
+
+            if trainer.is_datasets_available() and isinstance(
+                    train_dataset, datasets.Dataset):
+                train_dataset = self._remove_unused_columns(
+                    train_dataset, description='training')
+            else:
+                data_collator = self._get_collator_with_removed_columns(
+                    data_collator, description='training')
+
+            return ta_train_dataloader(train_dataset, data_collator,
+                                       self._get_train_sampler(), self.args,
+                                       self._train_batch_size)
+
+    def get_eval_dataloader(self, eval_dataset):
+        if not use_torchacc():
+            return super().get_eval_dataloader(eval_dataset)
+        else:
+            import torchacc as ta
+            if trainer.is_datasets_available():
+                import datasets
+
+            if eval_dataset is None and self.eval_dataset is None:
+                raise ValueError(
+                    'Trainer: evaluation requires an eval_dataset.')
+            eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
+            data_collator = self.data_collator
+
+            if trainer.is_datasets_available() and isinstance(
+                    eval_dataset, datasets.Dataset):
+                eval_dataset = self._remove_unused_columns(
+                    eval_dataset, description='evaluation')
+            else:
+                data_collator = self._get_collator_with_removed_columns(
+                    data_collator, description='evaluation')
+
+            return ta_eval_dataloader(eval_dataset, data_collator,
+                                      self._get_eval_sampler(eval_dataset),
+                                      self.args)
+
+    def get_test_dataloader(self, test_dataset):
+        if not use_torchacc():
+            return super().get_test_dataloader(test_dataset)
+        else:
+            import torchacc as ta
+            if trainer.is_datasets_available():
+                import datasets
+
+            data_collator = self.data_collator
+
+            if trainer.is_datasets_available() and isinstance(
+                    test_dataset, datasets.Dataset):
+                test_dataset = self._remove_unused_columns(
+                    test_dataset, description='test')
+            else:
+                data_collator = self._get_collator_with_removed_columns(
+                    data_collator, description='test')
+
+            return ta_test_dataloader(test_dataset, data_collator,
+                                      self._get_eval_sampler(test_dataset),
+                                      self.args)
+
 
 # monkey patching
 trainer.DEFAULT_PROGRESS_CALLBACK = ProgressCallbackNew
 trainer.DEFAULT_CALLBACKS = [DefaultFlowCallbackNew]
 trainer.PrinterCallback = PrinterCallbackNew
```

### Comparing `ms-swift-1.7.3/swift/trainers/utils.py` & `ms-swift-2.0.0/swift/trainers/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 
 from torch.nn import Module
 from transformers.trainer_callback import TrainerCallback
 from transformers.trainer_utils import (EvaluationStrategy, FSDPOption,
                                         HPSearchBackend, HubStrategy,
                                         IntervalStrategy, SchedulerType)
 
+from swift.utils import get_logger
+
 try:
     # https://github.com/huggingface/transformers/pull/25702
     from transformers.trainer_utils import ShardedDDPOption
 except ImportError:
     ShardedDDPOption = None
 
+logger = get_logger()
+
 
 def can_return_loss(model: Module) -> bool:
     """Check if a given model can return loss."""
     signature = inspect.signature(model.forward)
     for p in signature.parameters:
         if p == 'return_loss' and signature.parameters[p].default is True:
             return True
```

### Comparing `ms-swift-1.7.3/swift/tuners/__init__.py` & `ms-swift-2.0.0/swift/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/adapter.py` & `ms-swift-2.0.0/swift/tuners/adapter.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/base.py` & `ms-swift-2.0.0/swift/tuners/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 param_names, param_group = output.optimizer_group_callback(
                     self.model, **defaults)
                 if param_names and all_param_names & param_names:
                     raise ValueError(
                         'Cannot set one parameter to different param groups')
                 if param_names and param_group:
                     all_param_names.update(param_names)
-                    param_groups.append(param_group)
+                    param_groups.extend(param_group)
 
         decay_parameters = Trainer.get_decay_parameter_names(None, self.model)
         param_groups.extend([
             {
                 'params': [
                     p for n, p in self.model.named_parameters()
                     if (n in decay_parameters and n not in all_param_names
@@ -445,16 +445,17 @@
         else:
             with open(os.path.join(output_dir, 'README.md'), 'r') as f:
                 lines = f.readlines()
 
         quantization_config = None
         if hasattr(self.base_model, 'config') and hasattr(
                 self.base_model.config, 'quantization_config'):
-            quantization_config = self.base_model.config.quantization_config.to_dict(
-            )
+            if hasattr(self.base_model.config.quantization_config, 'to_dict'):
+                quantization_config = self.base_model.config.quantization_config.to_dict(
+                )
         training_config_text = ''
         # Adds quantization information if it was used
         if quantization_config is not None:
             training_config_text += '\nThe following `bitsandbytes` quantization config was used during training:\n'
             training_config_text += '\n'.join([
                 f'- {name}: {value}'
                 for name, value in quantization_config.items()
@@ -786,19 +787,16 @@
                 Extra kwargs needed by SwiftModel or PeftModel.
         Returns:
             The model wrapped by SwiftModel or PeftModel.
         """
 
         if isinstance(config, (SwiftConfig, dict)):
             return SwiftModel(model, config, **kwargs)
-        elif isinstance(
-                config,
-                PeftConfig) or config.__class__.__name__ == 'PeftWrapper':
+        else:
             return get_peft_model(model, config, **kwargs)
-        raise ValueError(f'Unsupported swift config type: {config.__class__}')
 
     @staticmethod
     def merge_and_unload(model: Union[PeftModel, SwiftModel], **kwargs):
         """Merge tuners into the base model and unload them.
 
         Args:
             model(`Union[PeftModel, SwiftModel]`): The model instance with tuners
@@ -842,70 +840,80 @@
         """
         from .lora_layers import LoraLayer, LoRALayer
         for sub_module in model.modules():
             if isinstance(sub_module, (LoraLayer, LoRALayer)):
                 sub_module.unmerge(**kwargs)
 
     @staticmethod
-    def save_to_peft_format(ckpt_dir: str, output_dir: str):
+    def save_to_peft_format(ckpt_dir: str, output_dir: str) -> None:
         """Save swift format to peft format
 
         Args:
             ckpt_dir(`str`): Original swift output dir
             output_dir(`str`): Converted peft format dir
         """
+        assert ckpt_dir and output_dir, 'Please pass in valid ckpt_dir and output_dir.'
+        assert os.path.exists(
+            ckpt_dir), f'ckpt_dir: {ckpt_dir} must exists in local disk.'
         if os.path.exists(os.path.join(ckpt_dir, SwiftModel.EXTRA_STATE_DIR)):
             raise AssertionError(
                 'Cannot transfer to peft format, because you are additional state dicts.'
             )
 
         adapter_names = [
             sub_dir for sub_dir in os.listdir(ckpt_dir)
             if os.path.isfile(os.path.join(ckpt_dir, sub_dir, CONFIG_NAME))
         ]
 
         def has_custom_content(_json):
-            if _json.get('swift_type') != SwiftTuners.LORA:
+            if _json.get('swift_type',
+                         _json.get('peft_type')) != SwiftTuners.LORA:
+                logger.warn('Only LoRA can be converted to peft format')
                 return True
 
             from swift import LoRAConfig
             return not LoRAConfig(**_json).can_be_saved_to_peft()
 
         for adapter in adapter_names:
             with open(os.path.join(ckpt_dir, adapter, CONFIG_NAME)) as f:
                 _json = json.load(f)
                 if has_custom_content(_json):
                     raise AssertionError(
                         'Cannot transfer to peft format, '
                         'because you have special parameters or adapter types.'
                     )
 
+        os.makedirs(output_dir, exist_ok=True)
+        if ckpt_dir != output_dir:
+            shutil.copytree(ckpt_dir, output_dir, dirs_exist_ok=True)
+
         for adapter in adapter_names:
             safe_serialization = os.path.isfile(
-                os.path.join(ckpt_dir, adapter, SAFETENSORS_WEIGHTS_NAME))
+                os.path.join(output_dir, adapter, SAFETENSORS_WEIGHTS_NAME))
             state_dict = SwiftModel.load_state_file(
-                os.path.join(ckpt_dir, adapter))
-            os.makedirs(os.path.join(output_dir, adapter), exist_ok=True)
+                os.path.join(output_dir, adapter))
             new_state_dict = {}
             for key, value in state_dict.items():
                 if not key.startswith('base_model.model.'):
                     key = 'base_model.model.' + key
                 key = key.replace(f'lora_A.{adapter}.', 'lora_A.')
                 key = key.replace(f'lora_B.{adapter}.', 'lora_B.')
                 key = key.replace(f'lora_embedding_A.{adapter}.',
                                   'lora_embedding_A.')
                 key = key.replace(f'lora_embedding_B.{adapter}.',
                                   'lora_embedding_B.')
+                key = key.replace(f'lora_magnitude_vector.{adapter}',
+                                  'lora_magnitude_vector')
                 new_state_dict[key] = value
             state_dict = new_state_dict
             SwiftModel._save_state_dict(state_dict,
                                         os.path.join(output_dir, adapter),
                                         safe_serialization)
             from swift import LoRAConfig
-            with open(os.path.join(ckpt_dir, adapter, CONFIG_NAME)) as f:
+            with open(os.path.join(output_dir, adapter, CONFIG_NAME)) as f:
                 _json = json.load(f)
                 peft_config = LoRAConfig(**_json).to_peft_config()
             peft_config.save_pretrained(os.path.join(output_dir, adapter))
 
         if 'default' in adapter_names:
             shutil.move(
                 os.path.join(output_dir, 'default', CONFIG_NAME),
```

### Comparing `ms-swift-1.7.3/swift/tuners/llamapro.py` & `ms-swift-2.0.0/swift/tuners/llamapro.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/longlora/llama.py` & `ms-swift-2.0.0/swift/tuners/longlora/llama.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,169 +1,134 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 # Part of the implementation is borrowed from dvlab-research/LongLoRA.
 
 import math
-import warnings
 from types import MethodType
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
-import transformers
-from einops import rearrange
 from torch import nn
+from transformers import Cache
 from transformers.models.llama.modeling_llama import (apply_rotary_pos_emb,
-                                                      repeat_kv, rotate_half)
+                                                      repeat_kv)
 
 from swift.utils import get_logger
 
 logger = get_logger()
 
 
-def forward_flashattn(
-    self,
-    hidden_states: torch.Tensor,
-    attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.Tensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
-    output_attentions: bool = False,
-    use_cache: bool = False,
-    padding_mask: Optional[torch.LongTensor] = None,
-) -> Tuple[torch.Tensor, Optional[torch.Tensor],
-           Optional[Tuple[torch.Tensor]]]:
-    """Input shape: Batch x Time x Channel
+def _preprocess_qkv_fa2(attn_module, query_states, key_states, value_states,
+                        attention_mask):
+    if attn_module.training:
+        bsz, q_len = query_states.shape[:2]
+        group_size = int(q_len * attn_module.config.group_size_ratio)
+        if q_len % group_size != 0:
+            raise ValueError(
+                f'The sequence length {q_len} should'
+                f'be able to be splitted by the group_ratio {attn_module.config.group_size_ratio}'
+            )
 
-    attention_mask: [bsz, q_len]
-    """
-    from flash_attn.flash_attn_interface import (
-        flash_attn_varlen_qkvpacked_func)
-    from flash_attn.bert_padding import unpad_input, pad_input
-    if not self.training:
-        raise ValueError(
-            'This function is only for training. For inference, please use forward_flashattn_inference.'
-        )
+        num_group = q_len // group_size
 
-    if output_attentions:
-        warnings.warn(
-            'Output attentions is not supported for patched `LlamaAttention`, returning `None` instead.'
-        )
+        def shift(qkv, bsz, q_len, group_size, num_heads, head_dim):
+            qkv[:, :, num_heads // 2:] = qkv[:, :, num_heads // 2:].roll(
+                -group_size // 2, dims=1)
+            qkv = qkv.reshape(bsz * num_group, group_size, num_heads, head_dim)
+            return qkv
 
-    bsz, q_len, _ = hidden_states.size()
+        query_states = shift(query_states, bsz, q_len, group_size,
+                             attn_module.num_heads, attn_module.head_dim)
+        key_states = shift(key_states, bsz, q_len, group_size,
+                           attn_module.num_heads, attn_module.head_dim)
+        value_states = shift(value_states, bsz, q_len, group_size,
+                             attn_module.num_heads, attn_module.head_dim)
+        if attention_mask is not None:
+            attention_mask = attention_mask[:, :group_size].repeat(
+                num_group, 1)
 
-    query_states = (
-        self.q_proj(hidden_states).view(bsz, q_len, self.num_heads,
-                                        self.head_dim).transpose(1, 2))
-    key_states = (
-        self.k_proj(hidden_states).view(bsz, q_len, self.num_key_value_heads,
-                                        self.head_dim).transpose(1, 2))
-    value_states = (
-        self.v_proj(hidden_states).view(bsz, q_len, self.num_key_value_heads,
-                                        self.head_dim).transpose(1, 2))
-    # [bsz, q_len, nh, hd]
-    # [bsz, nh, q_len, hd]
+    return query_states, key_states, value_states, attention_mask
 
-    kv_seq_len = key_states.shape[-2]
-    if past_key_value is not None:
-        kv_seq_len += past_key_value[0].shape[-2]
-    cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-    query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
-                                                    cos, sin, position_ids)
 
-    # Past Key value support
-    if past_key_value is not None:
-        # reuse k, v, self_attention
-        key_states = torch.cat([past_key_value[0], key_states], dim=2)
-        value_states = torch.cat([past_key_value[1], value_states], dim=2)
+def _preprocess_qkv(attn_module, query_states, key_states, value_states,
+                    attention_mask):
+    if attn_module.training:
+        bsz, _, q_len = query_states.shape[:3]
+        group_size = int(q_len * attn_module.config.group_size_ratio)
+        if q_len % group_size != 0:
+            raise ValueError(
+                f'The sequence length {q_len} should'
+                f'be able to be splitted by the group_ratio {attn_module.config.group_size_ratio}'
+            )
 
-    past_key_value = (key_states, value_states) if use_cache else None
+        num_group = q_len // group_size
 
-    # repeat k/v heads if n_kv_heads < n_heads
-    key_states = repeat_kv(key_states, self.num_key_value_groups)
-    value_states = repeat_kv(value_states, self.num_key_value_groups)
+        def shift(qkv, bsz, q_len, group_size, num_heads, head_dim):
+            qkv[:, num_heads // 2:] = qkv[:, num_heads // 2:].roll(
+                -group_size // 2, dims=2)
+            qkv = qkv.transpose(1, 2)
+            qkv = qkv.reshape(bsz * num_group, group_size, num_heads, head_dim)
+            return qkv.transpose(1, 2)
 
-    # Flash attention codes from
-    # https://github.com/HazyResearch/flash-attention/blob/main/flash_attn/flash_attention.py
+        query_states = shift(query_states, bsz, q_len, group_size,
+                             attn_module.num_heads, attn_module.head_dim)
+        key_states = shift(key_states, bsz, q_len, group_size,
+                           attn_module.num_heads, attn_module.head_dim)
+        value_states = shift(value_states, bsz, q_len, group_size,
+                             attn_module.num_heads, attn_module.head_dim)
+        if attention_mask is not None:
+            attention_mask = attention_mask[:, :, :group_size, :
+                                            group_size].repeat(
+                                                num_group, 1, 1, 1)
 
-    # transform the data into the format required by flash attention
-    qkv = torch.stack([query_states, key_states, value_states],
-                      dim=2)  # [bsz, nh, 3, q_len, hd]
-    qkv = qkv.transpose(1, 3)  # [bsz, q_len, 3, nh, hd]
-
-    # We have disabled _prepare_decoder_attention_mask in LlamaModel
-    # the attention_mask should be the same as the key_padding_mask
-
-    key_padding_mask = attention_mask.repeat(2, 1)
-    nheads = qkv.shape[-2]
-    # shift
-
-    group_size = int(q_len * self.config.group_size_ratio)
-
-    qkv = qkv.reshape(bsz, q_len, 3, 2, self.num_heads // 2,
-                      self.head_dim).permute(0, 3, 1, 2, 4, 5).reshape(
-                          bsz * 2, q_len, 3, self.num_heads // 2,
-                          self.head_dim)
-
-    x = rearrange(qkv, 'b s three h d -> b s (three h d)')
-    x_unpad, indices, cu_q_lens, max_s = unpad_input(x, key_padding_mask)
-    cu_q_len_tmp = torch.arange(
-        0,
-        max_s,
-        group_size,
-        device=key_padding_mask.device,
-        dtype=cu_q_lens.dtype)
-    cu_q_len_tmp2 = cu_q_len_tmp + group_size // 2
-    cu_q_len_tmp2[cu_q_len_tmp2 >= max_s] = torch.iinfo(
-        cu_q_len_tmp2.dtype).min
-    cu_q_len_tmp = torch.stack([cu_q_len_tmp, cu_q_len_tmp2]).repeat(
-        bsz, 1) + cu_q_lens[:-1].unsqueeze(-1)
-    cu_q_lens = torch.cat([cu_q_len_tmp, cu_q_lens[1:].unsqueeze(-1)],
-                          dim=-1).view(-1)
-    cu_q_lens = cu_q_lens[cu_q_lens >= 0]
-    x_unpad = rearrange(
-        x_unpad, 'nnz (three h d) -> nnz three h d', three=3, h=nheads // 2)
-    output_unpad = flash_attn_varlen_qkvpacked_func(
-        x_unpad, cu_q_lens, group_size, 0.0, softmax_scale=None, causal=True)
-    output = rearrange(
-        pad_input(
-            rearrange(output_unpad, 'nnz h d -> nnz (h d)'), indices, bsz * 2,
-            q_len),
-        'b s (h d) -> b s h d',
-        h=nheads // 2,
-    )
-    output = output.reshape(bsz, 2, q_len, nheads // 2,
-                            self.head_dim).transpose(1, 2).reshape(
-                                bsz, q_len, nheads, self.head_dim)
+    return query_states, key_states, value_states, attention_mask
+
+
+def _postprocess_qkv(attn_module, attn_output, q_len):
+    if attn_module.training:
+        group_size = int(q_len * attn_module.config.group_size_ratio)
+        attn_output = attn_output.transpose(1, 2)
+        attn_output = attn_output.reshape(-1, q_len, attn_module.num_heads,
+                                          attn_module.head_dim)
+        # shift back
+        attn_output[:, :, attn_module.num_heads
+                    // 2:] = attn_output[:, :,
+                                         attn_module.num_heads // 2:].roll(
+                                             group_size // 2, dims=1)
+    return attn_output.transpose(1, 2)
 
-    return self.o_proj(rearrange(output,
-                                 'b s h d -> b s (h d)')), None, past_key_value
+
+def _postprocess_qkv_fa2(attn_module, attn_output, q_len):
+    if attn_module.training:
+        group_size = int(q_len * attn_module.config.group_size_ratio)
+        attn_output = attn_output.reshape(-1, q_len, attn_module.num_heads,
+                                          attn_module.head_dim)
+        # shift back
+        attn_output[:, :, attn_module.num_heads
+                    // 2:] = attn_output[:, :,
+                                         attn_module.num_heads // 2:].roll(
+                                             group_size // 2, dims=1)
+    return attn_output
 
 
-def forward_noflashattn(
+# code borrowed from https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py#L316 # noqa
+def eager_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
+    past_key_value: Optional[Cache] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
-    padding_mask: Optional[torch.LongTensor] = None,
+    cache_position: Optional[torch.LongTensor] = None,
+    **kwargs,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor],
            Optional[Tuple[torch.Tensor]]]:
     bsz, q_len, _ = hidden_states.size()
 
-    group_size = int(q_len * self.config.group_size_ratio)
-
-    if q_len % group_size != 0:
-        raise ValueError(
-            f'The sequence length {q_len} should'
-            f'be able to be splitted by the group_ratio {self.config.group_size_ratio}'
-        )
-
-    num_group = q_len // group_size
-
     if self.config.pretraining_tp > 1:
         key_value_slicing = (self.num_key_value_heads
                              * self.head_dim) // self.config.pretraining_tp
         query_slices = self.q_proj.weight.split(
             (self.num_heads * self.head_dim) // self.config.pretraining_tp,
             dim=0)
         key_slices = self.k_proj.weight.split(key_value_slicing, dim=0)
@@ -195,72 +160,58 @@
     query_states = query_states.view(bsz, q_len, self.num_heads,
                                      self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads,
                                  self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads,
                                      self.head_dim).transpose(1, 2)
 
-    kv_seq_len = key_states.shape[-2]
-    if past_key_value is not None:
-        kv_seq_len += past_key_value[0].shape[-2]
-    cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
+    past_key_value = getattr(self, 'past_key_value', past_key_value)
+    cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
-                                                    cos, sin, position_ids)
+                                                    cos, sin)
 
     if past_key_value is not None:
-        # reuse k, v, self_attention
-        key_states = torch.cat([past_key_value[0], key_states], dim=2)
-        value_states = torch.cat([past_key_value[1], value_states], dim=2)
+        # sin and cos are specific to RoPE models; position_ids needed for the static cache
+        cache_kwargs = {
+            'sin': sin,
+            'cos': cos,
+            'cache_position': cache_position
+        }
+        key_states, value_states = past_key_value.update(
+            key_states, value_states, self.layer_idx, cache_kwargs)
 
-    past_key_value = (key_states, value_states) if use_cache else None
-
-    # repeat k/v heads if n_kv_heads < n_heads
     key_states = repeat_kv(key_states, self.num_key_value_groups)
     value_states = repeat_kv(value_states, self.num_key_value_groups)
 
-    if self.training:
-        # shift
-        def shift(qkv, bsz, q_len, group_size, num_heads, head_dim):
-            qkv[:, num_heads // 2:] = qkv[:, num_heads // 2:].roll(
-                -group_size // 2, dims=2)
-            qkv = qkv.transpose(1, 2).reshape(bsz * (q_len // group_size),
-                                              group_size, num_heads,
-                                              head_dim).transpose(1, 2)
-            return qkv
-
-        query_states = shift(query_states, bsz, q_len, group_size,
-                             self.num_heads, self.head_dim)
-        key_states = shift(key_states, bsz, q_len, group_size, self.num_heads,
-                           self.head_dim)
-        value_states = shift(value_states, bsz, q_len, group_size,
-                             self.num_heads, self.head_dim)
-        if attention_mask is not None:
-            attention_mask = attention_mask[:, :, :group_size, :
-                                            group_size].repeat(
-                                                num_group, 1, 1, 1)
+    # patch position rolling
+    query_states, key_states, value_states, attention_mask = _preprocess_qkv(
+        self, query_states, key_states, value_states, attention_mask)
 
     attn_weights = torch.matmul(query_states, key_states.transpose(
         2, 3)) / math.sqrt(self.head_dim)
 
-    if attention_mask is not None:
-        attn_weights = attn_weights + attention_mask
+    if attention_mask is not None:  # no matter the length, we just slice it
+        if cache_position is not None and not self.training:
+            causal_mask = attention_mask[:, :,
+                                         cache_position, :key_states.shape[-2]]
+            attn_weights = attn_weights + causal_mask
+        else:
+            attn_weights = attn_weights + attention_mask
 
     # upcast attention to fp32
     attn_weights = nn.functional.softmax(
         attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
+    attn_weights = nn.functional.dropout(
+        attn_weights, p=self.attention_dropout, training=self.training)
     attn_output = torch.matmul(attn_weights, value_states)
-    attn_output = attn_output.transpose(1, 2).contiguous()
-    attn_output = attn_output.reshape(bsz, q_len, self.num_heads,
-                                      self.head_dim)
 
-    if self.training:
-        # shift back
-        attn_output[:, :, self.num_heads
-                    // 2:] = attn_output[:, :, self.num_heads // 2:].roll(
-                        group_size // 2, dims=1)
+    # patch position unrolling
+    attn_output = _postprocess_qkv(self, attn_output, q_len)
+
+    attn_output = attn_output.transpose(1, 2).contiguous()
 
     attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
 
     if self.config.pretraining_tp > 1:
         attn_output = attn_output.split(
             self.hidden_size // self.config.pretraining_tp, dim=2)
         o_proj_slices = self.o_proj.weight.split(
@@ -274,161 +225,222 @@
 
     if not output_attentions:
         attn_weights = None
 
     return attn_output, attn_weights, past_key_value
 
 
-def forward_flashattn_inference(
+# code borrowed from https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py#L417 # noqa
+def fa2_forward(
     self,
     hidden_states: torch.Tensor,
-    attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.Tensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
+    attention_mask: Optional[torch.LongTensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_value: Optional[Cache] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
-    padding_mask: Optional[torch.Tensor] = None,
+    cache_position: Optional[torch.LongTensor] = None,
+    **kwargs,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor],
            Optional[Tuple[torch.Tensor]]]:
-    from flash_attn import __version__ as flash_attn_version
-    from flash_attn.flash_attn_interface import (
-        flash_attn_func, flash_attn_varlen_kvpacked_func)
-    from flash_attn.bert_padding import unpad_input, pad_input
-    if output_attentions:
-        warnings.warn(
-            'Output attentions is not supported for patched `LlamaAttention`, returning `None` instead.'
-        )
+    output_attentions = False
 
     bsz, q_len, _ = hidden_states.size()
-    kv_heads = getattr(self, 'num_key_value_heads', self.num_heads)
 
-    # shape: (b, s, num_heads, head_dim)
-    q, k, v = (op(hidden_states).view(bsz, q_len, nh, self.head_dim)
-               for op, nh in (
-                   (self.q_proj, self.num_heads),
-                   (self.k_proj, kv_heads),
-                   (self.v_proj, kv_heads),
-               ))  # noqa
-
-    kv_seq_len = k.shape[1]
-    if past_key_value is not None and len(past_key_value):
-        past_kv_len = past_key_value.seen_tokens
-        kv_seq_len += past_kv_len
-
-    cos_sin = self.rotary_emb(v, seq_len=kv_seq_len)
-    q, k = apply_rotary_pos_emb(
-        q.transpose(1, 2), k.transpose(1, 2), *cos_sin, position_ids)
-    q = q.transpose(1, 2)
-    k = k.transpose(1, 2)
-
-    if use_cache:
-        k, v = past_key_value.update(
-            k.transpose(1, 2), v.transpose(1, 2), layer_idx=self.idx)
-        k = k.transpose(1, 2)
-        v = v.transpose(1, 2)
-    else:
-        past_key_value = None
+    query_states = self.q_proj(hidden_states)
+    key_states = self.k_proj(hidden_states)
+    value_states = self.v_proj(hidden_states)
+
+    # Flash attention requires the input to have the shape
+    # batch_size x seq_length x head_dim x hidden_dim
+    # therefore we just need to keep the original shape
+    query_states = query_states.view(bsz, q_len, self.num_heads,
+                                     self.head_dim).transpose(1, 2)
+    key_states = key_states.view(bsz, q_len, self.num_key_value_heads,
+                                 self.head_dim).transpose(1, 2)
+    value_states = value_states.view(bsz, q_len, self.num_key_value_heads,
+                                     self.head_dim).transpose(1, 2)
 
-    if attention_mask is None:
-        output = flash_attn_func(
-            q, k, v, 0.0, softmax_scale=None,
-            causal=True).view(bsz, q_len, -1)
-    else:
-        q, indices, cu_q_lens, max_s = unpad_input(q, attention_mask[:,
-                                                                     -q_len:])
-        # We can skip concat and call unpad twice but seems better to call unpad only once.
-        kv, _, cu_k_lens, max_k = unpad_input(
-            torch.stack((k, v), dim=2), attention_mask)
-        output_unpad = flash_attn_varlen_kvpacked_func(
-            q,
-            kv,
-            cu_q_lens,
-            cu_k_lens,
-            max_s,
-            max_k,
-            0.0,
-            softmax_scale=None,
-            causal=True,
-        )
-        output_unpad = output_unpad.reshape(-1, self.num_heads * self.head_dim)
-        output = pad_input(output_unpad, indices, bsz, q_len)
+    cos, sin = self.rotary_emb(value_states, position_ids)
+    query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
+                                                    cos, sin)
 
-    return self.o_proj(output), None, past_key_value
+    past_key_value = getattr(self, 'past_key_value', past_key_value)
 
+    if past_key_value is not None:
+        # sin and cos are specific to RoPE models; position_ids needed for the static cache
+        cache_kwargs = {
+            'sin': sin,
+            'cos': cos,
+            'cache_position': cache_position
+        }
+        key_states, value_states = past_key_value.update(
+            key_states, value_states, self.layer_idx, cache_kwargs)
+
+    # TODO: These transpose are quite inefficient but Flash Attention
+    #  requires the layout [batch_size, sequence_length, num_heads, head_dim]. We would need to refactor the KV cache
+    # to be able to avoid many of these transpose/reshape/view.
+    query_states = query_states.transpose(1, 2)
+    key_states = key_states.transpose(1, 2)
+    value_states = value_states.transpose(1, 2)
+
+    dropout_rate = self.attention_dropout if self.training else 0.0
+
+    # In PEFT, usually we cast the layer norms in float32 for training stability reasons
+    # therefore the input hidden states gets silently casted in float32. Hence, we need
+    # cast them back in the correct dtype just to be sure everything works as expected.
+    # This might slowdown training & inference so it is recommended to not cast the LayerNorms
+    # in fp32. (LlamaRMSNorm handles it correctly)
+
+    input_dtype = query_states.dtype
+    if input_dtype == torch.float32:
+        if torch.is_autocast_enabled():
+            target_dtype = torch.get_autocast_gpu_dtype()
+        # Handle the case where the model is quantized
+        elif hasattr(self.config, '_pre_quantization_dtype'):
+            target_dtype = self.config._pre_quantization_dtype
+        else:
+            target_dtype = self.q_proj.weight.dtype
 
-# Disable the transformation of the attention mask in LlamaModel as the flash attention
-# requires the attention mask to be the same as the key_padding_mask
-def _prepare_decoder_attention_mask(self, attention_mask, input_shape,
-                                    inputs_embeds, past_key_values_length):
-    if self.training:
-        return attention_mask
-    else:
-        # [bsz, seq_len]
-        if past_key_values_length > 0 and attention_mask is not None:
-            attention_mask = torch.cat(
-                (
-                    torch.full(
-                        (input_shape[0], past_key_values_length),
-                        True,
-                        dtype=attention_mask.dtype,
-                        device=attention_mask.device,
-                    ),
-                    attention_mask,
-                ),
-                dim=-1,
-            )
+        logger.warning_once(
+            f'The input hidden states seems to be silently casted in float32, this might be related to'
+            f' the fact you have upcasted embedding or layer norm layers in float32. We will cast back the input in'
+            f' {target_dtype}.')
+
+        query_states = query_states.to(target_dtype)
+        key_states = key_states.to(target_dtype)
+        value_states = value_states.to(target_dtype)
+
+    # patch position rolling
+    query_states, key_states, value_states, attention_mask = _preprocess_qkv_fa2(
+        self, query_states, key_states, value_states, attention_mask)
+
+    attn_output = self._flash_attention_forward(
+        query_states,
+        key_states,
+        value_states,
+        attention_mask,
+        query_states.shape[1],
+        dropout=dropout_rate)
+
+    # patch position unrolling
+    attn_output = _postprocess_qkv_fa2(self, attn_output, q_len)
+
+    attn_output = attn_output.reshape(bsz, q_len,
+                                      self.hidden_size).contiguous()
+    attn_output = self.o_proj(attn_output)
 
-        if attention_mask is not None and torch.all(attention_mask):
-            return None  # This uses the faster call when training with full samples
+    if not output_attentions:
+        attn_weights = None
 
-        return attention_mask
+    return attn_output, attn_weights, past_key_value
 
 
-def forward_flashattn_inference_s2_attn(
+# code borrowed from https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py#L605  # noqa
+def sdpa_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.Tensor] = None,
-    past_key_value: Optional[Tuple[torch.Tensor]] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_value: Optional[Cache] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
-    padding_mask: Optional[torch.Tensor] = None,
+    cache_position: Optional[torch.LongTensor] = None,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor],
            Optional[Tuple[torch.Tensor]]]:
-    if self.training:
-        return forward_flashattn(self, hidden_states, attention_mask,
-                                 position_ids, past_key_value,
-                                 output_attentions, use_cache, padding_mask)
-    else:
-        return forward_flashattn_inference(self, hidden_states, attention_mask,
-                                           position_ids, past_key_value,
-                                           output_attentions, use_cache,
-                                           padding_mask)
+    if output_attentions:
+        # TODO: Improve this warning with e.g. `model.config.attn_implementation = "manual"` once this is implemented.
+        logger.warning_once(
+            'LlamaModel is using LlamaSdpaAttention, but `torch.nn.functional.scaled_dot_product_attention` does not support `output_attentions=True`. Falling back to the manual attention implementation, '  # noqa
+            'but specifying the manual implementation will be required from Transformers version v5.0.0 onwards. This warning can be removed using the argument `attn_implementation="eager"` when loading the model.'  # noqa
+        )
+        return super().forward(
+            hidden_states=hidden_states,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
+            past_key_value=past_key_value,
+            output_attentions=output_attentions,
+            use_cache=use_cache,
+            cache_position=cache_position,
+        )
 
+    bsz, q_len, _ = hidden_states.size()
 
-def patch_llama_forward(model: nn.Module, forward_function) -> None:
-    # Compatible with transformers device_map
-    for idx, m in enumerate(model.model.layers):
-        new_forward = MethodType(forward_function, m.self_attn)
-        if hasattr(model, '_old_forward'):
-            m.self_attn._old_forward = new_forward
-        else:
-            m.self_attn.forward = new_forward
-        m.self_attn.idx = idx
+    query_states = self.q_proj(hidden_states)
+    key_states = self.k_proj(hidden_states)
+    value_states = self.v_proj(hidden_states)
+
+    query_states = query_states.view(bsz, q_len, self.num_heads,
+                                     self.head_dim).transpose(1, 2)
+    key_states = key_states.view(bsz, q_len, self.num_key_value_heads,
+                                 self.head_dim).transpose(1, 2)
+    value_states = value_states.view(bsz, q_len, self.num_key_value_heads,
+                                     self.head_dim).transpose(1, 2)
 
+    cos, sin = self.rotary_emb(value_states, position_ids)
+    query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
+                                                    cos, sin)
 
-def replace_llama_attn(model: nn.Module, use_flash_attn=True):
-    if use_flash_attn:
-        cuda_major, cuda_minor = torch.cuda.get_device_capability()
-        if cuda_major < 8:
-            warnings.warn(
-                'Flash attention is only supported on A100 or H100 GPU during training due to head dim > 64 backward.'
-                'ref: https://github.com/HazyResearch/flash-attention/issues/190#issuecomment-1523359593'
-            )
-        transformers.models.llama.modeling_llama.LlamaModel._prepare_decoder_attention_mask = (
-            _prepare_decoder_attention_mask)
-        patch_llama_forward(model, forward_flashattn_inference_s2_attn)
-    else:
-        logger.warn(
-            'The source code of LongLoRA without flash '
-            'attention may has some problems, please use with careful.')
-        patch_llama_forward(model, forward_noflashattn)
+    # In case static cache is used, it is an instance attribute.
+    past_key_value = getattr(self, 'past_key_value', past_key_value)
+
+    if past_key_value is not None:
+        # sin and cos are specific to RoPE models; position_ids needed for the static cache
+        cache_kwargs = {
+            'sin': sin,
+            'cos': cos,
+            'cache_position': cache_position
+        }
+        key_states, value_states = past_key_value.update(
+            key_states, value_states, self.layer_idx, cache_kwargs)
+
+    key_states = repeat_kv(key_states, self.num_key_value_groups)
+    value_states = repeat_kv(value_states, self.num_key_value_groups)
+
+    causal_mask = attention_mask
+    if attention_mask is not None and cache_position is not None:
+        causal_mask = causal_mask[:, :, cache_position, :key_states.shape[-2]]
+
+    # SDPA with memory-efficient backend is currently (torch==2.1.2) bugged with non-contiguous inputs with custom attn_mask,  # noqa
+    # Reference: https://github.com/pytorch/pytorch/issues/112577.  # noqa
+    if query_states.device.type == 'cuda' and causal_mask is not None:
+        query_states = query_states.contiguous()
+        key_states = key_states.contiguous()
+        value_states = value_states.contiguous()
+
+    # patch position rolling
+    query_states, key_states, value_states, causal_mask = _preprocess_qkv(
+        self, query_states, key_states, value_states, causal_mask)
+
+    attn_output = torch.nn.functional.scaled_dot_product_attention(
+        query_states,
+        key_states,
+        value_states,
+        attn_mask=causal_mask,
+        dropout_p=self.attention_dropout if self.training else 0.0,
+    )
+
+    # patch position unrolling
+    attn_output = _postprocess_qkv(self, attn_output, q_len)
+
+    attn_output = attn_output.transpose(1, 2).contiguous()
+    attn_output = attn_output.view(bsz, q_len, self.hidden_size)
+
+    attn_output = self.o_proj(attn_output)
+
+    return attn_output, None, past_key_value
+
+
+def replace_llama_attn(model: nn.Module):
+    for idx, m in enumerate(model.model.layers):
+        if model.config._attn_implementation == 'flash_attention_2':
+            cuda_major, cuda_minor = torch.cuda.get_device_capability()
+            if cuda_major < 8:
+                logger.warn(
+                    'Flash attention is only supported on A100 or H100 GPU during training due to head dim > 64 backward.'  # noqa
+                    'ref: https://github.com/HazyResearch/flash-attention/issues/190#issuecomment-1523359593'
+                )
+            m.self_attn.forward = MethodType(fa2_forward, m.self_attn)
+        elif model.config._attn_implementation == 'eager':
+            m.self_attn.forward = MethodType(eager_forward, m.self_attn)
+        elif model.config._attn_implementation == 'sdpa':
+            m.self_attn.forward = MethodType(sdpa_forward, m.self_attn)
```

### Comparing `ms-swift-1.7.3/swift/tuners/longlora/longlora.py` & `ms-swift-2.0.0/swift/tuners/longlora/longlora.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     The Config for the LongLoRA adapter.
     LongLoRA:[Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
     This adapter uses S2-attention to shorten the attention window for long context training scenarios.
     Args:
         embedder_and_normalizer: LongLoRA allows the embedder and normalizer to be trainable, this parameter specifies
             the names of the embedders and normalizers.
         model_type: The model type, now support llama only
-        use_flash_attn: Use flash attention version of forward
         group_size_ratio: The group size window ratio of the sequence length.
             Note: The sequence length should be split to smaller sequences by the ratio.
     """
 
     embedder_and_normalizer: Union[str, List[str], Tuple[str]] = field(
         default=('embed', 'norm'),
         metadata={
@@ -39,17 +38,14 @@
 
     model_type: str = field(
         default=None,
         metadata={
             'help': 'The model type, now only support `llama` structure.'
         })
 
-    use_flash_attn: bool = field(
-        default=False, metadata={'help': 'Use flash attention or not.'})
-
     group_size_ratio: float = field(
         default=0.25, metadata={'help': 'The S2 attention group ratio'})
 
     def __post_init__(self):
         from swift.tuners.mapping import SwiftTuners
         self.swift_type = SwiftTuners.LONGLORA
 
@@ -80,15 +76,15 @@
         def mark_trainable_callback(model):
             mark_lora_as_trainable(model, adapter_name, config.bias)
             mark_embedding_normalizer_as_trainable(
                 model, config.embedder_and_normalizer)
 
         if config.model_type == LongLoRAModelType.LLAMA:
             from .llama import replace_llama_attn
-            replace_llama_attn(model, use_flash_attn=config.use_flash_attn)
+            replace_llama_attn(model)
             # only support code base from transformers
             model.config.group_size_ratio = config.group_size_ratio
 
         return SwiftOutput(config, state_dict_callback,
                            mark_trainable_callback)
```

### Comparing `ms-swift-1.7.3/swift/tuners/lora_layers.py` & `ms-swift-2.0.0/swift/tuners/lora_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,32 +302,60 @@
 if is_auto_gptq_available():
     from peft.tuners.lora import QuantLinear as _QuantLinear
 
     class QuantLinear(LoRAActivationMixin, _QuantLinear):
 
         def __init__(
             self,
-            *args,
+            base_layer,
+            adapter_name: str,
+            module_key: str,
+            r: int = 0,
+            lora_alpha: int = 1,
+            lora_dropout: float = 0.0,
+            init_lora_weights: bool = True,
+            use_rslora: bool = False,
+            use_dora: bool = False,
             use_qa_lora=False,
             group_size=None,
-            module_key: str,
             **kwargs,
         ):
             super(QuantLinear, self).__init__(module_key)
-            self.set_activation(args[1], True)
-            super(ActivationMixin, self).__init__(*args, **kwargs)
+            self.set_activation(adapter_name, True)
+            nn.Module.__init__(self)
             self.group_size = group_size
             self.use_qa_lora = use_qa_lora
             if self.use_qa_lora:
                 assert self.group_size is not None, 'To use qa_lora you need to pass in the `group_size` param.'
-            if self.use_qa_lora:
                 self.qa_pool = torch.nn.AvgPool1d(
                     self.group_size
                 )  # using pooling layer to conduct sum operation
 
+            LoraLayer.__init__(self, base_layer)
+            if use_dora:
+                raise ValueError(
+                    f'{_QuantLinear.__name__} does not support DoRA yet, please set it to False'
+                )
+            if self.use_qa_lora:
+                self.in_features = self.in_features // self.group_size
+            # self.base_layer and self.quant_linear_module are the same;
+            # we need the former for consistency and the latter
+            # for backwards compatibility
+            self.quant_linear_module = base_layer
+            self._active_adapter = adapter_name
+            self.update_layer(
+                adapter_name,
+                r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                init_lora_weights=init_lora_weights,
+                use_rslora=use_rslora,
+                use_dora=use_dora,
+            )
+
         def forward(self, x: torch.Tensor):
             # note: logic differs from default Linear because merging is not supported
             result = self.quant_linear_module(x)
 
             if self.disable_adapters:
                 return result
 
@@ -501,14 +529,80 @@
 class Linear(LoRAActivationMixin, _Linear):
 
     def __init__(self, *args, module_key: str, **kwargs):
         super(Linear, self).__init__(module_key)
         self.set_activation(args[1], True)
         super(ActivationMixin, self).__init__(*args, **kwargs)
 
+        def device_hook(module, args):
+            for active_adapter in self.active_adapters:
+                self.lora_A[active_adapter].to(args[0].device)
+                self.lora_B[active_adapter].to(args[0].device)
+
+        self.register_forward_pre_hook(device_hook)
+
+    def update_layer(self,
+                     adapter_name,
+                     r,
+                     lora_alpha,
+                     lora_dropout,
+                     init_lora_weights,
+                     use_rslora,
+                     use_dora: bool = False):
+        # This code works for linear layers, override for other layer types
+        if r <= 0:
+            raise ValueError(
+                f'`r` should be a positive integer value but the value passed is {r}'
+            )
+
+        self.r[adapter_name] = r
+        self.lora_alpha[adapter_name] = lora_alpha
+        if lora_dropout > 0.0:
+            lora_dropout_layer = nn.Dropout(p=lora_dropout)
+        else:
+            lora_dropout_layer = nn.Identity()
+
+        self.lora_dropout.update(
+            nn.ModuleDict({adapter_name: lora_dropout_layer}))
+        # Actual trainable parameters
+        self.lora_A[adapter_name] = nn.Linear(self.in_features, r, bias=False)
+        self.lora_B[adapter_name] = nn.Linear(r, self.out_features, bias=False)
+        if use_rslora:
+            self.scaling[adapter_name] = lora_alpha / math.sqrt(r)
+        else:
+            self.scaling[adapter_name] = lora_alpha / r
+
+        if init_lora_weights == 'loftq':
+            self.loftq_init(adapter_name)
+        elif init_lora_weights:
+            self.reset_lora_parameters(adapter_name, init_lora_weights)
+
+        # check weight and qweight (for GPTQ)
+        for weight_name in ('weight', 'qweight'):
+            weight = getattr(self.get_base_layer(), weight_name, None)
+            if weight is not None:
+                if weight.device != torch.device('meta'):
+                    # the layer is already completely initialized, this is an update
+                    if weight.dtype.is_floating_point or weight.dtype.is_complex:
+                        self.to(weight.device, dtype=weight.dtype)
+                    else:
+                        self.to(weight.device)
+                    break
+                elif weight.dtype.is_floating_point or weight.dtype.is_complex:
+                    self.to(dtype=weight.dtype)
+                    break
+
+        if use_dora:
+            self.dora_init(adapter_name)
+            self.use_dora[adapter_name] = True
+        else:
+            self.use_dora[adapter_name] = False
+
+        self.set_adapter(self.active_adapters)
+
 
 class Conv2d(LoRAActivationMixin, _Conv2d):
 
     def __init__(self, *args, module_key: str, **kwargs):
         super(Conv2d, self).__init__(module_key)
         self.set_activation(args[1], True)
         super(ActivationMixin, self).__init__(*args, **kwargs)
@@ -529,14 +623,33 @@
     def __init__(self, model, config, adapter_name):
         if config is not None:
             super().__init__(model, config, adapter_name)
         else:
             nn.Module.__init__(self)
             self.model = model
 
+    def _mark_only_adapters_as_trainable(self, model: nn.Module) -> None:
+        for active_adapter in self.active_adapters:
+            bias = self.peft_config[active_adapter].bias
+            if bias == 'none':
+                continue
+
+            if bias == 'all':
+                for n, p in model.named_parameters():
+                    if 'bias' in n:
+                        p.requires_grad = True
+            elif bias == 'lora_only':
+                for m in model.modules():
+                    if isinstance(m, LoraLayer) and hasattr(
+                            m, 'bias') and m.bias is not None:
+                        m.bias.requires_grad = True
+            else:
+                raise NotImplementedError(
+                    f'Requested bias: {bias}, is not implemented.')
+
     def inject_adapter(self, model: nn.Module, adapter_name: str):
         r"""
         Override code:
         1. ModulesToSaveWrapper construction method: add module_key=key argument to offload to cpu
         """
         peft_config = self.peft_config[adapter_name]
         # Note: If possible, all checks should be performed *at the start of this method*.
@@ -710,28 +823,60 @@
             if new_module is not None:
                 if adapter_name != self.active_adapter:
                     # adding an additional adapter: it is not automatically trainable
                     new_module.requires_grad_(False)
                 self._replace_module(parent, target_name, new_module, target)
                 self._convert_dtype(new_module, lora_config.lora_dtype)
 
+    def _replace_module(self, parent, child_name, new_module, child):
+        setattr(parent, child_name, new_module)
+        # It's not necessary to set requires_grad here, as that is handled by
+        # _mark_only_adapters_as_trainable
+
+        # child layer wraps the original module, unpack it
+        if hasattr(child, 'base_layer'):
+            child = child.base_layer
+
+        if not hasattr(new_module, 'base_layer'):
+            new_module.weight = child.weight
+            if hasattr(child, 'bias'):
+                new_module.bias = child.bias
+
+        if getattr(child, 'state', None) is not None:
+            if hasattr(new_module, 'base_layer'):
+                new_module.base_layer.state = child.state
+            else:
+                new_module.state = child.state
+            new_module.to(child.weight.device)
+
+        # dispatch to correct device
+        for name, module in new_module.named_modules():
+            if (self.prefix in name) or ('ranknum' in name):
+                weight = child.qweight if hasattr(child,
+                                                  'qweight') else child.weight
+                if weight.device != torch.device('meta'):
+                    module.to(weight.device)
+
     @staticmethod
     def _create_new_module(lora_config, adapter_name, target, **kwargs):
         """
         Override code:
         1. Support current_key argument
         2. Support MergedLinear
         3. Support skipping NonDynamicallyQuantizableLinear(Move to dispatcher)
         4. Use Class type defined here(Move to dispatcher)
         5. return None instead of raising error when target type not found
         """
         # Collect dispatcher functions to decide what backend to use for the replaced LoRA layer. The order matters,
         # because the first match is always used. Therefore, the default layers should be checked last.
         current_key = kwargs.pop('current_key')
         new_module = None
+        if lora_config.use_qa_lora:
+            kwargs['use_qa_lora'] = True
+            kwargs['group_size'] = lora_config.group_size
         if lora_config.use_merged_linear:
             bias = kwargs.pop('bias', False)
             new_module = MergedLinear(
                 adapter_name,
                 current_key,
                 target,
                 bias=bias,
@@ -909,15 +1054,15 @@
         return
     elif bias == 'all':
         for n, p in model.named_parameters():
             if 'bias' in n:
                 p.requires_grad = True
     elif bias == 'lora_only':
         for n, m in model.named_modules():
-            if f'loramodule_{adapter_name}' in n and \
+            if 'lora_' in n and f'.{adapter_name}' in n and \
                     hasattr(m, 'bias') and \
                     m.bias is not None:
                 m.bias.requires_grad = True
     else:
         raise NotImplementedError
 
 
@@ -940,9 +1085,9 @@
                 if bias_name in state_dict:
                     to_return[bias_name] = state_dict[bias_name]
     else:
         raise NotImplementedError
     return {
         k: v
         for k, v in to_return.items()
-        if (('lora_' in k and f'.{adapter_name}.' in k) or ('bias' in k))
+        if (('lora_' in k and f'.{adapter_name}' in k) or ('bias' in k))
     }
```

### Comparing `ms-swift-1.7.3/swift/tuners/mapping.py` & `ms-swift-2.0.0/swift/tuners/mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/module_mapping.py` & `ms-swift-2.0.0/swift/tuners/module_mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/neftune.py` & `ms-swift-2.0.0/swift/tuners/neftune.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/prompt.py` & `ms-swift-2.0.0/swift/tuners/prompt.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/restuning.py` & `ms-swift-2.0.0/swift/tuners/restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/restuning_components.py` & `ms-swift-2.0.0/swift/tuners/restuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/compute_u.py` & `ms-swift-2.0.0/swift/tuners/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/compute_v.py` & `ms-swift-2.0.0/swift/tuners/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/context_template.py` & `ms-swift-2.0.0/swift/tuners/rome/context_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/nethook.py` & `ms-swift-2.0.0/swift/tuners/rome/nethook.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/repr_tools.py` & `ms-swift-2.0.0/swift/tuners/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/rome.py` & `ms-swift-2.0.0/swift/tuners/rome/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/rome/rome_hparams.py` & `ms-swift-2.0.0/swift/tuners/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/scetuning/scetuning.py` & `ms-swift-2.0.0/swift/tuners/scetuning/scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/scetuning/scetuning_components.py` & `ms-swift-2.0.0/swift/tuners/scetuning/scetuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/side.py` & `ms-swift-2.0.0/swift/tuners/side.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/tuners/utils.py` & `ms-swift-2.0.0/swift/tuners/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/app.py` & `ms-swift-2.0.0/swift/ui/app.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/base.py` & `ms-swift-2.0.0/swift/ui/base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_infer/generate.py` & `ms-swift-2.0.0/swift/ui/llm_infer/generate.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_infer/llm_infer.py` & `ms-swift-2.0.0/swift/ui/llm_infer/llm_infer.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_infer/model.py` & `ms-swift-2.0.0/swift/ui/llm_infer/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_infer/runtime.py` & `ms-swift-2.0.0/swift/ui/llm_infer/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                     latest_lines = latest_data.split('\n')
                     if latest_data[-1] != '\n':
                         latest_data = latest_lines[-1]
                         latest_lines = latest_lines[:-1]
                     else:
                         latest_data = ''
                     lines.extend(latest_lines)
-                    yield ['\n'.join(lines)]
+                    yield '\n'.join(lines)
         except IOError:
             pass
 
     @staticmethod
     def get_all_ports():
         process_name = 'swift'
         cmd_name = 'deploy'
@@ -169,20 +169,22 @@
                 cmdlines = proc.cmdline()
             except (psutil.ZombieProcess, psutil.AccessDenied,
                     psutil.NoSuchProcess):
                 cmdlines = []
             if any([process_name in cmdline
                     for cmdline in cmdlines]) and any(  # noqa
                         [cmd_name == cmdline for cmdline in cmdlines]):  # noqa
-
-                ports.add(
-                    int(
-                        Runtime.parse_info_from_cmdline(
-                            Runtime.construct_running_task(proc)).get(
-                                'port', 8000)))
+                try:
+                    ports.add(
+                        int(
+                            Runtime.parse_info_from_cmdline(
+                                Runtime.construct_running_task(proc)).get(
+                                    'port', 8000)))
+                except IndexError:
+                    pass
         return ports
 
     @staticmethod
     def refresh_tasks(running_task=None):
         log_file = running_task if not running_task or 'pid:' not in running_task else None
         process_name = 'swift'
         cmd_name = 'deploy'
```

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/advanced.py` & `ms-swift-2.0.0/swift/ui/llm_train/advanced.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/dataset.py` & `ms-swift-2.0.0/swift/ui/llm_train/dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/hyper.py` & `ms-swift-2.0.0/swift/ui/llm_train/hyper.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/llm_train.py` & `ms-swift-2.0.0/swift/ui/llm_train/llm_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,14 +161,44 @@
             },
             'info': {
                 'zh':
                 '使用neftune提升训练效果, 一般设置为5或者10',
                 'en':
                 'Use neftune to improve performance, normally the value should be 5 or 10'
             }
+        },
+        'use_galore': {
+            'label': {
+                'zh': '使用GaLore',
+                'en': 'Use GaLore'
+            },
+            'info': {
+                'zh':
+                '使用Galore来减少全参数训练的显存消耗',
+                'en':
+                'Use Galore to reduce GPU memory usage in full parameter training'
+            }
+        },
+        'galore_rank': {
+            'label': {
+                'zh': 'Galore的秩',
+                'en': 'The rank of Galore'
+            },
+        },
+        'galore_update_proj_gap': {
+            'label': {
+                'zh': 'Galore project matrix更新频率',
+                'en': 'The updating gap of the project matrix'
+            },
+        },
+        'galore_optim_per_parameter': {
+            'label': {
+                'zh': '为每个Galore Parameter创建单独的optimizer',
+                'en': 'Create unique optimizer for per Galore parameter'
+            },
         }
     }
 
     choice_dict = BaseUI.get_choices_from_dataclass(SftArguments)
     default_dict = BaseUI.get_default_value_from_dataclass(SftArguments)
 
     @classmethod
@@ -192,14 +222,29 @@
                     gr.Slider(
                         elem_id='neftune_noise_alpha',
                         minimum=0.0,
                         maximum=20.0,
                         step=0.5,
                         scale=4)
                 with gr.Row():
+                    gr.Checkbox(elem_id='use_galore', scale=4)
+                    gr.Slider(
+                        elem_id='galore_rank',
+                        minimum=8,
+                        maximum=256,
+                        step=8,
+                        scale=4)
+                    gr.Slider(
+                        elem_id='galore_update_proj_gap',
+                        minimum=10,
+                        maximum=1000,
+                        step=50,
+                        scale=4)
+                    gr.Checkbox(elem_id='galore_optim_per_parameter', scale=4)
+                with gr.Row():
                     gr.Dropdown(
                         elem_id='gpu_id',
                         multiselect=True,
                         choices=[str(i) for i in range(gpu_count)] + ['cpu'],
                         value=default_device,
                         scale=8)
                     gr.Textbox(elem_id='gpu_memory_fraction', scale=4)
```

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/lora.py` & `ms-swift-2.0.0/swift/ui/llm_train/lora.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,36 @@
         },
         'lora_dropout_p': {
             'label': {
                 'zh': 'LoRA的dropout',
                 'en': 'The LoRA dropout'
             }
         },
+        'use_rslora': {
+            'label': {
+                'zh': '使用rslora',
+                'en': 'Use rslora'
+            }
+        },
+        'use_dora': {
+            'label': {
+                'zh': '使用dora',
+                'en': 'Use dora'
+            }
+        },
+        'lora_lr_ratio': {
+            'label': {
+                'zh': 'Lora+学习率倍率',
+                'en': 'The lr ratio of Lora+'
+            },
+            'info': {
+                'zh': '建议值16.0',
+                'en': 'Suggested value: 16.0'
+            }
+        },
     }
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.Accordion(elem_id='lora_tab', open=True):
             with gr.Blocks():
                 with gr.Row():
@@ -68,14 +90,18 @@
                         step=8)
                     gr.Slider(
                         elem_id='lora_alpha',
                         value=8,
                         minimum=1,
                         maximum=512,
                         step=8)
+                    gr.Dropdown(elem_id='lora_dtype')
+                    gr.Textbox(elem_id='lora_lr_ratio')
+                    gr.Checkbox(elem_id='use_rslora')
+                    gr.Checkbox(elem_id='use_dora')
                     gr.Textbox(elem_id='lora_dropout_p')
 
             def update_lora(choice):
                 if choice is not None:
                     return ' '.join(
                         MODEL_MAPPING[choice]['lora_target_modules'])
                 return None
```

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/model.py` & `ms-swift-2.0.0/swift/ui/llm_train/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
             default_system = getattr(
                 TEMPLATE_MAPPING[MODEL_MAPPING[choice]['template']]
                 ['template'], 'default_system', None)
             template = MODEL_MAPPING[choice]['template']
             return model_id_or_path, default_system, template
 
         def update_model_id_or_path(model_type, model_id_or_path, model_state):
+            if model_type is None or isinstance(model_type, list):
+                return model_state
             model_state[model_type] = model_id_or_path
             return model_state
 
         def reset(model_type):
             model_id_or_path, default_system, template = update_input_model(
                 model_type)
             return model_id_or_path, default_system, template, {}
```

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/quantization.py` & `ms-swift-2.0.0/swift/ui/llm_train/quantization.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/runtime.py` & `ms-swift-2.0.0/swift/ui/llm_train/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,20 @@
         if not task:
             return [None] * len(Runtime.sft_plot)
         all_args = Runtime.parse_info_from_cmdline(task)
         tb_dir = all_args['logging_dir']
         fname = [
             fname for fname in os.listdir(tb_dir)
             if os.path.isfile(os.path.join(tb_dir, fname))
-        ][0]
+            and fname.startswith('events.out')
+        ]
+        if fname:
+            fname = fname[0]
+        else:
+            return [None] * len(Runtime.sft_plot)
         tb_path = os.path.join(tb_dir, fname)
         data = read_tensorboard_file(tb_path)
 
         plots = []
         for k in Runtime.sft_plot:
             name = k['name']
             smooth = k['smooth']
```

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/save.py` & `ms-swift-2.0.0/swift/ui/llm_train/save.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/self_cog.py` & `ms-swift-2.0.0/swift/ui/llm_train/self_cog.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/ui/llm_train/utils.py` & `ms-swift-2.0.0/swift/ui/llm_train/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/__init__.py` & `ms-swift-2.0.0/swift/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from .run_utils import get_main
 from .tb_utils import (TB_COLOR, TB_COLOR_SMOOTH, plot_images,
                        read_tensorboard_file, tensorboard_smoothing)
 from .torch_utils import (activate_model_parameters, broadcast_string,
                           freeze_model_parameters, get_dist_setting,
                           get_model_info, is_ddp_plus_mp, is_dist,
                           is_local_master, is_master, is_mp, is_on_same_device,
-                          show_layers, time_synchronize)
+                          show_layers, time_synchronize, use_torchacc)
 from .utils import (add_version_to_work_dir, check_json_format,
                     get_pai_tensorboard_dir, is_pai_training_job, lower_bound,
                     parse_args, read_multi_line, seed_everything,
                     subprocess_run, test_time, upper_bound)
```

### Comparing `ms-swift-1.7.3/swift/utils/constants.py` & `ms-swift-2.0.0/swift/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/hub.py` & `ms-swift-2.0.0/swift/utils/hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/import_utils.py` & `ms-swift-2.0.0/swift/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/io_utils.py` & `ms-swift-2.0.0/swift/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/logger.py` & `ms-swift-2.0.0/swift/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/metric.py` & `ms-swift-2.0.0/swift/utils/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 
 from typing import Dict, Literal
 
-import jieba
 import numpy as np
 from nltk.translate.bleu_score import SmoothingFunction, sentence_bleu
 from rouge.rouge import Rouge
 from torch import Tensor
 from transformers.trainer_utils import EvalPrediction
 
 from .logger import get_logger
 
 logger = get_logger()
 
 
 def compute_nlg_metrics(prediction, tokenizer):
+    import jieba
     preds, labels = prediction[0], prediction[1]
 
     score_dict = {'rouge-1': [], 'rouge-2': [], 'rouge-l': [], 'bleu-4': []}
 
     def _decode(tokens, ignore_pad_token_for_loss=False):
         if ignore_pad_token_for_loss:
             tokens = np.where(tokens != -100, tokens, tokenizer.pad_token_id)
```

### Comparing `ms-swift-1.7.3/swift/utils/np_utils.py` & `ms-swift-2.0.0/swift/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/run_utils.py` & `ms-swift-2.0.0/swift/utils/run_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/tb_utils.py` & `ms-swift-2.0.0/swift/utils/tb_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/swift/utils/torch_utils.py` & `ms-swift-2.0.0/swift/utils/torch_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,21 +70,29 @@
 
 
 def is_local_master():
     local_rank = get_dist_setting()[1]
     return local_rank in {-1, 0}
 
 
+def use_torchacc() -> bool:
+    return os.getenv('USE_TORCHACC', '0') == '1'
+
+
 def is_dist():
     """Determine if the training is distributed"""
+    if use_torchacc():
+        return False
     rank, local_rank, _, _ = get_dist_setting()
     return rank >= 0 and local_rank >= 0
 
 
 def is_mp() -> bool:
+    if use_torchacc():
+        return False
     n_gpu = torch.cuda.device_count()
     local_world_size = get_dist_setting()[3]
     assert n_gpu % local_world_size == 0
     if n_gpu // local_world_size >= 2:
         return True
     return False
```

### Comparing `ms-swift-1.7.3/swift/utils/utils.py` & `ms-swift-2.0.0/swift/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -173,7 +173,57 @@
                    env: Optional[Dict[str, str]] = None,
                    stdout=None,
                    stderr=None) -> None:
     # stdoutm stderr: e.g. subprocess.PIPE.
     resp = subprocess.run(command, env=env, stdout=stdout, stderr=stderr)
     resp.check_returncode()
     return resp
+
+
+def split_str_parts_by(text: str, delimiters: List[str]):
+    """Split the text field into parts.
+
+    Args:
+        text: A text to be split.
+        delimiters: The delimiters.
+
+    Returns:
+        The split text in list of dicts.
+    """
+    all_start_chars = [d[0] for d in delimiters]
+    all_length = [len(d) for d in delimiters]
+
+    text_list = []
+    last_words = ''
+
+    while len(text) > 0:
+        for char_idx, char in enumerate(text):
+            match_index = [
+                idx for idx, start_char in enumerate(all_start_chars)
+                if start_char == char
+            ]
+            is_delimiter = False
+            for index in match_index:
+                if text[char_idx:char_idx
+                        + all_length[index]] == delimiters[index]:
+                    if last_words:
+                        if text_list:
+                            text_list[-1]['content'] = last_words
+                        else:
+                            text_list.append({
+                                'key': '',
+                                'content': last_words
+                            })
+                    last_words = ''
+                    text_list.append({'key': delimiters[index]})
+                    text = text[char_idx + all_length[index]:]
+                    is_delimiter = True
+                    break
+            if not is_delimiter:
+                last_words += char
+            else:
+                break
+        if last_words == text:
+            text = ''
+
+    text_list[-1]['content'] = last_words
+    return text_list
```

### Comparing `ms-swift-1.7.3/tests/hub/test_check_model.py` & `ms-swift-2.0.0/tests/hub/test_check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/llm/test_dataset.py` & `ms-swift-2.0.0/tests/llm/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/llm/test_run.py` & `ms-swift-2.0.0/tests/llm/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,25 @@
             'alpaca.csv', 'chatml.jsonl', 'swift_pre.jsonl',
             'swift_single.csv', 'swift_multi.jsonl', 'swift_multi.json'
         ]
         val_dataset_fnames = [
             'alpaca.jsonl', 'alpaca2.csv', 'conversations.jsonl',
             'swift_pre.csv', 'swift_single.jsonl'
         ]
+        mixture_dataset = val_dataset_fnames
         folder = os.path.join(os.path.dirname(__file__), 'data')
         sft_args = SftArguments(
             model_type='qwen-7b-chat',
             custom_train_dataset_path=[
                 os.path.join(folder, fname) for fname in train_dataset_fnames
             ],
+            train_dataset_mix_ds=[
+                os.path.join(folder, fname) for fname in mixture_dataset
+            ],
+            train_dataset_mix_ratio=0.1,
             check_dataset_strategy='warning')
         torch.cuda.empty_cache()
         best_model_checkpoint = sft_main(sft_args)['best_model_checkpoint']
         for load_args_from_ckpt_dir in [True, False]:
             kwargs = {}
             if load_args_from_ckpt_dir is False:
                 kwargs = {'model_type': 'qwen-7b-chat'}
```

### Comparing `ms-swift-1.7.3/tests/llm/test_template.py` & `ms-swift-2.0.0/tests/llm/test_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/llm/test_utils.py` & `ms-swift-2.0.0/tests/llm/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/llm/test_vllm_utils.py` & `ms-swift-2.0.0/tests/llm/test_vllm_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/model_tag.py` & `ms-swift-2.0.0/tests/model_tag.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/run.py` & `ms-swift-2.0.0/tests/run.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/test_utils.py` & `ms-swift-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/tuners/test_extra_state_dict.py` & `ms-swift-2.0.0/tests/tuners/test_extra_state_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import math
 import os.path
 import shutil
 import tempfile
 import unittest
 
+import peft
 import torch
-from modelscope import Model, Preprocessor
-from torch import nn
+from modelscope import Model
+from packaging import version
 
 from swift import LoRAConfig, Swift
 from swift.tuners.utils import ModulesToSaveWrapper
 
 
+@unittest.skipIf(
+    version.parse(peft.__version__) >= version.parse('0.10.0'),
+    reason='version not match')
 class TestExtraStateDict(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
         self.tmp_dir = tempfile.TemporaryDirectory().name
         if not os.path.exists(self.tmp_dir):
             os.makedirs(self.tmp_dir)
```

### Comparing `ms-swift-1.7.3/tests/tuners/test_merged_linear.py` & `ms-swift-2.0.0/tests/tuners/test_merged_linear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import math
 import unittest
 
+import peft
 import torch
 from modelscope import Model, Preprocessor
+from packaging import version
 from torch import nn
 
 from swift import LoRAConfig, Swift
 
 
+@unittest.skipIf(
+    version.parse(peft.__version__) >= version.parse('0.10.0'),
+    reason='version not match')
 class TestMergedLinear(unittest.TestCase):
 
     def test_swift_lora_forward(self):
 
         from swift.tuners.lora import MergedLinear
 
         def reset_parameters(self):
```

### Comparing `ms-swift-1.7.3/tests/tuners/test_neft.py` & `ms-swift-2.0.0/tests/tuners/test_neft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import shutil
 import tempfile
 import unittest
 
+import peft
 import torch
 from modelscope import AutoModel, AutoTokenizer, Preprocessor
+from packaging import version
 from peft.utils import WEIGHTS_NAME
 from transformers import PreTrainedModel
 
-from swift import LoRAConfig, Swift
+from swift import LoraConfig, Swift
 from swift.tuners import NEFTuneConfig
 
 
 class TestNEFT(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
@@ -71,21 +73,24 @@
             self.assertTrue(key in state_dict2)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict2[key]).flatten().detach().cpu()))
         PreTrainedModel.save_pretrained = PreTrainedModel.origin_save_pretrained
 
+    @unittest.skipIf(
+        version.parse(peft.__version__) >= version.parse('0.10.0'),
+        reason='version not match')
     def test_neft_lora(self):
         model = AutoModel.from_pretrained('AI-ModelScope/bert-base-uncased')
         preprocessor = Preprocessor.from_pretrained(
             'damo/nlp_structbert_sentence-similarity_chinese-base')
         inputs = preprocessor('how are you')
         config = NEFTuneConfig()
-        config2 = LoRAConfig(target_modules=['query', 'key', 'value'])
+        config2 = LoraConfig(target_modules=['query', 'key', 'value'])
 
         t1 = model.embeddings.word_embeddings(inputs['input_ids'])
         model = Swift.prepare_model(model, {'c1': config, 'c2': config2})
         model.train()
         t2 = model.embeddings.word_embeddings(inputs['input_ids'])
         model.deactivate_adapter('c1')
         t3 = model.embeddings.word_embeddings(inputs['input_ids'])
```

### Comparing `ms-swift-1.7.3/tests/tuners/test_peft.py` & `ms-swift-2.0.0/tests/tuners/test_peft.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import copy
 import os
 import shutil
 import tempfile
 import unittest
 
+import peft
 import torch
 from modelscope import Preprocessor
 from modelscope.models.nlp.structbert import (SbertConfig,
                                               SbertForSequenceClassification)
+from packaging import version
 from peft import PeftModel, inject_adapter_in_model
+from peft.config import PeftConfigMixin
 from peft.tuners.lora import Linear
 from peft.utils import WEIGHTS_NAME
 from torch import nn
 
 from swift import AdaLoraConfig, LoraConfig, LoRAConfig, Swift, get_peft_model
 
 
@@ -115,14 +118,17 @@
         for key in state_dict:
             self.assertTrue(key in state_dict3)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict3[key]).flatten().detach().cpu()))
 
+    @unittest.skipIf(
+        version.parse(peft.__version__) >= version.parse('0.10.0'),
+        reason='version not match')
     def test_lora_reload_by_peft(self):
         lora_config = LoRAConfig(target_modules=['query', 'key', 'value'])
         model = SbertForSequenceClassification(SbertConfig())
         model2 = copy.deepcopy(model)
         model = Swift.prepare_model(model, lora_config)
         model.save_pretrained(self.tmp_dir, peft_format=True)
         model2 = PeftModel.from_pretrained(model2, self.tmp_dir)
@@ -155,7 +161,38 @@
         state_dict2 = model2.state_dict()
         for key in state_dict:
             self.assertTrue(key in state_dict2)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict2[key]).flatten().detach().cpu()))
+
+    def test_peft_lora_dtype(self):
+        model = SbertForSequenceClassification(SbertConfig())
+        model2 = copy.deepcopy(model)
+        model3 = copy.deepcopy(model)
+        lora_config = LoraConfig(
+            target_modules=['query', 'key', 'value'], lora_dtype='fp16')
+        model = Swift.prepare_model(model, lora_config)
+        model.save_pretrained(self.tmp_dir, safe_serialization=False)
+        self.assertTrue(
+            os.path.exists(
+                os.path.join(self.tmp_dir, 'additional_config.json')))
+        model2 = Swift.from_pretrained(model2, self.tmp_dir)
+        self.assertTrue(model2.base_model.model.bert.encoder.layer[0].attention
+                        .self.key.lora_A.default.weight.dtype == torch.float16)
+        self.assertTrue(model2.peft_config['default'].lora_dtype == 'fp16')
+        state_dict = model.state_dict()
+        state_dict2 = model2.state_dict()
+        for key in state_dict:
+            self.assertTrue(key in state_dict2)
+            self.assertTrue(
+                all(
+                    torch.isclose(state_dict[key],
+                                  state_dict2[key]).flatten().detach().cpu()))
+
+        PeftConfigMixin.from_pretrained = PeftConfigMixin.from_pretrained_origin
+        model3 = peft.PeftModel.from_pretrained(model3, self.tmp_dir)
+        self.assertTrue(model3.base_model.model.bert.encoder.layer[0].attention
+                        .self.key.lora_A.default.weight.dtype == torch.float32)
+        self.assertTrue(
+            isinstance(model3.peft_config['default'], peft.LoraConfig))
```

### Comparing `ms-swift-1.7.3/tests/tuners/test_rome.py` & `ms-swift-2.0.0/tests/tuners/test_rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/tuners/test_scetuning.py` & `ms-swift-2.0.0/tests/tuners/test_scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/tuners/test_swift_base.py` & `ms-swift-2.0.0/tests/tuners/test_swift_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 import math
 import os
 import shutil
 import tempfile
 import unittest
 from concurrent.futures import ThreadPoolExecutor
 
+import peft
 import torch
 from modelscope import Model, Preprocessor
 from modelscope.models.nlp.structbert import (SbertConfig,
                                               SbertForSequenceClassification)
+from packaging import version
 from peft import PeftModel
 from peft.utils import WEIGHTS_NAME
 from torch import nn
 
 from swift import (AdapterConfig, LoRAConfig, PromptConfig, ResTuningConfig,
                    SideConfig, Swift, SwiftModel)
 
 
+@unittest.skipIf(
+    version.parse(peft.__version__) >= version.parse('0.10.0'),
+    reason='version not match')
 class TestSwift(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
         self.tmp_dir = tempfile.TemporaryDirectory().name
         if not os.path.exists(self.tmp_dir):
             os.makedirs(self.tmp_dir)
@@ -266,25 +271,55 @@
             self.assertTrue(False)
         except AssertionError as e:
             print(e)
             pass
 
     def test_save_to_peft_ok(self):
         model = SbertForSequenceClassification(SbertConfig())
-        lora_config = LoRAConfig(target_modules=['query', 'key', 'value'])
-        lora2_config = LoRAConfig(target_modules=['query', 'key', 'value'])
+        lora_config = LoRAConfig(
+            target_modules=['query', 'key', 'value'], use_dora=True)
+        lora2_config = LoRAConfig(
+            target_modules=['query', 'key', 'value'], use_dora=True)
         model = Swift.prepare_model(
             model, config={
                 'default': lora_config,
                 'lora': lora2_config
             })
         model.save_pretrained(os.path.join(self.tmp_dir, 'original'))
         Swift.save_to_peft_format(
             os.path.join(self.tmp_dir, 'original'),
             os.path.join(self.tmp_dir, 'converted'))
+        # A duplicate conversion
+        Swift.save_to_peft_format(
+            os.path.join(self.tmp_dir, 'original'),
+            os.path.join(self.tmp_dir, 'converted'))
+
+        # -------------------base case--------------------
+        model2 = SbertForSequenceClassification(SbertConfig())
+        model2 = PeftModel.from_pretrained(
+            model2, os.path.join(self.tmp_dir, 'converted'))
+        model2.load_adapter(
+            os.path.join(os.path.join(self.tmp_dir, 'converted'), 'lora'),
+            'lora')
+        state_dict = model.state_dict()
+        state_dict2 = {
+            key[len('base_model.model.'):]: value
+            for key, value in model2.state_dict().items() if 'lora' in key
+        }
+        for key in state_dict:
+            self.assertTrue(key in state_dict2)
+            self.assertTrue(
+                all(
+                    torch.isclose(state_dict[key],
+                                  state_dict2[key]).flatten().detach().cpu()))
+
+        # -------------------override case--------------------
+        Swift.save_to_peft_format(
+            os.path.join(self.tmp_dir, 'converted'),
+            os.path.join(self.tmp_dir, 'converted'))
         model2 = SbertForSequenceClassification(SbertConfig())
         model2 = PeftModel.from_pretrained(
             model2, os.path.join(self.tmp_dir, 'converted'))
         model2.load_adapter(
             os.path.join(os.path.join(self.tmp_dir, 'converted'), 'lora'),
             'lora')
         state_dict = model.state_dict()
```

### Comparing `ms-swift-1.7.3/tests/tuners/test_swift_device_map.py` & `ms-swift-2.0.0/tests/tuners/test_swift_device_map.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/tuners/test_swift_restuning.py` & `ms-swift-2.0.0/tests/tuners/test_swift_restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-1.7.3/tests/utils/test_io_utils.py` & `ms-swift-2.0.0/tests/utils/test_io_utils.py`

 * *Files identical despite different names*

