# Comparing `tmp/ecs_composex-1.1.0rc1.tar.gz` & `tmp/ecs_composex-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_composex-1.1.0rc1.tar", max compression
+gzip compressed data, was "ecs_composex-1.1.0rc2.tar", max compression
```

## Comparing `ecs_composex-1.1.0rc1.tar` & `ecs_composex-1.1.0rc2.tar`

### file list

```diff
@@ -1,370 +1,370 @@
--rw-r--r--   0        0        0    16725 2021-05-14 10:51:20.077071 ecs_composex-1.1.0rc1/LICENSE
--rw-r--r--   0        0        0      385 2022-06-16 18:49:16.792466 ecs_composex-1.1.0rc1/MANIFEST.in
--rw-r--r--   0        0        0     1068 2023-08-07 12:54:52.746417 ecs_composex-1.1.0rc1/NOTICES.rst
--rw-r--r--   0        0        0     6976 2023-01-11 09:54:17.357527 ecs_composex-1.1.0rc1/README.rst
--rw-r--r--   0        0        0       19 2021-03-04 09:40:13.458136 ecs_composex-1.1.0rc1/ecs_composex/.gitignore
--rw-r--r--   0        0        0      222 2024-03-31 16:06:38.942101 ecs_composex-1.1.0rc1/ecs_composex/__init__.py
--rw-r--r--   0        0        0      117 2024-03-23 20:44:00.309060 ecs_composex-1.1.0rc1/ecs_composex/acm/__init__.py
--rw-r--r--   0        0        0      419 2024-03-23 20:44:00.401059 ecs_composex-1.1.0rc1/ecs_composex/acm/acm_module.py
--rw-r--r--   0        0        0     1546 2024-03-23 20:44:00.178062 ecs_composex-1.1.0rc1/ecs_composex/acm/acm_params.py
--rw-r--r--   0        0        0     5773 2024-03-23 20:44:00.185062 ecs_composex-1.1.0rc1/ecs_composex/acm/acm_stack.py
--rw-r--r--   0        0        0     7634 2024-03-23 20:44:00.125063 ecs_composex-1.1.0rc1/ecs_composex/acm/acm_stack_helpers.py
--rw-r--r--   0        0        0     1327 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/acm/x-acm.spec.json
--rw-r--r--   0        0        0      416 2024-03-23 20:44:00.390059 ecs_composex-1.1.0rc1/ecs_composex/alarms/__init__.py
--rw-r--r--   0        0        0     9162 2024-03-23 20:44:00.121063 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_ecs.py
--rw-r--r--   0        0        0     6292 2024-03-23 20:44:00.005065 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_elbv2.py
--rw-r--r--   0        0        0     8575 2024-03-23 20:43:59.927066 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_helpers.py
--rw-r--r--   0        0        0      416 2024-03-23 20:44:00.139063 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_module.py
--rw-r--r--   0        0        0      532 2024-03-23 20:44:00.388059 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_params.py
--rw-r--r--   0        0        0     4520 2024-03-23 20:43:59.894066 ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_stack.py
--rw-r--r--   0        0        0     1920 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/alarms/x-alarms.spec.json
--rw-r--r--   0        0        0       44 2022-06-16 18:49:16.909464 ecs_composex-1.1.0rc1/ecs_composex/appmesh/README.rst
--rw-r--r--   0        0        0      288 2024-03-23 20:44:00.220061 ecs_composex-1.1.0rc1/ecs_composex/appmesh/__init__.py
--rw-r--r--   0        0        0     2268 2024-03-23 20:43:59.826068 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_aws.py
--rw-r--r--   0        0        0     1479 2024-03-23 20:44:00.369059 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_conditions.py
--rw-r--r--   0        0        0     9620 2024-03-23 20:44:00.022064 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_mesh.py
--rw-r--r--   0        0        0    12953 2024-03-23 20:44:00.203061 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_node.py
--rw-r--r--   0        0        0     1222 2024-03-23 20:43:59.819068 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_params.py
--rw-r--r--   0        0        0    10944 2024-03-23 20:44:00.127063 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_router.py
--rw-r--r--   0        0        0     6917 2024-03-23 20:44:00.367059 ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_service.py
--rw-r--r--   0        0        0     4576 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/appmesh/x-appmesh.spec.json
--rw-r--r--   0        0        0      121 2024-03-23 20:43:59.931066 ecs_composex-1.1.0rc1/ecs_composex/aps/__init__.py
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.240061 ecs_composex-1.1.0rc1/ecs_composex/aps/aps_module.py
--rw-r--r--   0        0        0      938 2024-03-23 20:44:00.136062 ecs_composex-1.1.0rc1/ecs_composex/aps/aps_parameters.py
--rw-r--r--   0        0        0      492 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/aps/aps_perms.json
--rw-r--r--   0        0        0     7896 2024-03-23 20:44:00.467057 ecs_composex-1.1.0rc1/ecs_composex/aps/aps_stack.py
--rw-r--r--   0        0        0     1219 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/aps/x-aps.spec.json
--rw-r--r--   0        0        0     6802 2024-03-23 20:44:00.151062 ecs_composex-1.1.0rc1/ecs_composex/cli.py
--rw-r--r--   0        0        0      481 2024-03-23 20:44:00.271061 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/__init__.py
--rw-r--r--   0        0        0     7347 2024-03-23 20:44:00.090063 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_ecs.py
--rw-r--r--   0        0        0     5364 2024-03-23 20:43:59.853067 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_helpers.py
--rw-r--r--   0        0        0      481 2024-03-23 20:43:59.986065 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_module.py
--rw-r--r--   0        0        0     2100 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_params.py
--rw-r--r--   0        0        0    12308 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_stack.py
--rw-r--r--   0        0        0     7790 2024-03-23 20:43:59.886067 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_x_resources.py
--rw-r--r--   0        0        0     1486 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/cloudmap/x-cloudmap.spec.json
--rw-r--r--   0        0        0      500 2024-03-23 20:44:00.107063 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/__init__.py
--rw-r--r--   0        0        0     1761 2024-03-23 20:44:00.321060 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py
--rw-r--r--   0        0        0      500 2024-03-23 20:44:00.359059 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_module.py
--rw-r--r--   0        0        0      603 2024-03-23 20:44:00.419058 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_params.py
--rw-r--r--   0        0        0      188 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_perms.json
--rw-r--r--   0        0        0     5053 2024-03-23 20:43:59.897066 ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py
--rw-r--r--   0        0        0      489 2024-03-23 20:44:00.009065 ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/__init__.py
--rw-r--r--   0        0        0      909 2024-03-23 20:43:59.840067 ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/cognito_params.py
--rw-r--r--   0        0        0      489 2024-03-23 20:43:59.828067 ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/cognito_userpool_module.py
--rw-r--r--   0        0        0     4821 2024-03-23 20:43:59.961065 ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/cognito_userpool_stack.py
--rw-r--r--   0        0        0      375 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/x-cognito_userpool.spec.json
--rw-r--r--   0        0        0     2314 2024-03-23 20:44:00.088063 ecs_composex-1.1.0rc1/ecs_composex/common/__init__.py
--rw-r--r--   0        0        0    13821 2024-03-23 20:43:59.947065 ecs_composex-1.1.0rc1/ecs_composex/common/aws.py
--rw-r--r--   0        0        0     1209 2024-03-23 20:44:00.432058 ecs_composex-1.1.0rc1/ecs_composex/common/cfn_conditions.py
--rw-r--r--   0        0        0     1258 2024-03-23 20:43:59.901066 ecs_composex-1.1.0rc1/ecs_composex/common/cfn_params.py
--rw-r--r--   0        0        0      408 2024-03-23 20:44:00.103063 ecs_composex-1.1.0rc1/ecs_composex/common/ecs_composex.py
--rw-r--r--   0        0        0     1465 2024-03-23 22:36:48.972815 ecs_composex-1.1.0rc1/ecs_composex/common/envsubst.py
--rw-r--r--   0        0        0     9180 2024-03-23 20:43:59.971065 ecs_composex-1.1.0rc1/ecs_composex/common/files.py
--rw-r--r--   0        0        0     1937 2024-03-23 20:43:59.921066 ecs_composex-1.1.0rc1/ecs_composex/common/logging.py
--rw-r--r--   0        0        0    24735 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc1/ecs_composex/common/settings.py
--rw-r--r--   0        0        0    14081 2024-03-23 20:44:00.463057 ecs_composex-1.1.0rc1/ecs_composex/common/stacks/__init__.py
--rw-r--r--   0        0        0     8705 2024-03-23 20:44:00.333059 ecs_composex-1.1.0rc1/ecs_composex/common/tagging.py
--rw-r--r--   0        0        0    10189 2024-03-23 20:43:59.845067 ecs_composex-1.1.0rc1/ecs_composex/common/troposphere_tools.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.277060 ecs_composex-1.1.0rc1/ecs_composex/compose/__init__.py
--rw-r--r--   0        0        0     1629 2024-03-23 20:44:00.131063 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_networks.py
--rw-r--r--   0        0        0     9238 2024-03-23 20:44:00.042064 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/__init__.py
--rw-r--r--   0        0        0     3632 2024-03-23 20:44:00.229061 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/ecs_family_helpers.py
--rw-r--r--   0        0        0     1490 2024-03-23 20:44:00.222061 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/helpers.py
--rw-r--r--   0        0        0     1292 2024-03-23 20:44:00.227061 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/services_helpers.py
--rw-r--r--   0        0        0    37531 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/__init__.py
--rw-r--r--   0        0        0     6697 2024-03-23 20:43:59.903066 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/docker_tools.py
--rw-r--r--   0        0        0     3399 2024-03-23 20:44:00.001065 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/env_files_helpers.py
--rw-r--r--   0        0        0     9848 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/helpers.py
--rw-r--r--   0        0        0     3658 2024-03-23 20:44:00.275061 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/kernel_options_helpers.py
--rw-r--r--   0        0        0     8042 2024-03-23 20:44:00.129063 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/__init__.py
--rw-r--r--   0        0        0     2719 2024-03-23 20:44:00.375059 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/docker_opts.py
--rw-r--r--   0        0        0     3911 2024-03-23 20:43:59.892066 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/ecr_helpers.py
--rw-r--r--   0        0        0    10829 2024-03-23 20:44:00.167062 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py
--rw-r--r--   0        0        0     5119 2024-03-23 20:44:00.261061 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_logging/__init__.py
--rw-r--r--   0        0        0     5036 2024-03-23 20:43:59.855067 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_logging/helpers.py
--rw-r--r--   0        0        0     3873 2024-03-23 20:43:59.983065 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/__init__.py
--rw-r--r--   0        0        0     6846 2024-03-23 20:44:00.069064 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/ecs_family_helpers.py
--rw-r--r--   0        0        0     1459 2024-03-23 20:44:00.331060 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/helpers.py
--rw-r--r--   0        0        0     5651 2024-03-23 20:44:00.096063 ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/services_helpers.py
--rw-r--r--   0        0        0    30750 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/__init__.py
--rw-r--r--   0        0        0     1672 2024-03-23 20:43:59.911066 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/api_x_resources.py
--rw-r--r--   0        0        0      922 2024-03-23 20:44:00.461058 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/environment_x_resources.py
--rw-r--r--   0        0        0     4657 2024-03-23 20:44:00.123063 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/helpers.py
--rw-r--r--   0        0        0     6435 2024-03-23 20:44:00.048064 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/network_x_resources.py
--rw-r--r--   0        0        0     8806 2024-03-23 20:43:59.838067 ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/services_resources.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.017064 ecs_composex-1.1.0rc1/ecs_composex/dashboards/__init__.py
--rw-r--r--   0        0        0      472 2024-03-23 20:43:59.842067 ecs_composex-1.1.0rc1/ecs_composex/dashboards/dashboards_module.py
--rw-r--r--   0        0        0     5539 2024-03-23 20:44:00.329059 ecs_composex-1.1.0rc1/ecs_composex/dashboards/dashboards_services_metrics.py
--rw-r--r--   0        0        0     4831 2024-03-23 20:44:00.035064 ecs_composex-1.1.0rc1/ecs_composex/dashboards/dashboards_stack.py
--rw-r--r--   0        0        0     1224 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/dashboards/x-dashboards.spec.json
--rw-r--r--   0        0        0      413 2024-03-23 20:44:00.259061 ecs_composex-1.1.0rc1/ecs_composex/docdb/__init__.py
--rw-r--r--   0        0        0      413 2024-03-23 20:43:59.915066 ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_module.py
--rw-r--r--   0        0        0      833 2024-03-23 20:44:00.346059 ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_params.py
--rw-r--r--   0        0        0      164 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_perms.json
--rw-r--r--   0        0        0     7772 2024-03-23 20:43:59.876067 ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_stack.py
--rw-r--r--   0        0        0     6450 2024-03-23 20:44:00.063064 ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_template.py
--rw-r--r--   0        0        0     2241 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/docdb/x-docdb.spec.json
--rw-r--r--   0        0        0      289 2024-03-23 20:44:00.046064 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/__init__.py
--rw-r--r--   0        0        0     7795 2024-03-23 20:44:00.248061 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_autoscaling.py
--rw-r--r--   0        0        0      422 2024-03-23 20:44:00.117063 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_module.py
--rw-r--r--   0        0        0      412 2024-03-23 20:43:59.966065 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_params.py
--rw-r--r--   0        0        0     1096 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_perms.json
--rw-r--r--   0        0        0     4131 2024-03-23 20:44:00.355059 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_stack.py
--rw-r--r--   0        0        0     2916 2024-03-23 20:44:00.075064 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_template.py
--rw-r--r--   0        0        0     2777 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/dynamodb/x-dynamodb.spec.json
--rw-r--r--   0        0        0     1050 2024-03-23 20:44:00.094063 ecs_composex-1.1.0rc1/ecs_composex/ecs/__init__.py
--rw-r--r--   0        0        0     3532 2024-03-23 20:43:59.955065 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_conditions.py
--rw-r--r--   0        0        0    27633 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/__init__.py
--rw-r--r--   0        0        0    14849 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/__init__.py
--rw-r--r--   0        0        0     1316 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py
--rw-r--r--   0        0        0     1912 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py
--rw-r--r--   0        0        0     8788 2024-03-23 20:43:59.870067 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_logging/__init__.py
--rw-r--r--   0        0        0     4123 2024-03-23 20:44:00.061064 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py
--rw-r--r--   0        0        0     2940 2024-03-23 20:43:59.880066 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_template.py
--rw-r--r--   0        0        0     3502 2024-03-23 20:43:59.861067 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/task_execute_command.py
--rw-r--r--   0        0        0     2626 2024-03-23 20:44:00.015065 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/task_runtime.py
--rw-r--r--   0        0        0      163 2024-03-23 20:44:00.381059 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/__init__.py
--rw-r--r--   0        0        0    10598 2024-03-23 20:43:59.949066 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py
--rw-r--r--   0        0        0     5822 2024-03-23 20:44:00.098063 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py
--rw-r--r--   0        0        0     5548 2024-03-23 20:44:00.282060 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py
--rw-r--r--   0        0        0     3067 2024-03-23 20:43:59.882067 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py
--rw-r--r--   0        0        0      609 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2
--rw-r--r--   0        0        0     3408 2024-03-23 20:44:00.451058 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py
--rw-r--r--   0        0        0      613 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2
--rw-r--r--   0        0        0     3807 2024-03-23 20:44:00.225061 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py
--rw-r--r--   0        0        0     5267 2024-03-23 20:44:00.363059 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py
--rw-r--r--   0        0        0     6883 2024-03-23 20:44:00.348059 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py
--rw-r--r--   0        0        0     2548 2024-03-23 20:44:00.323060 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py
--rw-r--r--   0        0        0      161 2024-03-23 20:43:59.909066 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/__init__.py
--rw-r--r--   0        0        0     2293 2024-03-23 20:44:00.340059 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py
--rw-r--r--   0        0        0     3812 2024-03-23 20:44:00.511057 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py
--rw-r--r--   0        0        0     3561 2024-03-23 20:44:00.353059 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py
--rw-r--r--   0        0        0     5752 2024-03-23 20:44:00.425058 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_params.py
--rw-r--r--   0        0        0     4482 2024-03-23 20:44:00.092063 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/__init__.py
--rw-r--r--   0        0        0     4829 2024-03-23 20:44:00.211061 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py
--rw-r--r--   0        0        0     9763 2024-03-23 20:43:59.990065 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/emf_processors.py
--rw-r--r--   0        0        0     6413 2024-03-23 20:43:59.860067 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/helpers.py
--rw-r--r--   0        0        0     3525 2024-03-23 20:43:59.866067 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_service/__init__.py
--rw-r--r--   0        0        0     4688 2024-03-23 20:44:00.067064 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_service/helpers.py
--rw-r--r--   0        0        0     5588 2024-03-30 09:27:30.584324 ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_stack.py
--rw-r--r--   0        0        0     1927 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc1/ecs_composex/ecs/helpers/__init__.py
--rw-r--r--   0        0        0     2857 2024-03-23 20:44:00.159062 ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/__init__.py
--rw-r--r--   0        0        0     1414 2024-03-23 20:44:00.284060 ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py
--rw-r--r--   0        0        0     2805 2024-03-23 20:44:00.200062 ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/aws_xray.py
--rw-r--r--   0        0        0      960 2024-03-23 20:43:59.874067 ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py
--rw-r--r--   0        0        0     6182 2024-03-23 20:43:59.907066 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_alarms/__init__.py
--rw-r--r--   0        0        0     3158 2024-03-23 20:44:00.434058 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_alarms/service_predefined_alarms.py
--rw-r--r--   0        0        0     5545 2024-03-23 20:44:00.361059 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_compute/__init__.py
--rw-r--r--   0        0        0     1861 2024-03-23 20:44:00.379059 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_compute/helpers.py
--rw-r--r--   0        0        0    11217 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/__init__.py
--rw-r--r--   0        0        0     3209 2024-03-23 20:44:00.501057 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/helpers.py
--rw-r--r--   0        0        0    15299 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/ingress_helpers.py
--rw-r--r--   0        0        0     9051 2024-03-23 20:44:00.059064 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_scaling/__init__.py
--rw-r--r--   0        0        0    12114 2024-03-23 20:44:00.386059 ecs_composex-1.1.0rc1/ecs_composex/ecs/service_scaling/helpers.py
--rw-r--r--   0        0        0     5012 2024-03-23 20:44:00.206061 ecs_composex-1.1.0rc1/ecs_composex/ecs/task_compute/__init__.py
--rw-r--r--   0        0        0     3831 2024-03-23 20:43:59.847067 ecs_composex-1.1.0rc1/ecs_composex/ecs/task_compute/helpers.py
--rw-r--r--   0        0        0     5414 2024-03-23 20:43:59.884066 ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/__init__.py
--rw-r--r--   0        0        0     2208 2024-03-23 20:43:59.943066 ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/helpers.py
--rw-r--r--   0        0        0     7042 2024-03-23 20:44:00.056064 ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/task_role.py
--rw-r--r--   0        0        0    20480 2024-03-23 20:44:00.078064 ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/__init__.py
--rw-r--r--   0        0        0      509 2024-03-23 20:44:00.267061 ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/ecs_cluster_params.py
--rw-r--r--   0        0        0     7216 2024-03-23 20:44:00.029064 ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/ecs_family_helpers.py
--rw-r--r--   0        0        0     3504 2024-03-23 20:44:00.101063 ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/helpers.py
--rw-r--r--   0        0        0    12357 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc1/ecs_composex/ecs_composex.py
--rw-r--r--   0        0        0      326 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc1/ecs_composex/ecs_ingress/__init__.py
--rw-r--r--   0        0        0     3409 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc1/ecs_composex/ecs_ingress/ecs_ingress_stack.py
--rw-r--r--   0        0        0      125 2024-03-23 20:44:00.396058 ecs_composex-1.1.0rc1/ecs_composex/efs/__init__.py
--rw-r--r--   0        0        0    12388 2024-03-23 20:44:00.054064 ecs_composex-1.1.0rc1/ecs_composex/efs/efs_ecs.py
--rw-r--r--   0        0        0      403 2024-03-23 20:44:00.286060 ecs_composex-1.1.0rc1/ecs_composex/efs/efs_module.py
--rw-r--r--   0        0        0     1139 2024-03-23 20:44:00.172062 ecs_composex-1.1.0rc1/ecs_composex/efs/efs_params.py
--rw-r--r--   0        0        0     7434 2024-03-23 20:43:59.832067 ecs_composex-1.1.0rc1/ecs_composex/efs/efs_stack.py
--rw-r--r--   0        0        0     1026 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/efs/x-efs.spec.json
--rw-r--r--   0        0        0      482 2024-03-23 20:43:59.933066 ecs_composex-1.1.0rc1/ecs_composex/elasticache/__init__.py
--rw-r--r--   0        0        0     5725 2024-03-23 20:44:00.505057 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_aws.py
--rw-r--r--   0        0        0     3106 2024-03-23 20:44:00.427058 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_ecs.py
--rw-r--r--   0        0        0      482 2024-03-23 20:44:00.342059 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_module.py
--rw-r--r--   0        0        0     2926 2024-03-23 20:43:59.929066 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_params.py
--rw-r--r--   0        0        0     8927 2024-03-23 20:44:00.040064 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_stack.py
--rw-r--r--   0        0        0     8942 2024-03-23 20:44:00.156062 ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_template.py
--rw-r--r--   0        0        0      413 2024-03-23 20:44:00.507057 ecs_composex-1.1.0rc1/ecs_composex/elbv2/__init__.py
--rw-r--r--   0        0        0    27727 2024-03-23 20:44:00.231061 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_ecs.py
--rw-r--r--   0        0        0      413 2024-03-23 20:43:59.899066 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_module.py
--rw-r--r--   0        0        0     2143 2024-03-23 20:43:59.945066 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_params.py
--rw-r--r--   0        0        0     2957 2024-03-23 20:44:00.430058 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/__init__.py
--rw-r--r--   0        0        0    22478 2024-03-23 20:44:00.082064 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2.py
--rw-r--r--   0        0        0    10921 2024-03-23 20:44:00.242061 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py
--rw-r--r--   0        0        0    10200 2024-03-23 20:43:59.868067 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py
--rw-r--r--   0        0        0    22054 2024-03-23 20:44:00.470057 ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/helpers.py
--rw-r--r--   0        0        0    14439 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/elbv2/x-elbv2.spec.json
--rw-r--r--   0        0        0      414 2024-03-23 20:44:00.319060 ecs_composex-1.1.0rc1/ecs_composex/events/__init__.py
--rw-r--r--   0        0        0     8913 2024-03-23 20:44:00.065064 ecs_composex-1.1.0rc1/ecs_composex/events/events_ecs.py
--rw-r--r--   0        0        0     1882 2024-03-23 20:44:00.350059 ecs_composex-1.1.0rc1/ecs_composex/events/events_helpers.py
--rw-r--r--   0        0        0      414 2024-03-23 20:44:00.454058 ecs_composex-1.1.0rc1/ecs_composex/events/events_module.py
--rw-r--r--   0        0        0     6645 2024-03-23 20:44:00.174062 ecs_composex-1.1.0rc1/ecs_composex/events/events_stack.py
--rw-r--r--   0        0        0     2053 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/events/x-events.spec.json
--rw-r--r--   0        0        0      480 2024-03-23 20:44:00.183062 ecs_composex-1.1.0rc1/ecs_composex/exceptions.py
--rw-r--r--   0        0        0     2487 2024-03-23 20:44:00.238061 ecs_composex-1.1.0rc1/ecs_composex/iam/__init__.py
--rw-r--r--   0        0        0     6262 2024-03-23 20:43:59.999065 ecs_composex-1.1.0rc1/ecs_composex/iam/iam_ecs_helpers.py
--rw-r--r--   0        0        0      950 2024-03-23 20:44:00.149062 ecs_composex-1.1.0rc1/ecs_composex/iam/iam_params.py
--rw-r--r--   0        0        0     3415 2024-03-23 20:44:00.503057 ecs_composex-1.1.0rc1/ecs_composex/iam/iam_stack.py
--rw-r--r--   0        0        0     1781 2024-03-23 20:44:00.314060 ecs_composex-1.1.0rc1/ecs_composex/iam/import_sam_policies.py
--rw-r--r--   0        0        0    67793 2024-03-31 16:06:41.621053 ecs_composex-1.1.0rc1/ecs_composex/iam/sam_policies.json
--rw-r--r--   0        0        0    14701 2024-03-23 20:44:00.298060 ecs_composex-1.1.0rc1/ecs_composex/ingress_settings.py
--rw-r--r--   0        0        0      421 2024-03-23 20:44:00.080063 ecs_composex-1.1.0rc1/ecs_composex/kinesis/__init__.py
--rw-r--r--   0        0        0     4732 2023-11-29 08:40:57.722589 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kcl_helpers.py
--rw-r--r--   0        0        0     2984 2024-03-23 20:44:00.113063 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_kinesis_firehose.py
--rw-r--r--   0        0        0      421 2024-03-23 20:44:00.013064 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_module.py
--rw-r--r--   0        0        0      535 2024-03-23 20:43:59.864067 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_params.py
--rw-r--r--   0        0        0     1022 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_perms.json
--rw-r--r--   0        0        0     7714 2024-03-23 20:44:00.294060 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_stack.py
--rw-r--r--   0        0        0     2630 2024-03-23 20:44:00.365059 ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_template.py
--rw-r--r--   0        0        0     2692 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/kinesis/x-kinesis.spec.json
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.213061 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/__init__.py
--rw-r--r--   0        0        0     2946 2024-03-23 20:44:00.246061 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py
--rw-r--r--   0        0        0     4602 2024-03-23 20:43:59.821067 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.190062 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_module.py
--rw-r--r--   0        0        0      624 2024-03-23 20:43:59.996065 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_params.py
--rw-r--r--   0        0        0      205 2024-03-31 16:06:39.592089 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_perms.json
--rw-r--r--   0        0        0     6686 2024-03-23 20:44:00.421058 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py
--rw-r--r--   0        0        0     4278 2024-03-23 20:44:00.436058 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_template.py
--rw-r--r--   0        0        0     1858 2024-03-31 16:06:39.592089 ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.044064 ecs_composex-1.1.0rc1/ecs_composex/kms/__init__.py
--rw-r--r--   0        0        0     2102 2024-03-23 20:44:00.452058 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_ecs_cluster.py
--rw-r--r--   0        0        0     4549 2024-03-23 20:43:59.905066 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_kinesis_firehose.py
--rw-r--r--   0        0        0      409 2024-03-23 20:44:00.312060 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_module.py
--rw-r--r--   0        0        0      956 2024-03-23 20:44:00.327060 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_params.py
--rw-r--r--   0        0        0     1169 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_perms.json
--rw-r--r--   0        0        0     2556 2024-03-23 20:44:00.216061 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_s3.py
--rw-r--r--   0        0        0     2311 2024-03-23 20:43:59.888066 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_sqs.py
--rw-r--r--   0        0        0     9013 2024-03-23 20:44:00.292060 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_stack.py
--rw-r--r--   0        0        0     1479 2024-03-23 20:43:59.951065 ecs_composex-1.1.0rc1/ecs_composex/kms/kms_template.py
--rw-r--r--   0        0        0      826 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/kms/x-kms.spec.json
--rw-r--r--   0        0        0    12383 2024-03-23 20:43:59.988065 ecs_composex-1.1.0rc1/ecs_composex/mods_manager.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.052064 ecs_composex-1.1.0rc1/ecs_composex/neptune/__init__.py
--rw-r--r--   0        0        0      478 2024-03-23 20:44:00.208062 ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_module.py
--rw-r--r--   0        0        0      864 2024-03-23 20:43:59.941066 ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_params.py
--rw-r--r--   0        0        0      337 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_perms.json
--rw-r--r--   0        0        0     9212 2024-03-23 20:44:00.459057 ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_stack.py
--rw-r--r--   0        0        0     5088 2024-03-23 20:44:00.250061 ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_template.py
--rw-r--r--   0        0        0     3013 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/neptune/x-neptune.spec.json
--rw-r--r--   0        0        0      488 2024-03-23 20:43:59.858067 ecs_composex-1.1.0rc1/ecs_composex/opensearch/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-23 20:44:00.188062 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_aws.py
--rw-r--r--   0        0        0      487 2024-03-23 20:43:59.981065 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_module.py
--rw-r--r--   0        0        0      950 2024-03-23 20:44:00.007065 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_params.py
--rw-r--r--   0        0        0      983 2024-03-31 16:06:39.600089 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_perms.json
--rw-r--r--   0        0        0     6315 2024-03-23 20:44:00.073063 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_stack.py
--rw-r--r--   0        0        0    22533 2024-03-23 20:44:00.325060 ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_template.py
--rw-r--r--   0        0        0     3216 2024-03-31 16:06:39.600089 ecs_composex-1.1.0rc1/ecs_composex/opensearch/x-opensearch.spec.json
--rw-r--r--   0        0        0       19 2021-03-04 09:40:13.444136 ecs_composex-1.1.0rc1/ecs_composex/rds/.gitignore
--rw-r--r--   0        0        0      146 2024-03-23 20:43:59.813068 ecs_composex-1.1.0rc1/ecs_composex/rds/__init__.py
--rw-r--r--   0        0        0     1703 2024-03-23 20:44:00.465057 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_conditions.py
--rw-r--r--   0        0        0    20461 2024-03-23 20:43:59.939066 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_db_template.py
--rw-r--r--   0        0        0     5939 2024-03-23 20:44:00.180062 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_features.py
--rw-r--r--   0        0        0     5448 2024-03-23 20:44:00.509057 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_features_define.py
--rw-r--r--   0        0        0      455 2024-03-23 20:44:00.417058 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_module.py
--rw-r--r--   0        0        0     3624 2024-03-23 20:44:00.146062 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_parameter_groups_helper.py
--rw-r--r--   0        0        0     2898 2024-03-23 20:44:00.305060 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_params.py
--rw-r--r--   0        0        0      164 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_perms.json
--rw-r--r--   0        0        0    10438 2024-03-23 20:43:59.953065 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_stack.py
--rw-r--r--   0        0        0     4557 2024-03-23 20:44:00.164062 ecs_composex-1.1.0rc1/ecs_composex/rds/rds_template.py
--rw-r--r--   0        0        0     5948 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/rds/x-rds.spec.json
--rw-r--r--   0        0        0    22702 2024-03-23 20:44:00.457058 ecs_composex-1.1.0rc1/ecs_composex/rds_resources_settings.py
--rw-r--r--   0        0        0    27883 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc1/ecs_composex/resource_settings.py
--rw-r--r--   0        0        0     8660 2024-03-23 20:44:00.440058 ecs_composex-1.1.0rc1/ecs_composex/resources_import.py
--rw-r--r--   0        0        0        0 2022-06-16 20:44:41.834935 ecs_composex-1.1.0rc1/ecs_composex/route53/__init__.py
--rw-r--r--   0        0        0     4385 2024-03-23 20:44:00.037064 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_acm.py
--rw-r--r--   0        0        0     5433 2024-03-23 20:44:00.134063 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_elbv2.py
--rw-r--r--   0        0        0     3983 2024-03-23 20:44:00.371059 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_helpers.py
--rw-r--r--   0        0        0      429 2024-03-23 20:44:00.303060 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_module.py
--rw-r--r--   0        0        0     1136 2024-03-23 20:44:00.154062 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_params.py
--rw-r--r--   0        0        0     7828 2024-03-23 20:44:00.448058 ecs_composex-1.1.0rc1/ecs_composex/route53/route53_stack.py
--rw-r--r--   0        0        0     1476 2024-03-31 16:06:39.599089 ecs_composex-1.1.0rc1/ecs_composex/route53/x-route53.spec.json
--rw-r--r--   0        0        0      283 2024-03-23 20:44:00.111063 ecs_composex-1.1.0rc1/ecs_composex/s3/__init__.py
--rw-r--r--   0        0        0     7451 2024-03-23 20:43:59.913066 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_bucket.py
--rw-r--r--   0        0        0     2581 2024-03-23 20:44:00.033064 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_ecs_cluster.py
--rw-r--r--   0        0        0     3848 2024-03-23 20:44:00.307060 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_kinesis_firehose.py
--rw-r--r--   0        0        0      406 2024-03-23 20:44:00.105063 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_module.py
--rw-r--r--   0        0        0     2289 2024-03-23 20:44:00.031064 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_params.py
--rw-r--r--   0        0        0     3566 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_perms.json
--rw-r--r--   0        0        0     5135 2024-03-23 20:44:00.438058 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_stack.py
--rw-r--r--   0        0        0     7858 2024-03-23 20:44:00.115063 ecs_composex-1.1.0rc1/ecs_composex/s3/s3_template.py
--rw-r--r--   0        0        0     3232 2024-03-31 16:06:39.596089 ecs_composex-1.1.0rc1/ecs_composex/s3/x-s3.spec.json
--rw-r--r--   0        0        0     2948 2024-03-23 20:44:00.003065 ecs_composex-1.1.0rc1/ecs_composex/secrets/__init__.py
--rw-r--r--   0        0        0     2005 2024-03-23 20:44:00.198062 ecs_composex-1.1.0rc1/ecs_composex/secrets/secrets_aws.py
--rw-r--r--   0        0        0      493 2024-03-23 20:44:00.290060 ecs_composex-1.1.0rc1/ecs_composex/secrets/secrets_params.py
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.338060 ecs_composex-1.1.0rc1/ecs_composex/sns/__init__.py
--rw-r--r--   0        0        0     2625 2024-03-23 20:44:00.218061 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_helpers.py
--rw-r--r--   0        0        0      407 2024-03-23 20:43:59.872067 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_module.py
--rw-r--r--   0        0        0      698 2024-03-23 20:44:00.257061 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_params.py
--rw-r--r--   0        0        0      128 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_perms.json
--rw-r--r--   0        0        0     2377 2024-03-23 20:44:00.233061 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_stack.py
--rw-r--r--   0        0        0     1286 2024-03-23 20:43:59.823068 ecs_composex-1.1.0rc1/ecs_composex/sns/sns_templates.py
--rw-r--r--   0        0        0      696 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/sns/x-sns.spec.json
--rw-r--r--   0        0        0      281 2024-03-23 20:44:00.446058 ecs_composex-1.1.0rc1/ecs_composex/specs/__init__.py
--rw-r--r--   0        0        0      742 2024-03-23 20:44:00.143062 ecs_composex-1.1.0rc1/ecs_composex/specs/_core.py
--rw-r--r--   0        0        0    29055 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/compose-spec.json
--rw-r--r--   0        0        0     2455 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/specs/ingress.spec.json
--rw-r--r--   0        0        0     1234 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/secrets.x-secrets.spec.json
--rw-r--r--   0        0        0     2266 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/services-xray.spec.json
--rw-r--r--   0        0        0     1404 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-alarms.spec.json
--rw-r--r--   0        0        0      403 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-codeguru_profiler.spec.json
--rw-r--r--   0        0        0      501 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-docker_opts.spec.json
--rw-r--r--   0        0        0     1853 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-ecr.spec.json
--rw-r--r--   0        0        0     2745 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-ecs.spec.json
--rw-r--r--   0        0        0      836 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-environment.spec.json
--rw-r--r--   0        0        0     2175 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-iam.spec.json
--rw-r--r--   0        0        0     7429 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-logging.spec.json
--rw-r--r--   0        0        0     1986 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-monitoring.spec.json
--rw-r--r--   0        0        0     4477 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-network.spec.json
--rw-r--r--   0        0        0     4724 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-prometheus.spec.json
--rw-r--r--   0        0        0     4105 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-scaling.spec.json
--rw-r--r--   0        0        0     2133 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/x-cluster.spec.json
--rw-r--r--   0        0        0     6706 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/specs/x-rds-common.spec.json
--rw-r--r--   0        0        0     6559 2024-03-31 16:06:39.595089 ecs_composex-1.1.0rc1/ecs_composex/specs/x-resources.common.spec.json
--rw-r--r--   0        0        0      816 2024-03-31 16:06:39.594089 ecs_composex-1.1.0rc1/ecs_composex/specs/x-tags.spec.json
--rw-r--r--   0        0        0      285 2024-03-23 20:44:00.279060 ecs_composex-1.1.0rc1/ecs_composex/sqs/__init__.py
--rw-r--r--   0        0        0     4737 2024-03-23 20:43:59.937066 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_ecs_scaling.py
--rw-r--r--   0        0        0     3592 2024-03-23 20:43:59.890066 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_helpers.py
--rw-r--r--   0        0        0      407 2024-03-23 20:43:59.836067 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_module.py
--rw-r--r--   0        0        0      865 2024-03-23 20:44:00.141063 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_params.py
--rw-r--r--   0        0        0      515 2024-03-31 16:06:39.597089 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_perms.json
--rw-r--r--   0        0        0     5463 2024-03-23 20:44:00.050064 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_s3.py
--rw-r--r--   0        0        0     2938 2024-03-23 20:44:00.383059 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_sqs.py
--rw-r--r--   0        0        0     4375 2024-03-23 20:43:59.917066 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_stack.py
--rw-r--r--   0        0        0     7648 2024-03-23 20:44:00.273060 ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_template.py
--rw-r--r--   0        0        0      744 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/sqs/x-sqs.spec.json
--rw-r--r--   0        0        0      488 2024-03-23 20:44:00.020064 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/__init__.py
--rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.195062 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_helpers.py
--rw-r--r--   0        0        0      488 2024-03-23 20:43:59.935066 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_module.py
--rw-r--r--   0        0        0      905 2024-03-23 20:44:00.263061 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_params.py
--rw-r--r--   0        0        0      820 2024-03-31 16:06:39.593089 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_perms.json
--rw-r--r--   0        0        0     3924 2024-03-23 20:44:00.011065 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_stack.py
--rw-r--r--   0        0        0     2243 2024-03-31 16:06:39.592089 ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json
--rw-r--r--   0        0        0       88 2024-03-23 20:44:00.296060 ecs_composex-1.1.0rc1/ecs_composex/utils/__init__.py
--rw-r--r--   0        0        0      820 2024-03-23 20:44:00.344059 ecs_composex-1.1.0rc1/ecs_composex/utils/init_ecs.py
--rw-r--r--   0        0        0     1797 2024-03-23 20:43:59.992065 ecs_composex-1.1.0rc1/ecs_composex/utils/init_s3.py
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.497057 ecs_composex-1.1.0rc1/ecs_composex/vpc/__init__.py
--rw-r--r--   0        0        0      616 2024-03-23 20:44:00.255061 ecs_composex-1.1.0rc1/ecs_composex/vpc/aws_mappings.py
--rw-r--r--   0        0        0     3997 2024-03-23 20:43:59.919066 ecs_composex-1.1.0rc1/ecs_composex/vpc/helpers.py
--rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.071064 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_aws.py
--rw-r--r--   0        0        0     1338 2024-03-23 20:44:00.357059 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_cloudmap.py
--rw-r--r--   0        0        0       88 2024-03-23 20:43:59.834067 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_conditions.py
--rw-r--r--   0        0        0     1953 2024-03-23 20:44:00.377059 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_maths.py
--rw-r--r--   0        0        0      423 2024-03-23 20:44:00.499057 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_module.py
--rw-r--r--   0        0        0     2217 2024-03-23 20:44:00.253061 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_params.py
--rw-r--r--   0        0        0    14983 2024-03-23 20:44:00.442058 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_stack.py
--rw-r--r--   0        0        0    10517 2024-03-23 20:44:00.161062 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_subnets.py
--rw-r--r--   0        0        0     4709 2024-03-23 20:44:00.109063 ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_template.py
--rw-r--r--   0        0        0     3504 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/vpc/x-vpc.spec.json
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.336059 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/__init__.py
--rw-r--r--   0        0        0      697 2024-03-23 20:44:00.119063 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/validators_wafv2.py
--rw-r--r--   0        0        0     2255 2024-03-23 20:44:00.288060 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py
--rw-r--r--   0        0        0      497 2024-03-23 20:44:00.169062 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_module.py
--rw-r--r--   0        0        0     1079 2024-03-23 20:43:59.850067 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_params.py
--rw-r--r--   0        0        0      185 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_perms.json
--rw-r--r--   0        0        0     9460 2024-03-23 20:44:00.373059 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py
--rw-r--r--   0        0        0     1357 2024-03-23 20:44:00.423058 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_template.py
--rw-r--r--   0        0        0     1772 2024-03-31 16:06:39.598089 ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json
--rw-r--r--   0        0        0     3476 2024-03-31 16:06:38.942101 ecs_composex-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     8907 1970-01-01 00:00:00.000000 ecs_composex-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2021-05-14 10:51:20.077071 ecs_composex-1.1.0rc2/LICENSE
+-rw-r--r--   0        0        0      385 2022-06-16 18:49:16.792466 ecs_composex-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     1068 2023-08-07 12:54:52.746417 ecs_composex-1.1.0rc2/NOTICES.rst
+-rw-r--r--   0        0        0     6976 2023-01-11 09:54:17.357527 ecs_composex-1.1.0rc2/README.rst
+-rw-r--r--   0        0        0       19 2021-03-04 09:40:13.458136 ecs_composex-1.1.0rc2/ecs_composex/.gitignore
+-rw-r--r--   0        0        0      222 2024-04-14 21:59:40.442106 ecs_composex-1.1.0rc2/ecs_composex/__init__.py
+-rw-r--r--   0        0        0      117 2024-03-23 20:44:00.309060 ecs_composex-1.1.0rc2/ecs_composex/acm/__init__.py
+-rw-r--r--   0        0        0      419 2024-03-23 20:44:00.401059 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_module.py
+-rw-r--r--   0        0        0     1546 2024-03-23 20:44:00.178062 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_params.py
+-rw-r--r--   0        0        0     5773 2024-03-23 20:44:00.185062 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack.py
+-rw-r--r--   0        0        0     7634 2024-03-23 20:44:00.125063 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack_helpers.py
+-rw-r--r--   0        0        0     1327 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/acm/x-acm.spec.json
+-rw-r--r--   0        0        0      416 2024-03-23 20:44:00.390059 ecs_composex-1.1.0rc2/ecs_composex/alarms/__init__.py
+-rw-r--r--   0        0        0     9162 2024-03-23 20:44:00.121063 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_ecs.py
+-rw-r--r--   0        0        0     6292 2024-03-23 20:44:00.005065 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_elbv2.py
+-rw-r--r--   0        0        0     8575 2024-03-23 20:43:59.927066 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_helpers.py
+-rw-r--r--   0        0        0      416 2024-03-23 20:44:00.139063 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_module.py
+-rw-r--r--   0        0        0      532 2024-03-23 20:44:00.388059 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_params.py
+-rw-r--r--   0        0        0     4520 2024-03-23 20:43:59.894066 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_stack.py
+-rw-r--r--   0        0        0     1920 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/alarms/x-alarms.spec.json
+-rw-r--r--   0        0        0       44 2022-06-16 18:49:16.909464 ecs_composex-1.1.0rc2/ecs_composex/appmesh/README.rst
+-rw-r--r--   0        0        0      288 2024-03-23 20:44:00.220061 ecs_composex-1.1.0rc2/ecs_composex/appmesh/__init__.py
+-rw-r--r--   0        0        0     2268 2024-03-23 20:43:59.826068 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_aws.py
+-rw-r--r--   0        0        0     1479 2024-03-23 20:44:00.369059 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_conditions.py
+-rw-r--r--   0        0        0     9620 2024-03-23 20:44:00.022064 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_mesh.py
+-rw-r--r--   0        0        0    12953 2024-03-23 20:44:00.203061 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_node.py
+-rw-r--r--   0        0        0     1222 2024-03-23 20:43:59.819068 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_params.py
+-rw-r--r--   0        0        0    10944 2024-03-23 20:44:00.127063 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_router.py
+-rw-r--r--   0        0        0     6917 2024-03-23 20:44:00.367059 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_service.py
+-rw-r--r--   0        0        0     4576 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/appmesh/x-appmesh.spec.json
+-rw-r--r--   0        0        0      121 2024-03-23 20:43:59.931066 ecs_composex-1.1.0rc2/ecs_composex/aps/__init__.py
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.240061 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_module.py
+-rw-r--r--   0        0        0      938 2024-03-23 20:44:00.136062 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_parameters.py
+-rw-r--r--   0        0        0      492 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_perms.json
+-rw-r--r--   0        0        0     7896 2024-03-23 20:44:00.467057 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_stack.py
+-rw-r--r--   0        0        0     1219 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/aps/x-aps.spec.json
+-rw-r--r--   0        0        0     6802 2024-03-23 20:44:00.151062 ecs_composex-1.1.0rc2/ecs_composex/cli.py
+-rw-r--r--   0        0        0      481 2024-03-23 20:44:00.271061 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/__init__.py
+-rw-r--r--   0        0        0     7347 2024-03-23 20:44:00.090063 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_ecs.py
+-rw-r--r--   0        0        0     5364 2024-03-23 20:43:59.853067 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_helpers.py
+-rw-r--r--   0        0        0      481 2024-03-23 20:43:59.986065 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_module.py
+-rw-r--r--   0        0        0     2100 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_params.py
+-rw-r--r--   0        0        0    12308 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_stack.py
+-rw-r--r--   0        0        0     7790 2024-03-23 20:43:59.886067 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_x_resources.py
+-rw-r--r--   0        0        0     1486 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/x-cloudmap.spec.json
+-rw-r--r--   0        0        0      500 2024-03-23 20:44:00.107063 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/__init__.py
+-rw-r--r--   0        0        0     1761 2024-03-23 20:44:00.321060 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py
+-rw-r--r--   0        0        0      500 2024-03-23 20:44:00.359059 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_module.py
+-rw-r--r--   0        0        0      603 2024-03-23 20:44:00.419058 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_params.py
+-rw-r--r--   0        0        0      188 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_perms.json
+-rw-r--r--   0        0        0     5053 2024-03-23 20:43:59.897066 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py
+-rw-r--r--   0        0        0      489 2024-03-23 20:44:00.009065 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/__init__.py
+-rw-r--r--   0        0        0      909 2024-03-23 20:43:59.840067 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_params.py
+-rw-r--r--   0        0        0      489 2024-03-23 20:43:59.828067 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_module.py
+-rw-r--r--   0        0        0     4821 2024-03-23 20:43:59.961065 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_stack.py
+-rw-r--r--   0        0        0      375 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/x-cognito_userpool.spec.json
+-rw-r--r--   0        0        0     2314 2024-03-23 20:44:00.088063 ecs_composex-1.1.0rc2/ecs_composex/common/__init__.py
+-rw-r--r--   0        0        0    13821 2024-03-23 20:43:59.947065 ecs_composex-1.1.0rc2/ecs_composex/common/aws.py
+-rw-r--r--   0        0        0     1209 2024-03-23 20:44:00.432058 ecs_composex-1.1.0rc2/ecs_composex/common/cfn_conditions.py
+-rw-r--r--   0        0        0     1258 2024-03-23 20:43:59.901066 ecs_composex-1.1.0rc2/ecs_composex/common/cfn_params.py
+-rw-r--r--   0        0        0      408 2024-03-23 20:44:00.103063 ecs_composex-1.1.0rc2/ecs_composex/common/ecs_composex.py
+-rw-r--r--   0        0        0     1465 2024-03-23 22:36:48.972815 ecs_composex-1.1.0rc2/ecs_composex/common/envsubst.py
+-rw-r--r--   0        0        0     9180 2024-03-23 20:43:59.971065 ecs_composex-1.1.0rc2/ecs_composex/common/files.py
+-rw-r--r--   0        0        0     1937 2024-03-23 20:43:59.921066 ecs_composex-1.1.0rc2/ecs_composex/common/logging.py
+-rw-r--r--   0        0        0    24735 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/common/settings.py
+-rw-r--r--   0        0        0    14081 2024-03-23 20:44:00.463057 ecs_composex-1.1.0rc2/ecs_composex/common/stacks/__init__.py
+-rw-r--r--   0        0        0     8705 2024-03-23 20:44:00.333059 ecs_composex-1.1.0rc2/ecs_composex/common/tagging.py
+-rw-r--r--   0        0        0    10189 2024-03-23 20:43:59.845067 ecs_composex-1.1.0rc2/ecs_composex/common/troposphere_tools.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.277060 ecs_composex-1.1.0rc2/ecs_composex/compose/__init__.py
+-rw-r--r--   0        0        0     1629 2024-03-23 20:44:00.131063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_networks.py
+-rw-r--r--   0        0        0     9238 2024-03-23 20:44:00.042064 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/__init__.py
+-rw-r--r--   0        0        0     3632 2024-03-23 20:44:00.229061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/ecs_family_helpers.py
+-rw-r--r--   0        0        0     1490 2024-03-23 20:44:00.222061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/helpers.py
+-rw-r--r--   0        0        0     1292 2024-03-23 20:44:00.227061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/services_helpers.py
+-rw-r--r--   0        0        0    37531 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/__init__.py
+-rw-r--r--   0        0        0     6697 2024-03-23 20:43:59.903066 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/docker_tools.py
+-rw-r--r--   0        0        0     3399 2024-03-23 20:44:00.001065 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/env_files_helpers.py
+-rw-r--r--   0        0        0     9848 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/helpers.py
+-rw-r--r--   0        0        0     3658 2024-03-23 20:44:00.275061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/kernel_options_helpers.py
+-rw-r--r--   0        0        0     8042 2024-03-23 20:44:00.129063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/__init__.py
+-rw-r--r--   0        0        0     2719 2024-03-23 20:44:00.375059 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/docker_opts.py
+-rw-r--r--   0        0        0     3911 2024-03-23 20:43:59.892066 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_helpers.py
+-rw-r--r--   0        0        0    10829 2024-03-23 20:44:00.167062 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py
+-rw-r--r--   0        0        0     5119 2024-03-23 20:44:00.261061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/__init__.py
+-rw-r--r--   0        0        0     5036 2024-03-23 20:43:59.855067 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/helpers.py
+-rw-r--r--   0        0        0     3873 2024-03-23 20:43:59.983065 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/__init__.py
+-rw-r--r--   0        0        0     6846 2024-03-23 20:44:00.069064 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/ecs_family_helpers.py
+-rw-r--r--   0        0        0     1459 2024-03-23 20:44:00.331060 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/helpers.py
+-rw-r--r--   0        0        0     5651 2024-03-23 20:44:00.096063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/services_helpers.py
+-rw-r--r--   0        0        0    30750 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/__init__.py
+-rw-r--r--   0        0        0     1672 2024-03-23 20:43:59.911066 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/api_x_resources.py
+-rw-r--r--   0        0        0      922 2024-03-23 20:44:00.461058 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/environment_x_resources.py
+-rw-r--r--   0        0        0     4657 2024-03-23 20:44:00.123063 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/helpers.py
+-rw-r--r--   0        0        0     6435 2024-03-23 20:44:00.048064 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/network_x_resources.py
+-rw-r--r--   0        0        0     8806 2024-03-23 20:43:59.838067 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/services_resources.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.017064 ecs_composex-1.1.0rc2/ecs_composex/dashboards/__init__.py
+-rw-r--r--   0        0        0      472 2024-03-23 20:43:59.842067 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_module.py
+-rw-r--r--   0        0        0     5539 2024-03-23 20:44:00.329059 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_services_metrics.py
+-rw-r--r--   0        0        0     4831 2024-03-23 20:44:00.035064 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_stack.py
+-rw-r--r--   0        0        0     1224 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/dashboards/x-dashboards.spec.json
+-rw-r--r--   0        0        0      413 2024-03-23 20:44:00.259061 ecs_composex-1.1.0rc2/ecs_composex/docdb/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:43:59.915066 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_module.py
+-rw-r--r--   0        0        0      833 2024-03-23 20:44:00.346059 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_params.py
+-rw-r--r--   0        0        0      164 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_perms.json
+-rw-r--r--   0        0        0     7772 2024-03-23 20:43:59.876067 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_stack.py
+-rw-r--r--   0        0        0     6450 2024-03-23 20:44:00.063064 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_template.py
+-rw-r--r--   0        0        0     2241 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/docdb/x-docdb.spec.json
+-rw-r--r--   0        0        0      289 2024-03-23 20:44:00.046064 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/__init__.py
+-rw-r--r--   0        0        0     7795 2024-03-23 20:44:00.248061 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_autoscaling.py
+-rw-r--r--   0        0        0      422 2024-03-23 20:44:00.117063 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_module.py
+-rw-r--r--   0        0        0      412 2024-03-23 20:43:59.966065 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_params.py
+-rw-r--r--   0        0        0     1096 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_perms.json
+-rw-r--r--   0        0        0     4131 2024-03-23 20:44:00.355059 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_stack.py
+-rw-r--r--   0        0        0     2916 2024-03-23 20:44:00.075064 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_template.py
+-rw-r--r--   0        0        0     2777 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/x-dynamodb.spec.json
+-rw-r--r--   0        0        0     1050 2024-03-23 20:44:00.094063 ecs_composex-1.1.0rc2/ecs_composex/ecs/__init__.py
+-rw-r--r--   0        0        0     3532 2024-03-23 20:43:59.955065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_conditions.py
+-rw-r--r--   0        0        0    27604 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/__init__.py
+-rw-r--r--   0        0        0    14849 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/__init__.py
+-rw-r--r--   0        0        0     1316 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py
+-rw-r--r--   0        0        0     1912 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py
+-rw-r--r--   0        0        0     8788 2024-03-23 20:43:59.870067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/__init__.py
+-rw-r--r--   0        0        0     4123 2024-03-23 20:44:00.061064 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py
+-rw-r--r--   0        0        0     2940 2024-03-23 20:43:59.880066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_template.py
+-rw-r--r--   0        0        0     3502 2024-03-23 20:43:59.861067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_execute_command.py
+-rw-r--r--   0        0        0     2626 2024-03-23 20:44:00.015065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_runtime.py
+-rw-r--r--   0        0        0      163 2024-03-23 20:44:00.381059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/__init__.py
+-rw-r--r--   0        0        0    10598 2024-03-23 20:43:59.949066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py
+-rw-r--r--   0        0        0     5822 2024-03-23 20:44:00.098063 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py
+-rw-r--r--   0        0        0     5548 2024-03-23 20:44:00.282060 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py
+-rw-r--r--   0        0        0     3067 2024-03-23 20:43:59.882067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py
+-rw-r--r--   0        0        0      609 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2
+-rw-r--r--   0        0        0     3408 2024-03-23 20:44:00.451058 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py
+-rw-r--r--   0        0        0      613 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2
+-rw-r--r--   0        0        0     3807 2024-03-23 20:44:00.225061 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py
+-rw-r--r--   0        0        0     5267 2024-03-23 20:44:00.363059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py
+-rw-r--r--   0        0        0     6883 2024-03-23 20:44:00.348059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py
+-rw-r--r--   0        0        0     2548 2024-03-23 20:44:00.323060 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py
+-rw-r--r--   0        0        0      161 2024-03-23 20:43:59.909066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/__init__.py
+-rw-r--r--   0        0        0     2293 2024-03-23 20:44:00.340059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py
+-rw-r--r--   0        0        0     3812 2024-03-23 20:44:00.511057 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py
+-rw-r--r--   0        0        0     3561 2024-03-23 20:44:00.353059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py
+-rw-r--r--   0        0        0     5752 2024-03-23 20:44:00.425058 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_params.py
+-rw-r--r--   0        0        0     4482 2024-03-23 20:44:00.092063 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/__init__.py
+-rw-r--r--   0        0        0     4829 2024-03-23 20:44:00.211061 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py
+-rw-r--r--   0        0        0     9763 2024-03-23 20:43:59.990065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/emf_processors.py
+-rw-r--r--   0        0        0     6413 2024-03-23 20:43:59.860067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/helpers.py
+-rw-r--r--   0        0        0     3525 2024-03-23 20:43:59.866067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/__init__.py
+-rw-r--r--   0        0        0     4688 2024-03-23 20:44:00.067064 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/helpers.py
+-rw-r--r--   0        0        0     5588 2024-03-30 09:27:30.584324 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_stack.py
+-rw-r--r--   0        0        0     1927 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs/helpers/__init__.py
+-rw-r--r--   0        0        0     2857 2024-03-23 20:44:00.159062 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/__init__.py
+-rw-r--r--   0        0        0     1414 2024-03-23 20:44:00.284060 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py
+-rw-r--r--   0        0        0     2805 2024-03-23 20:44:00.200062 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_xray.py
+-rw-r--r--   0        0        0      960 2024-03-23 20:43:59.874067 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py
+-rw-r--r--   0        0        0     6182 2024-03-23 20:43:59.907066 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/__init__.py
+-rw-r--r--   0        0        0     3158 2024-03-23 20:44:00.434058 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/service_predefined_alarms.py
+-rw-r--r--   0        0        0     5545 2024-03-23 20:44:00.361059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/__init__.py
+-rw-r--r--   0        0        0     1861 2024-03-23 20:44:00.379059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/helpers.py
+-rw-r--r--   0        0        0    10734 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/helpers.py
+-rw-r--r--   0        0        0    15293 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/ingress_helpers.py
+-rw-r--r--   0        0        0     9051 2024-03-23 20:44:00.059064 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/__init__.py
+-rw-r--r--   0        0        0    12114 2024-03-23 20:44:00.386059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/helpers.py
+-rw-r--r--   0        0        0     5012 2024-03-23 20:44:00.206061 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/__init__.py
+-rw-r--r--   0        0        0     3831 2024-03-23 20:43:59.847067 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/helpers.py
+-rw-r--r--   0        0        0     5414 2024-03-23 20:43:59.884066 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/__init__.py
+-rw-r--r--   0        0        0     2208 2024-03-23 20:43:59.943066 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/helpers.py
+-rw-r--r--   0        0        0     7042 2024-03-23 20:44:00.056064 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/task_role.py
+-rw-r--r--   0        0        0    20480 2024-03-23 20:44:00.078064 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/__init__.py
+-rw-r--r--   0        0        0      509 2024-03-23 20:44:00.267061 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_cluster_params.py
+-rw-r--r--   0        0        0     7216 2024-03-23 20:44:00.029064 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_family_helpers.py
+-rw-r--r--   0        0        0     3504 2024-03-23 20:44:00.101063 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/helpers.py
+-rw-r--r--   0        0        0    12357 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs_composex.py
+-rw-r--r--   0        0        0      326 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/__init__.py
+-rw-r--r--   0        0        0     3409 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/ecs_ingress_stack.py
+-rw-r--r--   0        0        0      125 2024-03-23 20:44:00.396058 ecs_composex-1.1.0rc2/ecs_composex/efs/__init__.py
+-rw-r--r--   0        0        0    12388 2024-03-23 20:44:00.054064 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_ecs.py
+-rw-r--r--   0        0        0      403 2024-03-23 20:44:00.286060 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_module.py
+-rw-r--r--   0        0        0     1139 2024-03-23 20:44:00.172062 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_params.py
+-rw-r--r--   0        0        0     7434 2024-03-23 20:43:59.832067 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_stack.py
+-rw-r--r--   0        0        0     1026 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/efs/x-efs.spec.json
+-rw-r--r--   0        0        0      482 2024-03-23 20:43:59.933066 ecs_composex-1.1.0rc2/ecs_composex/elasticache/__init__.py
+-rw-r--r--   0        0        0     5725 2024-03-23 20:44:00.505057 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_aws.py
+-rw-r--r--   0        0        0     3106 2024-03-23 20:44:00.427058 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_ecs.py
+-rw-r--r--   0        0        0      482 2024-03-23 20:44:00.342059 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_module.py
+-rw-r--r--   0        0        0     2926 2024-03-23 20:43:59.929066 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_params.py
+-rw-r--r--   0        0        0     8927 2024-03-23 20:44:00.040064 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_stack.py
+-rw-r--r--   0        0        0     8942 2024-03-23 20:44:00.156062 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_template.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:44:00.507057 ecs_composex-1.1.0rc2/ecs_composex/elbv2/__init__.py
+-rw-r--r--   0        0        0    27727 2024-03-23 20:44:00.231061 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_ecs.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:43:59.899066 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_module.py
+-rw-r--r--   0        0        0     2143 2024-03-23 20:43:59.945066 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_params.py
+-rw-r--r--   0        0        0     2957 2024-04-03 16:23:37.606364 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/__init__.py
+-rw-r--r--   0        0        0    22478 2024-03-23 20:44:00.082064 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2.py
+-rw-r--r--   0        0        0    10921 2024-03-23 20:44:00.242061 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py
+-rw-r--r--   0        0        0    10216 2024-04-05 21:17:25.394956 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py
+-rw-r--r--   0        0        0    22054 2024-03-23 20:44:00.470057 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/helpers.py
+-rw-r--r--   0        0        0    14439 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/elbv2/x-elbv2.spec.json
+-rw-r--r--   0        0        0      414 2024-03-23 20:44:00.319060 ecs_composex-1.1.0rc2/ecs_composex/events/__init__.py
+-rw-r--r--   0        0        0     8913 2024-03-23 20:44:00.065064 ecs_composex-1.1.0rc2/ecs_composex/events/events_ecs.py
+-rw-r--r--   0        0        0     1882 2024-03-23 20:44:00.350059 ecs_composex-1.1.0rc2/ecs_composex/events/events_helpers.py
+-rw-r--r--   0        0        0      414 2024-03-23 20:44:00.454058 ecs_composex-1.1.0rc2/ecs_composex/events/events_module.py
+-rw-r--r--   0        0        0     6645 2024-03-23 20:44:00.174062 ecs_composex-1.1.0rc2/ecs_composex/events/events_stack.py
+-rw-r--r--   0        0        0     2053 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/events/x-events.spec.json
+-rw-r--r--   0        0        0      480 2024-03-23 20:44:00.183062 ecs_composex-1.1.0rc2/ecs_composex/exceptions.py
+-rw-r--r--   0        0        0     2487 2024-03-23 20:44:00.238061 ecs_composex-1.1.0rc2/ecs_composex/iam/__init__.py
+-rw-r--r--   0        0        0     6262 2024-03-23 20:43:59.999065 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_ecs_helpers.py
+-rw-r--r--   0        0        0      950 2024-03-23 20:44:00.149062 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_params.py
+-rw-r--r--   0        0        0     3415 2024-03-23 20:44:00.503057 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_stack.py
+-rw-r--r--   0        0        0     1781 2024-03-23 20:44:00.314060 ecs_composex-1.1.0rc2/ecs_composex/iam/import_sam_policies.py
+-rw-r--r--   0        0        0    67793 2024-04-14 21:59:42.080076 ecs_composex-1.1.0rc2/ecs_composex/iam/sam_policies.json
+-rw-r--r--   0        0        0    15021 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ingress_settings.py
+-rw-r--r--   0        0        0      421 2024-03-23 20:44:00.080063 ecs_composex-1.1.0rc2/ecs_composex/kinesis/__init__.py
+-rw-r--r--   0        0        0     4732 2023-11-29 08:40:57.722589 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kcl_helpers.py
+-rw-r--r--   0        0        0     2984 2024-03-23 20:44:00.113063 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_kinesis_firehose.py
+-rw-r--r--   0        0        0      421 2024-03-23 20:44:00.013064 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_module.py
+-rw-r--r--   0        0        0      535 2024-03-23 20:43:59.864067 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_params.py
+-rw-r--r--   0        0        0     1022 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_perms.json
+-rw-r--r--   0        0        0     7714 2024-03-23 20:44:00.294060 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_stack.py
+-rw-r--r--   0        0        0     2630 2024-03-23 20:44:00.365059 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_template.py
+-rw-r--r--   0        0        0     2692 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kinesis/x-kinesis.spec.json
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.213061 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/__init__.py
+-rw-r--r--   0        0        0     2946 2024-03-23 20:44:00.246061 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py
+-rw-r--r--   0        0        0     4602 2024-03-23 20:43:59.821067 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.190062 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_module.py
+-rw-r--r--   0        0        0      624 2024-03-23 20:43:59.996065 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_params.py
+-rw-r--r--   0        0        0      205 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_perms.json
+-rw-r--r--   0        0        0     6686 2024-03-23 20:44:00.421058 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py
+-rw-r--r--   0        0        0     4278 2024-03-23 20:44:00.436058 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_template.py
+-rw-r--r--   0        0        0     1858 2024-04-14 21:59:41.106094 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.044064 ecs_composex-1.1.0rc2/ecs_composex/kms/__init__.py
+-rw-r--r--   0        0        0     2102 2024-03-23 20:44:00.452058 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_ecs_cluster.py
+-rw-r--r--   0        0        0     4549 2024-03-23 20:43:59.905066 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_kinesis_firehose.py
+-rw-r--r--   0        0        0      409 2024-03-23 20:44:00.312060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_module.py
+-rw-r--r--   0        0        0      956 2024-03-23 20:44:00.327060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_params.py
+-rw-r--r--   0        0        0     1169 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_perms.json
+-rw-r--r--   0        0        0     2556 2024-03-23 20:44:00.216061 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_s3.py
+-rw-r--r--   0        0        0     2311 2024-03-23 20:43:59.888066 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_sqs.py
+-rw-r--r--   0        0        0     9013 2024-03-23 20:44:00.292060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_stack.py
+-rw-r--r--   0        0        0     1479 2024-03-23 20:43:59.951065 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_template.py
+-rw-r--r--   0        0        0      826 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kms/x-kms.spec.json
+-rw-r--r--   0        0        0    12383 2024-03-23 20:43:59.988065 ecs_composex-1.1.0rc2/ecs_composex/mods_manager.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.052064 ecs_composex-1.1.0rc2/ecs_composex/neptune/__init__.py
+-rw-r--r--   0        0        0      478 2024-03-23 20:44:00.208062 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_module.py
+-rw-r--r--   0        0        0      864 2024-03-23 20:43:59.941066 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_params.py
+-rw-r--r--   0        0        0      337 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_perms.json
+-rw-r--r--   0        0        0     9212 2024-03-23 20:44:00.459057 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_stack.py
+-rw-r--r--   0        0        0     5088 2024-03-23 20:44:00.250061 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_template.py
+-rw-r--r--   0        0        0     3013 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/neptune/x-neptune.spec.json
+-rw-r--r--   0        0        0      488 2024-03-23 20:43:59.858067 ecs_composex-1.1.0rc2/ecs_composex/opensearch/__init__.py
+-rw-r--r--   0        0        0     2441 2024-03-23 20:44:00.188062 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_aws.py
+-rw-r--r--   0        0        0      487 2024-03-23 20:43:59.981065 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_module.py
+-rw-r--r--   0        0        0      950 2024-03-23 20:44:00.007065 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_params.py
+-rw-r--r--   0        0        0      983 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_perms.json
+-rw-r--r--   0        0        0     6315 2024-03-23 20:44:00.073063 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_stack.py
+-rw-r--r--   0        0        0    22533 2024-03-23 20:44:00.325060 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_template.py
+-rw-r--r--   0        0        0     3216 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/opensearch/x-opensearch.spec.json
+-rw-r--r--   0        0        0       19 2021-03-04 09:40:13.444136 ecs_composex-1.1.0rc2/ecs_composex/rds/.gitignore
+-rw-r--r--   0        0        0      146 2024-03-23 20:43:59.813068 ecs_composex-1.1.0rc2/ecs_composex/rds/__init__.py
+-rw-r--r--   0        0        0     1703 2024-03-23 20:44:00.465057 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_conditions.py
+-rw-r--r--   0        0        0    20461 2024-03-23 20:43:59.939066 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_db_template.py
+-rw-r--r--   0        0        0     5939 2024-03-23 20:44:00.180062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features.py
+-rw-r--r--   0        0        0     5448 2024-03-23 20:44:00.509057 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features_define.py
+-rw-r--r--   0        0        0      455 2024-03-23 20:44:00.417058 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_module.py
+-rw-r--r--   0        0        0     3624 2024-03-23 20:44:00.146062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_parameter_groups_helper.py
+-rw-r--r--   0        0        0     2898 2024-03-23 20:44:00.305060 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_params.py
+-rw-r--r--   0        0        0      164 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_perms.json
+-rw-r--r--   0        0        0    10438 2024-03-23 20:43:59.953065 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_stack.py
+-rw-r--r--   0        0        0     4557 2024-03-23 20:44:00.164062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_template.py
+-rw-r--r--   0        0        0     5948 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/rds/x-rds.spec.json
+-rw-r--r--   0        0        0    22462 2024-04-14 21:58:44.889124 ecs_composex-1.1.0rc2/ecs_composex/rds_resources_settings.py
+-rw-r--r--   0        0        0    27883 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/resource_settings.py
+-rw-r--r--   0        0        0     8660 2024-03-23 20:44:00.440058 ecs_composex-1.1.0rc2/ecs_composex/resources_import.py
+-rw-r--r--   0        0        0        0 2022-06-16 20:44:41.834935 ecs_composex-1.1.0rc2/ecs_composex/route53/__init__.py
+-rw-r--r--   0        0        0     4385 2024-03-23 20:44:00.037064 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_acm.py
+-rw-r--r--   0        0        0     5433 2024-03-23 20:44:00.134063 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_elbv2.py
+-rw-r--r--   0        0        0     3983 2024-03-23 20:44:00.371059 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_helpers.py
+-rw-r--r--   0        0        0      429 2024-03-23 20:44:00.303060 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_module.py
+-rw-r--r--   0        0        0     1136 2024-03-23 20:44:00.154062 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_params.py
+-rw-r--r--   0        0        0     7828 2024-03-23 20:44:00.448058 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_stack.py
+-rw-r--r--   0        0        0     1476 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/route53/x-route53.spec.json
+-rw-r--r--   0        0        0      283 2024-03-23 20:44:00.111063 ecs_composex-1.1.0rc2/ecs_composex/s3/__init__.py
+-rw-r--r--   0        0        0     7451 2024-03-23 20:43:59.913066 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_bucket.py
+-rw-r--r--   0        0        0     2581 2024-03-23 20:44:00.033064 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_ecs_cluster.py
+-rw-r--r--   0        0        0     3848 2024-03-23 20:44:00.307060 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_kinesis_firehose.py
+-rw-r--r--   0        0        0      406 2024-03-23 20:44:00.105063 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_module.py
+-rw-r--r--   0        0        0     2289 2024-03-23 20:44:00.031064 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_params.py
+-rw-r--r--   0        0        0     3566 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_perms.json
+-rw-r--r--   0        0        0     5135 2024-03-23 20:44:00.438058 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_stack.py
+-rw-r--r--   0        0        0     7858 2024-03-23 20:44:00.115063 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_template.py
+-rw-r--r--   0        0        0     3232 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/s3/x-s3.spec.json
+-rw-r--r--   0        0        0     2948 2024-03-23 20:44:00.003065 ecs_composex-1.1.0rc2/ecs_composex/secrets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-03-23 20:44:00.198062 ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_aws.py
+-rw-r--r--   0        0        0      493 2024-03-23 20:44:00.290060 ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_params.py
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.338060 ecs_composex-1.1.0rc2/ecs_composex/sns/__init__.py
+-rw-r--r--   0        0        0     2625 2024-03-23 20:44:00.218061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_helpers.py
+-rw-r--r--   0        0        0      407 2024-03-23 20:43:59.872067 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_module.py
+-rw-r--r--   0        0        0      698 2024-03-23 20:44:00.257061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_params.py
+-rw-r--r--   0        0        0      128 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_perms.json
+-rw-r--r--   0        0        0     2377 2024-03-23 20:44:00.233061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_stack.py
+-rw-r--r--   0        0        0     1286 2024-03-23 20:43:59.823068 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_templates.py
+-rw-r--r--   0        0        0      696 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/sns/x-sns.spec.json
+-rw-r--r--   0        0        0      281 2024-03-23 20:44:00.446058 ecs_composex-1.1.0rc2/ecs_composex/specs/__init__.py
+-rw-r--r--   0        0        0      742 2024-03-23 20:44:00.143062 ecs_composex-1.1.0rc2/ecs_composex/specs/_core.py
+-rw-r--r--   0        0        0    29055 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/compose-spec.json
+-rw-r--r--   0        0        0     2455 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/ingress.spec.json
+-rw-r--r--   0        0        0     1234 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/secrets.x-secrets.spec.json
+-rw-r--r--   0        0        0     2266 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services-xray.spec.json
+-rw-r--r--   0        0        0     1404 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-alarms.spec.json
+-rw-r--r--   0        0        0      403 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-codeguru_profiler.spec.json
+-rw-r--r--   0        0        0      501 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-docker_opts.spec.json
+-rw-r--r--   0        0        0     1853 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecr.spec.json
+-rw-r--r--   0        0        0     2745 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecs.spec.json
+-rw-r--r--   0        0        0      836 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-environment.spec.json
+-rw-r--r--   0        0        0     2175 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-iam.spec.json
+-rw-r--r--   0        0        0     7429 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-logging.spec.json
+-rw-r--r--   0        0        0     1986 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-monitoring.spec.json
+-rw-r--r--   0        0        0     4477 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-network.spec.json
+-rw-r--r--   0        0        0     4724 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-prometheus.spec.json
+-rw-r--r--   0        0        0     4105 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-scaling.spec.json
+-rw-r--r--   0        0        0     2133 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-cluster.spec.json
+-rw-r--r--   0        0        0     6706 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-rds-common.spec.json
+-rw-r--r--   0        0        0     6559 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/x-resources.common.spec.json
+-rw-r--r--   0        0        0      816 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-tags.spec.json
+-rw-r--r--   0        0        0      285 2024-03-23 20:44:00.279060 ecs_composex-1.1.0rc2/ecs_composex/sqs/__init__.py
+-rw-r--r--   0        0        0     4737 2024-03-23 20:43:59.937066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_ecs_scaling.py
+-rw-r--r--   0        0        0     3592 2024-03-23 20:43:59.890066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_helpers.py
+-rw-r--r--   0        0        0      407 2024-03-23 20:43:59.836067 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_module.py
+-rw-r--r--   0        0        0      865 2024-03-23 20:44:00.141063 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_params.py
+-rw-r--r--   0        0        0      515 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_perms.json
+-rw-r--r--   0        0        0     5463 2024-03-23 20:44:00.050064 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_s3.py
+-rw-r--r--   0        0        0     2938 2024-03-23 20:44:00.383059 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_sqs.py
+-rw-r--r--   0        0        0     4375 2024-03-23 20:43:59.917066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_stack.py
+-rw-r--r--   0        0        0     7648 2024-03-23 20:44:00.273060 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_template.py
+-rw-r--r--   0        0        0      744 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/sqs/x-sqs.spec.json
+-rw-r--r--   0        0        0      488 2024-03-23 20:44:00.020064 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/__init__.py
+-rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.195062 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_helpers.py
+-rw-r--r--   0        0        0      488 2024-03-23 20:43:59.935066 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_module.py
+-rw-r--r--   0        0        0      905 2024-03-23 20:44:00.263061 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_params.py
+-rw-r--r--   0        0        0      820 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_perms.json
+-rw-r--r--   0        0        0     3924 2024-03-23 20:44:00.011065 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_stack.py
+-rw-r--r--   0        0        0     2243 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json
+-rw-r--r--   0        0        0       88 2024-03-23 20:44:00.296060 ecs_composex-1.1.0rc2/ecs_composex/utils/__init__.py
+-rw-r--r--   0        0        0      820 2024-03-23 20:44:00.344059 ecs_composex-1.1.0rc2/ecs_composex/utils/init_ecs.py
+-rw-r--r--   0        0        0     1797 2024-03-23 20:43:59.992065 ecs_composex-1.1.0rc2/ecs_composex/utils/init_s3.py
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.497057 ecs_composex-1.1.0rc2/ecs_composex/vpc/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-23 20:44:00.255061 ecs_composex-1.1.0rc2/ecs_composex/vpc/aws_mappings.py
+-rw-r--r--   0        0        0     3997 2024-03-23 20:43:59.919066 ecs_composex-1.1.0rc2/ecs_composex/vpc/helpers.py
+-rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.071064 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_aws.py
+-rw-r--r--   0        0        0     1338 2024-03-23 20:44:00.357059 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_cloudmap.py
+-rw-r--r--   0        0        0       88 2024-03-23 20:43:59.834067 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_conditions.py
+-rw-r--r--   0        0        0     1953 2024-03-23 20:44:00.377059 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_maths.py
+-rw-r--r--   0        0        0      423 2024-03-23 20:44:00.499057 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_module.py
+-rw-r--r--   0        0        0     2217 2024-03-23 20:44:00.253061 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_params.py
+-rw-r--r--   0        0        0    14983 2024-03-23 20:44:00.442058 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_stack.py
+-rw-r--r--   0        0        0    10517 2024-03-23 20:44:00.161062 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_subnets.py
+-rw-r--r--   0        0        0     4709 2024-03-23 20:44:00.109063 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_template.py
+-rw-r--r--   0        0        0     3504 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/vpc/x-vpc.spec.json
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.336059 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/__init__.py
+-rw-r--r--   0        0        0      697 2024-03-23 20:44:00.119063 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/validators_wafv2.py
+-rw-r--r--   0        0        0     2255 2024-03-23 20:44:00.288060 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py
+-rw-r--r--   0        0        0      497 2024-03-23 20:44:00.169062 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_module.py
+-rw-r--r--   0        0        0     1079 2024-03-23 20:43:59.850067 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_params.py
+-rw-r--r--   0        0        0      185 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_perms.json
+-rw-r--r--   0        0        0     9460 2024-03-23 20:44:00.373059 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py
+-rw-r--r--   0        0        0     1357 2024-03-23 20:44:00.423058 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_template.py
+-rw-r--r--   0        0        0     1772 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json
+-rw-r--r--   0        0        0     3476 2024-04-14 21:59:40.442106 ecs_composex-1.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     8907 1970-01-01 00:00:00.000000 ecs_composex-1.1.0rc2/PKG-INFO
```

### Comparing `ecs_composex-1.1.0rc1/LICENSE` & `ecs_composex-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/NOTICES.rst` & `ecs_composex-1.1.0rc2/NOTICES.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/README.rst` & `ecs_composex-1.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/acm/acm_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/acm/acm_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/acm/acm_stack_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/acm/x-acm.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/acm/x-acm.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_elbv2.py` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/alarms_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/alarms/x-alarms.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/alarms/x-alarms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_conditions.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_mesh.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_mesh.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_node.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_node.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_router.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_router.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/appmesh_service.py` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_service.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/appmesh/x-appmesh.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/appmesh/x-appmesh.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/aps/aps_parameters.py` & `ecs_composex-1.1.0rc2/ecs_composex/aps/aps_parameters.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/aps/aps_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/aps/aps_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/aps/x-aps.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/aps/x-aps.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cli.py` & `ecs_composex-1.1.0rc2/ecs_composex/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/cloudmap_x_resources.py` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cloudmap/x-cloudmap.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/x-cloudmap.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/cognito_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/cognito_userpool/cognito_userpool_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/cfn_conditions.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/cfn_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/cfn_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/cfn_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/envsubst.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/envsubst.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/files.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/files.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/logging.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/settings.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/stacks/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/tagging.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/tagging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/common/troposphere_tools.py` & `ecs_composex-1.1.0rc2/ecs_composex/common/troposphere_tools.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_networks.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_networks.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/ecs_family_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_secrets/services_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/services_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/docker_tools.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/docker_tools.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/env_files_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/env_files_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/kernel_options_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/kernel_options_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/docker_opts.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/docker_opts.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/ecr_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_logging/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_services/service_logging/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/ecs_family_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/compose_volumes/services_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/services_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/api_x_resources.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/api_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/environment_x_resources.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/environment_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/network_x_resources.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/network_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/compose/x_resources/services_resources.py` & `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/services_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dashboards/dashboards_services_metrics.py` & `ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_services_metrics.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dashboards/dashboards_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dashboards/x-dashboards.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/dashboards/x-dashboards.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/docdb/docdb_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/docdb/x-docdb.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/docdb/x-docdb.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_autoscaling.py` & `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_autoscaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dynamodb/dynamodb_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/dynamodb/x-dynamodb.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/x-dynamodb.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_conditions.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,17 +300,18 @@
         """
         Generates a list of CFN outputs for the ECS Service and Task Definition
         """
         if self.service_networking.security_group:
             self.outputs.append(
                 CfnOutput(
                     f"{self.logical_name}GroupId",
-                    Value=GetAtt(self.service_networking.security_group, "GroupId"),
+                    Value=Ref(self.service_networking.security_group.parameter.title),
                 )
             )
+        if ecs_params.SERVICE_SUBNETS.title in self.stack.stack_template.parameters:
             self.outputs.append(
                 CfnOutput(
                     ecs_params.SERVICE_SUBNETS.title,
                     Value=Join(",", self.service_networking.subnets_output),
                 )
             )
 
@@ -419,34 +420,32 @@
 
     def init_network_settings(
         self, settings: ComposeXSettings, vpc_stack: ComposeXStack, families_sg_stack
     ) -> None:
         """
         Once we have figured out the compute settings (EXTERNAL vs other)
         """
-        from ecs_composex.ecs.service_networking.helpers import add_security_group
 
         self.service_networking = ServiceNetworking(self, families_sg_stack)
         self.finalize_services_networking_settings(settings)
         if self.service_compute.launch_type == "EXTERNAL":
             LOG.debug(f"{self.name} Ingress cannot be set (EXTERNAL mode). Skipping")
         else:
             if vpc_stack.vpc_resource.mappings:
                 self.stack.set_vpc_params_from_vpc_lookup(vpc_stack, settings)
             else:
                 self.stack.set_vpc_parameters_from_vpc_stack(vpc_stack, settings)
-            add_security_group(self)
             self.service_networking.ingress.set_aws_sources_ingress(
                 settings,
                 self.logical_name,
-                GetAtt(self.service_networking.security_group, "GroupId"),
+                Ref(self.service_networking.security_group.parameter.title),
             )
             self.service_networking.ingress.set_ext_sources_ingress(
                 self.logical_name,
-                GetAtt(self.service_networking.security_group, "GroupId"),
+                Ref(self.service_networking.security_group.parameter.title),
             )
             self.service_networking.ingress.associate_aws_ingress_rules(self.template)
             self.service_networking.ingress.associate_ext_ingress_rules(self.template)
             self.service_networking.add_self_ingress()
 
     def finalize_family_settings(self, settings: ComposeXSettings):
         """
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_logging/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/family_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/task_execute_command.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_execute_command.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_family/task_runtime.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_runtime.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/emf_processors.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/emf_processors.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_prometheus/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_service/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_service/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/ecs_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/helpers/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/aws_xray.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_xray.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_alarms/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_alarms/service_predefined_alarms.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/service_predefined_alarms.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_compute/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_compute/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from ecs_composex.ecs.ecs_family import ComposeFamily
     from ecs_composex.cloudmap.cloudmap_ecs import EcsDiscoveryService
     from ecs_composex.ecs_ingress.ecs_ingress_stack import (
         XStack as EcsIngressStack,
         ServiceSecurityGroup,
     )
     from ecs_composex.common.settings import ComposeXSettings
+    from troposphere.ecs import ServiceConnectConfiguration
 
 from itertools import chain
 
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from troposphere import (
     AWS_ACCOUNT_ID,
     AWSHelperFn,
@@ -72,19 +73,18 @@
             )
             self.network_mode = "bridge"
         self.ports = []
         self.networks = {}
         self.merge_services_ports()
         self.merge_networks()
         self.definition = merge_family_services_networking(family)
-        self._security_group = None
-        self.inter_services_sg: ServiceSecurityGroup = (
-            families_sg_stack.services_mappings[family.name]
-        )
-        self.extra_security_groups = [self.inter_services_sg.parameter]
+        self.security_group: ServiceSecurityGroup = families_sg_stack.services_mappings[
+            family.name
+        ]
+        self.extra_security_groups = [self.security_group.parameter]
         self._subnets = Ref(APP_SUBNETS)
         self.cloudmap_config = (
             merge_cloudmap_settings(family, self.ports) if self.ports else {}
         )
         self.ecs_connect_config: ServiceConnectConfiguration | None = None
         self.ingress = Ingress(self.definition[Ingress.master_key], self.ports)
 
@@ -135,46 +135,29 @@
                 "At least one service in definition has AssignPublicIp set to True."
             )
             return "ENABLED"
         return "DISABLED"
 
     @property
     def security_groups(self) -> list:
-        groups = [Ref(self.security_group)]
+        groups = [Ref(self.security_group.parameter.title)]
         for extra_group in self.extra_security_groups:
             if (
                 isinstance(extra_group, SecurityGroup)
                 and extra_group.title in self.family.template.resources
             ):
                 groups.append(Ref(extra_group))
             elif isinstance(extra_group, Parameter):
                 add_parameters(self.family.template, [extra_group])
                 groups.append(Ref(extra_group))
             elif isinstance(extra_group, FindInMap):
                 groups.append(extra_group)
         return groups
 
     @property
-    def security_group(self):
-        return self._security_group
-
-    @security_group.setter
-    def security_group(self, value):
-        if isinstance(value, SecurityGroup):
-            self._security_group = value
-        else:
-            raise TypeError(
-                "Service security group must be",
-                SecurityGroup,
-                "Got",
-                value,
-                type(value),
-            )
-
-    @property
     def network_mode(self):
         """
         The network mode used for the Task/Service. valid are host/bridge/awsvpc.
         Defaults to awsvpc. Only override is to bridge/host based on the Launch Type
         """
         return self._network_mode
 
@@ -266,19 +249,19 @@
             self.ingress.to_self_rules.append(
                 SecurityGroupIngress(
                     f"AllowingInterCommunicationPort{target_port}{port['protocol']}",
                     template=self.family.template,
                     FromPort=target_port,
                     ToPort=target_port,
                     IpProtocol=port["protocol"],
-                    GroupId=GetAtt(
-                        self.family.service_networking.security_group, "GroupId"
+                    GroupId=Ref(
+                        self.family.service_networking.security_group.parameter
                     ),
-                    SourceSecurityGroupId=GetAtt(
-                        self.family.service_networking.security_group, "GroupId"
+                    SourceSecurityGroupId=Ref(
+                        self.family.service_networking.security_group.parameter
                     ),
                     SourceSecurityGroupOwnerId=Ref(AWS_ACCOUNT_ID),
                     Description=Sub(
                         f"Internal traffic on {target_port}/{port['protocol']}"
                     ),
                 )
             )
@@ -295,17 +278,15 @@
             return
         for port in self.ports:
             title = f"FromLB{lb_name}To{self.family.stack.title}On{port['target']}"
             common_args = {
                 "FromPort": port["target"],
                 "ToPort": port["target"],
                 "IpProtocol": port["protocol"],
-                "GroupId": GetAtt(
-                    self.family.service_networking.security_group, "GroupId"
-                ),
+                "GroupId": Ref(self.security_group.parameter.title),
                 "SourceSecurityGroupOwnerId": Ref(AWS_ACCOUNT_ID),
                 "Description": Sub(
                     f"From ELB {lb_name} to ${{{SERVICE_NAME.title}}} on port {port['target']}"
                 ),
             }
             if title in self.family.template.resources:
                 return
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,27 @@
 #  SPDX-License-Identifier: MPL-2.0
 #  Copyright 2020-2022 John Mille <john@compose-x.io>
 
-from troposphere import Ref, StackName, Sub, Tags
-from troposphere.ec2 import SecurityGroup
+from __future__ import annotations
 
-from ecs_composex.common.cfn_conditions import define_stack_name
-from ecs_composex.common.logging import LOG
-from ecs_composex.common.troposphere_tools import add_resource
-from ecs_composex.ecs.ecs_params import SERVICE_NAME, SG_T
-from ecs_composex.vpc.vpc_params import VPC_ID
+from typing import TYPE_CHECKING
 
+if TYPE_CHECKING:
+    from ecs_composex.ecs.ecs_family import ComposeFamily
+    from ecs_composex.common.settings import ComposeXSettings
 
-def add_security_group(family) -> None:
-    """
-    Creates a new EC2 SecurityGroup and assigns to ecs_service.network_settings
-    Adds the security group to the family template resources.
+from troposphere import Ref
 
-    :param ecs_composex.ecs.ecs_family.ComposeFamily family:
-    """
-    family.service_networking.security_group = SecurityGroup(
-        SG_T,
-        GroupDescription=Sub(
-            f"SG for ${{{SERVICE_NAME.title}}} - ${{STACK_NAME}}",
-            STACK_NAME=define_stack_name(),
-        ),
-        Tags=Tags(
-            {
-                "Name": Sub(
-                    f"${{{SERVICE_NAME.title}}}-${{STACK_NAME}}",
-                    STACK_NAME=define_stack_name(),
-                ),
-                "StackName": StackName,
-                "MicroserviceName": Ref(SERVICE_NAME),
-            }
-        ),
-        VpcId=Ref(VPC_ID),
-    )
-    add_resource(family.template, family.service_networking.security_group)
+from ecs_composex.common.logging import LOG
 
 
-def update_family_subnets(family, settings) -> None:
+def update_family_subnets(family: ComposeFamily, settings: ComposeXSettings) -> None:
     """
-    Method to update the stack parameters
-
-    :param ecs_composex.ecs.ecs_family.ComposeFamily family:
-    :param ecs_composex.common.settings.ComposeXSettings settings:
+    Update the stack parameters of the family stack AppSubnets Parameter value to the one matching with
+    networks.x-vpc and networks.[]
     """
     network_names = list(family.service_networking.networks.keys())
     for network in settings.networks:
         if not network.subnet_name:
             continue
         if network.name in network_names:
             family.service_networking.subnets = Ref(network.subnet_name)
@@ -59,15 +32,19 @@
             break
     else:
         LOG.error(
             f"{family.name}.networks - unable to assign AppSubnets to a top-level defined network"
         )
 
 
-def set_family_hostname(family):
+def set_family_hostname(family: ComposeFamily):
+    """
+    Sets the hostname to use for the Family in Cloudmap.
+    If it has been set on more than one service container, it uses the first one.
+    """
     svcs_hostnames = any(svc.family_hostname for svc in family.services)
     if not svcs_hostnames or not family.family_hostname:
         LOG.debug(
             f"{family.name} - No ecs.task.family.hostname defined on any of the services. "
             f"Setting to {family.family_hostname}"
         )
         return
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_networking/ingress_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/ingress_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,19 +212,19 @@
                 f"On{target_port}{_service_port_def['protocol'].title()}"
             )
             add_resource(
                 families_sg_stack.stack_template,
                 SecurityGroupIngress(
                     ingress_title,
                     SourceSecurityGroupId=GetAtt(
-                        _service.family.service_networking.inter_services_sg.cfn_resource,
+                        _service.family.service_networking.security_group.cfn_resource,
                         "GroupId",
                     ),
                     GroupId=GetAtt(
-                        dst_family.service_networking.inter_services_sg.cfn_resource,
+                        dst_family.service_networking.security_group.cfn_resource,
                         "GroupId",
                     ),
                     **common_args,
                 ),
             )
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_scaling/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/service_scaling/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/task_compute/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/task_compute/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs/task_iam/task_role.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/task_role.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/ecs_family_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs_cluster/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs_composex.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs_composex.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ecs_ingress/ecs_ingress_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/ecs_ingress_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/efs/efs_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/efs/efs_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/efs/efs_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/efs/x-efs.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/efs/x-efs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elasticache/elasticache_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                     raise ValueError(
                         f"{self.lb.module.res_key}.{self.lb.name} - Listener {self.port}"
                         f" - Target {target['name']} is not a valid value. Must match",
                         LISTENER_TARGET_RE.pattern,
                     )
                 if (
                     f"{target_parts.group('family')}:{target_parts.group('container')}"
-                    not in [svc["name"] for svc in self.lb.services]
+                    not in [_family_service for _family_service in self.lb.services]
                 ):
                     self.definition["Targets"].remove(target)
         if not self.definition["Targets"]:
             return
 
     def handle_cognito_pools(self, settings, listener_stack):
         """
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/elbv2_stack/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/elbv2/x-elbv2.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/elbv2/x-elbv2.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/events/events_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/events/events_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/events/events_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/events/events_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/events/events_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/events/events_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/events/x-events.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/events/x-events.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/iam_ecs_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_ecs_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/iam_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/iam_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/import_sam_policies.py` & `ecs_composex-1.1.0rc2/ecs_composex/iam/import_sam_policies.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/iam/sam_policies.json` & `ecs_composex-1.1.0rc2/ecs_composex/iam/sam_policies.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ingress_settings.py` & `ecs_composex-1.1.0rc2/ecs_composex/ingress_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2020-2022 John Mille <john@compose-x.io>
 
 """
 Module to help with defining the network settings for the ECS Service based on the family services definitions.
 """
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from troposphere import AWSHelperFn
+    from ecs_composex.common.settings import ComposeXSettings
+
 import re
 from copy import deepcopy
 from ipaddress import IPv4Interface
 from json import dumps
 
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from troposphere import AWS_ACCOUNT_ID, AWS_NO_VALUE, Ref, Sub
@@ -149,22 +157,16 @@
                     "published": port,
                     "target": port,
                 }
             )
     return service_ports
 
 
-def lookup_security_group(settings, lookup):
-    """
-    Function to fetch the security group ID based on lookup details
-
-    :param ecs_composex.common.settings.ComposeXSettings settings:
-    :param lookup:
-    :return:
-    """
+def lookup_security_group(settings: ComposeXSettings, lookup: dict | list) -> str:
+    """Function to fetch the security group ID based on lookup details"""
     sg_re = re.compile(
         r"^arn:aws(?:-[a-z]+)?:ec2:[a-z0-9-]+:\d{12}:security-group/([\S]+)$"
     )
     ec2_types = {
         "ec2:security-group": {"regexp": sg_re.pattern},
     }
     lookup_session = define_lookup_role_from_info(lookup, settings.session)
@@ -235,22 +237,56 @@
         self.aws_ingress_rules = []
         self.ext_ingress_rules = []
         self.to_self_rules = []
 
     def __repr__(self):
         return dumps(self.definition, indent=2)
 
-    def set_aws_sources_ingress(self, settings, destination_title, sg_ref) -> None:
+    def handle_security_group_source(
+        self,
+        source,
+        common_args: dict,
+        destination_title: str,
+        target_port: int,
+        settings,
+    ) -> None:
         """
-        Method to define AWS Sources ingresses
-
-        :param settings:
-        :param destination_title:
-        :param sg_ref:
+        Method to handle SecurityGroup sources
+        It updates the list of AWS sources ingress rules that will later be added to the stack template of the family
         """
+        if keyisset("Id", source):
+            sg_id = source["Id"]
+        elif keyisset("Lookup", source):
+            sg_id = lookup_security_group(settings, source["Lookup"])
+        else:
+            raise KeyError(
+                "Information missing to identify the SecurityGroup. Requires either Id or Lookup"
+            )
+        common_args.update(
+            {
+                "Description": Sub(
+                    f"From {sg_id} to {destination_title} on port {target_port}"
+                )
+            }
+        )
+        self.aws_ingress_rules.append(
+            SecurityGroupIngress(
+                f"From{NONALPHANUM.sub('', sg_id)}ToServiceOn{target_port}",
+                SourceSecurityGroupId=sg_id,
+                SourceSecurityGroupOwnerId=set_else_none(
+                    "AccountOwner", source, Ref(AWS_ACCOUNT_ID)
+                ),
+                **common_args,
+            )
+        )
+
+    def set_aws_sources_ingress(
+        self, settings: ComposeXSettings, destination_title: str, sg_ref: AWSHelperFn
+    ) -> None:
+        """Method to define AWS Sources ingresses"""
         for source in self.aws_sources:
             for port in self.ports:
                 if (
                     keyisset("Ports", source)
                     and keyisset("published", port)
                     and port["published"] not in source["Ports"]
                 ):
@@ -265,50 +301,28 @@
                 common_args = {
                     "FromPort": target_port,
                     "ToPort": target_port,
                     "IpProtocol": port["protocol"],
                     "GroupId": sg_ref,
                 }
                 if source["Type"] == "SecurityGroup":
-                    if keyisset("Id", source):
-                        sg_id = source["Id"]
-                    elif keyisset("Lookup", source):
-                        sg_id = lookup_security_group(settings, source["Lookup"])
-                    else:
-                        raise KeyError(
-                            "Information missing to identify the SecurityGroup. Requires either Id or Lookup"
-                        )
-                    common_args.update(
-                        {
-                            "Description": Sub(
-                                f"From {sg_id} to {destination_title} on port {target_port}"
-                            )
-                        }
-                    )
-                    self.aws_ingress_rules.append(
-                        SecurityGroupIngress(
-                            f"From{NONALPHANUM.sub('', sg_id)}ToServiceOn{target_port}",
-                            SourceSecurityGroupId=sg_id,
-                            SourceSecurityGroupOwnerId=set_else_none(
-                                "AccountOwner", source, Ref(AWS_ACCOUNT_ID)
-                            ),
-                            **common_args,
-                        )
+                    self.handle_security_group_source(
+                        source, common_args, destination_title, target_port, settings
                     )
                 elif source["Type"] == "PrefixList":
                     self.aws_ingress_rules.append(
                         SecurityGroupIngress(
                             f"From{NONALPHANUM.sub('', source['Id'])}ToServiceOn{target_port}",
                             SourcePrefixListId=source["Id"],
                             **common_args,
                         )
                     )
 
     def create_ext_sources_ingress_rule(
-        self, destination_title, allowed_source, security_group, **props
+        self, destination_title, allowed_source, security_group: AWSHelperFn, **props
     ) -> None:
         """
         Creates the Security Ingress rule for a CIDR based rule
 
         :param str destination_title:
         :param dict allowed_source:
         :param security_group:
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kcl_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kcl_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_kinesis_firehose.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/kinesis_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis/x-kinesis.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis/x-kinesis.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/kinesis_firehose_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_ecs_cluster.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_ecs_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_kinesis_firehose.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_s3.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_sqs.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_sqs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/kms_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/kms/x-kms.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/kms/x-kms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/mods_manager.py` & `ecs_composex-1.1.0rc2/ecs_composex/mods_manager.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/neptune/neptune_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/neptune/x-neptune.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/neptune/x-neptune.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/opensearch_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/opensearch/x-opensearch.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/opensearch/x-opensearch.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_conditions.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_db_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_db_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_features.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_features_define.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features_define.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_parameter_groups_helper.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_parameter_groups_helper.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/rds_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds/x-rds.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/rds/x-rds.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/rds_resources_settings.py` & `ecs_composex-1.1.0rc2/ecs_composex/rds_resources_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from ecs_composex.ecs.ecs_family import ComposeFamily
     from ecs_composex.common.settings import ComposeXSettings
     from ecs_composex.compose.x_resources.network_x_resources import (
         NetworkXResource,
         DatabaseXResource,
     )
     from ecs_composex.common.stacks import ComposeXStack
+    from ecs_composex.ecs.ecs_stack import ServiceStack
 
 from botocore.exceptions import ClientError
 from compose_x_common.aws import get_account_id
 from compose_x_common.aws.rds import RDS_DB_ID_CLUSTER_ARN_RE
 from compose_x_common.compose_x_common import keyisset, keypresent, set_else_none
 from troposphere import FindInMap, GetAtt, Ref, Sub
 from troposphere.ec2 import SecurityGroupIngress
@@ -376,33 +377,28 @@
     :param tuple target:
     """
     db_secrets = define_db_secrets(db, secret_import, target)
     for db_secret in db_secrets:
         extend_container_secrets(service.container_definition, db_secret)
 
 
-def add_security_group_ingress(service_stack: ComposeXStack, db_name: str, sg_id, port):
+def add_security_group_ingress(family: ComposeFamily, db_name: str, sg_id, port):
     """
-    Function to add a SecurityGroupIngress rule into the ECS Service template
-
-    :param ecs_composex.ecs.ServicesStack service_stack: The root stack for the services
-    :param str db_name: the name of the database to use for imports
-    :param sg_id: The security group Id to use for ingress. DB Security group, not service's
-    :param port: The port for Ingress to the DB.
+    Add a SecurityGroupIngress rule into the ECS Service template, allowing the Service access to the DB.
     """
     add_resource(
-        service_stack.stack_template,
+        family.stack.stack_template,
         SecurityGroupIngress(
-            f"AllowFrom{service_stack.title}to{db_name}",
+            f"AllowFrom{family.stack.title}to{db_name}",
             GroupId=sg_id,
             FromPort=port,
             ToPort=port,
-            Description=Sub(f"Allow FROM {service_stack.title} TO {db_name}"),
-            SourceSecurityGroupId=GetAtt(
-                service_stack.stack_template.resources[SG_T], "GroupId"
+            Description=Sub(f"Allow FROM {family.stack.title} TO {db_name}"),
+            SourceSecurityGroupId=Ref(
+                family.service_networking.security_group.parameter.title
             ),
             SourceSecurityGroupOwnerId=Ref("AWS::AccountId"),
             IpProtocol="6",
         ),
     )
 
 
@@ -549,15 +545,15 @@
         add_secrets_access_policy(
             target[0],
             db.attributes_outputs[db.db_secret_arn_parameter]["ImportValue"],
             db,
             use_task_role=grant_task_role_access,
         )
     add_security_group_ingress(
-        target[0].stack,
+        target[0],
         db.logical_name,
         sg_id=db.attributes_outputs[db.security_group_param]["ImportValue"],
         port=db.attributes_outputs[db.port_param]["ImportValue"],
     )
 
 
 def import_dbs(
@@ -600,15 +596,15 @@
                 target[0].stack, sg_parameter, settings
             )
             port_id = resource.add_attribute_to_another_stack(
                 target[0].stack, port_parameter, settings
             )
 
             add_security_group_ingress(
-                target[0].stack,
+                target[0],
                 resource.logical_name,
                 sg_id=Ref(sg_id["ImportParameter"]),
                 port=Ref(port_id["ImportParameter"]),
             )
         else:
             LOG.warning(
                 f"{resource.module.res_key}.{resource.name} - "
```

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/resource_settings.py` & `ecs_composex-1.1.0rc2/ecs_composex/resource_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/resources_import.py` & `ecs_composex-1.1.0rc2/ecs_composex/resources_import.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/route53_acm.py` & `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_acm.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/route53_elbv2.py` & `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/route53_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/route53_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/route53_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/route53/x-route53.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/route53/x-route53.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_bucket.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_ecs_cluster.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_ecs_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_kinesis_firehose.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/s3_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/s3/x-s3.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/s3/x-s3.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/secrets/__init__.py` & `ecs_composex-1.1.0rc2/ecs_composex/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/secrets/secrets_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sns/sns_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sns/sns_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sns/sns_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sns/sns_templates.py` & `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_templates.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sns/x-sns.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/sns/x-sns.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/_core.py` & `ecs_composex-1.1.0rc2/ecs_composex/specs/_core.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/compose-spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/compose-spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/ingress.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/ingress.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/secrets.x-secrets.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/secrets.x-secrets.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services-xray.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services-xray.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-alarms.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-alarms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-ecr.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecr.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-ecs.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-environment.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-environment.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-iam.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-iam.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-logging.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-logging.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-monitoring.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-monitoring.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-network.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-network.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-prometheus.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-prometheus.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/services.x-scaling.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-scaling.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/x-cluster.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/x-cluster.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/x-rds-common.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/x-rds-common.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/x-resources.common.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/x-resources.common.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/specs/x-tags.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/specs/x-tags.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_ecs_scaling.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_ecs_scaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_s3.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_sqs.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_sqs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/sqs_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/sqs/x-sqs.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/sqs/x-sqs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_perms.json` & `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/ssm_parameter_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/utils/init_ecs.py` & `ecs_composex-1.1.0rc2/ecs_composex/utils/init_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/utils/init_s3.py` & `ecs_composex-1.1.0rc2/ecs_composex/utils/init_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/aws_mappings.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/aws_mappings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/helpers.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_aws.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_cloudmap.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_cloudmap.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_maths.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_maths.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_subnets.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_subnets.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/vpc_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/vpc/x-vpc.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/vpc/x-vpc.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/validators_wafv2.py` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/validators_wafv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_params.py` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/wafv2_webacl_template.py` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json` & `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc1/pyproject.toml` & `ecs_composex-1.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_composex"
-version = "1.1.0-rc1"
+version = "1.1.0-rc2"
 description = "Manage, Configure and Deploy your services and AWS services and applications from your docker-compose definition"
 authors = ["John Preston <john@compose-x.io>"]
 maintainers = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 readme = "README.rst"
 keywords = ["compose-x", "aws", "cloudformation", "docker", "compose"]
 classifiers = [
@@ -80,15 +80,15 @@
 sphinx-jsonschema = "^1.19.1"
 sphinx-material = "^0.0.35"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs_composex"
 
 [tool.tbump.version]
-current = "1.1.0-rc1"
+current = "1.1.0-rc2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `ecs_composex-1.1.0rc1/PKG-INFO` & `ecs_composex-1.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs_composex
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Manage, Configure and Deploy your services and AWS services and applications from your docker-compose definition
 License: MPL-2.0
 Keywords: compose-x,aws,cloudformation,docker,compose
 Author: John Preston
 Author-email: john@compose-x.io
 Maintainer: John Preston
 Maintainer-email: john@compose-x.io
```

