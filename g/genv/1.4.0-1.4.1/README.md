# Comparing `tmp/genv-1.4.0.tar.gz` & `tmp/genv-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genv-1.4.0.tar", last modified: Sun Feb 18 16:31:32 2024, max compression
+gzip compressed data, was "genv-1.4.1.tar", last modified: Mon Apr 15 12:00:51 2024, max compression
```

## Comparing `genv-1.4.0.tar` & `genv-1.4.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.328279 genv-1.4.0/
--rw-r--r--   0 raz       (1001) raz       (1001)    34523 2022-12-27 17:45:39.000000 genv-1.4.0/LICENSE
--rw-r--r--   0 raz       (1001) raz       (1001)     4764 2024-02-18 16:31:32.328279 genv-1.4.0/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     4036 2024-02-18 16:28:21.000000 genv-1.4.0/README.md
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.320279 genv-1.4.0/genv/
--rw-r--r--   0 raz       (1001) raz       (1001)      318 2024-02-18 16:28:21.000000 genv-1.4.0/genv/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.321279 genv-1.4.0/genv/_ray/
--rw-r--r--   0 raz       (1001) raz       (1001)       27 2024-02-18 16:28:21.000000 genv-1.4.0/genv/_ray/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1737 2024-02-18 16:28:21.000000 genv-1.4.0/genv/_ray/remote.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.323279 genv-1.4.0/genv/cli/
--rw-r--r--   0 raz       (1001) raz       (1001)        0 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5444 2024-02-18 12:59:25.000000 genv-1.4.0/genv/cli/__main__.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2755 2024-02-14 12:55:54.000000 genv-1.4.0/genv/cli/activate.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/attach.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/config.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/deactivate.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/detach.py
--rw-r--r--   0 raz       (1001) raz       (1001)    10817 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3227 2023-06-21 17:25:32.000000 genv-1.4.0/genv/cli/enforce.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/envs.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/home.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     5367 2024-02-18 16:28:21.000000 genv-1.4.0/genv/cli/llm.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/lock.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2004 2024-02-11 16:13:17.000000 genv-1.4.0/genv/cli/monitor.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)    22328 2024-02-18 16:28:21.000000 genv-1.4.0/genv/cli/remote.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5133 2024-02-18 16:28:21.000000 genv-1.4.0/genv/cli/shell.py
--rw-r--r--   0 raz       (1001) raz       (1001)      892 2023-06-12 07:39:27.000000 genv-1.4.0/genv/cli/status.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2024-02-18 16:28:21.000000 genv-1.4.0/genv/cli/usage.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      307 2024-02-18 12:59:25.000000 genv-1.4.0/genv/cli/version.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.323279 genv-1.4.0/genv/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      143 2024-02-12 16:28:14.000000 genv-1.4.0/genv/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5677 2024-02-18 16:28:21.000000 genv-1.4.0/genv/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3703 2024-02-13 16:26:00.000000 genv-1.4.0/genv/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      894 2024-02-18 16:28:21.000000 genv-1.4.0/genv/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-06-12 07:39:27.000000 genv-1.4.0/genv/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1425 2024-02-08 16:53:09.000000 genv-1.4.0/genv/core/system.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1424 2023-06-12 07:39:27.000000 genv-1.4.0/genv/core/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.323279 genv-1.4.0/genv/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       49 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1288 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.324279 genv-1.4.0/genv/enforce/rules/
--rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/rules/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      864 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/rules/env_devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1394 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/rules/env_memory.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1449 2023-06-21 17:59:41.000000 genv-1.4.0/genv/enforce/rules/max_devices_per_user.py
--rw-r--r--   0 raz       (1001) raz       (1001)      642 2023-06-12 07:39:27.000000 genv-1.4.0/genv/enforce/rules/non_env_processes.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.324279 genv-1.4.0/genv/entities/
--rw-r--r--   0 raz       (1001) raz       (1001)      119 2024-02-08 13:14:41.000000 genv-1.4.0/genv/entities/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.324279 genv-1.4.0/genv/entities/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      165 2024-02-08 13:14:41.000000 genv-1.4.0/genv/entities/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     7231 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     6009 2024-02-18 16:28:21.000000 genv-1.4.0/genv/entities/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3484 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      982 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)      428 2024-02-08 13:14:41.000000 genv-1.4.0/genv/entities/core/system.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.324279 genv-1.4.0/genv/entities/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       54 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      270 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/enforce/report.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1126 2023-06-12 07:39:27.000000 genv-1.4.0/genv/entities/enforce/survey.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)      184 2024-02-06 09:11:01.000000 genv-1.4.0/genv/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4773 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.319279 genv-1.4.0/genv/metrics/export/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/export/grafana/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/export/grafana/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)    22349 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/export/grafana/dashboards/overview.json
--rw-r--r--   0 raz       (1001) raz       (1001)      182 2024-02-18 16:28:21.000000 genv-1.4.0/genv/metrics/export/grafana/grafana.ini
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.319279 genv-1.4.0/genv/metrics/export/grafana/provisioning/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/export/grafana/provisioning/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)      114 2023-06-12 07:39:27.000000 genv-1.4.0/genv/metrics/export/grafana/provisioning/dashboards/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/export/grafana/provisioning/datasources/
--rw-r--r--   0 raz       (1001) raz       (1001)      134 2023-06-12 07:39:27.000000 genv-1.4.0/genv/metrics/export/grafana/provisioning/datasources/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/metrics/export/prometheus/
--rw-r--r--   0 raz       (1001) raz       (1001)      155 2023-06-12 07:39:27.000000 genv-1.4.0/genv/metrics/export/prometheus/prometheus.yml
--rw-r--r--   0 raz       (1001) raz       (1001)      966 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/metric.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2663 2024-02-18 16:28:21.000000 genv-1.4.0/genv/metrics/publisher.py
--rw-r--r--   0 raz       (1001) raz       (1001)      846 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/spec.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4277 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/specs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      174 2024-02-08 13:14:41.000000 genv-1.4.0/genv/metrics/type.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/ray/
--rw-r--r--   0 raz       (1001) raz       (1001)       21 2023-07-04 15:54:42.000000 genv-1.4.0/genv/ray/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.325279 genv-1.4.0/genv/remote/
--rw-r--r--   0 raz       (1001) raz       (1001)       87 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.326279 genv-1.4.0/genv/remote/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      123 2024-02-08 13:14:41.000000 genv-1.4.0/genv/remote/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      381 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)      377 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      387 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      834 2024-02-18 16:28:21.000000 genv-1.4.0/genv/remote/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1530 2024-02-18 16:28:21.000000 genv-1.4.0/genv/remote/core/system.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.326279 genv-1.4.0/genv/remote/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      637 2024-02-18 16:28:21.000000 genv-1.4.0/genv/remote/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.326279 genv-1.4.0/genv/remote/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1523 2024-02-08 13:14:41.000000 genv-1.4.0/genv/remote/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.326279 genv-1.4.0/genv/remote/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)       40 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3206 2024-02-18 16:28:21.000000 genv-1.4.0/genv/remote/utils/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-06-12 07:39:27.000000 genv-1.4.0/genv/remote/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.327279 genv-1.4.0/genv/sdk/
--rw-r--r--   0 raz       (1001) raz       (1001)      272 2023-06-12 07:39:27.000000 genv-1.4.0/genv/sdk/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4132 2024-02-18 16:28:21.000000 genv-1.4.0/genv/sdk/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4280 2024-02-18 16:28:21.000000 genv-1.4.0/genv/sdk/env.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1300 2024-02-18 16:28:21.000000 genv-1.4.0/genv/sdk/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.327279 genv-1.4.0/genv/serialization/
--rw-r--r--   0 raz       (1001) raz       (1001)       44 2023-06-12 07:39:27.000000 genv-1.4.0/genv/serialization/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1803 2023-06-12 07:39:27.000000 genv-1.4.0/genv/serialization/json_.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.327279 genv-1.4.0/genv/shims/
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.4.0/genv/shims/docker
--rwxr-xr-x   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.4.0/genv/shims/nvidia-smi
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.328279 genv-1.4.0/genv/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)      107 2023-06-12 07:39:27.000000 genv-1.4.0/genv/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1393 2024-02-06 06:29:02.000000 genv-1.4.0/genv/utils/nvidia_smi.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3526 2024-02-18 16:28:21.000000 genv-1.4.0/genv/utils/os_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-06-12 07:39:27.000000 genv-1.4.0/genv/utils/poll.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.328279 genv-1.4.0/genv/utils/runners/
--rw-r--r--   0 raz       (1001) raz       (1001)       93 2023-06-12 07:39:27.000000 genv-1.4.0/genv/utils/runners/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      483 2024-02-08 13:14:41.000000 genv-1.4.0/genv/utils/runners/local.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1606 2024-02-08 13:14:41.000000 genv-1.4.0/genv/utils/runners/runner.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1543 2024-02-18 12:59:25.000000 genv-1.4.0/genv/utils/runners/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3446 2023-06-12 07:39:27.000000 genv-1.4.0/genv/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-02-18 16:31:32.321279 genv-1.4.0/genv.egg-info/
--rw-r--r--   0 raz       (1001) raz       (1001)     4764 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     2548 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/SOURCES.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        1 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/dependency_links.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       48 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/entry_points.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       94 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/requires.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        5 2024-02-18 16:31:32.000000 genv-1.4.0/genv.egg-info/top_level.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       38 2024-02-18 16:31:32.328279 genv-1.4.0/setup.cfg
--rw-r--r--   0 raz       (1001) raz       (1001)     1225 2024-02-18 16:28:47.000000 genv-1.4.0/setup.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/
+-rw-r--r--   0 raz       (1001) raz       (1001)    34523 2024-04-15 08:51:52.000000 genv-1.4.1/LICENSE
+-rw-r--r--   0 raz       (1001) raz       (1001)     7822 2024-04-15 12:00:51.506082 genv-1.4.1/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     7094 2024-04-15 12:00:19.000000 genv-1.4.1/README.md
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.499082 genv-1.4.1/genv/
+-rw-r--r--   0 raz       (1001) raz       (1001)      318 2024-04-15 12:00:19.000000 genv-1.4.1/genv/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.500082 genv-1.4.1/genv/_ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       27 2024-04-15 12:00:19.000000 genv-1.4.1/genv/_ray/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1737 2024-04-15 12:00:19.000000 genv-1.4.1/genv/_ray/remote.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.501082 genv-1.4.1/genv/cli/
+-rw-r--r--   0 raz       (1001) raz       (1001)        0 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5444 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/__main__.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2755 2024-02-14 12:55:54.000000 genv-1.4.1/genv/cli/activate.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/attach.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/config.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/deactivate.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/detach.py
+-rw-r--r--   0 raz       (1001) raz       (1001)    10817 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3227 2024-04-15 08:53:25.000000 genv-1.4.1/genv/cli/enforce.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/envs.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/home.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     6072 2024-04-15 11:53:54.000000 genv-1.4.1/genv/cli/llm.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.4.1/genv/cli/lock.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2004 2024-02-11 16:13:17.000000 genv-1.4.1/genv/cli/monitor.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)    22328 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/remote.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5133 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/shell.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      892 2024-04-15 08:53:35.000000 genv-1.4.1/genv/cli/status.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2024-04-15 12:00:19.000000 genv-1.4.1/genv/cli/usage.py
+-rwxrw-rw-   0 raz       (1001) raz       (1001)      307 2024-02-18 12:59:25.000000 genv-1.4.1/genv/cli/version.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      143 2024-04-15 08:53:40.000000 genv-1.4.1/genv/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5677 2024-04-15 12:00:19.000000 genv-1.4.1/genv/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3703 2024-04-15 08:53:45.000000 genv-1.4.1/genv/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      894 2024-04-15 12:00:19.000000 genv-1.4.1/genv/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      379 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1425 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/system.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1424 2024-04-15 08:54:06.000000 genv-1.4.1/genv/core/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       49 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1288 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/enforce/rules/
+-rw-r--r--   0 raz       (1001) raz       (1001)      176 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      864 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/env_devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1394 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/env_memory.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1449 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/max_devices_per_user.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      642 2024-04-15 08:54:06.000000 genv-1.4.1/genv/enforce/rules/non_env_processes.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.502082 genv-1.4.1/genv/entities/
+-rw-r--r--   0 raz       (1001) raz       (1001)      119 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/entities/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      165 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     7231 2024-04-15 08:54:06.000000 genv-1.4.1/genv/entities/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     6009 2024-04-15 12:00:19.000000 genv-1.4.1/genv/entities/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3484 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      982 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      428 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/core/system.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/entities/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       54 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      270 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/report.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1126 2024-04-15 08:54:16.000000 genv-1.4.1/genv/entities/enforce/survey.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)      184 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4773 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.498082 genv-1.4.1/genv/metrics/export/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)    22349 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/dashboards/overview.json
+-rw-r--r--   0 raz       (1001) raz       (1001)      182 2024-04-15 08:59:58.000000 genv-1.4.1/genv/metrics/export/grafana/grafana.ini
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.498082 genv-1.4.1/genv/metrics/export/grafana/provisioning/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.503082 genv-1.4.1/genv/metrics/export/grafana/provisioning/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)      114 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/provisioning/dashboards/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/metrics/export/grafana/provisioning/datasources/
+-rw-r--r--   0 raz       (1001) raz       (1001)      134 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/grafana/provisioning/datasources/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/metrics/export/prometheus/
+-rw-r--r--   0 raz       (1001) raz       (1001)      155 2024-04-15 08:54:38.000000 genv-1.4.1/genv/metrics/export/prometheus/prometheus.yml
+-rw-r--r--   0 raz       (1001) raz       (1001)      966 2024-04-15 08:54:23.000000 genv-1.4.1/genv/metrics/metric.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2663 2024-04-15 12:00:19.000000 genv-1.4.1/genv/metrics/publisher.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      846 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/spec.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4277 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/specs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      174 2024-04-15 08:54:29.000000 genv-1.4.1/genv/metrics/type.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       21 2024-04-15 08:54:48.000000 genv-1.4.1/genv/ray/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/
+-rw-r--r--   0 raz       (1001) raz       (1001)       87 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      123 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      381 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      377 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      387 2024-04-15 08:54:48.000000 genv-1.4.1/genv/remote/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      834 2024-04-15 09:00:02.000000 genv-1.4.1/genv/remote/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1530 2024-04-15 09:00:05.000000 genv-1.4.1/genv/remote/core/system.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.504082 genv-1.4.1/genv/remote/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2024-04-15 08:54:55.000000 genv-1.4.1/genv/remote/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      637 2024-04-15 09:00:08.000000 genv-1.4.1/genv/remote/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/remote/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)       35 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1523 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/remote/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)       40 2024-04-15 08:55:02.000000 genv-1.4.1/genv/remote/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3206 2024-04-15 12:00:19.000000 genv-1.4.1/genv/remote/utils/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      515 2024-04-15 08:55:09.000000 genv-1.4.1/genv/remote/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/sdk/
+-rw-r--r--   0 raz       (1001) raz       (1001)      272 2024-04-15 08:55:09.000000 genv-1.4.1/genv/sdk/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4132 2024-04-15 09:00:29.000000 genv-1.4.1/genv/sdk/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4280 2024-04-15 12:00:19.000000 genv-1.4.1/genv/sdk/env.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1300 2024-04-15 12:00:19.000000 genv-1.4.1/genv/sdk/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/serialization/
+-rw-r--r--   0 raz       (1001) raz       (1001)       44 2024-04-15 08:55:20.000000 genv-1.4.1/genv/serialization/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1803 2024-04-15 08:55:20.000000 genv-1.4.1/genv/serialization/json_.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.505082 genv-1.4.1/genv/shims/
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.4.1/genv/shims/docker
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.4.1/genv/shims/nvidia-smi
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/genv/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)      107 2024-04-15 08:55:20.000000 genv-1.4.1/genv/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1393 2024-04-15 08:55:20.000000 genv-1.4.1/genv/utils/nvidia_smi.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3526 2024-04-15 12:00:19.000000 genv-1.4.1/genv/utils/os_.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1253 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/poll.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.506082 genv-1.4.1/genv/utils/runners/
+-rw-r--r--   0 raz       (1001) raz       (1001)       93 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      483 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/local.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1606 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/runner.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1543 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/runners/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3446 2024-04-15 08:55:33.000000 genv-1.4.1/genv/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2024-04-15 12:00:51.500082 genv-1.4.1/genv.egg-info/
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     7822 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/PKG-INFO
+-rwxrw-rw-   0 raz       (1001) raz       (1001)     2548 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/SOURCES.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)        1 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/dependency_links.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)       48 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/entry_points.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)       94 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/requires.txt
+-rwxrw-rw-   0 raz       (1001) raz       (1001)        5 2024-04-15 12:00:51.000000 genv-1.4.1/genv.egg-info/top_level.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       38 2024-04-15 12:00:51.506082 genv-1.4.1/setup.cfg
+-rw-r--r--   0 raz       (1001) raz       (1001)     1225 2024-04-15 11:57:43.000000 genv-1.4.1/setup.py
```

### Comparing `genv-1.4.0/LICENSE` & `genv-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/_ray/remote.py` & `genv-1.4.1/genv/_ray/remote.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/__main__.py` & `genv-1.4.1/genv/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/activate.py` & `genv-1.4.1/genv/cli/activate.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/attach.py` & `genv-1.4.1/genv/cli/attach.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/config.py` & `genv-1.4.1/genv/cli/config.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/deactivate.py` & `genv-1.4.1/genv/cli/deactivate.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/devices.py` & `genv-1.4.1/genv/cli/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/enforce.py` & `genv-1.4.1/genv/cli/enforce.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/envs.py` & `genv-1.4.1/genv/cli/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/home.py` & `genv-1.4.1/genv/cli/home.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/llm.py` & `genv-1.4.1/genv/cli/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import argparse
 import os
+import re
+import socket
 import shutil
 from typing import Iterable, NoReturn, Optional
 
 import psutil
 
 from genv.entities import Env
 import genv.sdk
 
 
 def _find_port(env: Env) -> Optional[int]:
     """Finds any port an LLM server environment listens on."""
 
+    match = re.match(r"^llm/[^/]+/(\d+)$", env.config.name)
+    if match:
+        return int(match.group(1))
+
+    # this is a fallback for environments that were ran before 1.4.1
     for pid in env.pids:
         try:
             ports = genv.utils.get_process_listen_ports(pid)
 
             if len(ports) > 0:
                 return ports[0]
         except psutil.NoSuchProcess:
             continue
 
 
+def _find_available_port() -> int:
+    """Finds an available port to listen on."""
+
+    with socket.socket() as sock:
+        sock.bind(("", 0))
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return sock.getsockname()[1]
+
+
 def _exec_ollama(args: Iterable[str], host: str, port: int) -> NoReturn:
     """
     Executes ollama.
     Raises RuntimeError if ollama is not properly installed.
 
     :param args: Arguments to pass to ollama.
     :param host: Hostname to pass to ollama.
@@ -52,15 +68,24 @@
 
     :param model: Model name.
     """
 
     with genv.utils.global_lock():
         envs = genv.core.envs.snapshot()
 
-    for env in envs.filter(name=f"llm/{model}"):
+    for env in envs:
+        if not env.config.name:
+            continue
+
+        if not (
+            env.config.name.startswith(f"llm/{model}/")
+            or env.config.name == f"llm/{model}"  # before 1.4.1
+        ):
+            continue
+
         port = _find_port(env)
 
         if port:
             # TODO(raz): we currently attach to the first replica; we should pick a replica in a smarter way.
             _exec_ollama(["run", model], host="localhost", port=port)
 
     raise RuntimeError(f"Could not find LLM model '{model}'")
@@ -87,34 +112,41 @@
                 "MODEL       PORT    CREATED              EID     USER            PID(S)"
             )
 
     for env in envs:
         if not (env.config.name and env.config.name.startswith("llm/")):
             continue
 
-        model = env.config.name.split("llm/")[1]
+        model = env.config.name.split("/")[1]
         port = _find_port(env) or "N/A"
         created = env.creation if timestamp else genv.utils.time_since(env.creation)
         eid = env.eid
         user = f"{env.username}({env.uid})" if env.username else env.uid
         pids = " ".join(str(pid) for pid in env.pids)
 
         if format == "csv":
             print(f"{model},{port},{created},{eid},{user}{pids}")
         elif format == "tui":
             print(f"{model:<12}{port:<8}{created:<21}{eid:<8}{user:<16}{pids}")
 
 
 def do_serve(
-    model: str, host: str, port: int, gpus: Optional[int], gpu_memory: Optional[str]
+    model: str,
+    host: str,
+    port: Optional[int],
+    gpus: Optional[int],
+    gpu_memory: Optional[str],
 ) -> NoReturn:
     """Runs an LLM server in a newly created environment."""
 
+    if not port:
+        port = _find_available_port()
+
     with genv.sdk.env.activate(
-        config=Env.Config(name=f"llm/{model}", gpus=gpus, gpu_memory=gpu_memory)
+        config=Env.Config(name=f"llm/{model}/{port}", gpus=gpus, gpu_memory=gpu_memory)
     ):
         _exec_ollama(["serve"], host=host, port=port)
 
 
 def add_arguments(parser: argparse.ArgumentParser) -> None:
     """
     Adds "genv llm" arguments to a parser.
@@ -145,17 +177,15 @@
     def serve(parser):
         parser.add_argument("model")
 
         configuration = parser.add_argument_group("configuration")
         configuration.add_argument(
             "--host", default="127.0.0.1", help="Network interface to bind"
         )
-        configuration.add_argument(
-            "-p", "--port", type=int, default=0, help="Port to bind"
-        )
+        configuration.add_argument("-p", "--port", type=int, help="Port to bind")
 
         env = parser.add_argument_group("env")
         env.add_argument("--gpus", type=int, help="Device count")
         env.add_argument("--gpu-memory", help="Device memory capacity (e.g. 4g)")
 
     for command, help in [
         (attach, "Attach to a running LLM model"),
```

### Comparing `genv-1.4.0/genv/cli/lock.py` & `genv-1.4.1/genv/cli/lock.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/monitor.py` & `genv-1.4.1/genv/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/remote.py` & `genv-1.4.1/genv/cli/remote.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/shell.py` & `genv-1.4.1/genv/cli/shell.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/status.py` & `genv-1.4.1/genv/cli/status.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/cli/usage.py` & `genv-1.4.1/genv/cli/usage.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/core/devices.py` & `genv-1.4.1/genv/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/core/envs.py` & `genv-1.4.1/genv/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/core/processes.py` & `genv-1.4.1/genv/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/core/system.py` & `genv-1.4.1/genv/core/system.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/core/utils.py` & `genv-1.4.1/genv/core/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/enforce/execute.py` & `genv-1.4.1/genv/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/enforce/rules/env_devices.py` & `genv-1.4.1/genv/enforce/rules/env_devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/enforce/rules/env_memory.py` & `genv-1.4.1/genv/enforce/rules/env_memory.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/enforce/rules/max_devices_per_user.py` & `genv-1.4.1/genv/enforce/rules/max_devices_per_user.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/enforce/rules/non_env_processes.py` & `genv-1.4.1/genv/enforce/rules/non_env_processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/entities/core/devices.py` & `genv-1.4.1/genv/entities/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/entities/core/envs.py` & `genv-1.4.1/genv/entities/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/entities/core/processes.py` & `genv-1.4.1/genv/entities/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/entities/core/snapshot.py` & `genv-1.4.1/genv/entities/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/entities/enforce/survey.py` & `genv-1.4.1/genv/entities/enforce/survey.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/collection.py` & `genv-1.4.1/genv/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/export/grafana/dashboards/overview.json` & `genv-1.4.1/genv/metrics/export/grafana/dashboards/overview.json`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/metric.py` & `genv-1.4.1/genv/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/publisher.py` & `genv-1.4.1/genv/metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/spec.py` & `genv-1.4.1/genv/metrics/spec.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/metrics/specs.py` & `genv-1.4.1/genv/metrics/specs.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/core/snapshot.py` & `genv-1.4.1/genv/remote/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/core/system.py` & `genv-1.4.1/genv/remote/core/system.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/enforce/execute.py` & `genv-1.4.1/genv/remote/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/metrics/collection.py` & `genv-1.4.1/genv/remote/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/utils/ssh.py` & `genv-1.4.1/genv/remote/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/remote/utils/utils.py` & `genv-1.4.1/genv/remote/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/sdk/devices.py` & `genv-1.4.1/genv/sdk/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/sdk/env.py` & `genv-1.4.1/genv/sdk/env.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/sdk/utils.py` & `genv-1.4.1/genv/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/serialization/json_.py` & `genv-1.4.1/genv/serialization/json_.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/shims/docker` & `genv-1.4.1/genv/shims/docker`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/shims/nvidia-smi` & `genv-1.4.1/genv/shims/nvidia-smi`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/nvidia_smi.py` & `genv-1.4.1/genv/utils/nvidia_smi.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/os_.py` & `genv-1.4.1/genv/utils/os_.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/poll.py` & `genv-1.4.1/genv/utils/poll.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/runners/runner.py` & `genv-1.4.1/genv/utils/runners/runner.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/runners/ssh.py` & `genv-1.4.1/genv/utils/runners/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv/utils/utils.py` & `genv-1.4.1/genv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/genv.egg-info/SOURCES.txt` & `genv-1.4.1/genv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genv-1.4.0/setup.py` & `genv-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="genv",
-    version="1.4.0",
+    version="1.4.1",
     author="Run.ai",
     author_email="pypi@run.ai",
     description="GPU environment and cluster management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/run-ai/genv",
     packages=setuptools.find_packages(),
```

