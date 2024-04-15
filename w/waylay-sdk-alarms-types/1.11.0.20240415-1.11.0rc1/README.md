# Comparing `tmp/waylay_sdk_alarms_types-1.11.0.20240415.tar.gz` & `tmp/waylay-sdk-alarms-types-1.11.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_alarms_types-1.11.0.20240415.tar", last modified: Mon Apr 15 08:23:28 2024, max compression
+gzip compressed data, was "waylay-sdk-alarms-types-1.11.0rc1.tar", last modified: Wed Mar 27 16:12:59 2024, max compression
```

## Comparing `waylay_sdk_alarms_types-1.11.0.20240415.tar` & `waylay-sdk-alarms-types-1.11.0rc1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.782854 waylay_sdk_alarms_types-1.11.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-15 08:23:28.782854 waylay_sdk_alarms_types-1.11.0.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:23:28.782854 waylay_sdk_alarms_types-1.11.0.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.766854 waylay_sdk_alarms_types-1.11.0.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.766854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.766854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.766854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.778854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/a_batch_alarms_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_audit_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_changes_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type_one_of2.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_severity_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_source_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_status_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_timeline_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_type_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarms_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarms_timeline_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_alarm_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_delete_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_delete_alarm_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_enqueued.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_operation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_update_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_update_alarm_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/bulk_query_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/bulk_query_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/create_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/error_response_with_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/failure_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/id_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/list_order_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/list_sort_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/nd_json_response_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/operation_result_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/operation_result_object_results.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/queued_operation_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/queued_operation_summary_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/ss_event_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/success_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.778854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarm_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarms_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:15.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:23:28.778854 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-15 08:23:28.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-15 08:23:28.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:23:28.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-15 08:23:28.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:23:28.000000 waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.797406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/a_batch_alarms_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_audit_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_source_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_timeline_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_type_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_timeline_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/create_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/failure_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/id_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_order_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_sort_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/nd_json_response_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/ss_event_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/success_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.797406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarm_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/LICENSE.txt` & `waylay-sdk-alarms-types-1.11.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/PKG-INFO` & `waylay-sdk-alarms-types-1.11.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms-types
-Version: 1.11.0.20240415
+Version: 1.11.0rc1
 Summary: Waylay Alarms Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-alarms==1.11.0.20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,54 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/README.md` & `waylay-sdk-alarms-types-1.11.0rc1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/pyproject.toml` & `waylay-sdk-alarms-types-1.11.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-alarms-types"
-version = "1.11.0.20240415"
+version = "1.11.0rc1"
 description = "Waylay Alarms Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Alarms" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
-    "waylay-sdk-alarms == 1.11.0.20240415",
+    "waylay-sdk ~= 0.0.4rc5",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-alarms-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/alarms.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/__init__.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "1.11.0.20240415"
+__version__ = "1.11.0rc1"
 
 # import models into model package
 from .a_batch_alarms_specification import ABatchAlarmsSpecification
 from .alarm_audit_record import AlarmAuditRecord
 from .alarm_entity import AlarmEntity
 from .alarm_event import AlarmEvent
 from .alarm_event_alarm import AlarmEventAlarm
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/a_batch_alarms_specification.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/a_batch_alarms_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_audit_record.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_audit_record.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_entity.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_alarm.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_changes_inner.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_event_type_one_of1.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_severity_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_status_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_timeline_info.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_timeline_info.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarm_update.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_update.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarms_query_result.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_query_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/alarms_timeline_item.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_timeline_item.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_delete_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_enqueued.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_operation.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_result.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_operation_results.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_results.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/batch_update_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/bulk_query_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/bulk_query_ids.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_ids.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event_data.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/create_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/create_alarm.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/error_response.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/error_response_with_details.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response_with_details.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/failure_operation_result_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/failure_operation_result_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/id_object.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/id_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/list_sort_parameter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_sort_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/nd_json_response_stream.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/nd_json_response_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/operation_result_object.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/operation_result_object_results.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object_results.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/queued_operation_summary.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/ss_event_stream.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/ss_event_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/success_operation_result_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/success_operation_result_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/models/version_response.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/version_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/about_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/version_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarm_events_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarm_events_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarms_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay/services/alarms/queries/alarms_batch_operations_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_batch_operations_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/PKG-INFO` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms-types
-Version: 1.11.0.20240415
+Version: 1.11.0rc1
 Summary: Waylay Alarms Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-alarms==1.11.0.20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,54 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240415/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 src/waylay/services/alarms/models/queued_operation_summary.py
 src/waylay/services/alarms/models/queued_operation_summary_action.py
 src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
 src/waylay/services/alarms/models/ss_event_stream.py
 src/waylay/services/alarms/models/success_operation_result_value.py
 src/waylay/services/alarms/models/version_response.py
 src/waylay/services/alarms/queries/__init__.py
-src/waylay/services/alarms/queries/about_api.py
 src/waylay/services/alarms/queries/alarm_events_api.py
 src/waylay/services/alarms/queries/alarms_api.py
 src/waylay/services/alarms/queries/alarms_batch_operations_api.py
 src/waylay/services/alarms/queries/py.typed
+src/waylay/services/alarms/queries/version_api.py
 src/waylay_sdk_alarms_types.egg-info/PKG-INFO
 src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
 src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
 src/waylay_sdk_alarms_types.egg-info/requires.txt
 src/waylay_sdk_alarms_types.egg-info/top_level.txt
```

