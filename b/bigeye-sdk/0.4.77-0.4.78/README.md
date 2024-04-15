# Comparing `tmp/bigeye_sdk-0.4.77.tar.gz` & `tmp/bigeye_sdk-0.4.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.77.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.78.tar", max compression
```

## Comparing `bigeye_sdk-0.4.77.tar` & `bigeye_sdk-0.4.78.tar`

### file list

```diff
@@ -1,69 +1,75 @@
--rw-r--r--   0        0        0     2092 2024-03-26 20:10:15.103396 bigeye_sdk-0.4.77/LICENSE
--rw-r--r--   0        0        0      873 2024-03-26 20:10:15.103476 bigeye_sdk-0.4.77/README.md
--rw-r--r--   0        0        0     3727 2024-03-26 20:10:15.103593 bigeye_sdk-0.4.77/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 20:10:15.103676 bigeye_sdk-0.4.77/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.103753 bigeye_sdk-0.4.77/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    20437 2024-04-11 16:32:04.911659 bigeye_sdk-0.4.77/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0    12403 2024-03-26 20:10:15.103988 bigeye_sdk-0.4.77/bigeye_sdk/authentication/config.py
--rw-r--r--   0        0        0     1182 2024-03-26 20:10:15.104056 bigeye_sdk-0.4.77/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2024-03-26 20:10:15.104126 bigeye_sdk-0.4.77/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104202 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10366 2024-03-26 20:10:15.104359 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2024-03-26 20:10:15.104508 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2024-03-26 20:10:15.104585 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      736 2024-03-26 20:10:15.104656 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9363 2024-03-26 20:10:15.104804 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3900 2024-03-26 20:10:15.104890 bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104964 bigeye_sdk-0.4.77/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2024-03-26 20:10:15.105053 bigeye_sdk-0.4.77/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2024-03-26 20:10:15.105125 bigeye_sdk-0.4.77/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105194 bigeye_sdk-0.4.77/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 20:10:15.105276 bigeye_sdk-0.4.77/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39844 2024-04-11 16:32:04.913155 bigeye_sdk-0.4.77/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2024-03-26 20:10:15.105478 bigeye_sdk-0.4.77/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    52140 2024-03-28 11:45:06.797716 bigeye_sdk-0.4.77/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105719 bigeye_sdk-0.4.77/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-26 20:10:15.105839 bigeye_sdk-0.4.77/bigeye_sdk/controller/delta_controller.py
--rw-r--r--   0        0        0    15116 2024-03-28 11:45:06.797906 bigeye_sdk-0.4.77/bigeye_sdk/controller/lineage_controller.py
--rw-r--r--   0        0        0     3209 2024-03-26 20:10:15.106039 bigeye_sdk-0.4.77/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    38904 2024-04-12 15:53:26.266034 bigeye_sdk-0.4.77/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106304 bigeye_sdk-0.4.77/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2024-03-26 20:10:15.106404 bigeye_sdk-0.4.77/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2024-03-26 20:10:15.106520 bigeye_sdk-0.4.77/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1582 2024-03-26 20:10:15.106598 bigeye_sdk-0.4.77/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106671 bigeye_sdk-0.4.77/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2024-03-26 20:10:15.106799 bigeye_sdk-0.4.77/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2024-03-26 20:10:15.106912 bigeye_sdk-0.4.77/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     2450 2024-03-26 20:10:15.106994 bigeye_sdk-0.4.77/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2024-03-26 20:10:15.107087 bigeye_sdk-0.4.77/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2024-03-26 20:10:15.107178 bigeye_sdk-0.4.77/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0      370 2024-03-26 20:10:15.107269 bigeye_sdk-0.4.77/bigeye_sdk/functions/dbt.py
--rw-r--r--   0        0        0     4580 2024-03-26 20:10:15.107401 bigeye_sdk-0.4.77/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2814 2024-03-26 20:10:15.107482 bigeye_sdk-0.4.77/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      706 2024-03-26 20:10:15.107556 bigeye_sdk-0.4.77/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0      410 2024-03-26 20:10:15.107645 bigeye_sdk-0.4.77/bigeye_sdk/functions/issue_functions.py
--rw-r--r--   0        0        0    21897 2024-03-26 20:10:15.107751 bigeye_sdk-0.4.77/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2701 2024-03-26 20:10:15.107850 bigeye_sdk-0.4.77/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2024-03-26 20:10:15.107923 bigeye_sdk-0.4.77/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2024-03-26 20:10:15.107998 bigeye_sdk-0.4.77/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5350 2024-04-12 16:47:06.829137 bigeye_sdk-0.4.77/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2024-03-26 20:10:15.108209 bigeye_sdk-0.4.77/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2024-03-26 20:10:15.108284 bigeye_sdk-0.4.77/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2024-04-12 17:58:15.559015 bigeye_sdk-0.4.77/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0      993 2024-03-26 20:10:15.109440 bigeye_sdk-0.4.77/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2024-03-26 20:10:15.109559 bigeye_sdk-0.4.77/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      492 2024-03-26 20:10:15.109643 bigeye_sdk-0.4.77/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    37552 2024-03-26 20:10:15.109766 bigeye_sdk-0.4.77/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2024-03-26 20:10:15.109855 bigeye_sdk-0.4.77/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0      872 2024-03-26 20:10:15.109935 bigeye_sdk-0.4.77/bigeye_sdk/model/dbt_manifest.py
--rw-r--r--   0        0        0     4518 2024-03-26 20:10:15.110060 bigeye_sdk-0.4.77/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     5521 2024-03-26 20:10:15.110183 bigeye_sdk-0.4.77/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0       89 2024-03-26 20:10:15.110260 bigeye_sdk-0.4.77/bigeye_sdk/model/enums.py
--rw-r--r--   0        0        0     9459 2024-03-26 20:10:15.110414 bigeye_sdk-0.4.77/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     9611 2024-03-26 20:10:15.110560 bigeye_sdk-0.4.77/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      221 2024-03-26 20:10:15.110628 bigeye_sdk-0.4.77/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    56945 2024-03-26 20:10:15.110758 bigeye_sdk-0.4.77/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2024-03-26 20:10:15.110847 bigeye_sdk-0.4.77/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7599 2024-03-26 20:10:15.110966 bigeye_sdk-0.4.77/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3373 2024-04-12 17:57:49.568722 bigeye_sdk-0.4.77/pyproject.toml
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.77/PKG-INFO
+-rw-r--r--   0        0        0     2092 2024-03-26 20:10:15.103396 bigeye_sdk-0.4.78/LICENSE
+-rw-r--r--   0        0        0      873 2024-03-26 20:10:15.103476 bigeye_sdk-0.4.78/README.md
+-rw-r--r--   0        0        0     3727 2024-03-26 20:10:15.103593 bigeye_sdk-0.4.78/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 20:10:15.103676 bigeye_sdk-0.4.78/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.103753 bigeye_sdk-0.4.78/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    20437 2024-04-11 16:32:04.911659 bigeye_sdk-0.4.78/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0    12403 2024-04-15 10:41:37.041949 bigeye_sdk-0.4.78/bigeye_sdk/authentication/config.py
+-rw-r--r--   0        0        0     1182 2024-03-26 20:10:15.104056 bigeye_sdk-0.4.78/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2024-03-26 20:10:15.104126 bigeye_sdk-0.4.78/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104202 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10366 2024-03-26 20:10:15.104359 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2024-03-26 20:10:15.104508 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2024-03-26 20:10:15.104585 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      736 2024-03-26 20:10:15.104656 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9363 2024-03-26 20:10:15.104804 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3900 2024-03-26 20:10:15.104890 bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104964 bigeye_sdk-0.4.78/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2024-03-26 20:10:15.105053 bigeye_sdk-0.4.78/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2024-03-26 20:10:15.105125 bigeye_sdk-0.4.78/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105194 bigeye_sdk-0.4.78/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 20:10:15.105276 bigeye_sdk-0.4.78/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39844 2024-04-11 16:32:04.913155 bigeye_sdk-0.4.78/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2024-03-26 20:10:15.105478 bigeye_sdk-0.4.78/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    52140 2024-03-28 11:45:06.797716 bigeye_sdk-0.4.78/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105719 bigeye_sdk-0.4.78/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0     2666 2024-03-26 20:10:15.105839 bigeye_sdk-0.4.78/bigeye_sdk/controller/delta_controller.py
+-rw-r--r--   0        0        0    15116 2024-03-28 11:45:06.797906 bigeye_sdk-0.4.78/bigeye_sdk/controller/lineage_controller.py
+-rw-r--r--   0        0        0     3209 2024-03-26 20:10:15.106039 bigeye_sdk-0.4.78/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    38904 2024-04-12 15:53:26.266034 bigeye_sdk-0.4.78/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106304 bigeye_sdk-0.4.78/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2024-03-26 20:10:15.106404 bigeye_sdk-0.4.78/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2024-03-26 20:10:15.106520 bigeye_sdk-0.4.78/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1582 2024-03-26 20:10:15.106598 bigeye_sdk-0.4.78/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106671 bigeye_sdk-0.4.78/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2024-03-26 20:10:15.106799 bigeye_sdk-0.4.78/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2024-03-26 20:10:15.106912 bigeye_sdk-0.4.78/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     2450 2024-03-26 20:10:15.106994 bigeye_sdk-0.4.78/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2024-03-26 20:10:15.107087 bigeye_sdk-0.4.78/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2024-03-26 20:10:15.107178 bigeye_sdk-0.4.78/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0      370 2024-03-26 20:10:15.107269 bigeye_sdk-0.4.78/bigeye_sdk/functions/dbt.py
+-rw-r--r--   0        0        0     4580 2024-03-26 20:10:15.107401 bigeye_sdk-0.4.78/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2814 2024-03-26 20:10:15.107482 bigeye_sdk-0.4.78/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      706 2024-03-26 20:10:15.107556 bigeye_sdk-0.4.78/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0      410 2024-03-26 20:10:15.107645 bigeye_sdk-0.4.78/bigeye_sdk/functions/issue_functions.py
+-rw-r--r--   0        0        0    21897 2024-03-26 20:10:15.107751 bigeye_sdk-0.4.78/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2701 2024-03-26 20:10:15.107850 bigeye_sdk-0.4.78/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2024-03-26 20:10:15.107923 bigeye_sdk-0.4.78/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2024-03-26 20:10:15.107998 bigeye_sdk-0.4.78/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5350 2024-04-12 19:18:05.455153 bigeye_sdk-0.4.78/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2024-03-26 20:10:15.108209 bigeye_sdk-0.4.78/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2024-03-26 20:10:15.108284 bigeye_sdk-0.4.78/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:56:01.558988 bigeye_sdk-0.4.78/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:56:01.559111 bigeye_sdk-0.4.78/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:56:01.559213 bigeye_sdk-0.4.78/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:56:01.559298 bigeye_sdk-0.4.78/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   280404 2024-04-15 10:56:01.559414 bigeye_sdk-0.4.78/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:56:01.559585 bigeye_sdk-0.4.78/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2024-04-15 10:56:01.559744 bigeye_sdk-0.4.78/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      993 2024-03-26 20:10:15.109440 bigeye_sdk-0.4.78/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2024-03-26 20:10:15.109559 bigeye_sdk-0.4.78/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      492 2024-03-26 20:10:15.109643 bigeye_sdk-0.4.78/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    37552 2024-03-26 20:10:15.109766 bigeye_sdk-0.4.78/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2024-03-26 20:10:15.109855 bigeye_sdk-0.4.78/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0      872 2024-03-26 20:10:15.109935 bigeye_sdk-0.4.78/bigeye_sdk/model/dbt_manifest.py
+-rw-r--r--   0        0        0     4518 2024-03-26 20:10:15.110060 bigeye_sdk-0.4.78/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     5521 2024-03-26 20:10:15.110183 bigeye_sdk-0.4.78/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0       89 2024-03-26 20:10:15.110260 bigeye_sdk-0.4.78/bigeye_sdk/model/enums.py
+-rw-r--r--   0        0        0     9459 2024-03-26 20:10:15.110414 bigeye_sdk-0.4.78/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     9611 2024-03-26 20:10:15.110560 bigeye_sdk-0.4.78/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      221 2024-03-26 20:10:15.110628 bigeye_sdk-0.4.78/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    56945 2024-03-26 20:10:15.110758 bigeye_sdk-0.4.78/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2024-03-26 20:10:15.110847 bigeye_sdk-0.4.78/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7599 2024-03-26 20:10:15.110966 bigeye_sdk-0.4.78/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3373 2024-04-15 10:49:26.130197 bigeye_sdk-0.4.78/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.78/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.77/LICENSE` & `bigeye_sdk-0.4.78/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/README.md` & `bigeye_sdk-0.4.78/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.78/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.78/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/authentication/config.py` & `bigeye_sdk-0.4.78/bigeye_sdk/authentication/config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.78/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.78/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.78/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.78/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.78/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/controller/delta_controller.py` & `bigeye_sdk-0.4.78/bigeye_sdk/controller/delta_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/controller/lineage_controller.py` & `bigeye_sdk-0.4.78/bigeye_sdk/controller/lineage_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/controller/metric_controller.py` & `bigeye_sdk-0.4.78/bigeye_sdk/controller/metric_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.78/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/helpers.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.78/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/log/__init__.py` & `bigeye_sdk-0.4.78/bigeye_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/dbt_manifest.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/dbt_manifest.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.78/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.78/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.77/pyproject.toml` & `bigeye_sdk-0.4.78/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.77"
+version = "0.4.78"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.77/PKG-INFO` & `bigeye_sdk-0.4.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.77
+Version: 0.4.78
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

