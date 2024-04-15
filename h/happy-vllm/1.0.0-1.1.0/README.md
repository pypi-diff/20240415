# Comparing `tmp/happy_vllm-1.0.0.tar.gz` & `tmp/happy_vllm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_vllm-1.0.0.tar", last modified: Thu Apr 11 09:11:18 2024, max compression
+gzip compressed data, was "happy_vllm-1.1.0.tar", last modified: Mon Apr 15 09:37:02 2024, max compression
```

## Comparing `happy_vllm-1.0.0.tar` & `happy_vllm-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.140568 happy_vllm-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.140568 happy_vllm-1.0.0/src/happy_vllm/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/core/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/logits_processors/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/middlewares/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/model/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/model/model_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/request.json
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/response.json
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/utils_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/src/happy_vllm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_routers_functionnal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_routers_technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_schemas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils_parse_logits_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 09:11:16.000000 happy_vllm-1.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.782080 happy_vllm-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/logits_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/middlewares/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/openai_serving_chat_fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/utils_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_routers_functionnal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_routers_technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_schemas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils_parse_logits_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 09:37:00.000000 happy_vllm-1.1.0/version.txt
```

### Comparing `happy_vllm-1.0.0/LICENSE` & `happy_vllm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/PKG-INFO` & `happy_vllm-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.0.0
+Version: 1.1.0
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vllm<1.0,>=0.4.0
 Requires-Dist: fastapi<1.0,>=0.110.1
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
@@ -52,27 +52,27 @@
 ```
 
 ## Quickstart
 
 Just use the entrypoint `happy-vllm` (see [arguments](https://oss-pole-emploi.github.io/happy_vllm/arguments/) for a list of all possible arguments)
 
 ```bash
-happy_vllm --model path_to_model --host 127.0.0.1 --port 5000
+happy_vllm --model path_to_model --host 127.0.0.1 --port 5000 --model-name my_model
 ```
 
 It will launch the API and you can directly query it for example with 
 
 ```bash
-curl 127.0.0.1:5000/info
+curl 127.0.0.1:5000/v1/info
 ```
 
 To get various information on the application or 
 
 ```bash
-curl 127.0.0.1:5000/generate -d '{"prompt": "Hey,"}'
+curl 127.0.0.1:5000/v1/completions -d '{"prompt": "Hey,", "model": "my_model"}'
 ```
 
 if you want to generate your first LLM response using happy_vLLM. See [endpoints](https://oss-pole-emploi.github.io/happy_vllm/endpoints/endpoints) for more details on all the endpoints provided by happy_vLLM. 
 
 ## Deploy with Docker image
 
 A docker image is available from the [Github Container Registry](https://github.com/OSS-Pole-Emploi/happy_vllm/pkgs/container/happy_vllm) :
```

### Comparing `happy_vllm-1.0.0/README.md` & `happy_vllm-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 ```
 
 ## Quickstart
 
 Just use the entrypoint `happy-vllm` (see [arguments](https://oss-pole-emploi.github.io/happy_vllm/arguments/) for a list of all possible arguments)
 
 ```bash
-happy_vllm --model path_to_model --host 127.0.0.1 --port 5000
+happy_vllm --model path_to_model --host 127.0.0.1 --port 5000 --model-name my_model
 ```
 
 It will launch the API and you can directly query it for example with 
 
 ```bash
-curl 127.0.0.1:5000/info
+curl 127.0.0.1:5000/v1/info
 ```
 
 To get various information on the application or 
 
 ```bash
-curl 127.0.0.1:5000/generate -d '{"prompt": "Hey,"}'
+curl 127.0.0.1:5000/v1/completions -d '{"prompt": "Hey,", "model": "my_model"}'
 ```
 
 if you want to generate your first LLM response using happy_vLLM. See [endpoints](https://oss-pole-emploi.github.io/happy_vllm/endpoints/endpoints) for more details on all the endpoints provided by happy_vLLM. 
 
 ## Deploy with Docker image
 
 A docker image is available from the [Github Container Registry](https://github.com/OSS-Pole-Emploi/happy_vllm/pkgs/container/happy_vllm) :
```

### Comparing `happy_vllm-1.0.0/pyproject.toml` & `happy_vllm-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/application.py` & `happy_vllm-1.1.0/src/happy_vllm/application.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,31 +13,33 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from fastapi import FastAPI
 from argparse import Namespace
-from fastapi.middleware.cors import CORSMiddleware
-
 from .routers import main_routeur
 from .core.resources import get_lifespan
-from happy_vllm.middlewares.exception import ExceptionHandlerMiddleware
 from prometheus_client import make_asgi_app
+from fastapi.middleware.cors import CORSMiddleware
+
+from happy_vllm import utils
+from happy_vllm.middlewares.exception import ExceptionHandlerMiddleware
 
 def declare_application(args: Namespace) -> FastAPI:
     """Create the FastAPI application
 
     See https://fastapi.tiangolo.com/tutorial/first-steps/ to learn how to
     customize your FastAPI application
     """
     app = FastAPI(
-        title=f"REST API for vLLM",
+        title=f"A REST API for vLLM",
         description=f"A REST API for vLLM, production ready",
-        lifespan=get_lifespan(args=args)
+        lifespan=get_lifespan(args=args),
+        version=utils.get_package_version()
     )
 
     # Add prometheus asgi middleware to route /metrics requests
     metrics_app = make_asgi_app()
     app.mount("/metrics", metrics_app)
 
     # CORS middleware that allows all origins to avoid CORS problems
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/core/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/core/config.py` & `happy_vllm-1.1.0/src/happy_vllm/core/config.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/core/logtools.py` & `happy_vllm-1.1.0/src/happy_vllm/core/logtools.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/core/resources.py` & `happy_vllm-1.1.0/src/happy_vllm/core/resources.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/launch.py` & `happy_vllm-1.1.0/src/happy_vllm/launch.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/logits_processors/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/logits_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/logits_processors/json_format.py` & `happy_vllm-1.1.0/src/happy_vllm/logits_processors/json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/logits_processors/response_pool.py` & `happy_vllm-1.1.0/src/happy_vllm/logits_processors/response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py` & `happy_vllm-1.1.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/middlewares/exception.py` & `happy_vllm-1.1.0/src/happy_vllm/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/model/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/model/model_base.py` & `happy_vllm-1.1.0/src/happy_vllm/model/model_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,24 @@
 import logging
 from pathlib import Path
 from argparse import Namespace
 from transformers import AutoTokenizer
 from typing import Any, Tuple, Union, List
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
+from vllm.entrypoints.openai.serving_completion import OpenAIServingCompletion
 from vllm.transformers_utils.tokenizer_group.tokenizer_group import TokenizerGroup
 from lmformatenforcer.integrations.transformers import build_token_enforcer_tokenizer_data
 
 from happy_vllm import utils
+# We use our own version of OpenAIServingChat to avoid this issue (https://github.com/vllm-project/vllm/issues/2683)
+# To solve this issue, we do what is described in this PR (https://github.com/vllm-project/vllm/pull/2727)
+# When it is resolved, please go back to the vLLM version of OpenAIServingChat and delete this one
+# from vllm.entrypoints.openai.serving_chat import OpenAIServingChat
+from happy_vllm.model.openai_serving_chat_fixed import OpenAIServingChat
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     """Parent model class.
     """
@@ -73,14 +79,19 @@
             if isinstance(self._model.engine.tokenizer, TokenizerGroup): # type: ignore
                 self._tokenizer = self._model.engine.tokenizer.tokenizer # type: ignore
             else:
                 self._tokenizer = self._model.engine.tokenizer # type: ignore
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
             self.max_model_len = self._model.engine.model_config.max_model_len # type: ignore
             self.original_truncation_side = self._tokenizer.truncation_side
+            self.openai_serving_chat = OpenAIServingChat(self._model, args.model_name,
+                                                        args.response_role,
+                                                        args.lora_modules,
+                                                        args.chat_template)
+            self.openai_serving_completion = OpenAIServingCompletion(self._model, args.model_name, args.lora_modules)
         # For test purpose
         else:
             self.max_model_len = 2048
             self.original_truncation_side = 'right'
             self._tokenizer = AutoTokenizer.from_pretrained(utils.TEST_TOKENIZER_NAME,
                                                      cache_dir=os.environ["TEST_MODELS_DIR"], truncation_side=self.original_truncation_side)
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
@@ -268,8 +279,10 @@
 class MockOutput():
     
     def __init__(self, text):
         self.text = text
         if text[-len("don't you ?"):] == "don't you ?":
             self.finish_reason = "stop"
         else:
-            self.finish_reason = None
+            self.finish_reason = None
+
+
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/functional.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/functional.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,25 +19,28 @@
 from vllm.utils import random_uuid
 from fastapi import APIRouter, Body
 from pydantic import BaseModel, Field
 from starlette.requests import Request
 from vllm.sampling_params import SamplingParams
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from lmformatenforcer import TokenEnforcerTokenizerData
-from typing import Annotated, AsyncGenerator, Tuple, List
+from vllm.entrypoints.openai import protocol as vllm_protocol
+from typing import Annotated, AsyncGenerator, Tuple, List, Union
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from starlette.responses import JSONResponse, Response, StreamingResponse
 
+
 from happy_vllm import utils
 from happy_vllm.logits_processors.response_pool import VLLMLogitsProcessorResponsePool
 from happy_vllm.logits_processors.utils_parse_logits_processors import logits_processors_parser, detect_logits_processors_incompatibilities
 
 from ..model.model_base import Model
 from ..core.resources import RESOURCE_MODEL, RESOURCES
-from .schemas.functional import ResponseGenerate, RequestGenerate, ResponseTokenizer, RequestTokenizer, ResponseDecode, RequestDecode, ResponseSplitText, RequestSplitText, ResponseMetadata, RequestMetadata
+from happy_vllm.routers.schemas import functional as functional_schema
+
 
 
 # Load the response examples
 directory = os.path.dirname(os.path.abspath(__file__))
 request_examples_path = os.path.join(directory, "schemas", "examples", "request.json")
 with open(request_examples_path, 'r') as file:
     request_openapi_examples = json.load(file)
@@ -114,22 +117,22 @@
             min_tokens = sampling_params.min_tokens
             reponse_pool = logits_processor.possible_tokens_responses
             if min_tokens > 0 and len(reponse_pool):
                 raise ValueError(f"min_tokens : {min_tokens} is incompatible with the `response_pool` keyword")
     return prompt, prompt_in_response, sampling_params
 
 
-@router.post("/generate", response_model=ResponseGenerate)
+@router.post("/v1/generate", response_model=functional_schema.ResponseGenerate)
 async def generate(
     request: Request,
     request_type: Annotated[
-        RequestGenerate,
+        functional_schema.RequestGenerate,
         Body(openapi_examples=request_openapi_examples["generate"])] = None
     ) -> Response:
-    """Generate completion for the request.
+    """DEPRECATED. Generate completion for the request.
 
     The request should be a JSON object with the following fields:
     - prompt: The prompt to use for the generation.
     - other fields: The sampling parameters (See `SamplingParams` from vLLM for more details : 
                                              https://github.com/vllm-project/vllm/blob/main/vllm/sampling_params.py).
     """
     
@@ -157,21 +160,21 @@
     finish_reasons = ["None" if finish_reason is None else finish_reason for finish_reason in finish_reasons]
     ret = {"responses": text_outputs, "finish_reasons": finish_reasons}
     if prompt_in_response:
         ret['prompt'] = prompt
     return JSONResponse(ret)
 
 
-@router.post("/generate_stream", response_model=ResponseGenerate)
+@router.post("/v1/generate_stream", response_model=functional_schema.ResponseGenerate)
 async def generate_stream(request: Request,
     request_type: Annotated[
-        RequestGenerate,
+        functional_schema.RequestGenerate,
         Body(openapi_examples=request_openapi_examples["generate_stream"])] = None
     ) -> StreamingResponse:
-    """Generate completion for the request.
+    """DEPRECATED. Generate completion for the request.
 
     The request should be a JSON object with the following fields:
     - prompt: The prompt to use for the generation.
     - other fields: The sampling parameters (See `SamplingParams` for details).
     """
     model: Model = RESOURCES.get(RESOURCE_MODEL)
     request_dict = await request.json()
@@ -192,18 +195,18 @@
             if prompt_in_response:
                 ret['prompt'] = prompt
             yield (json.dumps(ret) + "\n")#.encode("utf-8")
 
     return StreamingResponse(stream_results())
 
 
-@router.post("/tokenizer", response_model=ResponseTokenizer)
+@router.post("/v1/tokenizer", response_model=functional_schema.ResponseTokenizer)
 async def tokenizer(request: Request,
     request_type: Annotated[
-        RequestTokenizer,
+        functional_schema.RequestTokenizer,
         Body(openapi_examples=request_openapi_examples["tokenizer"])] = None
     ) -> Response:
     """Tokenizes a text
 
     The request should be a JSON object with the following fields:
     - text: The text to tokenize
     - with_tokens_str (optional): Whether we want the tokens strings in the output
@@ -227,18 +230,18 @@
 
     ret = {"tokens_ids": tokens_ids, "tokens_nb": len(tokens_ids)}
     if with_tokens_str:
         ret['tokens_str'] = tokens_str
     return JSONResponse(ret)
 
 
-@router.post("/decode", response_model=ResponseDecode)
+@router.post("/v1/decode", response_model=functional_schema.ResponseDecode)
 async def decode(request: Request,
     request_type: Annotated[
-        RequestDecode,
+        functional_schema.RequestDecode,
         Body(openapi_examples=request_openapi_examples["decode"])] = None
     ) -> Response:
     """Decodes token ids
 
     The request should be a JSON object with the following fields:
     - token_ids: The ids of the tokens
     - with_tokens_str : If the result should also include a list of str
@@ -262,18 +265,18 @@
 
     ret = {"decoded_string": decoded_string}
     if with_tokens_str:
         ret[ "tokens_str"] = tokens_str
     return JSONResponse(ret)
 
 
-@router.post("/split_text", response_model=ResponseSplitText)
+@router.post("/v1/split_text", response_model=functional_schema.ResponseSplitText)
 async def split_text(request: Request,
     request_type: Annotated[
-        RequestSplitText,
+        functional_schema.RequestSplitText,
         Body(openapi_examples=request_openapi_examples["split_text"])] = None
     ):
     """Splits a text with a minimal number of token in each chunk. Each chunk is delimited by a separator
 
     The request should be a JSON object with the following fields:
     - text: The text to split
     - num_tokens_in_chunk (optional): The minimal number of tokens we want in each chunk
@@ -284,18 +287,18 @@
     request_dict = await request.json()
     split_text = model.split_text(**request_dict)
     response = {"split_text": split_text}
 
     return JSONResponse(response)
 
 
-@router.post("/metadata_text", response_model=ResponseMetadata)
+@router.post("/v1/metadata_text", response_model=functional_schema.ResponseMetadata)
 async def metadata_text(request: Request,
     request_type: Annotated[
-        RequestMetadata,
+        functional_schema.RequestMetadata,
         Body(openapi_examples=request_openapi_examples["metadata_text"])] = None):
     """Gives meta data on a text
 
     The request should be a JSON object with the following fields:
     - text: The text to parse
     - truncation_side (optional): The truncation side of the tokenizer
     - max_length (optional) : The max length before truncation
@@ -306,8 +309,44 @@
 
     request_dict = await request.json()
 
     tokens_ids = model.tokenize(request_dict['text'])
     truncated_text = model.extract_text_outside_truncation(**request_dict)
     ret = {"tokens_nb": len(tokens_ids), "truncated_text": truncated_text}
 
-    return JSONResponse(ret)
+    return JSONResponse(ret)
+
+
+@router.post("/v1/chat/completions", response_model=functional_schema.HappyvllmChatCompletionResponse)
+async def create_chat_completion(request: Annotated[vllm_protocol.ChatCompletionRequest, Body(openapi_examples=request_openapi_examples["chat_completions"])],
+                                 raw_request: Request):
+    """Open AI compatible chat completion. See https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html for more details
+    """
+    model: Model = RESOURCES.get(RESOURCE_MODEL)
+    generator = await model.openai_serving_chat.create_chat_completion(
+        request, raw_request)
+    if isinstance(generator, vllm_protocol.ErrorResponse):
+        return JSONResponse(content=generator.model_dump(),
+                            status_code=generator.code)
+    if request.stream:
+        return StreamingResponse(content=generator,
+                                 media_type="text/event-stream")
+    else:
+        return JSONResponse(content=generator.model_dump())
+
+
+@router.post("/v1/completions", response_model=functional_schema.HappyvllmCompletionResponse)
+async def create_completion(request: Annotated[vllm_protocol.CompletionRequest, Body(openapi_examples=request_openapi_examples["completions"])],
+                            raw_request: Request):
+    """Open AI compatible completion. See https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html for more details
+    """
+    model: Model = RESOURCES.get(RESOURCE_MODEL)
+    generator = await model.openai_serving_completion.create_completion(
+        request, raw_request)
+    if isinstance(generator, vllm_protocol.ErrorResponse):
+        return JSONResponse(content=generator.model_dump(),
+                            status_code=generator.code)
+    if request.stream:
+        return StreamingResponse(content=generator,
+                                 media_type="text/event-stream")
+    else:
+        return JSONResponse(content=generator.model_dump())
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/__init__.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/request.json` & `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/request.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'chat_completions'": "OrderedDict([('nominal_case', OrderedDict([('summary', 'Nominal case'), "*

 * *                       "('description', 'A nominal case'), ('value', OrderedDict([('messages', "*

 * *                       "[OrderedDict([('role', 'system'), ('content', 'You are a helpful "*

 * *                       "assistant.')]), OrderedDict([('role', 'user'), ('content', 'Who won the "*

 * *                       "world series in 2020?')]), OrderedDict([('role', 'assistant'), ('content', "*

 * *                       "'Th […]*

```diff
@@ -1,8 +1,113 @@
 {
+    "chat_completions": {
+        "nominal_case": {
+            "description": "A nominal case",
+            "summary": "Nominal case",
+            "value": {
+                "messages": [
+                    {
+                        "content": "You are a helpful assistant.",
+                        "role": "system"
+                    },
+                    {
+                        "content": "Who won the world series in 2020?",
+                        "role": "user"
+                    },
+                    {
+                        "content": "The Los Angeles Dodgers won the World Series in 2020.",
+                        "role": "assistant"
+                    },
+                    {
+                        "content": "Where was it played?",
+                        "role": "user"
+                    }
+                ],
+                "model": "my_model"
+            }
+        }
+    },
+    "completions": {
+        "Nominal case": {
+            "description": "The nominal case where we we use all default values",
+            "summary": "Nominal case",
+            "value": {
+                "model": "my_model",
+                "prompt": "This is a prompt example. Please complete it with a joke. JOKE:"
+            }
+        },
+        "choices": {
+            "description": "How to use `guided_choice`. In this example, the LLM will answer one of the three proposed responses, even if the choices are not present in the prompt",
+            "summary": "Use of guided choices",
+            "value": {
+                "guided_choice": [
+                    "mathematician",
+                    "astronaut",
+                    "show writer"
+                ],
+                "model": "my_model",
+                "prompt": "Was was the occupation of Ada Lovelace ?",
+                "temperature": 0
+            }
+        },
+        "guided_json": {
+            "description": "How to use `guided_json` with a json schema. In this example, we are not obligated to put in the prompt what json we are expecting even if it may help the LLM answer correctly. For more complex json schema, please read the corresponding documentation : https://json-schema.org/",
+            "summary": "Use of guided_json with a json schema",
+            "value": {
+                "guided_json": {
+                    "properties": {
+                        "age": {
+                            "type": "integer"
+                        },
+                        "height_in_meters": {
+                            "type": "number"
+                        },
+                        "is_alive": {
+                            "type": "boolean"
+                        },
+                        "name": {
+                            "type": "string"
+                        },
+                        "names_of_children": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        }
+                    },
+                    "required": [
+                        "name",
+                        "age",
+                        "is_alive",
+                        "height_in_meters",
+                        "names_of_children"
+                    ],
+                    "type": "object"
+                },
+                "max_tokens": 100,
+                "model": "my_model",
+                "prompt": "Describe Ada Lovelace. Your answer should be in form of a json with the keywords name, age, is_alive, height_in_meters, names_of_children.",
+                "repetition_penalty": 1,
+                "temperature": 0,
+                "top_p": 0.8
+            }
+        },
+        "simple_case": {
+            "description": "A simple case where we use some vLLM sampling parameters",
+            "summary": "Simple case",
+            "value": {
+                "max_tokens": 100,
+                "model": "my_model",
+                "prompt": "This is a prompt example. Please complete it with a joke. JOKE:",
+                "repetition_penalty": 1.1,
+                "temperature": 0.5,
+                "top_p": 0.8
+            }
+        }
+    },
     "decode": {
         "nominal_case": {
             "description": "Decode a list of token ids. It is the inverse of the endpoint tokenizer. For more details on what is the vanilla version of the tokenizer or not, please read the documentation : https://oss-pole-emploi.github.io/happy_vllm/",
             "summary": "Nominal case",
             "value": {
                 "token_ids": [
                     1,
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/functional.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/functional.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Functional schemas"""
 
 import os
 import json
-from pydantic import BaseModel, Field
 from starlette.responses import JSONResponse
+from pydantic import BaseModel, Field, conint
 from typing import Any, List, Union, Optional
+from vllm.entrypoints.openai.protocol import ResponseFormat, CompletionResponse, ChatCompletionResponse
 
 from .utils import NumpyArrayEncoder
 
 # Load the response examples
 directory = os.path.dirname(os.path.abspath(__file__))
 response_examples_path = os.path.join(directory, "examples", "response.json")
 with open(response_examples_path, "r") as file:
@@ -124,7 +125,15 @@
     }
 
 
 class RequestMetadata(BaseModel):
     text: str = Field(None, title="Input text")
     truncation_side: str = Field(None, title="Side of truncation")
     max_length: int = Field(None, title="Max length before truncation")
+
+
+class HappyvllmCompletionResponse(CompletionResponse):
+    model_config = {"json_schema_extra": {"examples": [response_examples["completion_response"]]}}
+
+
+class HappyvllmChatCompletionResponse(ChatCompletionResponse):
+    model_config = {"json_schema_extra": {"examples": [response_examples["chat_completion_response"]]}}
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/technical.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/technical.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 
 """Technical schemas"""
 import os
 import json
 from pydantic import BaseModel, Field
 
+from vllm.entrypoints.openai.protocol import ModelList
+
 # Load the response examples
 directory = os.path.dirname(os.path.abspath(__file__))
 response_examples_path = os.path.join(directory, "examples", "response.json")
 with open(response_examples_path, 'r') as file:
     response_examples = json.load(file)
 
 
@@ -81,7 +83,11 @@
             "examples": [
                 response_examples["live_metrics"]
             ]
         }
     }
 
 
+class HappyvllmModelList(ModelList):
+    model_config = {"json_schema_extra": {"examples": [response_examples["models"]]}}
+
+
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/utils.py` & `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/utils.py` & `happy_vllm-1.1.0/src/happy_vllm/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/src/happy_vllm/utils_args.py` & `happy_vllm-1.1.0/src/happy_vllm/utils_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 
 from typing import Optional
 from pydantic_settings import BaseSettings, SettingsConfigDict
 from argparse import Namespace, ArgumentParser, BooleanOptionalAction
 
 from vllm.engine.arg_utils import AsyncEngineArgs
+from vllm.entrypoints.openai.cli_args import LoRAParserAction
 
 
 DEFAULT_MODEL_NAME = '?'
 DEFAULT_APP_NAME = "happy_vllm"
 DEFAULT_API_ENDPOINT_PREFIX = ""
 DEFAULT_HOST = "127.0.0.1"
 DEFAULT_PORT = 5000
@@ -38,14 +39,17 @@
 DEFAULT_UVICORN_LOG_LEVEL = 'info'
 CHOICES_UVICORN_LOG_LEVEL = ['debug', 'info', 'warning', 'error', 'critical', 'trace']
 DEFAULT_SSL_KEYFILE = None
 DEFAULT_SSL_CERTFILE = None
 DEFAULT_SSL_CA_CERTS = None
 DEFAULT_SSL_CERT_REQS = int(ssl.CERT_NONE)
 DEFAULT_ROOT_PATH = None
+DEFAULT_LORA_MODULES = None
+DEFAULT_CHAT_TEMPLATE = None
+DEFAULT_RESPONSE_ROLE = "assistant"
 
 
 class ApplicationSettings(BaseSettings):
     """Application settings
 
     This class is used for settings management purpose, have a look at the pydantic
     documentation for more details : https://pydantic-docs.helpmanual.io/usage/settings/
@@ -66,14 +70,17 @@
     ssl_keyfile: Optional[str] = DEFAULT_SSL_KEYFILE
     ssl_certfile: Optional[str] = DEFAULT_SSL_CERTFILE
     ssl_ca_certs: Optional[str] = DEFAULT_SSL_CA_CERTS
     ssl_cert_reqs: int = DEFAULT_SSL_CERT_REQS
     root_path: Optional[str] = DEFAULT_ROOT_PATH
     app_name: str = DEFAULT_APP_NAME
     api_endpoint_prefix: str = DEFAULT_API_ENDPOINT_PREFIX
+    lora_modules: Optional[str] = DEFAULT_LORA_MODULES
+    chat_template : Optional[str] = DEFAULT_CHAT_TEMPLATE
+    response_role: str = DEFAULT_RESPONSE_ROLE
 
     model_config = SettingsConfigDict(env_file=".env", extra='ignore', protected_namespaces=('settings', ))
 
 
 def get_model_settings(parser: ArgumentParser) -> BaseSettings:
     """Gets the model settings. It corresponds to the variables added via AsyncEngineArgs.add_cli_args plus model-name.
     First we use the parser to get the default values of vLLM for these variables. We instantiate a BaseSettings model
@@ -221,16 +228,33 @@
                         type=int,
                         default=application_settings.ssl_cert_reqs,
                         help="Whether client certificate is required (see stdlib ssl module's)")
     parser.add_argument("--root-path",
                         type=str,
                         default=application_settings.root_path,
                         help="FastAPI root_path when app is behind a path based routing proxy")
+    parser.add_argument("--lora-modules",
+                        type=str,
+                        default=application_settings.lora_modules,
+                        nargs='+',
+                        action=LoRAParserAction,
+                        help="LoRA module configurations in the format name=path. "
+                        "Multiple modules can be specified.")
+    parser.add_argument("--chat-template",
+                        type=str,
+                        default=application_settings.chat_template,
+                        help="The file path to the chat template, "
+                        "or the template in single-line form "
+                        "for the specified model")
+    parser.add_argument("--response-role",
+                        type=str,
+                        default=application_settings.response_role,
+                        help="The role name to return if "
+                        "`request.add_generation_prompt=true`.")
     parser = AsyncEngineArgs.add_cli_args(parser)
-
     return parser
 
 
 def parse_args() -> Namespace:
     """Parses the args. We want this priority : args from cli > environnement variables > .env variables.
     In order to do this, we get from pydantic BaseSetting the value from environnement variables or .env variables
     with the proper priority. Then we set the default value of the cli parser to those value so that if the cli args
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm.egg-info/PKG-INFO` & `happy_vllm-1.1.0/src/happy_vllm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.0.0
+Version: 1.1.0
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vllm<1.0,>=0.4.0
 Requires-Dist: fastapi<1.0,>=0.110.1
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
@@ -52,27 +52,27 @@
 ```
 
 ## Quickstart
 
 Just use the entrypoint `happy-vllm` (see [arguments](https://oss-pole-emploi.github.io/happy_vllm/arguments/) for a list of all possible arguments)
 
 ```bash
-happy_vllm --model path_to_model --host 127.0.0.1 --port 5000
+happy_vllm --model path_to_model --host 127.0.0.1 --port 5000 --model-name my_model
 ```
 
 It will launch the API and you can directly query it for example with 
 
 ```bash
-curl 127.0.0.1:5000/info
+curl 127.0.0.1:5000/v1/info
 ```
 
 To get various information on the application or 
 
 ```bash
-curl 127.0.0.1:5000/generate -d '{"prompt": "Hey,"}'
+curl 127.0.0.1:5000/v1/completions -d '{"prompt": "Hey,", "model": "my_model"}'
 ```
 
 if you want to generate your first LLM response using happy_vLLM. See [endpoints](https://oss-pole-emploi.github.io/happy_vllm/endpoints/endpoints) for more details on all the endpoints provided by happy_vLLM. 
 
 ## Deploy with Docker image
 
 A docker image is available from the [Github Container Registry](https://github.com/OSS-Pole-Emploi/happy_vllm/pkgs/container/happy_vllm) :
```

### Comparing `happy_vllm-1.0.0/src/happy_vllm.egg-info/SOURCES.txt` & `happy_vllm-1.1.0/src/happy_vllm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/happy_vllm/logits_processors/json_format.py
 src/happy_vllm/logits_processors/response_pool.py
 src/happy_vllm/logits_processors/utils_parse_logits_processors.py
 src/happy_vllm/middlewares/__init__.py
 src/happy_vllm/middlewares/exception.py
 src/happy_vllm/model/__init__.py
 src/happy_vllm/model/model_base.py
+src/happy_vllm/model/openai_serving_chat_fixed.py
 src/happy_vllm/routers/__init__.py
 src/happy_vllm/routers/functional.py
 src/happy_vllm/routers/technical.py
 src/happy_vllm/routers/schemas/__init__.py
 src/happy_vllm/routers/schemas/functional.py
 src/happy_vllm/routers/schemas/technical.py
 src/happy_vllm/routers/schemas/utils.py
```

### Comparing `happy_vllm-1.0.0/tests/test_json_format.py` & `happy_vllm-1.1.0/tests/test_json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_model_base.py` & `happy_vllm-1.1.0/tests/test_model_base.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_response_pool.py` & `happy_vllm-1.1.0/tests/test_response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_routers_functionnal.py` & `happy_vllm-1.1.0/tests/test_routers_functionnal.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,40 +164,40 @@
     temperature = 0
     request_dict = {"temperature": temperature, "response_pool": ["Yes", "No"], "prompt": prompt_ini, "min_tokens": 10, "max_tokens": 100}
     with pytest.raises(ValueError):
         prompt, prompt_in_response, sampling_params = functional.parse_generate_parameters(request_dict, model, tokenizer, tokenizer_lmformatenforcer)
 
 
 def test_generate(test_complete_client: TestClient):
-    """Test the route generate thanks to the test_complete_client we created in conftest.py"""
+    """Test the route /v1/generate thanks to the test_complete_client we created in conftest.py"""
     model = init_model()
     tokenizer = model._tokenizer
 
     def get_response(tokenizer, prompt, i, max_tokens):
         prompt_tot = f"n={i} "*i + prompt + " This is the generated text. I find it really good don't you ?"
         token_ids = tokenizer(prompt_tot, add_special_tokens=False)['input_ids']
         token_ids = token_ids[:max_tokens]
         return tokenizer.decode(token_ids)
     
     # Nominal case
     max_tokens = 500
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens}
-    response = test_complete_client.post("/tests/generate", json=body)
+    response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
     assert response_json["responses"] == [get_response(tokenizer, prompt, 0, max_tokens)]
     assert response_json["finish_reasons"] == ["stop"]
     assert set(response_json) == {"responses", "finish_reasons"}
 
     # Several responses and prompt_in_response
     max_tokens = 500
     prompt = "Hello there"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3, "prompt_in_response": True}
-    response = test_complete_client.post("/tests/generate", json=body)
+    response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
     for i in [0, 1, 2]:
         target_response = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
@@ -208,15 +208,15 @@
     assert response_json["prompt"] == "Hello there"
     assert set(response_json) == {"responses", "finish_reasons", "prompt"}
 
     # Generations stopped
     max_tokens = 5
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3}
-    response = test_complete_client.post("/tests/generate", json=body)
+    response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
     for i in [0, 1, 2]:
         target_response = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
@@ -226,15 +226,15 @@
             assert response_json["finish_reasons"][i] == "length"
     assert set(response_json) == {"responses", "finish_reasons"}
 
     # Some Generation stopped
     max_tokens = 18
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3}
-    response = test_complete_client.post("/tests/generate", json=body)
+    response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
     for i in [0, 1, 2]:
         target_response = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
@@ -242,192 +242,192 @@
             assert response_json["finish_reasons"][i] == "stop"
         else:
             assert response_json["finish_reasons"][i] == "length"
     assert set(response_json) == {"responses", "finish_reasons"}
 
 
 def test_tokenizer(test_complete_client: TestClient):
-    """Test the functional route /tokenizer"""
+    """Test the functional route /v1/tokenizer"""
     model = init_model()
     # Vanilla
     for text in ["How do you do?", "I am Lliam. How are you ?", "Marvelous, it works !"]:
         body = {"text": text, "vanilla": True}
-        response = test_complete_client.post("/tests/tokenizer", json=body)
+        response = test_complete_client.post("/tests/v1/tokenizer", json=body)
         assert response.status_code == 200
         response_json = response.json()
         target_tokens_ids = model._tokenizer(text)['input_ids']
         assert response_json["tokens_ids"] == target_tokens_ids
         assert response_json["tokens_nb"] == len(target_tokens_ids)
         assert set(response_json) == {"tokens_ids", "tokens_nb"}
 
         # With with_tokens_str
         body = {"text": text, "with_tokens_str": True, "vanilla": True}
-        response = test_complete_client.post("/tests/tokenizer", json=body)
+        response = test_complete_client.post("/tests/v1/tokenizer", json=body)
         assert response.status_code == 200
         response_json = response.json()
         target_tokens_ids = model._tokenizer(text)['input_ids']
         assert response_json["tokens_ids"] == target_tokens_ids
         assert response_json["tokens_nb"] == len(target_tokens_ids)
         tokens_str = model._tokenizer.convert_ids_to_tokens(target_tokens_ids)
         assert response_json["tokens_str"] == tokens_str
         assert set(response_json) == {"tokens_ids", "tokens_nb", "tokens_str"}
 
     #Non Vanilla
     for text in ["How do you do?", "I am Lliam. How are you ?", "Marvelous, it works !"]:
         body = {"text": text, "vanilla": False}
-        response = test_complete_client.post("/tests/tokenizer", json=body)
+        response = test_complete_client.post("/tests/v1/tokenizer", json=body)
         assert response.status_code == 200
         response_json = response.json()
         target_tokens_ids = list(utils.proper_tokenization(model._tokenizer, text))
         assert response_json["tokens_ids"] == target_tokens_ids
         assert response_json["tokens_nb"] == len(target_tokens_ids)
         assert set(response_json) == {"tokens_ids", "tokens_nb"}
 
         # With with_tokens_str
         body = {"text": text, "with_tokens_str": True, "vanilla": False}
-        response = test_complete_client.post("/tests/tokenizer", json=body)
+        response = test_complete_client.post("/tests/v1/tokenizer", json=body)
         assert response.status_code == 200
         response_json = response.json()
         target_tokens_ids = list(utils.proper_tokenization(model._tokenizer, text))
         assert response_json["tokens_ids"] == target_tokens_ids
         assert response_json["tokens_nb"] == len(target_tokens_ids)
         tokens_str = [utils.proper_decode(model._tokenizer, token_id) for token_id in target_tokens_ids]
         assert response_json["tokens_str"] == tokens_str
         assert set(response_json) == {"tokens_ids", "tokens_nb", "tokens_str"}
 
 
 def test_decode(test_complete_client: TestClient):
-    """Test the functional route /decode"""
+    """Test the functional route /v1/decode"""
     model = init_model()
 
     # Vanilla
     for text in ["How do you do?", "I am Lliam. How are you ?", "Marvelous, it works !"]:
         token_ids = model._tokenizer(text)['input_ids']
 
         body = {'token_ids': token_ids, "vanilla": True}
-        response = test_complete_client.post("/tests/decode", json=body)
+        response = test_complete_client.post("/tests/v1/decode", json=body)
         assert response.status_code == 200
         response_json = response.json()
         assert response_json["decoded_string"] == model._tokenizer.decode(token_ids)
         assert set(response_json) == {"decoded_string"}
 
         # With with_tokens_str
         body = {'token_ids': token_ids, "vanilla": True, "with_tokens_str": True}
-        response = test_complete_client.post("/tests/decode", json=body)
+        response = test_complete_client.post("/tests/v1/decode", json=body)
         assert response.status_code == 200
         response_json = response.json()
         assert response_json["decoded_string"] == model._tokenizer.decode(token_ids)
         assert response_json["tokens_str"] == model._tokenizer.convert_ids_to_tokens(token_ids)
         assert set(response_json) == {"decoded_string", "tokens_str"}
 
     #Non Vanilla
     for text in ["How do you do?", "I am Lliam. How are you ?", "Marvelous, it works !"]:
         token_ids = model._tokenizer(text)['input_ids']
 
         body = {'token_ids': token_ids, "vanilla": False}
-        response = test_complete_client.post("/tests/decode", json=body)
+        response = test_complete_client.post("/tests/v1/decode", json=body)
         assert response.status_code == 200
         response_json = response.json()
         assert response_json["decoded_string"] == utils.proper_decode(model._tokenizer, token_ids)
         assert set(response_json) == {"decoded_string"}
 
         # With with_tokens_str
         body = {'token_ids': token_ids, "vanilla": False, "with_tokens_str": True}
-        response = test_complete_client.post("/tests/decode", json=body)
+        response = test_complete_client.post("/tests/v1/decode", json=body)
         assert response.status_code == 200
         response_json = response.json()
         assert response_json["decoded_string"] == utils.proper_decode(model._tokenizer, token_ids)
         assert response_json["tokens_str"] == [utils.proper_decode(model._tokenizer, token_id) for token_id in token_ids]
         assert set(response_json) == {"decoded_string", "tokens_str"}
 
 
 def test_split_text(test_complete_client: TestClient):
-    """Test the route split_text thanks to the test_complete_client we created in conftest.py"""
+    """Test the route /v1/split_text thanks to the test_complete_client we created in conftest.py"""
     text = "Hey, my name is LLM. How are you ? Fine, you ? That's wonderful news : I'm also fine. But do you think it will last ?"
 
     body = {"text": text,
             "num_tokens_in_chunk": 2}
-    response = test_complete_client.post("/tests/split_text", json=body)
+    response = test_complete_client.post("/tests/v1/split_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     target_split_text = ["Hey, my name is LLM.",
                         " How are you ?", 
                         " Fine, you ?",
                         " That's wonderful news : I'm also fine.",
                         " But do you think it will last ?"]
     assert json_response == {"split_text": target_split_text}
 
     body = {"text": text,
             "num_tokens_in_chunk": 6}
-    response = test_complete_client.post("/tests/split_text", json=body)
+    response = test_complete_client.post("/tests/v1/split_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     target_split_text = ["Hey, my name is LLM.",
                         " How are you ? Fine, you ?",
                         " That's wonderful news : I'm also fine.",
                         " But do you think it will last ?"]
     assert json_response == {"split_text": target_split_text}
 
     body = {"text": text,
             "num_tokens_in_chunk": 1000}
-    response = test_complete_client.post("/tests/split_text", json=body)
+    response = test_complete_client.post("/tests/v1/split_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     target_split_text = [text]
     assert json_response == {"split_text": target_split_text}
 
     body = {"text": text,
             "num_tokens_in_chunk": 2,
             "separators": [" ?"]}
-    response = test_complete_client.post("/tests/split_text", json=body)
+    response = test_complete_client.post("/tests/v1/split_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     target_split_text = target_split_text = ["Hey, my name is LLM. How are you ?",
                         " Fine, you ?",
                         " That's wonderful news : I'm also fine. But do you think it will last ?"]
     assert json_response == {"split_text": target_split_text}
 
 
 def test_metadata_text(test_complete_client: TestClient):
-    """Test the route metadata_text thanks to the test_complete_client we created in conftest.py"""
+    """Test the route /v1/metadata_text thanks to the test_complete_client we created in conftest.py"""
     text = "Hey, my name is LLM. How are you ? Fine, and you ? Great."
     model = init_model()
     tokenizer = model._tokenizer
 
     text_tot = text * 73
     truncation_side = "left"
     max_length = 1234
     body = {"text": text_tot,
             "truncation_side": truncation_side,
             "max_length": max_length}
-    response = test_complete_client.post("/tests/metadata_text", json=body)
+    response = test_complete_client.post("/tests/v1/metadata_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     truncated_text = model.extract_text_outside_truncation(text_tot, truncation_side, max_length)
     assert json_response["tokens_nb"] == len(utils.proper_tokenization(tokenizer, text_tot))
     assert json_response["truncated_text"] == truncated_text
 
     text_tot = text * 73
     truncation_side = "right"
     max_length = 1234
     body = {"text": text_tot,
             "truncation_side": truncation_side,
             "max_length":1234}
-    response = test_complete_client.post("/tests/metadata_text", json=body)
+    response = test_complete_client.post("/tests/v1/metadata_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     truncated_text = model.extract_text_outside_truncation(text_tot, truncation_side, max_length)
     assert json_response["tokens_nb"] == len(utils.proper_tokenization(tokenizer, text_tot))
     assert json_response["truncated_text"] == truncated_text
 
     text_tot = text
     truncation_side = "left"
     max_length = 1234
     body = {"text": text,
             "truncation_side": "left",
             "max_length":1234}
-    response = test_complete_client.post("/tests/metadata_text", json=body)
+    response = test_complete_client.post("/tests/v1/metadata_text", json=body)
     assert response.status_code == 200
     json_response = response.json()
     truncated_text = model.extract_text_outside_truncation(text_tot, truncation_side, max_length)
     assert json_response["tokens_nb"] == len(utils.proper_tokenization(tokenizer, text_tot))
     assert json_response["truncated_text"] == truncated_text
```

### Comparing `happy_vllm-1.0.0/tests/test_routers_technical.py` & `happy_vllm-1.1.0/tests/test_routers_technical.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     """Test the technical route /readiness when the model is fully loaded"""
     response = test_complete_client.get("/tests/readiness")
     assert response.status_code == 200
     assert response.json() == {"ready": "ok"}
 
 
 def test_info(test_complete_client: TestClient):
-    """Test the technical route /info"""
-    response = test_complete_client.get("/tests/info")
+    """Test the technical route /v1/info"""
+    response = test_complete_client.get("/tests/v1/info")
     assert response.status_code == 200
     response_json = response.json()
     assert response_json["application"] == "APP_TESTS"
     assert response_json["version"] == utils.get_package_version()
     assert response_json["model_name"] == "TEST MODEL"
     assert response_json["truncation_side"] == "right"
     assert response_json["max_length"] == 2048
```

### Comparing `happy_vllm-1.0.0/tests/test_schemas_utils.py` & `happy_vllm-1.1.0/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_utils.py` & `happy_vllm-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_utils_args.py` & `happy_vllm-1.1.0/tests/test_utils_args.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.0.0/tests/test_utils_parse_logits_processors.py` & `happy_vllm-1.1.0/tests/test_utils_parse_logits_processors.py`

 * *Files identical despite different names*

