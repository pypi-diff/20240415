# Comparing `tmp/uge-pycl-8.8.1.tar.gz` & `tmp/uge-pycl-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uge-pycl-8.8.1.tar", last modified: Mon Sep 25 08:10:46 2023, max compression
+gzip compressed data, was "dist/uge-pycl-8.9.0.tar", last modified: Sun Apr 14 10:19:37 2024, max compression
```

## Comparing `uge-pycl-8.8.1.tar` & `uge-pycl-8.9.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2758 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/README.md
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      476 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test_values.json
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/exceptions/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1502 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/qmaster_unreachable.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1504 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/object_already_exists.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2389 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/command_failed.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3227 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/ar_exception.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1490 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/invalid_argument.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/configuration_error.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/authorization_error.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1486 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/invalid_request.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3169 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/qconf_exception.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1450 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1489 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/exceptions/object_not_found.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/utility/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4924 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/utility/uge_subprocess.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/utility/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/api/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11073 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/ar_api.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)   165937 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/qconf_api.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      912 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/api/impl/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4103 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/share_tree_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1665 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/operator_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2200 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/job_class_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2164 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/calendar_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1860 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/admin_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1915 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/ar_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1810 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/submit_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4110 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/list_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3448 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/complex_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5375 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/qrdel_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2146 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/user_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6500 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/dict_list_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1996 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/cluster_queue_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2644 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/execution_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4514 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/access_list_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1663 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/manager_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7286 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/qconf_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    13007 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/dict_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2202 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/host_group_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1923 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/resource_quota_set_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6267 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/qrstat_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2212 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/scheduler_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2016 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/parallel_environment_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2028 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/checkpointing_environment_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2166 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/project_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3017 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/cluster_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5443 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/api/impl/qrsub_executor.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/constants/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1084 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/constants/uge_status.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/constants/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/log/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3585 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/logger_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1666 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/trace_log_record.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12739 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/log_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2498 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/trace_logger.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1581 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/stream_log_handler.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1780 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/log/timed_rotating_file_log_handler.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/cli/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2806 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/cli/qconf_convert.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7353 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/cli/qconf_cli.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/cli/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/objects/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2418 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/user_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5306 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/qconf_dict_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    17367 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/complex_configuration_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4201 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/resource_quota_set_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5107 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/ar_object_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6306 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/cluster_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2711 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/qconf_name_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3077 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/share_tree_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2766 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/checkpointing_environment_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2629 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/advance_reservation_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2970 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/execution_host_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2500 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/host_group_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2841 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/parallel_environment_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2416 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/calendar_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4403 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/scheduler_configuration_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4173 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/job_class_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    16092 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/complex_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2557 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/access_list_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4271 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/job_class_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4205 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/job_class_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12097 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/qconf_object_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7796 2023-09-19 04:36:53.000000 uge-pycl-8.8.1/uge/objects/uge_release_object_map.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4366 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/scheduler_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6276 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/cluster_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6752 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/complex_configuration_base.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2920 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/parallel_environment_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4311 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/cluster_queue_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14875 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/qconf_object.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22217 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/complex_configuration_v4_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15716 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/complex_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4373 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/cluster_queue_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4200 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/scheduler_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4232 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/job_class_v4_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2531 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/objects/project_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      846 2023-09-19 04:36:53.000000 uge-pycl-8.8.1/uge/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge/config/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11839 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/config/config_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/uge/config/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       60 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/MANIFEST.in
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/dependency_links.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3972 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/SOURCES.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       61 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/entry_points.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/PKG-INFO
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       20 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/requires.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      105 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/uge_pycl.egg-info/top_level.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/PKG-INFO
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/test/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3240 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_ar.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4260 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_job_class.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5894 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_user.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7437 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_project.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6629 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_access_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5859 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_share_tree.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2665 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_admin_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5599 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_parallel_environment.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5764 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_cluster_queue.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2259 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_operator.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5705 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_checkpointing_environment.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2262 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_cluster_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2471 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_submit_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3322 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_complex_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3164 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_resource_quota_set.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2238 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2277 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_scheduler_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6386 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_host_group.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5823 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_calendar.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5303 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/test_execution_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4885 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/test/utils.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2886 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/README.rst
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      237 2023-09-25 08:10:46.000000 uge-pycl-8.8.1/setup.cfg
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2834 2023-09-18 15:40:41.000000 uge-pycl-8.8.1/setup.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2758 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/README.md
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      476 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test_values.json
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/exceptions/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1500 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/qmaster_unreachable.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1502 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/object_already_exists.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2387 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/command_failed.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3225 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/ar_exception.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1488 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/invalid_argument.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1494 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/configuration_error.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1494 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/authorization_error.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1484 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/invalid_request.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3167 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/qconf_exception.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1446 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1487 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/exceptions/object_not_found.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/utility/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4922 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/utility/uge_subprocess.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/utility/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/api/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11149 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/ar_api.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)   165933 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/qconf_api.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      908 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/api/impl/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4035 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/share_tree_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1663 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/operator_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2198 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/job_class_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2162 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/calendar_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1858 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/admin_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1855 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/ar_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1808 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/submit_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4089 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/list_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3446 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/complex_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5373 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/qrdel_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2144 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/user_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6484 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/dict_list_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1994 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/cluster_queue_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2642 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/execution_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4501 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/access_list_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1661 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/manager_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7199 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/qconf_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12969 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/dict_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2200 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/host_group_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1921 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/resource_quota_set_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6170 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/qrstat_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2210 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/scheduler_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1956 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/parallel_environment_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1968 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/checkpointing_environment_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2164 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/project_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2985 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/cluster_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5441 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/api/impl/qrsub_executor.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/constants/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1079 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/constants/uge_status.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/constants/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/log/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3583 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/logger_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1664 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/trace_log_record.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12737 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/log_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2496 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/trace_logger.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1579 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/stream_log_handler.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1778 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/log/timed_rotating_file_log_handler.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/cli/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2804 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/cli/qconf_convert.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7325 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/cli/qconf_cli.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/cli/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/objects/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2415 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/user_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5304 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/qconf_dict_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    17364 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/complex_configuration_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4198 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/resource_quota_set_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5184 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/ar_object_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6265 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/cluster_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2709 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/qconf_name_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3074 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/share_tree_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2763 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/checkpointing_environment_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2626 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/advance_reservation_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2967 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/execution_host_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2497 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/host_group_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2838 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/parallel_environment_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2413 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/calendar_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4400 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/scheduler_configuration_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4170 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/job_class_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    16089 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/complex_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2554 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/access_list_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4268 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/job_class_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4202 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/job_class_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12174 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/qconf_object_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7529 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/uge_release_object_map.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4363 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/scheduler_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6235 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/cluster_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6723 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/complex_configuration_base.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2917 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/parallel_environment_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4308 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/cluster_queue_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14847 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/qconf_object.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22214 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/complex_configuration_v4_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15713 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/complex_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4370 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/cluster_queue_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4197 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/scheduler_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4229 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/job_class_v4_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2528 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/objects/project_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      842 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge/config/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11948 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/config/config_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/uge/config/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       60 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/MANIFEST.in
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/dependency_links.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3972 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/SOURCES.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       61 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/entry_points.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/PKG-INFO
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       20 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/requires.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      105 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/uge_pycl.egg-info/top_level.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/PKG-INFO
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/test/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3240 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_ar.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4260 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_job_class.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5894 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_user.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7437 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_project.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6629 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_access_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5859 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_share_tree.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2665 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_admin_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5599 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_parallel_environment.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5764 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_cluster_queue.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2259 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_operator.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5705 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_checkpointing_environment.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2262 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_cluster_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2471 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_submit_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3322 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_complex_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3164 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_resource_quota_set.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2238 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2277 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_scheduler_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6386 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_host_group.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5823 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_calendar.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5303 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/test_execution_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4885 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/test/utils.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2886 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/README.rst
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      237 2024-04-14 10:19:37.000000 uge-pycl-8.9.0/setup.cfg
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2834 2024-04-10 04:30:36.000000 uge-pycl-8.9.0/setup.py
```

### Comparing `uge-pycl-8.8.1/README.md` & `uge-pycl-8.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-(c) Copyright 2016-2022 Altair Engineering Inc.
+(c) Copyright 2016-2024 Altair Engineering Inc.
     Licensed under the Apache License, Version 2.0 (the "License"); you may not
     use this file except in compliance with the License.
 
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/qmaster_unreachable.py` & `uge-pycl-8.9.0/uge/exceptions/qmaster_unreachable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class QmasterUnreachable(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/object_already_exists.py` & `uge-pycl-8.9.0/uge/exceptions/object_already_exists.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class ObjectAlreadyExists(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/command_failed.py` & `uge-pycl-8.9.0/uge/exceptions/command_failed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class CommandFailed(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/ar_exception.py` & `uge-pycl-8.9.0/uge/exceptions/ar_exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 try:
     import exceptions
 except ImportError:
     import builtins as exceptions
 import json
 
 from uge.constants import uge_status
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/invalid_argument.py` & `uge-pycl-8.9.0/uge/exceptions/object_not_found.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,32 +14,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
-class InvalidArgument(QconfException):
+class ObjectNotFound(QconfException):
     """ 
-    Invalid argument error class.
+    Object not found error class.
 
-    Error code: uge_status.UGE_INVALID_ARGUMENT
+    Error code: uge_status.UGE_OBJECT_NOT_FOUND
     """
 
     def __init__(self, error='', **kwargs):
         """ 
         Class constructor. 
 
         :param error: Error message.
         :type error: str
 
         :param kwargs: Keyword arguments, may contain 'args=error_message', 'exception=exception_object', or 'error_details=details'.
         """
         QconfException.__init__(
-            self, error, uge_status.UGE_INVALID_ARGUMENT,
+            self, error, uge_status.UGE_OBJECT_NOT_FOUND,
             **kwargs)
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/configuration_error.py` & `uge-pycl-8.9.0/uge/exceptions/configuration_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class ConfigurationError(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/authorization_error.py` & `uge-pycl-8.9.0/uge/exceptions/authorization_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class AuthorizationError(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/invalid_request.py` & `uge-pycl-8.9.0/uge/exceptions/invalid_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
 class InvalidRequest(QconfException):
     """
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/qconf_exception.py` & `uge-pycl-8.9.0/uge/exceptions/qconf_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 try:
     import exceptions
 except ImportError:
     import builtins as exceptions
 import json
 
 from uge.constants import uge_status
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/__init__.py` & `uge-pycl-8.9.0/uge/exceptions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 from uge.exceptions.authorization_error import AuthorizationError
 from uge.exceptions.command_failed import CommandFailed
 from uge.exceptions.configuration_error import ConfigurationError
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.object_not_found import ObjectNotFound
```

### Comparing `uge-pycl-8.8.1/uge/exceptions/object_not_found.py` & `uge-pycl-8.9.0/uge/exceptions/invalid_argument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,32 +14,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions.qconf_exception import QconfException
 from uge.constants import uge_status
 
 
-class ObjectNotFound(QconfException):
+class InvalidArgument(QconfException):
     """ 
-    Object not found error class.
+    Invalid argument error class.
 
-    Error code: uge_status.UGE_OBJECT_NOT_FOUND
+    Error code: uge_status.UGE_INVALID_ARGUMENT
     """
 
     def __init__(self, error='', **kwargs):
         """ 
         Class constructor. 
 
         :param error: Error message.
         :type error: str
 
         :param kwargs: Keyword arguments, may contain 'args=error_message', 'exception=exception_object', or 'error_details=details'.
         """
         QconfException.__init__(
-            self, error, uge_status.UGE_OBJECT_NOT_FOUND,
+            self, error, uge_status.UGE_INVALID_ARGUMENT,
             **kwargs)
```

### Comparing `uge-pycl-8.8.1/uge/utility/uge_subprocess.py` & `uge-pycl-8.9.0/uge/utility/uge_subprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import os
 import subprocess
 
 from uge.log.log_manager import LogManager
 from uge.exceptions.command_failed import CommandFailed
```

### Comparing `uge-pycl-8.8.1/uge/utility/__init__.py` & `uge-pycl-8.9.0/uge/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
+__version__ = '8.9.0'
```

### Comparing `uge-pycl-8.8.1/uge/api/ar_api.py` & `uge-pycl-8.9.0/uge/api/ar_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,29 +15,33 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 #
-from uge.objects.ar_object_factory import AdvanceReservationObjectFactory
 
 __docformat__ = 'reStructuredText'
 
 import os
+import collections
+try:
+    collectionsAbc = collections.abc
+except AttributeError:
+    collectionsAbc = collections
 from functools import wraps
 from decorator import decorator
 from uge.log.log_manager import LogManager
 from uge.exceptions.ar_exception import AdvanceReservationException
 from uge.exceptions.configuration_error import ConfigurationError
 from uge.api.impl.qrstat_executor import QrstatExecutor
 from uge.api.impl.qrsub_executor import QrsubExecutor
 from uge.api.impl.qrdel_executor import QrdelExecutor
 from uge.api.impl.ar_manager import AdvanceReservationManager
-import collections
+from uge.objects.ar_object_factory import AdvanceReservationObjectFactory
 
 
 class AdvanceReservationApi(object):
     """ High-level advance reservation API class. """
 
     DEFAULT_SGE_CELL = 'default'
     DEFAULT_SGE_QMASTER_PORT = 6444
@@ -108,15 +112,15 @@
 
     def api_call2(func):
         @wraps(func)
         def wrapped_call(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
                 return result
-            except AdvanceReservationException as ex:
+            except AdvanceReservationException:
                 raise
             except Exception as ex:
                 raise AdvanceReservationException(exception=ex)
 
         return decorator(wrapped_call, func)
 
     # Make sure only ar specific exceptions are raised
@@ -131,18 +135,17 @@
                 except AdvanceReservationException as ex:
                     raise
                 except Exception as ex:
                     raise AdvanceReservationException(exception=ex)
 
             return decorator(wrapped_call, func)
 
-        if len(dargs) == 1 and isinstance(dargs[0], collections.Callable):
+        if len(dargs) == 1 and isinstance(dargs[0], collectionsAbc.Callable):
             return internal_call(dargs[0])
-        else:
-            return internal_call
+        return internal_call
 
     def get_uge_version(self):
         """ Get version of UGE qmaster that API is connected to.
 
         :returns: UGE version string.
 
         :raises AdvanceReservationException: in case of any errors.
```

### Comparing `uge-pycl-8.8.1/uge/api/qconf_api.py` & `uge-pycl-8.9.0/uge/api/qconf_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/env python
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 __docformat__ = 'reStructuredText'
 
 import os
-from functools import wraps
 from decorator import decorator
+from functools import wraps
 from uge.log.log_manager import LogManager
 from uge.exceptions.qconf_exception import QconfException
 from uge.exceptions.configuration_error import ConfigurationError
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from uge.api.impl.qconf_executor import QconfExecutor
 from uge.api.impl.cluster_queue_manager import ClusterQueueManager
 from uge.api.impl.execution_host_manager import ExecutionHostManager
```

### Comparing `uge-pycl-8.8.1/uge/api/__init__.py` & `uge-pycl-8.9.0/uge/api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 from uge.api.qconf_api import QconfApi
 from uge.api.ar_api import AdvanceReservationApi
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/share_tree_manager.py` & `uge-pycl-8.9.0/uge/api/impl/share_tree_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 import re
-import types
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_list_based_object_manager import DictListBasedObjectManager
 
 class ShareTreeManager(DictListBasedObjectManager):
@@ -59,19 +58,19 @@
     def delete_stnode(self, path):
         self.qconf_executor.execute_qconf('-dstnode %s' % (path), self.QCONF_ERROR_REGEX_LIST)
         return self.get_object()
 
     def object_exists(self):
         try:
             self.qconf_executor.execute_qconf('-sstree', self.QCONF_ERROR_SSTREE_REGEX_LIST)
-        except ObjectNotFound as ex:
+        except ObjectNotFound:
             return False
         return True
 
-    # The following methods implement behavior where no share tree 
+    # The following methods implement behavior where no share tree
     # is equivalent to empty list
     def get_object_if_exists(self):
         # Return empty list if share is not there
         if self.object_exists():
             stree = self.get_object()
         else:
             stree = self.generate_object(data=[], add_required_data=False)
@@ -84,21 +83,19 @@
 
     def modify_or_add_object(self, pycl_object=None, data=None,
                       metadata=None, json_string=None):
         # If empty list is provided, delete share tree
         if type(data) == list and not len(data):
             self.delete_object_if_exists()
             return self.generate_object(data=[], add_required_data=False)
-        else:     
-            # If share tree exists, modify it
-            # If share tree is not there, add it.
-            if self.object_exists():
-                stree = self.modify_object(pycl_object=pycl_object, data=data, metadata=metadata, json_string=json_string)
-            else:
-                stree = self.add_object(pycl_object=pycl_object, data=data, metadata=metadata, json_string=json_string)
+        # If share tree exists, modify it
+        # If share tree is not there, add it.
+        if self.object_exists():
+            stree = self.modify_object(pycl_object=pycl_object, data=data, metadata=metadata, json_string=json_string)
+        else:
+            stree = self.add_object(pycl_object=pycl_object, data=data, metadata=metadata, json_string=json_string)
         return stree
 
 #############################################################################
 # Testing.
 if __name__ == '__main__':
     pass
-
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/operator_manager.py` & `uge-pycl-8.9.0/uge/api/impl/operator_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from .list_based_object_manager import ListBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/job_class_manager.py` & `uge-pycl-8.9.0/uge/api/impl/job_class_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/calendar_manager.py` & `uge-pycl-8.9.0/uge/api/impl/calendar_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/admin_host_manager.py` & `uge-pycl-8.9.0/uge/api/impl/admin_host_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.invalid_request import InvalidRequest
 from .list_based_object_manager import ListBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/ar_manager.py` & `uge-pycl-8.9.0/uge/api/impl/cluster_queue_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,37 +14,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
-from uge.objects.ar_object_factory import AdvanceReservationObjectFactory
+from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
-class AdvanceReservationManager(DictBasedObjectManager):
-    AR_ERROR_REGEX_LIST = [
+class ClusterQueueManager(DictBasedObjectManager):
+    QCONF_ERROR_REGEX_LIST = [
         (re.compile('.*No cluster queue or queue instance matches.*'), ObjectNotFound),
         (re.compile('.*no cqueue list defined.*'), ObjectNotFound),
     ]
 
     # Failure incorrectly classified as successful outcome
-    AR_FAILURE_REGEX_LIST = []
+    QCONF_FAILURE_REGEX_LIST = []
+
+    GENERATE_OBJECT_FACTORY_METHOD = QconfObjectFactory.generate_cluster_queue
+    OBJECT_NAME_KEY = 'qname'
+    OBJECT_CLASS_NAME = 'ClusterQueue'
+    OBJECT_CLASS_UGE_NAME = 'q'
+    OBJECT_CLASS_UGE_LIST_DETAILS_NAME = 'ld'
 
-    GENERATE_OBJECT_FACTORY_METHOD = AdvanceReservationObjectFactory.generate_advance_reservation
-    OBJECT_NAME_KEY = 'id'
-    OBJECT_CLASS_NAME = 'AdvanceReservation'
-    OBJECT_CLASS_UGE_NAME = 'ar'
+    def __init__(self, qconf_executor):
+        DictBasedObjectManager.__init__(self, qconf_executor)
 
-    def __init__(self, qrstat_executor, qrsub_executor, qrdel_executor):
-        DictBasedObjectManager.__init__(self, qrstat_executor)
+    def get_bulk_dump_filename(self, object):
+        return 'conf_api_dump_' + object.data['qname']
 
 
 #############################################################################
 # Testing.
 if __name__ == '__main__':
     pass
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/submit_host_manager.py` & `uge-pycl-8.9.0/uge/api/impl/submit_host_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.api.impl.list_based_object_manager import ListBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/list_based_object_manager.py` & `uge-pycl-8.9.0/uge/api/impl/list_based_object_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,18 +14,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 import sys
-import types
 from uge.log.log_manager import LogManager
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.objects.qconf_object import QconfObject
 from uge.objects.qconf_name_list import QconfNameList
@@ -87,15 +86,15 @@
 
     def list_names(self):
         try:
             qconf_output = self.qconf_executor.execute_qconf('-s%s' % (self.OBJECT_CLASS_UGE_NAME),
                                                              self.QCONF_ERROR_REGEX_LIST).get_stdout()
             name_list = QconfNameList(metadata={'description': 'List of %s names' % (self.OBJECT_NAME)},
                                       data=QconfObject.get_list_from_qconf_output(qconf_output))
-        except ObjectNotFound as ex:
+        except ObjectNotFound:
             name_list = QconfNameList(metadata={'description': 'List of %s names' % (self.OBJECT_NAME)}, data=[])
         return name_list
 
 
 #############################################################################
 # Testing.
 if __name__ == '__main__':
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/complex_configuration_manager.py` & `uge-pycl-8.9.0/uge/api/impl/complex_configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/qrdel_executor.py` & `uge-pycl-8.9.0/uge/api/impl/qrdel_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 import os
 import tempfile
 from uge.utility.uge_subprocess import UgeSubprocess
 from uge.log.log_manager import LogManager
 from uge.exceptions.ar_exception import AdvanceReservationException
 from uge.exceptions.command_failed import CommandFailed
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/user_manager.py` & `uge-pycl-8.9.0/uge/api/impl/user_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/dict_list_based_object_manager.py` & `uge-pycl-8.9.0/uge/api/impl/dict_list_based_object_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,27 +14,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
-import re
+#
 import copy
 from uge.log.log_manager import LogManager
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from uge.objects.qconf_object import QconfObject
 from uge.objects.qconf_name_list import QconfNameList
 
 
+
 class DictListBasedObjectManager(object):
     QCONF_ERROR_REGEX_LIST = [
     ]
 
     # Failure incorrectly classified as successful outcome
     QCONF_FAILURE_REGEX_LIST = []
 
@@ -58,19 +58,19 @@
 
     def __prepare_object(self, pycl_object=None, data=None,
                          metadata=None, json_string=None,
                          add_required_data=True):
         uge_version = self.qconf_executor.get_uge_version()
         data2 = copy.copy(data)
         metadata2 = copy.copy(metadata)
-        # If pycl_object is provided, combine its metadata 
+        # If pycl_object is provided, combine its metadata
         # with provided metadata
         if pycl_object is not None:
             generated_object = self.GENERATE_OBJECT_FACTORY_METHOD(uge_version, add_required_data=False)
-            if not str(type(pycl_object)) == str(type(generated_object)):
+            if str(type(pycl_object)) != str(type(generated_object)):
                 raise InvalidArgument(
                     'The pycl_object argument must be an instance of %s.' % generated_object.__class__.__name__)
             data2 = copy.copy(pycl_object.data)
             if data:
                 data2 = copy.copy(data)
             metadata2 = copy.copy(pycl_object.metadata)
             if metadata:
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/cluster_queue_manager.py` & `uge-pycl-8.9.0/uge/api/impl/project_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,41 +14,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
-class ClusterQueueManager(DictBasedObjectManager):
+class ProjectManager(DictBasedObjectManager):
     QCONF_ERROR_REGEX_LIST = [
-        (re.compile('.*No cluster queue or queue instance matches.*'), ObjectNotFound),
-        (re.compile('.*no cqueue list defined.*'), ObjectNotFound),
+        (re.compile('.*is still referenced in.*'), InvalidRequest),
+        (re.compile('.*multiple occurances of userset.*'), InvalidRequest),
+        (re.compile('.*does not exist.*'), ObjectNotFound),
+        (re.compile('.*no project list defined.*'), ObjectNotFound),
+        (re.compile('.*is not known as project.*'), ObjectNotFound),
     ]
 
     # Failure incorrectly classified as successful outcome
     QCONF_FAILURE_REGEX_LIST = []
 
-    GENERATE_OBJECT_FACTORY_METHOD = QconfObjectFactory.generate_cluster_queue
-    OBJECT_NAME_KEY = 'qname'
-    OBJECT_CLASS_NAME = 'ClusterQueue'
-    OBJECT_CLASS_UGE_NAME = 'q'
+    GENERATE_OBJECT_FACTORY_METHOD = QconfObjectFactory.generate_project
+    OBJECT_NAME_KEY = 'name'
+    OBJECT_CLASS_NAME = 'Project'
+    OBJECT_CLASS_UGE_NAME = 'prj'
     OBJECT_CLASS_UGE_LIST_DETAILS_NAME = 'ld'
 
     def __init__(self, qconf_executor):
         DictBasedObjectManager.__init__(self, qconf_executor)
 
     def get_bulk_dump_filename(self, object):
-        return 'conf_api_dump_' + object.data['qname']
+        return 'conf_api_dump_' + object.data['name']
 
 
 #############################################################################
 # Testing.
 if __name__ == '__main__':
     pass
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/execution_host_manager.py` & `uge-pycl-8.9.0/uge/api/impl/execution_host_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 import os
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/access_list_manager.py` & `uge-pycl-8.9.0/uge/api/impl/access_list_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,14 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 #
 import re
-import types
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/manager_manager.py` & `uge-pycl-8.9.0/uge/api/impl/manager_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.object_already_exists import ObjectAlreadyExists
 from .list_based_object_manager import ListBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/qconf_executor.py` & `uge-pycl-8.9.0/uge/api/impl/qconf_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,26 +14,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 import os
-import tempfile
 from uge.utility.uge_subprocess import UgeSubprocess
 from uge.log.log_manager import LogManager
 from uge.exceptions.qconf_exception import QconfException
 from uge.exceptions.command_failed import CommandFailed
 from uge.exceptions.qmaster_unreachable import QmasterUnreachable
 from uge.exceptions.authorization_error import AuthorizationError
 from uge.exceptions.object_not_found import ObjectNotFound
-from uge.exceptions.object_already_exists import ObjectAlreadyExists
 
 
 class QconfExecutor(object):
     QCONF_ERROR_REGEX_LIST = [
         (re.compile('.*unable to send message to qmaster.*'), QmasterUnreachable),
         (re.compile('.*must be manager.*'), AuthorizationError),
         (re.compile('denied.*'), AuthorizationError),
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/dict_based_object_manager.py` & `uge-pycl-8.9.0/uge/api/impl/dict_based_object_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -76,15 +76,15 @@
     def __prepare_object(self, pycl_object=None, name=None, data=None,
                          metadata=None, json_string=None,
                          add_required_data=True):
         uge_version = self.qconf_executor.get_uge_version()
         data2 = copy.copy(data)
         metadata2 = copy.copy(metadata)
         name2 = name
-        # If pycl_object is provided, combine its data/metadata 
+        # If pycl_object is provided, combine its data/metadata
         # with provided data/metadata
         if pycl_object is not None:
             generated_object = self.GENERATE_OBJECT_FACTORY_METHOD(uge_version, add_required_data=False)
             if not str(type(pycl_object)) == str(type(generated_object)):
                 raise InvalidArgument(
                     'The pycl_object argument must be an instance of %s.' % generated_object.__class__.__name__)
             data2 = copy.copy(pycl_object.data)
@@ -114,15 +114,15 @@
         elif new_object.name:
             object_name = new_object.name
         else:
             object_name = ''
         try:
             old_object = self.get_object(object_name)
             raise ObjectAlreadyExists('%s %s already exists.' % (self.OBJECT_CLASS_NAME, object_name))
-        except ObjectNotFound as ex:
+        except ObjectNotFound:
             # ok
             pass
         new_object.remove_optional_keys()
         self.verify_object_before_add(new_object)
         self.qconf_executor.execute_qconf_with_object('-A%s' % self.OBJECT_CLASS_UGE_NAME, new_object,
                                                       self.QCONF_ERROR_REGEX_LIST)
         new_object.set_add_metadata()
@@ -131,20 +131,18 @@
     def add_objects(self, object_list, dirname=None):
         if not dirname:
             dirname = tempfile.mktemp()
         self.mk_object_dir(dirname)
         self.write_objects(object_list, dirname)
         self.add_objects_from_dir(dirname)
         self.rm_object_dir(dirname)
-        return
 
     def add_objects_from_dir(self, dirname):
         self.qconf_executor.execute_qconf_with_dir('-A%s' % self.OBJECT_CLASS_UGE_NAME, dirname,
                                                    self.QCONF_ERROR_REGEX_LIST)
-        return
 
     def verify_object_before_modify(self, pycl_object):
         return
 
     def modify_object(self, pycl_object=None, name=None, data=None,
                       metadata=None, json_string=None):
         generated_object = self.__prepare_object(
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/host_group_manager.py` & `uge-pycl-8.9.0/uge/api/impl/host_group_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_argument import InvalidArgument
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/resource_quota_set_manager.py` & `uge-pycl-8.9.0/uge/api/impl/resource_quota_set_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/qrstat_executor.py` & `uge-pycl-8.9.0/uge/api/impl/qrstat_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,29 +14,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
-import os
-import tempfile
 import xmltodict
 import json
 
 from uge.utility.uge_subprocess import UgeSubprocess
 from uge.log.log_manager import LogManager
 from uge.exceptions.ar_exception import AdvanceReservationException
 from uge.exceptions.command_failed import CommandFailed
 from uge.exceptions.qmaster_unreachable import QmasterUnreachable
 from uge.exceptions.authorization_error import AuthorizationError
 from uge.exceptions.object_not_found import ObjectNotFound
-from uge.exceptions.object_already_exists import ObjectAlreadyExists
 
 
 class QrstatExecutor(object):
     QRSTAT_ERROR_REGEX_LIST = [
         (re.compile('.*unable to send message to qmaster.*'), QmasterUnreachable),
         (re.compile('.*must be manager.*'), AuthorizationError),
         (re.compile('denied.*'), AuthorizationError),
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/scheduler_configuration_manager.py` & `uge-pycl-8.9.0/uge/api/impl/scheduler_configuration_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
 class SchedulerConfigurationManager(DictBasedObjectManager):
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/__init__.py` & `uge-pycl-8.9.0/uge/utility/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/parallel_environment_manager.py` & `uge-pycl-8.9.0/uge/api/impl/parallel_environment_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,18 +14,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
-from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
 class ParallelEnvironmentManager(DictBasedObjectManager):
     QCONF_ERROR_REGEX_LIST = [
         (re.compile('.*is not a parallel environment.*'), ObjectNotFound),
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/checkpointing_environment_manager.py` & `uge-pycl-8.9.0/uge/api/impl/checkpointing_environment_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,18 +14,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
-from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
 class CheckpointingEnvironmentManager(DictBasedObjectManager):
     QCONF_ERROR_REGEX_LIST = [
         (re.compile('.*is not a checkpointing.*'), ObjectNotFound),
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/cluster_configuration_manager.py` & `uge-pycl-8.9.0/uge/api/impl/cluster_configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 from uge.exceptions.object_not_found import ObjectNotFound
 from uge.exceptions.invalid_request import InvalidRequest
 from uge.objects.qconf_object_factory import QconfObjectFactory
 from .dict_based_object_manager import DictBasedObjectManager
 
 
@@ -46,22 +46,20 @@
         DictBasedObjectManager.__init__(self, qconf_executor)
 
     def verify_object_before_add(self, pycl_object):
         if not pycl_object.name:
             raise InvalidRequest('Cluster configuration name must be specified.')
         if pycl_object.name == 'global':
             raise InvalidRequest('Global cluster configuration cannot be added.')
-        return
 
     def verify_object_before_delete(self, pycl_object):
         if not pycl_object.name:
             raise InvalidRequest('Cluster configuration name must be specified.')
         if pycl_object.name == 'global':
             raise InvalidRequest('Global cluster configuration cannot be deleted.')
-        return
 
     def get_object(self, name):
         if name == 'global':
             # This avoids name resolution for 'global'
             pycl_object = DictBasedObjectManager.get_object(self, '')
             pycl_object.name = name
         else:
```

### Comparing `uge-pycl-8.8.1/uge/api/impl/qrsub_executor.py` & `uge-pycl-8.9.0/uge/api/impl/qrsub_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import re
 import os
 import tempfile
 from uge.utility.uge_subprocess import UgeSubprocess
 from uge.log.log_manager import LogManager
 from uge.exceptions.ar_exception import AdvanceReservationException
 from uge.exceptions.command_failed import CommandFailed
```

### Comparing `uge-pycl-8.8.1/uge/constants/uge_status.py` & `uge-pycl-8.9.0/uge/constants/uge_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 #!/usr/bin/env python
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 
 UGE_OK = 0
 UGE_ERROR = 1
 UGE_CONFIGURATION_ERROR = 2
 UGE_AUTHORIZATION_ERROR = 3
 UGE_COMMAND_FAILED = 4
 UGE_INVALID_REQUEST = 5
 UGE_INVALID_ARGUMENT = 6
 UGE_QMASTER_UNREACHABLE = 7
 UGE_OBJECT_NOT_FOUND = 8
 UGE_OBJECT_ALREADY_EXISTS = 9
-
```

### Comparing `uge-pycl-8.8.1/uge/constants/__init__.py` & `uge-pycl-8.9.0/uge/api/impl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/uge/log/logger_factory.py` & `uge-pycl-8.9.0/uge/log/logger_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 import re
 import logging
 
 from uge.log.trace_logger import TraceLogger
```

### Comparing `uge-pycl-8.8.1/uge/log/trace_log_record.py` & `uge-pycl-8.9.0/uge/log/trace_log_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 import logging
 import os
 import inspect
 
 
 class TraceLogRecord(logging.LogRecord):
```

### Comparing `uge-pycl-8.8.1/uge/log/log_manager.py` & `uge-pycl-8.9.0/uge/log/log_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 import logging
 import re
 import sys
 
 from uge.config.config_manager import ConfigManager
 from uge.exceptions.configuration_error import ConfigurationError
```

### Comparing `uge-pycl-8.8.1/uge/log/trace_logger.py` & `uge-pycl-8.9.0/uge/log/trace_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 import logging
 
 from .trace_log_record import TraceLogRecord
 
 
 class TraceLogger(logging.getLoggerClass()):
```

### Comparing `uge-pycl-8.8.1/uge/log/__init__.py` & `uge-pycl-8.9.0/uge/constants/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
```

### Comparing `uge-pycl-8.8.1/uge/log/stream_log_handler.py` & `uge-pycl-8.9.0/uge/log/stream_log_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from logging import StreamHandler
 
 from uge.config import config_manager
 
 
 class StreamLogHandler(StreamHandler):
```

### Comparing `uge-pycl-8.8.1/uge/log/timed_rotating_file_log_handler.py` & `uge-pycl-8.9.0/uge/log/timed_rotating_file_log_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from logging.handlers import TimedRotatingFileHandler
 
 from uge.config import config_manager
 
 
 class TimedRotatingFileLogHandler(TimedRotatingFileHandler):
```

### Comparing `uge-pycl-8.8.1/uge/cli/qconf_convert.py` & `uge-pycl-8.9.0/uge/cli/qconf_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.cli.qconf_cli import QconfCli
 from uge.api.qconf_api import QconfApi
 from uge.exceptions.invalid_request import InvalidRequest
 
 
 class QconfConvert(QconfCli):
     """ Qconf upgrade command. """
```

### Comparing `uge-pycl-8.8.1/uge/cli/qconf_cli.py` & `uge-pycl-8.9.0/uge/cli/qconf_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from __future__ import print_function
 import abc
 import logging
 import os
 import sys
 from optparse import OptionGroup
 from optparse import OptionParser
@@ -151,21 +151,19 @@
     def get_arg(self, i):
         """ Returns the i-th command line argument. """
         return self.args[i]
 
     @abc.abstractmethod
     def run_command(self):
         """ This method must be implemented by the derived class. """
-        pass
 
     def check_input_args(self):
         """ 
         This method should verify required arguments in the derived class.
         """
-        pass
 
     def run(self):
         """
         Run command. This method simply invokes run_command() and handles
         any exceptions.
         """
         try:
```

### Comparing `uge-pycl-8.8.1/uge/cli/__init__.py` & `uge-pycl-8.9.0/uge/log/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
```

### Comparing `uge-pycl-8.8.1/uge/objects/user_v1_0.py` & `uge-pycl-8.9.0/uge/objects/user_v1_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class User(QconfObject):
     """ This class encapsulates UGE user object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/qconf_dict_list.py` & `uge-pycl-8.9.0/uge/objects/qconf_dict_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,24 +14,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 from uge.exceptions import InvalidRequest
 
 try:
     import UserList
 except ImportError:
     import collections as UserList
-from .qconf_object import QconfObject
 from uge.exceptions.invalid_argument import InvalidArgument
+from .qconf_object import QconfObject
 
 
 class QconfDictList(QconfObject, UserList.UserList):
     """ This class encapsulates data and functionality common to all Qconf objects based on a list of dictionaries. """
 
     FIRST_KEY = None
     NAME_KEY = None
```

### Comparing `uge-pycl-8.8.1/uge/objects/complex_configuration_v3_0.py` & `uge-pycl-8.9.0/uge/objects/complex_configuration_v3_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.complex_configuration_base import ComplexConfigurationBase
 
 
 class ComplexConfiguration(ComplexConfigurationBase):
     """ This class encapsulates UGE complex configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '3.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/resource_quota_set_v1_0.py` & `uge-pycl-8.9.0/uge/objects/resource_quota_set_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ResourceQuotaSet(QconfObject):
     """ This class encapsulates UGE resource quota set object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'name'
 
     #: Object keys that must be provided by set.
     USER_PROVIDED_KEYS = ['name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/ar_object_factory.py` & `uge-pycl-8.9.0/uge/objects/ar_object_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,41 +14,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import imp
 import json
+import re
 
 from uge.exceptions.ar_exception import AdvanceReservationException
 from uge.exceptions.invalid_request import InvalidRequest
 from .uge_release_object_map import UGE_RELEASE_OBJECT_MAP
 
 
 class AdvanceReservationObjectFactory(object):
 
     @classmethod
     def __get_object_base_module_name(cls, class_name):
-        # This method relies on convention: 
+        # This method relies on convention:
         #     ResourceQuotaSet=>resource_quota_set
         base_module_name = class_name[0].lower()
         for letter in class_name[1:]:
             if letter.isupper():
                 base_module_name += '_%s' % letter.lower()
             else:
                 base_module_name += letter
         return base_module_name
 
     @classmethod
     def __get_object_class_from_uge_version(cls, uge_version, class_name, base_module_name=None):
         if not uge_version:
             raise InvalidRequest('Cannot generate %s object: UGE version must be specified.' % class_name)
+        uge_version = re.search(r'\d+.\d+.\d+', uge_version).group(0)
         if uge_version not in UGE_RELEASE_OBJECT_MAP:
             raise AdvanceReservationException('Unsupported UGE version: %s.' % uge_version)
         release_map = UGE_RELEASE_OBJECT_MAP.get(uge_version)
         object_version = release_map.get(class_name)
         return cls.__get_object_class_from_object_version(object_version, class_name, base_module_name)
 
     @classmethod
```

### Comparing `uge-pycl-8.8.1/uge/objects/cluster_configuration_v2_0.py` & `uge-pycl-8.9.0/uge/objects/cluster_configuration_v2_0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,34 +14,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import os
 import tempfile
-import string
 from .qconf_object import QconfObject
 
 
 class ClusterConfiguration(QconfObject):
     """ This class encapsulates UGE cluster configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
 
-    #: Default values for required data keys for the global configuration. 
+    #: Default values for required data keys for the global configuration.
     #: Value for execd_spool_dir key will depend on $SGE_ROOT and $SGE_CELL.
     REQUIRED_GLOBAL_DATA_DEFAULTS = {
         'execd_spool_dir': 'SGE_ROOT/SGE_CELL/spool',
         'mailer': '/bin/mail',
         'xterm': '/usr/bin/xterm',
         'load_sensor': None,
         'prolog': None,
@@ -96,15 +95,15 @@
         'cgroups_params': {'cgroup_path': None, 'cpuset': False, 'mount': False, 'freezer': False,
                            'freeze_pe_tasks': False, 'killing': False, 'forced_numa': False, 'h_vmem_limit': False,
                            'm_mem_free_hard': False, 'm_mem_free_soft': False, 'min_memory_limit': 0},
         'lost_job_timeout': '00:00:00',
         'enable_lost_job_reschedule': False,
     }
 
-    #: Default values for required data keys for the host configuration. 
+    #: Default values for required data keys for the host configuration.
     REQUIRED_HOST_DATA_DEFAULTS = {
         'mailer': '/bin/mail',
         'xterm': '/usr/bin/xterm',
     }
 
     BOOL_KEY_MAP = QconfObject.get_bool_key_map(REQUIRED_GLOBAL_DATA_DEFAULTS)
     INT_KEY_MAP = QconfObject.get_int_key_map(REQUIRED_GLOBAL_DATA_DEFAULTS)
@@ -151,23 +150,22 @@
         QconfObject.__init__(self, name=name, data=data, metadata=metadata, json_string=json_string)
         if not self.name:
             self.name = self.get_name_from_data()
             if not self.name:
                 self.name = 'global'
 
     def get_name_from_data(self):
-        for (key, value) in list(self.data.items()):
+        for (key, _) in list(self.data.items()):
             if key.startswith('#'):
                 return key[1:-1]  # remove comment and ending column characters
         return None
 
     def get_required_data_defaults(self):
         if self.name == 'global':
             return self.REQUIRED_GLOBAL_DATA_DEFAULTS
-        else:
-            return self.REQUIRED_HOST_DATA_DEFAULTS
+        return self.REQUIRED_HOST_DATA_DEFAULTS
 
     def get_tmp_file(self):
         tmp_dir_path = tempfile.mkdtemp()
         tmp_file_path = os.path.join(tmp_dir_path, self.name)
         tmp_file = open(tmp_file_path, 'w')
         return tmp_file, tmp_file_path, tmp_dir_path
```

### Comparing `uge-pycl-8.8.1/uge/objects/qconf_name_list.py` & `uge-pycl-8.9.0/uge/objects/qconf_name_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 try:
     import UserList
 except ImportError:
     import collections as UserList
 from uge.exceptions.invalid_argument import InvalidArgument
 from .qconf_object import QconfObject
```

### Comparing `uge-pycl-8.8.1/uge/objects/share_tree_v1_0.py` & `uge-pycl-8.9.0/uge/objects/share_tree_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,23 +14,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_dict_list import QconfDictList
 from .qconf_object import QconfObject
 
 
 class ShareTree(QconfDictList):
     """ This class encapsulates UGE share tree object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Key that designates start of an object in a list
     FIRST_KEY = 'id'
 
     #: Object name key.
     NAME_KEY = None
```

### Comparing `uge-pycl-8.8.1/uge/objects/checkpointing_environment_v1_0.py` & `uge-pycl-8.9.0/uge/objects/checkpointing_environment_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class CheckpointingEnvironment(QconfObject):
     """ This class encapsulates UGE checkpointing environment object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'ckpt_name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['ckpt_name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/advance_reservation_v1_0.py` & `uge-pycl-8.9.0/uge/objects/advance_reservation_v1_0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class AdvanceReservation(QconfObject):
     """ This class encapsulates UGE project object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/execution_host_v1_0.py` & `uge-pycl-8.9.0/uge/objects/execution_host_v1_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ExecutionHost(QconfObject):
     """ This class encapsulates UGE execution host object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'hostname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['hostname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/host_group_v1_0.py` & `uge-pycl-8.9.0/uge/objects/host_group_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class HostGroup(QconfObject):
     """ This class encapsulates UGE host group object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'group_name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['group_name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/parallel_environment_v1_0.py` & `uge-pycl-8.9.0/uge/objects/parallel_environment_v1_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ParallelEnvironment(QconfObject):
     """ This class encapsulates UGE parallel environment object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'pe_name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['pe_name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/calendar_v1_0.py` & `uge-pycl-8.9.0/uge/objects/calendar_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class Calendar(QconfObject):
     """ This class encapsulates UGE calendar object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'calendar_name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['calendar_name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/scheduler_configuration_v3_0.py` & `uge-pycl-8.9.0/uge/objects/scheduler_configuration_v3_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.qconf_object import QconfObject
 
 
 class SchedulerConfiguration(QconfObject):
     """ This class encapsulates UGE scheduler configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '3.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/job_class_v1_0.py` & `uge-pycl-8.9.0/uge/objects/job_class_v1_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class JobClass(QconfObject):
     """ This class encapsulates UGE job class object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'jcname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['jcname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/complex_configuration_v2_0.py` & `uge-pycl-8.9.0/uge/objects/complex_configuration_v2_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.complex_configuration_base import ComplexConfigurationBase
 
 
 class ComplexConfiguration(ComplexConfigurationBase):
     """ This class encapsulates UGE complex configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/access_list_v1_0.py` & `uge-pycl-8.9.0/uge/objects/access_list_v1_0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class AccessList(QconfObject):
     """ This class encapsulates UGE access list object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'name'
 
     #: Object keys that must be provided by access list.
     USER_PROVIDED_KEYS = ['name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/job_class_v3_0.py` & `uge-pycl-8.9.0/uge/objects/job_class_v3_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class JobClass(QconfObject):
     """ This class encapsulates UGE job class object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '3.0'
 
     #: Object name key.
     NAME_KEY = 'jcname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['jcname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/job_class_v2_0.py` & `uge-pycl-8.9.0/uge/objects/job_class_v2_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class JobClass(QconfObject):
     """ This class encapsulates UGE job class object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = 'jcname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['jcname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/qconf_object_factory.py` & `uge-pycl-8.9.0/uge/objects/qconf_object_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,40 +14,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import imp
 import json
+import re
 from uge.exceptions.qconf_exception import QconfException
 from uge.exceptions.invalid_request import InvalidRequest
 from .uge_release_object_map import UGE_RELEASE_OBJECT_MAP
 
 
 class QconfObjectFactory(object):
 
     @classmethod
     def __get_object_base_module_name(cls, class_name):
-        # This method relies on convention: 
+        # This method relies on convention:
         #     ResourceQuotaSet=>resource_quota_set
         base_module_name = class_name[0].lower()
         for letter in class_name[1:]:
             if letter.isupper():
                 base_module_name += '_%s' % letter.lower()
             else:
                 base_module_name += letter
         return base_module_name
 
     @classmethod
     def __get_object_class_from_uge_version(cls, uge_version, class_name, base_module_name=None):
         if not uge_version:
             raise InvalidRequest('Cannot generate %s object: UGE version must be specified.' % class_name)
+        uge_version = re.search(r'\d+.\d+.\d+', uge_version).group(0)
         if uge_version not in UGE_RELEASE_OBJECT_MAP:
             raise QconfException('Unsupported UGE version: %s.' % uge_version)
         release_map = UGE_RELEASE_OBJECT_MAP.get(uge_version)
         object_version = release_map.get(class_name)
         return cls.__get_object_class_from_object_version(object_version, class_name, base_module_name)
 
     @classmethod
```

### Comparing `uge-pycl-8.8.1/uge/objects/uge_release_object_map.py` & `uge-pycl-8.9.0/uge/objects/uge_release_object_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
 import copy
 
 UGE_RELEASE_OBJECT_MAP = {}
 
 # 8.3.1p9
 UGE_RELEASE_OBJECT_MAP['8.3.1p9'] = {
     'AccessList'               : '1.0',
@@ -44,15 +44,15 @@
 
 # 8.3.1p12
 UGE_RELEASE_OBJECT_MAP['8.3.1p12'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.3.1p9'])
 
 # 8.4.0
 UGE_RELEASE_OBJECT_MAP['8.4.0'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.3.1p9'])
 UGE_RELEASE_OBJECT_MAP['8.4.0']['ComplexConfiguration'] = '2.0'
-    
+
 # 8.4.3
 UGE_RELEASE_OBJECT_MAP['8.4.3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.4.0'])
 
 # 8.4.4
 UGE_RELEASE_OBJECT_MAP['8.4.4'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.4.0'])
 
 # 8.4.5
@@ -170,21 +170,20 @@
 # 8.7.2
 UGE_RELEASE_OBJECT_MAP['8.7.2prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 UGE_RELEASE_OBJECT_MAP['8.7.2prealpha2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 UGE_RELEASE_OBJECT_MAP['8.7.2prealpha3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 # if new version string shall be used (see uge/api/impl/*executor.py#get_uge_version)
 # UGE_RELEASE_OBJECT_MAP['2022.1.0pre3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
 
-UGE_RELEASE_OBJECT_MAP['8.7.2beta'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 UGE_RELEASE_OBJECT_MAP['8.7.2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 
 # 8.7.3
-UGE_RELEASE_OBJECT_MAP['8.7.3prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.2'])
+UGE_RELEASE_OBJECT_MAP['8.7.3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.2'])
 
 # 8.8.0
-UGE_RELEASE_OBJECT_MAP['8.8.0prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
-UGE_RELEASE_OBJECT_MAP['8.8.0prealpha2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
 UGE_RELEASE_OBJECT_MAP['8.8.0'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
 
 # 8.8.1
-UGE_RELEASE_OBJECT_MAP['8.8.1prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.8.0'])
 UGE_RELEASE_OBJECT_MAP['8.8.1'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.8.0'])
+
+# 8.9.0
+UGE_RELEASE_OBJECT_MAP['8.9.0'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.8.1'])
```

### Comparing `uge-pycl-8.8.1/uge/objects/scheduler_configuration_v2_0.py` & `uge-pycl-8.9.0/uge/objects/scheduler_configuration_v2_0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.qconf_object import QconfObject
 
 
 class SchedulerConfiguration(QconfObject):
     """ This class encapsulates UGE scheduler configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/cluster_configuration_v1_0.py` & `uge-pycl-8.9.0/uge/objects/cluster_configuration_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,34 +14,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import os
 import tempfile
-import string
 from .qconf_object import QconfObject
 
 
 class ClusterConfiguration(QconfObject):
     """ This class encapsulates UGE cluster configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
 
-    #: Default values for required data keys for the global configuration. 
+    #: Default values for required data keys for the global configuration.
     #: Value for execd_spool_dir key will depend on $SGE_ROOT and $SGE_CELL.
     REQUIRED_GLOBAL_DATA_DEFAULTS = {
         'execd_spool_dir': 'SGE_ROOT/SGE_CELL/spool',
         'mailer': '/bin/mail',
         'xterm': '/usr/bin/xterm',
         'load_sensor': None,
         'prolog': None,
@@ -95,15 +94,15 @@
         'cgroups_params': {'cgroup_path': None, 'cpuset': False, 'mount': False, 'freezer': False,
                            'freeze_pe_tasks': False, 'killing': False, 'forced_numa': False, 'h_vmem_limit': False,
                            'm_mem_free_hard': False, 'm_mem_free_soft': False, 'min_memory_limit': 0},
         'lost_job_timeout': '00:00:00',
         'enable_lost_job_reschedule': False,
     }
 
-    #: Default values for required data keys for the host configuration. 
+    #: Default values for required data keys for the host configuration.
     REQUIRED_HOST_DATA_DEFAULTS = {
         'mailer': '/bin/mail',
         'xterm': '/usr/bin/xterm',
     }
 
     BOOL_KEY_MAP = QconfObject.get_bool_key_map(REQUIRED_GLOBAL_DATA_DEFAULTS)
     INT_KEY_MAP = QconfObject.get_int_key_map(REQUIRED_GLOBAL_DATA_DEFAULTS)
@@ -150,23 +149,22 @@
         QconfObject.__init__(self, name=name, data=data, metadata=metadata, json_string=json_string)
         if not self.name:
             self.name = self.get_name_from_data()
             if not self.name:
                 self.name = 'global'
 
     def get_name_from_data(self):
-        for (key, value) in list(self.data.items()):
+        for (key, _) in list(self.data.items()):
             if key.startswith('#'):
                 return key[1:-1]  # remove comment and ending column characters
         return None
 
     def get_required_data_defaults(self):
         if self.name == 'global':
             return self.REQUIRED_GLOBAL_DATA_DEFAULTS
-        else:
-            return self.REQUIRED_HOST_DATA_DEFAULTS
+        return self.REQUIRED_HOST_DATA_DEFAULTS
 
     def get_tmp_file(self):
         tmp_dir_path = tempfile.mkdtemp()
         tmp_file_path = os.path.join(tmp_dir_path, self.name)
         tmp_file = open(tmp_file_path, 'w')
         return tmp_file, tmp_file_path, tmp_dir_path
```

### Comparing `uge-pycl-8.8.1/uge/objects/complex_configuration_base.py` & `uge-pycl-8.9.0/uge/objects/complex_configuration_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,18 +14,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
-import types
-from .qconf_object import QconfObject
+#
 from uge.exceptions.invalid_argument import InvalidArgument
+from .qconf_object import QconfObject
 
 
 class ComplexConfigurationBase(QconfObject):
     """ This class serves as a base for UGE complex configuration objects. """
 
     DEFAULT_DICT_DELIMITER = ' '
     DICT_KEY_MAP = {
@@ -83,15 +82,15 @@
             for key2 in ['shortcut', 'type', 'relop', 'requestable', 'consumable', 'default', 'urgency', 'aapre',
                          'affinity', 'do_report', 'is_static']:
                 lines += ' %s' % (self.py_to_uge(key2, value_dict[key2], value_dict.get('default_is_bool', False)))
             lines += '\n'
         return lines
 
     def convert_data_to_uge_keywords(self, data):
-        for (data_key, value_dict) in list(data.items()):
+        for (_, value_dict) in list(data.items()):
             for (key, value) in list(value_dict.items()):
                 value_dict[key] = self.py_to_uge(key, value, value_dict.get('default_is_bool', False))
 
     def py_to_uge(self, key, value, default_is_bool=False):
         items = list(self.UGE_PYTHON_OBJECT_MAP.items())
         if key == 'default' and default_is_bool:
             items = list(self.UGE_PYTHON_BOOL_VALUE_MAP.items())
@@ -111,15 +110,15 @@
         if uge_type and uge_type in self.UGE_PYTHON_TYPE_MAP:
             py_value = self.UGE_PYTHON_TYPE_MAP[uge_type](value)
             return py_value
         return value
 
     def is_uge_value_bool(self, value):
         uppercase_value = value.upper()
-        for (uge_value, py_value) in list(self.UGE_PYTHON_BOOL_VALUE_MAP.items()):
+        for (uge_value, _) in list(self.UGE_PYTHON_BOOL_VALUE_MAP.items()):
             if uge_value == uppercase_value:
                 return True
         return False
 
     def to_dict(self, input_string):
         lines = input_string.split('\n')
         object_data = {}
```

### Comparing `uge-pycl-8.8.1/uge/objects/parallel_environment_v2_0.py` & `uge-pycl-8.9.0/uge/objects/parallel_environment_v2_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ParallelEnvironment(QconfObject):
     """ This class encapsulates UGE parallel environment object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = 'pe_name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['pe_name']
```

### Comparing `uge-pycl-8.8.1/uge/objects/cluster_queue_v1_0.py` & `uge-pycl-8.9.0/uge/objects/cluster_queue_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ClusterQueue(QconfObject):
     """ This class encapsulates UGE cluster queue object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'qname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['qname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/qconf_object.py` & `uge-pycl-8.9.0/uge/objects/qconf_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 import copy
 import datetime
 import json
 import os
 import tempfile
 
 from uge.config.config_manager import ConfigManager
@@ -150,15 +150,15 @@
         if self.OPTIONAL_KEYS_ALLOWED:
             return
 
         if type(self.data) != dict:
             raise InvalidRequest('Data object is not a dictionary: %s.' % str(self.data))
 
         removed_keys = []
-        for (key, value) in list(self.data.items()):
+        for (key, _) in list(self.data.items()):
             if key not in self.get_required_data_defaults():
                 if key not in self.USER_PROVIDED_KEYS and not key.startswith('#'):
                     removed_keys.append(key)
         for key in removed_keys:
             del self.data[key]
 
     def update_with_required_data_defaults(self):
@@ -279,16 +279,15 @@
                 return py_value
         if key in self.LIST_KEY_MAP:
             # Key is designated as list key.
             # Try to split by corresponding delimiter.
             delimiter = self.LIST_KEY_MAP.get(key)
             if value.find(delimiter) > 0:
                 return value.split(delimiter)
-            else:
-                return [value]
+            return [value]
         elif key in self.DICT_KEY_MAP:
             # Key is designated as dict key.
             # Try to split by corresponding delimiter.
             return self.parse_value_as_dict(key, value)
         elif key in self.INT_KEY_MAP:
             try:
                 return int(value)
```

### Comparing `uge-pycl-8.8.1/uge/objects/complex_configuration_v4_0.py` & `uge-pycl-8.9.0/uge/objects/complex_configuration_v4_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.complex_configuration_base import ComplexConfigurationBase
 
 
 class ComplexConfiguration(ComplexConfigurationBase):
     """ This class encapsulates UGE complex configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '4.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/__init__.py` & `uge-pycl-8.9.0/uge/cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
```

### Comparing `uge-pycl-8.8.1/uge/objects/complex_configuration_v1_0.py` & `uge-pycl-8.9.0/uge/objects/complex_configuration_v1_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from uge.objects.complex_configuration_base import ComplexConfigurationBase
 
 
 class ComplexConfiguration(ComplexConfigurationBase):
     """ This class encapsulates UGE complex configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/cluster_queue_v2_0.py` & `uge-pycl-8.9.0/uge/objects/cluster_queue_v2_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class ClusterQueue(QconfObject):
     """ This class encapsulates UGE cluster queue object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '2.0'
 
     #: Object name key.
     NAME_KEY = 'qname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['qname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/scheduler_configuration_v1_0.py` & `uge-pycl-8.9.0/uge/objects/scheduler_configuration_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class SchedulerConfiguration(QconfObject):
     """ This class encapsulates UGE scheduler configuration object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = None
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = []
```

### Comparing `uge-pycl-8.8.1/uge/objects/job_class_v4_0.py` & `uge-pycl-8.9.0/uge/objects/job_class_v4_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class JobClass(QconfObject):
     """ This class encapsulates UGE job class object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '4.0'
 
     #: Object name key.
     NAME_KEY = 'jcname'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['jcname']
```

### Comparing `uge-pycl-8.8.1/uge/objects/project_v1_0.py` & `uge-pycl-8.9.0/uge/objects/project_v1_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,22 +14,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 from .qconf_object import QconfObject
 
 
 class Project(QconfObject):
     """ This class encapsulates UGE project object. """
 
-    #: Object version. 
+    #: Object version.
     VERSION = '1.0'
 
     #: Object name key.
     NAME_KEY = 'name'
 
     #: Object keys that must be provided by user.
     USER_PROVIDED_KEYS = ['name']
```

### Comparing `uge-pycl-8.8.1/uge/config/config_manager.py` & `uge-pycl-8.9.0/uge/config/config_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-# 
+#
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,19 +14,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-# 
+#
 
 import os
 import pwd
 import socket
+from uge import __version__
 
 try:
     import UserDict
 except ImportError:
     import collections as UserDict
 try:
     import ConfigParser
@@ -117,25 +118,24 @@
     def __set_from_env_variable(self, key, env_var):
         """
         Set value for the specified key from a given environment variable.
         This functions ignores errors for env. variables that are not set.
         """
         try:
             self[key] = os.environ[env_var]
-        except:
+        except: # pylint: disable=bare-except
             pass
 
     # This function will ignore errors if variable file is not present.
     def __set_from_var_file(self, key, var_file):
         """
         Set value for the specified key from a given file. The first line
         in the file is variable value.
         This functions ignores errors.
         """
-
         if os.path.exists(var_file):
             with open(var_file) as v:
                 self[key] = v.readline().lstrip().rstrip()
 
     def __get_key_value(self, key, default='__internal__'):
         """
         Get value for a given key.
@@ -148,16 +148,18 @@
             default_value = default
         return self.get(key, default_value)
 
     def clear_config_parser(self):
         """ Clear config parser. """
         self.config_parser = None
 
-    def get_config_parser(self, defaults={}):
+    def get_config_parser(self, defaults=None):
         """ Return config parser, or none if config file cannot be found. """
+        if defaults is None:
+            defaults = {}
         if self.config_parser is None:
             config_file = self.get_config_file()
             self.config_parser = ConfigParser.ConfigParser(defaults)
             if os.path.exists(config_file):
                 self.config_parser.read(config_file)
         if self.config_parser is not None:
             self.config_parser.defaults = defaults
@@ -259,27 +261,29 @@
         Get log date (timestamp) format. If the log date format has not
         been set, the function will return the specified default value.
         If the default value is not specified, internal (predefined)
         default will be returned.
         """
         return self.__get_key_value('logDateFormat', default)
 
-    def set_config_defaults(self, defaults={}):
+    def set_config_defaults(self, defaults=None):
         """ Set configuration defaults. """
+        if defaults is None:
+            defaults = {}
         config_parser = self.get_config_parser()
         if config_parser is not None:
             config_parser.defaults = defaults
 
     def get_config_option(self, config_section, key, default_value=None):
         """ Get specified option from the configuration file. """
         config_parser = self.get_config_parser()
         if self.has_config_section(config_section):
             try:
                 return config_parser.get(config_section, key, raw=True)
-            except ConfigParser.NoOptionError as ex:
+            except ConfigParser.NoOptionError:
                 # ok, return default
                 pass
         return default_value
 
     def get_config_sections(self):
         """ Return a list of the sections from the config file """
         config_parser = self.get_config_parser()
@@ -296,20 +300,18 @@
 
     def get_config_items(self, config_section):
         """ Get available (key,value) pairs from the configuration file. """
         config_parser = self.get_config_parser()
         if config_parser is not None and \
                 config_parser.has_section(config_section):
             return config_parser.items(config_section)
-        else:
-            return []
+        return []
 
     def get_version(self):
         """ Get software version."""
-        from uge import __version__
         return __version__
 
 
 #############################################################################
 # Testing
 if __name__ == '__main__':
     cm1 = ConfigManager.get_instance()
```

### Comparing `uge-pycl-8.8.1/uge/config/__init__.py` & `uge-pycl-8.9.0/uge/objects/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# 
-# ___INFO__MARK_BEGIN__ 
+#
+# ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
-# ___INFO__MARK_END__ 
-# 
+# ___INFO__MARK_END__
+#
```

### Comparing `uge-pycl-8.8.1/uge_pycl.egg-info/SOURCES.txt` & `uge-pycl-8.9.0/uge_pycl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.8.1/uge_pycl.egg-info/PKG-INFO` & `uge-pycl-8.9.0/uge_pycl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: uge-pycl
-Version: 8.8.1
+Version: 8.9.0
 Summary: UGE Python Configuration Library
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
-Description: (c) Copyright 2016-2022 Altair Engineering Inc.
+Description: (c) Copyright 2016-2024 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
             use this file except in compliance with the License.
         
             You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `uge-pycl-8.8.1/PKG-INFO` & `uge-pycl-8.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: uge-pycl
-Version: 8.8.1
+Version: 8.9.0
 Summary: UGE Python Configuration Library
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
-Description: (c) Copyright 2016-2022 Altair Engineering Inc.
+Description: (c) Copyright 2016-2024 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
             use this file except in compliance with the License.
         
             You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `uge-pycl-8.8.1/test/test_ar.py` & `uge-pycl-8.9.0/test/test_ar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_job_class.py` & `uge-pycl-8.9.0/test/test_job_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_user.py` & `uge-pycl-8.9.0/test/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_project.py` & `uge-pycl-8.9.0/test/test_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_access_list.py` & `uge-pycl-8.9.0/test/test_access_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_share_tree.py` & `uge-pycl-8.9.0/test/test_share_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__ 
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_admin_host.py` & `uge-pycl-8.9.0/test/test_admin_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__ 
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_parallel_environment.py` & `uge-pycl-8.9.0/test/test_parallel_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_cluster_queue.py` & `uge-pycl-8.9.0/test/test_cluster_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_operator.py` & `uge-pycl-8.9.0/test/test_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_checkpointing_environment.py` & `uge-pycl-8.9.0/test/test_checkpointing_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_cluster_configuration.py` & `uge-pycl-8.9.0/test/test_cluster_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_submit_host.py` & `uge-pycl-8.9.0/test/test_submit_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_complex_configuration.py` & `uge-pycl-8.9.0/test/test_complex_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_resource_quota_set.py` & `uge-pycl-8.9.0/test/test_resource_quota_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_manager.py` & `uge-pycl-8.9.0/test/test_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_scheduler_configuration.py` & `uge-pycl-8.9.0/test/test_scheduler_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_host_group.py` & `uge-pycl-8.9.0/test/test_host_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_calendar.py` & `uge-pycl-8.9.0/test/test_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/test_execution_host.py` & `uge-pycl-8.9.0/test/test_execution_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/test/utils.py` & `uge-pycl-8.9.0/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # 
 # ___INFO__MARK_BEGIN__
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `uge-pycl-8.8.1/README.rst` & `uge-pycl-8.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-(c) Copyright 2016-2022 Altair Engineering Inc.
+(c) Copyright 2016-2024 Altair Engineering Inc.
     Licensed under the Apache License, Version 2.0 (the "License"); you may not
     use this file except in compliance with the License.
 
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `uge-pycl-8.8.1/setup.py` & `uge-pycl-8.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 
 # ___INFO__MARK_BEGIN__ 
 #######################################################################################
-# Copyright 2016-2022 Altair Engineering Inc.
+# Copyright 2016-2024 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

