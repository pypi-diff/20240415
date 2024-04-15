# Comparing `tmp/spaceone-monitoring-2.0.dev8.tar.gz` & `tmp/spaceone-monitoring-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-monitoring-2.0.dev8.tar", last modified: Wed Dec 20 21:49:58 2023, max compression
+gzip compressed data, was "spaceone-monitoring-2.0.dev9.tar", last modified: Thu Dec 21 10:54:11 2023, max compression
```

## Comparing `spaceone-monitoring-2.0.dev8.tar` & `spaceone-monitoring-2.0.dev9.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.887457 spaceone-monitoring-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-20 21:49:58.887457 spaceone-monitoring-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 21:49:58.887457 spaceone-monitoring-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.871457 spaceone-monitoring-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.871457 spaceone-monitoring-2.0.dev8/spaceone/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.871457 spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/default_escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/router_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.871457 spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/datasource_plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/webhook_plugin_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.871457 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/event_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/project_alert_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/alert_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/data_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/escalation_policy_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/event_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/event_rule_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/log_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/metric_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/note_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/project_alert_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/webhook_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/event_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/project_alert_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/v1/monitoring_alert_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.875458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.879458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/alert_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/data_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/data_source_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/escalation_policy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/event_rule_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/inventory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/note_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/project_alert_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/repository_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/webhook_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/webhook_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.879458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/alert_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/data_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/escalation_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/event_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/event_rule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/note_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/plugin_metadata_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/project_alert_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/webhook_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/lib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/event/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/event/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/webhook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/webhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/webhook/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/webhook/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/webhook_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.883458 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/skeleton/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.887457 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/alert_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/data_source_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/escalation_policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14846 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/event_rule_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17668 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/note_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/project_alert_config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2023-12-20 21:49:51.000000 spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/webhook_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 21:49:58.887457 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-20 21:49:58.000000 spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.413227 spaceone-monitoring-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-21 10:54:11.413227 spaceone-monitoring-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 10:54:11.413227 spaceone-monitoring-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.393227 spaceone-monitoring-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.393227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.393227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/default_escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/router_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.393227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/datasource_plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/webhook_plugin_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.397227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/project_alert_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.397227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/alert_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/data_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/escalation_policy_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/event_rule_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/log_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/metric_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/note_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/project_alert_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/webhook_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.397227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.397227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/project_alert_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/v1/monitoring_alert_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.401227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/alert_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/data_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/data_source_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/escalation_policy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/event_rule_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/inventory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/note_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/project_alert_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/repository_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/webhook_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/webhook_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/alert_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/data_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/escalation_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/event_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/event_rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/note_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/plugin_metadata_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/project_alert_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/webhook_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/lib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.405227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/event/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/event/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.409227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/webhook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/webhook/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/webhook/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.409227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/webhook_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.409227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/skeleton/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.409227 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/alert_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14284 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/data_source_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/escalation_policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14846 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/event_rule_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17668 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/note_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/project_alert_config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2023-12-21 10:54:02.000000 spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/webhook_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:54:11.409227 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-21 10:54:11.000000 spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/top_level.txt
```

### Comparing `spaceone-monitoring-2.0.dev8/setup.py` & `spaceone-monitoring-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/conf/global_conf.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/datasource_plugin_connector.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/datasource_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/connector/webhook_plugin_connector.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/connector/webhook_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/alert.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/alert.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/data_source.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/data_source.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/error/metric.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/error/metric.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/__init__.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/alert_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/alert_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/data_source_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/data_source_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/escalation_policy_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/escalation_policy_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/event_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/event_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/event_rule_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/event_rule_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/metric_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/metric_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/note_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/note_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/project_alert_config_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/project_alert_config_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/info/webhook_info.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/info/webhook_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/__init__.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/alert.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/alert.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/data_source.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/data_source.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/escalation_policy.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/escalation_policy.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/event.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/event.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/event_rule.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/event_rule.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/metric.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/metric.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/note.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/note.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/project_alert_config.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/project_alert_config.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/grpc/webhook.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/grpc/webhook.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/alert.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/alert.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/rest/v1/event.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/rest/v1/event.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/interface/task/v1/monitoring_alert_scheduler.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/interface/task/v1/monitoring_alert_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/__init__.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/alert_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/alert_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/data_source_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/data_source_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/data_source_plugin_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/data_source_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/escalation_policy_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/escalation_policy_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/event_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/event_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/event_rule_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/event_rule_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/identity_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/inventory_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/inventory_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/job_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/note_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/note_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/notification_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/notification_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/plugin_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/project_alert_config_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/project_alert_config_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/repository_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/secret_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/webhook_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/webhook_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/manager/webhook_plugin_manager.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/manager/webhook_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/__init__.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/alert_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/alert_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/data_source_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/data_source_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/escalation_policy_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/escalation_policy_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/event_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/event_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/event_rule_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/event_rule_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/job_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/job_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/note_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/note_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/plugin_metadata_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/plugin_metadata_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/project_alert_config_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/project_alert_config_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/model/webhook_model.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/model/webhook_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/event.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/event.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/interface/grpc/webhook.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/interface/grpc/webhook.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/lib/server.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/lib/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/model/event/response.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/model/event/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/event_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/event_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/service/webhook_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/service/webhook_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/plugin/webhook/skeleton/main.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/plugin/webhook/skeleton/main.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/__init__.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/alert_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/alert_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/data_source_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/data_source_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/escalation_policy_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/escalation_policy_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/event_rule_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/event_rule_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/event_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/event_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/job_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/job_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/log_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/log_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/metric_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/note_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/note_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/project_alert_config_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/project_alert_config_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone/monitoring/service/webhook_service.py` & `spaceone-monitoring-2.0.dev9/spaceone/monitoring/service/webhook_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-monitoring-2.0.dev8/spaceone_monitoring.egg-info/SOURCES.txt` & `spaceone-monitoring-2.0.dev9/spaceone_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

