# Comparing `tmp/dcicutils-8.8.3.1b5.tar.gz` & `tmp/dcicutils-8.8.3.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.3.1b5.tar", max compression
+gzip compressed data, was "dcicutils-8.8.3.1b7.tar", max compression
```

## Comparing `dcicutils-8.8.3.1b5.tar` & `dcicutils-8.8.3.1b7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/README.rst
--rw-r--r--   0        0        0        0 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3108 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-13 19:51:24.789954 dcicutils-8.8.3.1b5/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/log_utils.py
--rw-r--r--   0        0        0   103041 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30480 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    15988 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-13 19:51:24.793954 dcicutils-8.8.3.1b5/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58450 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-13 19:51:24.797954 dcicutils-8.8.3.1b5/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-15 02:58:46.708385 dcicutils-8.8.3.1b7/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-15 02:58:46.708385 dcicutils-8.8.3.1b7/README.rst
+-rw-r--r--   0        0        0        0 2024-04-15 02:58:46.708385 dcicutils-8.8.3.1b7/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-15 02:58:46.708385 dcicutils-8.8.3.1b7/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-15 02:58:46.708385 dcicutils-8.8.3.1b7/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3108 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   103041 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-15 02:58:46.712385 dcicutils-8.8.3.1b7/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30480 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    16569 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58450 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-15 02:58:46.716385 dcicutils-8.8.3.1b7/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b7/PKG-INFO
```

### Comparing `dcicutils-8.8.3.1b5/LICENSE.txt` & `dcicutils-8.8.3.1b7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/README.rst` & `dcicutils-8.8.3.1b7/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/base.py` & `dcicutils-8.8.3.1b7/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/bundle_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/captured_output.py` & `dcicutils-8.8.3.1b7/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/codebuild_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/command_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/common.py` & `dcicutils-8.8.3.1b7/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/contribution_scripts.py` & `dcicutils-8.8.3.1b7/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/contribution_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/creds_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/data_readers.py` & `dcicutils-8.8.3.1b7/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/data_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/datetime_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/deployment_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/diff_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/docker_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ecr_scripts.py` & `dcicutils-8.8.3.1b7/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ecr_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ecs_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/env_base.py` & `dcicutils-8.8.3.1b7/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/env_manager.py` & `dcicutils-8.8.3.1b7/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/env_scripts.py` & `dcicutils-8.8.3.1b7/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/env_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.3.1b7/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/es_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/exceptions.py` & `dcicutils-8.8.3.1b7/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ff_mocks.py` & `dcicutils-8.8.3.1b7/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ff_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/file_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.3.1b7/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/glacier_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/jh_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.3.1b7/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/kibana/readme.md` & `dcicutils-8.8.3.1b7/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/lang_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.3.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/license_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/log_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/misc_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/opensearch_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/portal_object_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/portal_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/progress_bar.py` & `dcicutils-8.8.3.1b7/dcicutils/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,16 @@
                  interrupt_exit_message: Optional[Union[Callable, str]] = None,
                  interrupt_message: Optional[str] = None,
                  tidy_output_hack: bool = True,
                  capture_output_for_testing: bool = False) -> None:
         self._bar = None
         self._disabled = False
         self._done = False
+        self._really_done = False
+        self.foo = time.time()
         self._tidy_output_hack = (tidy_output_hack is True)
         self._started = time.time()
         self._stop_requested = False
         # Interrupt handling. We do not do the actual (signal) interrupt setup
         # in self._initialize as that could be called from a (sub) thread; and in
         # Python we can only set a signal (SIGINT in our case) on the main thread.
         self._catch_interrupt = (catch_interrupt is True)
@@ -100,62 +102,62 @@
             self._bar = TQDM(total=self._total, desc=self._description,
                              dynamic_ncols=True, bar_format=bar_format, unit="", file=sys.stdout)
             if self._disabled:
                 self._bar.disable = True
             return True
         return False
 
-    def set_total(self, value: int, reset_eta: bool = False) -> None:
+    def set_total(self, value: int) -> None:
         if value == self._total:
             # If the total has not changed since last set then do nothing.
-            if reset_eta and self._bar is not None:
-                self._bar.reset()
             return
         if isinstance(value, int) and value > 0:
             self._total = value
             if self._bar is not None:
                 # This reset is needed to get the ETA to reset properly when we reset
                 # the total during the course of a single ProgressBar instance.
                 self._bar.reset()
                 self._bar.total = value
                 self._bar.refresh()
 
-    def reset_eta(self) -> None:
-        # Since set_total does nothing if total is the same, provide
-        # a way to reset the ETA if starting over with the same total.
-        if self._bar is not None:
-            progress = self._bar.n
-            self._bar.reset()
-            self._bar.total = self._total
-            self._bar.n = progress
-            self._bar.refresh()
-
     def set_progress(self, value: int) -> None:
         if isinstance(value, int) and value >= 0:
             if (self._bar is not None) or self._initialize():
                 self._bar.n = value
                 self._bar.refresh()
 
     def increment_progress(self, value: int) -> None:
         if isinstance(value, int) and value > 0:
             if (self._bar is not None) or self._initialize():
                 self._bar.update(value)
                 self._bar.refresh()
 
-    def set_description(self, value: str) -> None:
-        self._description = self._format_description(value)
+    def reset_eta(self) -> None:
+        # Since set_total does nothing if total is the same, provide
+        # a way to reset the ETA if starting over with the same total.
+        # But NOTE that resetting ETA will ALSO reset the ELAPSED time.
         if self._bar is not None:
-            self._bar.set_description(self._description)
+            progress = self._bar.n
+            self._bar.reset()
+            self._bar.total = self._total
+            self._bar.n = progress
+            self._bar.refresh()
+
+    def set_description(self, value: str) -> None:
+        if isinstance(value, str):
+            self._description = self._format_description(value)
+            if self._bar is not None:
+                self._bar.set_description(self._description)
 
-    def done(self) -> None:
+    def done(self, description: Optional[str] = None) -> None:
         if self._done or self._bar is None:
             return
         self._ended = time.time()
         self.set_progress(self.total)
-        self._bar.set_description(self._description)
+        self.set_description(description)
         self._bar.refresh()
         # FYI: Do NOT do a bar.disable = True before a bar.close() or it messes up output
         # on multiple calls; found out the hard way; a couple hours will never get back :-/
         self._bar.close()
         if self._tidy_output_hack:
             self._tidy_output_hack.restore()
         if self._interrupt_handler:
@@ -198,14 +200,20 @@
     def duration(self) -> None:
         return time.time() - self._started
 
     @property
     def captured_output_for_testing(self) -> Optional[List[str]]:
         return self._captured_output_for_testing
 
+    @staticmethod
+    def format_captured_output_for_testing(description: str, total: int, progress: int) -> str:
+        percent = round((progress / total) * 100.0)
+        separator = "✓" if percent == 100 else "|"
+        return f"{description} {separator} {percent:>3}% ◀|### | {progress}/{total} | 0.0/s | 00:00 | ETA: 00:00"
+
     def _format_description(self, value: str) -> str:
         if not isinstance(value, str):
             value = ""
         if self._tidy_output_hack and not value.endswith(self._tidy_output_hack.sentinel):
             value += self._tidy_output_hack.sentinel
         return value
 
@@ -257,30 +265,27 @@
     def _define_tidy_output_hack(self) -> None:
         # Some minor tqdm output tidying-up which for annoying anomalies; tqdm forces
         # a colon (:) before the percentage, e.g. ":  25%|"; and while we're at it do
         # a little ASCII progress animation, requiring a special ([progress]) sentinal
         # string in the display string where the progress bar should actually go,
         # which we do in _format_description. Other minor things too; see below.
         sys_stdout_write = sys.stdout.write
-        last_total = None ; last_progress = None ; last_text = None  # noqa
+        last_text = None ; last_captured_output_text = None  # noqa
         def tidy_stdout_write(text: str) -> None:  # noqa
             nonlocal self, sys_stdout_write, sentinel_internal, spina, spini, spinn
-            nonlocal last_total, last_progress, last_text
+            nonlocal last_text, last_captured_output_text
             def replace_first(value: str, match: str, replacement: str) -> str:  # noqa
                 return value[:i] + replacement + value[i + len(match):] if (i := value.find(match)) >= 0 else value
             def remove_extra_trailing_spaces(text: str) -> str:  # noqa
                 while text.endswith("  "):
                     text = text[:-1]
                 return text
-            if not text:
+            if (not text) or (last_text == text) or self._really_done:
                 return
-            if self._bar:
-                if ((self._bar.total == last_total) and (self._bar.n == last_progress) and (last_text == text)):
-                    return
-                last_total = self._bar.total ; last_progress = self._bar.n ; last_text = text  # noqa
+            last_text = text
             if (self._disabled or self._done) and sentinel_internal in text:
                 # Another hack to really disable output on interrupt; in this case we set
                 # tqdm.disable to True, but output can still dribble out, so if the output
                 # looks like it is from tqdm and we are disabled/done then do no output.
                 return
             if sentinel_internal in text:
                 spinc = spina[spini % spinn] if not ("100%|" in text) else "✓" ; spini += 1  # noqa
@@ -289,33 +294,40 @@
                 text = remove_extra_trailing_spaces(text)
                 # Another oddity: for the rate sometimes tqdm intermittently prints
                 # something like "1.54s/" rather than "1.54/s"; something to do with
                 # the unit we gave, which is empty; idunno; just replace it here.
                 text = replace_first(text, "s/ ", "/s ")
             sys_stdout_write(text)
             sys.stdout.flush()
+            if self._done:
+                self._really_done = True
+                return
             if self._captured_output_for_testing is not None:
                 # For testing only we replace vacilliting values in the out like rate,
                 # time elapsed, and ETA with static values; so that something like this:
                 # > Working /  20% ◀|█████████▌  | 1/5 | 536.00/s | 00:01 | ETA: 00:02
                 # becomes something more static like this after calling this function:
                 # > Working |  20% ◀|### | 1/5 | 0.0/s | 00:00 | ETA: 00:00
                 # This function obviously has intimate knowledge of the output; better here than in tests.
-                def replace_vacillating_values_with_static(text: str) -> str:
+                def replace_time_dependent_values_with_static(text: str) -> str:
                     blocks = "\u2587|\u2588|\u2589|\u258a|\u258b|\u258c|\u258d|\u258e|\u258f"
                     if (n := find_nth_from_end(text, "|", 5)) >= 8:
                         pattern = re.compile(
                             rf"(\s*)(\d*%? ◀\|)(?:\s*{blocks}|#)*\s*(\|\s*\d+/\d+)?(\s*\|\s*)"
                             rf"(?:\d+\.?\d*|\?)(\/s\s*\|\s*)(?:\d+:\d+)?(\s*\|\s*ETA:\s*)(?:\d+:\d+|\?)?")
                         if match := pattern.match(text[n - 6:]):
                             if text[n - 8:n - 7] != "✓": text = set_nth(text, n - 8, "|")  # noqa
                             return (text[0:n - 6].replace("\r", "") +
                                     match.expand(rf"\g<1>\g<2>### \g<3>\g<4>0.0\g<5>00:00\g<6>00:00"))
                     return text
-                self._captured_output_for_testing.append(replace_vacillating_values_with_static(text))
+                if text != "\n":
+                    captured_output_text = replace_time_dependent_values_with_static(text)
+                    if captured_output_text != last_captured_output_text:
+                        self._captured_output_for_testing.append(captured_output_text)
+                        last_captured_output_text = captured_output_text
         def restore_stdout_write() -> None:  # noqa
             nonlocal sys_stdout_write
             if sys_stdout_write is not None:
                 sys.stdout.write = sys_stdout_write
         sys.stdout.write = tidy_stdout_write
         spina = ["|", "/", "—", "◦", "\\"] ; spini = 0 ; spinn = len(spina)  # noqa
         sentinel = "[progress]" ; sentinel_internal = f"{sentinel}:"  # noqa
```

### Comparing `dcicutils-8.8.3.1b5/dcicutils/project_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/qa_checkers.py` & `dcicutils-8.8.3.1b7/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/qa_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/redis_tools.py` & `dcicutils-8.8.3.1b7/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/redis_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/s3_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/schema_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.3.1b7/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.3.1b7/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.3.1b7/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/secrets_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/sheet_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/snapshot_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/structured_data.py` & `dcicutils-8.8.3.1b7/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.3.1b7/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.3.1b7/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/task_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/trace_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/validation_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/variant_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/dcicutils/zip_utils.py` & `dcicutils-8.8.3.1b7/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b5/pyproject.toml` & `dcicutils-8.8.3.1b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.3.1b5"  # TODO: To become 8.8.4
+version = "8.8.3.1b7"  # TODO: To become 8.8.4
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.3.1b5/PKG-INFO` & `dcicutils-8.8.3.1b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.3.1b5
+Version: 8.8.3.1b7
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

