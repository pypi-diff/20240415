# Comparing `tmp/nipyapi-0.9.0.tar.gz` & `tmp/nipyapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nipyapi-0.9.0.tar", last modified: Wed May 16 07:20:52 2018, max compression
+gzip compressed data, was "dist/nipyapi-0.9.1.tar", last modified: Fri May 18 12:20:36 2018, max compression
```

## Comparing `nipyapi-0.9.0.tar` & `nipyapi-0.9.1.tar`

### file list

```diff
@@ -1,417 +1,418 @@
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/
--rw-r--r--   0 dchaffey   (501) staff       (20)    16321 2018-05-16 07:20:52.000000 nipyapi-0.9.0/PKG-INFO
--rw-r--r--   0 dchaffey   (501) staff       (20)      594 2018-03-06 19:15:40.000000 nipyapi-0.9.0/LICENSE
--rw-r--r--   0 dchaffey   (501) staff       (20)      406 2018-03-06 22:24:08.000000 nipyapi-0.9.0/requirements.txt
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/demo/
--rw-r--r--   0 dchaffey   (501) staff       (20)     5845 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/console.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/demo/resources/
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/
--rw-r--r--   0 dchaffey   (501) staff       (20)     3121 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ks.jks
--rw-r--r--   0 dchaffey   (501) staff       (20)     1356 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.pem
--rw-r--r--   0 dchaffey   (501) staff       (20)      911 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.jks
--rw-r--r--   0 dchaffey   (501) staff       (20)     3488 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/client-ks.p12
--rw-r--r--   0 dchaffey   (501) staff       (20)     2673 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/client-cert.pem
--rw-r--r--   0 dchaffey   (501) staff       (20)     1144 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.p12
--rw-r--r--   0 dchaffey   (501) staff       (20)     3050 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/client-ks.jks
--rw-r--r--   0 dchaffey   (501) staff       (20)     4569 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/resources/keys/client-key.pem
--rw-r--r--   0 dchaffey   (501) staff       (20)        0 2018-05-01 17:07:19.000000 nipyapi-0.9.0/nipyapi/demo/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8262 2018-04-17 10:54:13.000000 nipyapi-0.9.0/nipyapi/demo/secure_connection.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     1432 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/demo/bbende_howdoideploymyflow.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     1088 2018-05-15 19:33:58.000000 nipyapi-0.9.0/nipyapi/system.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2881 2018-03-06 21:03:48.000000 nipyapi-0.9.0/nipyapi/config.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/nifi/
--rw-r--r--   0 dchaffey   (501) staff       (20)     7627 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/configuration.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/nifi/apis/
--rw-r--r--   0 dchaffey   (501) staff       (20)    41242 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/flowfile_queues_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    26509 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/policies_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9744 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/templates_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15335 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/connections_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15274 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/input_ports_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15065 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/labels_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    38958 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/data_transfer_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)   146919 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/process_groups_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    37965 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/processors_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    19574 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/provenance_events_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    34569 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/provenance_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10388 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/counters_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    66852 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/controller_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     1204 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    28981 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/reporting_tasks_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    38943 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/controller_services_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15317 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/output_ports_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15118 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/funnel_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)   181142 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/flow_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    14927 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/snippets_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5253 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/resources_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    50931 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/tenants_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5946 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/system_diagnostics_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    27280 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/remote_process_groups_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    73068 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/versions_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    47248 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/access_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9172 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/apis/site_to_site_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13406 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/rest.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18687 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/__init__.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/nifi/models/
--rw-r--r--   0 dchaffey   (501) staff       (20)     6590 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/link.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7879 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/user_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4799 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/explicit_restriction_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9138 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bulletin_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7856 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_funnel.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5123 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/create_template_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2778 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/uri_builder.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3995 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_comparison_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4425 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bulletin_board_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8778 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4683 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bundle.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4616 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    16390 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/drop_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5717 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/status_descriptor_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10496 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/version_info_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3688 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_state_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9598 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_configuration_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5002 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/lineage_results_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12286 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10708 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_label.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3565 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/registry_clients_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7172 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_difference_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    14327 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6006 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/action_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3501 2018-05-15 09:56:33.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_configuration_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8576 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_results_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5205 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/previous_value_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8185 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8321 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/affected_component_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    19542 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_remote_process_group.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4884 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/start_version_control_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9314 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_reference_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    17361 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7258 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7512 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/tenant_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7584 2018-05-15 12:13:10.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_breadcrumb_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3636 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/cluster_search_results_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4989 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_restriction_permission_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7400 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bucket.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8404 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/template_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4795 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4302 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/queue_size_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3356 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/peers_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5013 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/transaction_result_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3491 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4195 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/dimensions_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18254 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/counter_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11344 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    20433 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6916 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_reference_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5152 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/version_control_information_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15162 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_component_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5843 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_counters_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9194 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3774 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/create_active_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5425 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_status_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2805 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_details_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    17245 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4735 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_contents_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3443 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/snippet_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3395 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/labels_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18576 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5552 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/peer_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3690 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_history_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3540 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/drop_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5175 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/counters_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6034 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3623 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/cluste_summary_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    17413 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_file_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13619 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/listing_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9309 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/user_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3519 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/input_ports_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3341 2018-05-15 09:56:33.000000 nipyapi-0.9.0/nipyapi/nifi/models/about_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3827 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_options_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    22020 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5960 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/counter_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7995 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/template_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6105 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_bulletins_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/reporting_tasks_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8389 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_policy_summary_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7460 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bulletin_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10045 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9756 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5175 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/allowable_value_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6279 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/garbage_collection_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3546 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/output_ports_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6721 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_coordinates.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3476 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/resources_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3713 2018-05-15 09:56:33.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_configuration_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12562 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4207 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/banner_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2793 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/streaming_output.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3425 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/funnels_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4122 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/tenants_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    24088 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11156 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4610 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_services_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11369 2018-05-15 12:13:10.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_policy_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4245 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_metadata_set_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10693 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_file_summary_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5003 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/history_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3391 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/banner_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6650 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_link_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8808 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_port_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4883 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    36984 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4228 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/templates_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3450 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_file_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10520 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3775 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_types_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10825 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/documented_type_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    23680 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4241 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/required_permission_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4872 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/attribute_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4281 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3630 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/listing_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15410 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8268 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/instantiate_template_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4177 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_search_result_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7947 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/tenant_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3847 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/position_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4092 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/users_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6604 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/version_control_component_mapping_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9615 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4963 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/batch_settings_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5253 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/registry_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6390 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_remote_process_group_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3534 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/user_groups_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4099 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/search_result_group_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6119 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_status_snapshots_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3796 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_configuration_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5612 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_property_descriptor.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5576 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_searchable_field_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4891 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_event_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3570 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9990 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_port.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5444 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_step_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4581 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_history_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2796 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/action_details_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3750 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/property_descriptor_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4417 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/allowable_value_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4412 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_components_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8669 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/lineage_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4089 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/the_position_of_a_component_on_the_graph.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4868 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/history_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6872 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connectable_component.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6170 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_processor_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9299 2018-05-15 09:56:33.000000 nipyapi-0.9.0/nipyapi/nifi/models/about_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3690 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    31075 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4263 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10824 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    15084 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/snippet_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3823 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_groups_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/cluster_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4305 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_api_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    14246 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_port_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9690 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/user_group_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3311 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4734 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bundle_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10130 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/search_results_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3545 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connections_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8049 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/user_group_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4119 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/resource_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5097 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_metadata_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    14099 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/current_user_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5962 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/revision_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/lineage_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6878 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10289 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connectable_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11186 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_update_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4282 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7384 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6050 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_port_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3702 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/prioritizer_types_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7563 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/lineage_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3660 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_event_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4383 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/status_history_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5385 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_status_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13875 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_controller_service.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3624 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_groups_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18656 2018-05-15 13:46:10.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_connection.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9581 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/action_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6244 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_process_group_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11011 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_request_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9001 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_component_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4502 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/submit_replay_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4350 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/difference_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5273 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_breadcrumb_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10546 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_snippet_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5532 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/activate_controller_services_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    24490 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    43520 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_event_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3425 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/buckets_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7749 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_search_result_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5323 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bucket_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5080 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/permissions.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9434 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/storage_usage_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5370 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11226 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_status_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8201 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/registry_client_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8608 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/label_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8906 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_policy_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7947 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/funnel_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4571 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_flow_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7532 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5526 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13051 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_remote_group_port.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10262 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_node_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5090 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/state_map_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3311 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8389 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/status_history_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13168 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/property_descriptor_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4210 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/cluster_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3648 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_types_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6297 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/component_state_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7575 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/cluster_summary_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7451 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_flow_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4602 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bucket_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    21227 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4485 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/connection_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4888 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3883 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_types_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5308 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_configuration_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12380 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/version_control_information_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3491 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5397 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/schedule_components_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3431 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/counters_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9930 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/access_policy_summary_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6079 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_system_diagnostics_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3679 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/search_results_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    23457 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_processor.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5100 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/relationship_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    22094 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5893 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/state_entry_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8797 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/label_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5358 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/copy_snippet_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3515 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processors_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4332 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/counters_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    20875 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_config_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3723 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/property_history_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4398 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4451 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/processor_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6194 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/node_connection_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4572 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    29930 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4840 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_update_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13998 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_snapshot_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3720 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/provenance_options_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9212 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/flow_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6033 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/funnel_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3720 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5550 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_configuration_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4858 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/batch_size.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4318 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/permissions_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9174 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/affected_component_dto.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3600 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/bulletin_board_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8321 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/controller_service_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18132 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_process_group.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6097 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/update_controller_service_reference_request_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5787 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5185 2018-05-15 09:56:34.000000 nipyapi-0.9.0/nipyapi/nifi/models/port_status_snapshot_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:35.000000 nipyapi-0.9.0/nipyapi/nifi/models/versioned_flows_entity.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    24620 2018-05-16 06:51:09.000000 nipyapi-0.9.0/nipyapi/nifi/api_client.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18843 2018-04-11 09:40:35.000000 nipyapi-0.9.0/nipyapi/security.py
--rw-r--r--   0 dchaffey   (501) staff       (20)      452 2018-05-16 07:20:21.000000 nipyapi-0.9.0/nipyapi/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8110 2018-05-15 19:32:23.000000 nipyapi-0.9.0/nipyapi/templates.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12931 2018-05-15 08:38:21.000000 nipyapi-0.9.0/nipyapi/utils.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    25846 2018-05-16 06:43:43.000000 nipyapi-0.9.0/nipyapi/versioning.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/registry/
--rw-r--r--   0 dchaffey   (501) staff       (20)     7559 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/configuration.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/registry/apis/
--rw-r--r--   0 dchaffey   (501) staff       (20)    31584 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/policies_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13509 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/items_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)      324 2018-02-19 09:22:21.000000 nipyapi-0.9.0/nipyapi/registry/apis/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    26549 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/buckets_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    51710 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/bucket_flows_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5011 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/flows_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    44621 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/tenants_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    33636 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/apis/access_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13072 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/rest.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2647 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/__init__.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi/registry/models/
--rw-r--r--   0 dchaffey   (501) staff       (20)     6256 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/link.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7522 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_funnel.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2444 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/uri_builder.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7808 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/user_group.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4349 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/bundle.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7672 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/user.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12323 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_flow.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    10374 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_label.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4932 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/current_user.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8939 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_snapshot_metadata.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    19208 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_remote_process_group.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7137 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/bucket.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6943 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/tenant.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     2995 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/fields.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6387 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_coordinates.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7125 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/resource_permissions.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3752 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/resource.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     1969 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6125 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/access_policy_summary.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     5278 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_property_descriptor.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     9656 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_port.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3755 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/the_position_of_a_component_on_the_graph.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6538 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/connectable_component.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     3929 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/controller_service_api.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6568 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_snapshot.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    11200 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/bucket_item.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    13541 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_controller_service.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    18322 2018-02-26 14:30:32.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_connection.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4746 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/permissions.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    12717 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_remote_group_port.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     7571 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/access_policy.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    23123 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_processor.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4524 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/batch_size.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    17798 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/models/versioned_process_group.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    24260 2018-03-06 19:15:40.000000 nipyapi-0.9.0/nipyapi/registry/api_client.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    25896 2018-05-15 19:38:34.000000 nipyapi-0.9.0/nipyapi/canvas.py
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/tests/
--rw-r--r--   0 dchaffey   (501) staff       (20)    12936 2018-05-15 07:57:59.000000 nipyapi-0.9.0/tests/conftest.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     4448 2018-03-06 19:15:40.000000 nipyapi-0.9.0/tests/test_templates.py
--rw-r--r--   0 dchaffey   (501) staff       (20)        0 2018-02-19 09:22:21.000000 nipyapi-0.9.0/tests/__init__.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     8768 2018-04-11 09:40:35.000000 nipyapi-0.9.0/tests/test_canvas.py
--rw-r--r--   0 dchaffey   (501) staff       (20)    16259 2018-04-11 09:40:35.000000 nipyapi-0.9.0/tests/test_versioning.py
--rw-r--r--   0 dchaffey   (501) staff       (20)      683 2018-02-19 09:22:21.000000 nipyapi-0.9.0/tests/test_system.py
--rw-r--r--   0 dchaffey   (501) staff       (20)      292 2018-03-06 21:45:48.000000 nipyapi-0.9.0/MANIFEST.in
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/docs/
--rw-r--r--   0 dchaffey   (501) staff       (20)      306 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/index.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)      133 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/apiReference.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     3383 2018-02-19 09:22:21.000000 nipyapi-0.9.0/docs/contributing.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)      933 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/todo.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     6766 2018-02-19 09:22:21.000000 nipyapi-0.9.0/docs/Makefile
--rw-r--r--   0 dchaffey   (501) staff       (20)     4743 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/devnotes.rst
--rwxr-xr-x   0 dchaffey   (501) staff       (20)     8808 2018-03-06 23:41:25.000000 nipyapi-0.9.0/docs/conf.py
--rw-r--r--   0 dchaffey   (501) staff       (20)     6461 2018-02-19 09:22:21.000000 nipyapi-0.9.0/docs/make.bat
--rw-r--r--   0 dchaffey   (501) staff       (20)     8384 2018-05-16 07:06:42.000000 nipyapi-0.9.0/docs/history.rst
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/docs/nipyapi-docs/
--rw-r--r--   0 dchaffey   (501) staff       (20)    57383 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.models.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     1488 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     1439 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.apis.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)      623 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)      685 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     7261 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.models.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     5122 2018-05-16 06:53:55.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.apis.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     1032 2018-03-06 20:48:03.000000 nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.demo.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)     1123 2018-02-19 09:22:21.000000 nipyapi-0.9.0/docs/installation.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)      865 2018-03-06 19:15:40.000000 nipyapi-0.9.0/docs/authors.rst
--rw-r--r--   0 dchaffey   (501) staff       (20)       27 2018-02-19 09:22:21.000000 nipyapi-0.9.0/docs/readme.rst
-drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/
--rw-r--r--   0 dchaffey   (501) staff       (20)    16321 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/PKG-INFO
--rw-r--r--   0 dchaffey   (501) staff       (20)        1 2017-08-24 15:39:31.000000 nipyapi-0.9.0/nipyapi.egg-info/not-zip-safe
--rw-r--r--   0 dchaffey   (501) staff       (20)    16565 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/SOURCES.txt
--rw-r--r--   0 dchaffey   (501) staff       (20)       73 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/requires.txt
--rw-r--r--   0 dchaffey   (501) staff       (20)        8 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/top_level.txt
--rw-r--r--   0 dchaffey   (501) staff       (20)        1 2018-05-16 07:20:52.000000 nipyapi-0.9.0/nipyapi.egg-info/dependency_links.txt
--rw-r--r--   0 dchaffey   (501) staff       (20)     2339 2018-05-16 07:20:21.000000 nipyapi-0.9.0/setup.py
--rw-r--r--   0 dchaffey   (501) staff       (20)      418 2018-05-16 07:20:52.000000 nipyapi-0.9.0/setup.cfg
--rw-r--r--   0 dchaffey   (501) staff       (20)     4454 2018-05-16 06:55:09.000000 nipyapi-0.9.0/README.rst
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16695 2018-05-18 12:20:36.000000 nipyapi-0.9.1/PKG-INFO
+-rw-r--r--   0 dchaffey   (501) staff       (20)      594 2018-03-06 19:15:40.000000 nipyapi-0.9.1/LICENSE
+-rw-r--r--   0 dchaffey   (501) staff       (20)      406 2018-03-06 22:24:08.000000 nipyapi-0.9.1/requirements.txt
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/demo/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5970 2018-05-18 08:14:24.000000 nipyapi-0.9.1/nipyapi/demo/console.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/demo/resources/
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3121 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ks.jks
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1356 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.pem
+-rw-r--r--   0 dchaffey   (501) staff       (20)      911 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.jks
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3488 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/client-ks.p12
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2673 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/client-cert.pem
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1144 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.p12
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3050 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/client-ks.jks
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4569 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/resources/keys/client-key.pem
+-rw-r--r--   0 dchaffey   (501) staff       (20)        0 2018-05-01 17:07:19.000000 nipyapi-0.9.1/nipyapi/demo/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16673 2018-05-18 12:13:10.000000 nipyapi-0.9.1/nipyapi/demo/fdlc.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8260 2018-05-17 13:43:28.000000 nipyapi-0.9.1/nipyapi/demo/secure_connection.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1432 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/demo/bbende_howdoideploymyflow.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1088 2018-05-15 19:33:58.000000 nipyapi-0.9.1/nipyapi/system.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2881 2018-03-06 21:03:48.000000 nipyapi-0.9.1/nipyapi/config.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/nifi/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7627 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/configuration.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/nifi/apis/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    41242 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/flowfile_queues_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    26509 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/policies_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9744 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/templates_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15335 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/connections_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15274 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/input_ports_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15065 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/labels_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    38958 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/data_transfer_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)   146919 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/process_groups_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    37965 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/processors_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    19574 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/provenance_events_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    34569 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/provenance_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10388 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/counters_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    66852 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/controller_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1204 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    28981 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/reporting_tasks_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    38943 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/controller_services_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15317 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/output_ports_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15118 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/funnel_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)   181142 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/flow_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    14927 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/snippets_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5253 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/resources_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    50931 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/tenants_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5946 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/system_diagnostics_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    27280 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/remote_process_groups_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    73068 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/versions_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    47248 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/access_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9172 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/apis/site_to_site_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13406 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/rest.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18687 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/__init__.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/nifi/models/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6590 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/link.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7879 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/user_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4799 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/explicit_restriction_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9138 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bulletin_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7856 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_funnel.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5123 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/create_template_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2778 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/uri_builder.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3995 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_comparison_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4425 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bulletin_board_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8778 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4683 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bundle.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4616 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16390 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/drop_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5717 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/status_descriptor_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10496 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/version_info_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3688 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_state_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9598 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_configuration_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5002 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/lineage_results_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12286 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10708 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_label.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3565 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/registry_clients_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7172 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_difference_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    14327 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6006 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/action_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3501 2018-05-15 09:56:33.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_configuration_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8576 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_results_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5205 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/previous_value_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8185 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8321 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/affected_component_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    19542 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_remote_process_group.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4884 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/start_version_control_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9314 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_reference_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    17361 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7258 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7512 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/tenant_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7584 2018-05-15 12:13:10.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_breadcrumb_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3636 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/cluster_search_results_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4989 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_restriction_permission_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7400 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bucket.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8404 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/template_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4795 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4302 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/queue_size_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3356 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/peers_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5013 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/transaction_result_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3491 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4195 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/dimensions_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18254 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/counter_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11344 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    20433 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6916 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_reference_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5152 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/version_control_information_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15162 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_component_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5843 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_counters_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9194 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3774 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/create_active_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5425 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_status_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2805 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_details_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    17245 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4735 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_contents_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3443 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/snippet_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3395 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/labels_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18576 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5552 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/peer_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3690 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_history_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3540 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/drop_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5175 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/counters_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6034 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3623 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/cluste_summary_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    17413 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_file_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13619 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/listing_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9309 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/user_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3519 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/input_ports_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3341 2018-05-15 09:56:33.000000 nipyapi-0.9.1/nipyapi/nifi/models/about_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3827 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_options_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    22020 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5960 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/counter_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7995 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/template_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6105 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_bulletins_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/reporting_tasks_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8389 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_policy_summary_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7460 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bulletin_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10045 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9756 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5175 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/allowable_value_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6279 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/garbage_collection_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3546 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/output_ports_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6721 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_coordinates.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3476 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/resources_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3713 2018-05-15 09:56:33.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_configuration_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12562 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4207 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/banner_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2793 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/streaming_output.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3425 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/funnels_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4122 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/tenants_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    24088 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11156 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4610 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_services_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11369 2018-05-15 12:13:10.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_policy_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4245 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_metadata_set_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10693 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_file_summary_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5003 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/history_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3391 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/banner_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6650 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_link_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8808 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_port_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4883 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    36984 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4228 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/templates_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3450 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_file_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10520 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3775 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_types_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10825 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/documented_type_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    23680 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4241 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/required_permission_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4872 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/attribute_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4281 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3630 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/listing_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15410 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8268 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/instantiate_template_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4177 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_search_result_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7947 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/tenant_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3847 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/position_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4092 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/users_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6604 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/version_control_component_mapping_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9615 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4963 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/batch_settings_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5253 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/registry_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6390 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_remote_process_group_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3534 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/user_groups_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4099 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/search_result_group_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6119 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_status_snapshots_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3796 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_configuration_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5612 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_property_descriptor.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5576 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_searchable_field_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4891 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_event_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3570 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9990 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_port.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5444 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_step_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4581 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_history_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2796 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/action_details_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3750 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/property_descriptor_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4417 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/allowable_value_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4412 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_components_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8669 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/lineage_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4089 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/the_position_of_a_component_on_the_graph.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4868 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/history_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6872 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connectable_component.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6170 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_processor_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9299 2018-05-15 09:56:33.000000 nipyapi-0.9.1/nipyapi/nifi/models/about_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3690 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    31075 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4263 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10824 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    15084 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/snippet_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3823 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_groups_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/cluster_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4305 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_api_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    14246 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_port_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9690 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/user_group_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3311 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4734 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bundle_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10130 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/search_results_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3545 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connections_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8049 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/user_group_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4119 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/resource_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5097 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_metadata_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    14099 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/current_user_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5962 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/revision_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3401 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/lineage_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6878 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10289 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connectable_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11186 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_update_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4282 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7384 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6050 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_port_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3702 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/prioritizer_types_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7563 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/lineage_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3660 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_event_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4383 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/status_history_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5385 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_status_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13875 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_controller_service.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3624 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_groups_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18656 2018-05-15 13:46:10.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_connection.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9581 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/action_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6244 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_process_group_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11011 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_request_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9001 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_component_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4502 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/submit_replay_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4350 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/difference_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5273 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_breadcrumb_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10546 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_snippet_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5532 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/activate_controller_services_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    24490 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    43520 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_event_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3425 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/buckets_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7749 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_search_result_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5323 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bucket_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5080 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/permissions.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9434 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/storage_usage_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5370 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11226 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_status_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8201 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/registry_client_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8608 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/label_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8906 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_policy_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7947 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/funnel_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4571 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_flow_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7532 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5526 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13051 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_remote_group_port.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10262 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_node_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5090 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/state_map_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3311 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8389 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/status_history_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13168 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/property_descriptor_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4210 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/cluster_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3648 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_types_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6297 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/component_state_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7575 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/cluster_summary_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7451 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_flow_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4602 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bucket_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    21227 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4485 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/connection_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4888 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3883 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_types_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5308 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_configuration_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12380 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/version_control_information_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3491 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5397 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/schedule_components_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3431 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/counters_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9930 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/access_policy_summary_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6079 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_system_diagnostics_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3679 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/search_results_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    23457 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_processor.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5100 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/relationship_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    22094 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5893 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/state_entry_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8797 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/label_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5358 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/copy_snippet_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3515 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processors_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4332 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/counters_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    20875 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_config_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3723 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/property_history_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4398 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4451 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/processor_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6194 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/node_connection_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4572 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    29930 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4840 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_update_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13998 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_snapshot_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3720 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/provenance_options_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9212 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/flow_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6033 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/funnel_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3720 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5550 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_configuration_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4858 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/batch_size.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4318 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/permissions_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9174 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/affected_component_dto.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3600 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/bulletin_board_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8321 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/controller_service_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18132 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_process_group.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6097 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/update_controller_service_reference_request_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5787 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5185 2018-05-15 09:56:34.000000 nipyapi-0.9.1/nipyapi/nifi/models/port_status_snapshot_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3654 2018-05-15 09:56:35.000000 nipyapi-0.9.1/nipyapi/nifi/models/versioned_flows_entity.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    24620 2018-05-16 06:51:09.000000 nipyapi-0.9.1/nipyapi/nifi/api_client.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18843 2018-04-11 09:40:35.000000 nipyapi-0.9.1/nipyapi/security.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)      452 2018-05-18 12:14:01.000000 nipyapi-0.9.1/nipyapi/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8110 2018-05-15 19:32:23.000000 nipyapi-0.9.1/nipyapi/templates.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12931 2018-05-15 08:38:21.000000 nipyapi-0.9.1/nipyapi/utils.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    25846 2018-05-16 06:43:43.000000 nipyapi-0.9.1/nipyapi/versioning.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/registry/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7559 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/configuration.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/registry/apis/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    31584 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/policies_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13509 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/items_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)      324 2018-02-19 09:22:21.000000 nipyapi-0.9.1/nipyapi/registry/apis/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    26549 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/buckets_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    51710 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/bucket_flows_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5011 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/flows_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    44621 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/tenants_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    33636 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/apis/access_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13072 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/rest.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2647 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/__init__.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi/registry/models/
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6256 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/link.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7522 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_funnel.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2444 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/uri_builder.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7808 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/user_group.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4349 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/bundle.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7672 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/user.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12323 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_flow.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    10374 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_label.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4932 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/current_user.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8939 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_snapshot_metadata.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    19208 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_remote_process_group.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7137 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/bucket.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6943 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/tenant.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2995 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/fields.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6387 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_coordinates.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7125 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/resource_permissions.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3752 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/resource.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1969 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6125 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/access_policy_summary.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5278 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_property_descriptor.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     9656 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_port.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3755 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/the_position_of_a_component_on_the_graph.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6538 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/connectable_component.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3929 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/controller_service_api.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6568 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_snapshot.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    11200 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/bucket_item.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    13541 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_controller_service.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    18322 2018-02-26 14:30:32.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_connection.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4746 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/permissions.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12717 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_remote_group_port.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7571 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/access_policy.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    23123 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_processor.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4524 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/batch_size.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    17798 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/models/versioned_process_group.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    24260 2018-03-06 19:15:40.000000 nipyapi-0.9.1/nipyapi/registry/api_client.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    25896 2018-05-15 19:38:34.000000 nipyapi-0.9.1/nipyapi/canvas.py
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/tests/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    12936 2018-05-15 07:57:59.000000 nipyapi-0.9.1/tests/conftest.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4448 2018-03-06 19:15:40.000000 nipyapi-0.9.1/tests/test_templates.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)        0 2018-02-19 09:22:21.000000 nipyapi-0.9.1/tests/__init__.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8768 2018-04-11 09:40:35.000000 nipyapi-0.9.1/tests/test_canvas.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16259 2018-04-11 09:40:35.000000 nipyapi-0.9.1/tests/test_versioning.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)      683 2018-02-19 09:22:21.000000 nipyapi-0.9.1/tests/test_system.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)      292 2018-03-06 21:45:48.000000 nipyapi-0.9.1/MANIFEST.in
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/docs/
+-rw-r--r--   0 dchaffey   (501) staff       (20)      306 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/index.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)      133 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/apiReference.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     3383 2018-02-19 09:22:21.000000 nipyapi-0.9.1/docs/contributing.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)      933 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/todo.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6766 2018-02-19 09:22:21.000000 nipyapi-0.9.1/docs/Makefile
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4487 2018-05-18 12:18:44.000000 nipyapi-0.9.1/docs/devnotes.rst
+-rwxr-xr-x   0 dchaffey   (501) staff       (20)     8808 2018-03-06 23:41:25.000000 nipyapi-0.9.1/docs/conf.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)     6461 2018-02-19 09:22:21.000000 nipyapi-0.9.1/docs/make.bat
+-rw-r--r--   0 dchaffey   (501) staff       (20)     8678 2018-05-18 12:18:04.000000 nipyapi-0.9.1/docs/history.rst
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/docs/nipyapi-docs/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    57383 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.models.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1488 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1439 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.apis.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)      623 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)      685 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     7261 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.models.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     5122 2018-05-16 06:53:55.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.apis.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1339 2018-05-18 12:17:41.000000 nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.demo.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)     1123 2018-02-19 09:22:21.000000 nipyapi-0.9.1/docs/installation.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)      865 2018-03-06 19:15:40.000000 nipyapi-0.9.1/docs/authors.rst
+-rw-r--r--   0 dchaffey   (501) staff       (20)       27 2018-02-19 09:22:21.000000 nipyapi-0.9.1/docs/readme.rst
+drwxr-xr-x   0 dchaffey   (501) staff       (20)        0 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16695 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/PKG-INFO
+-rw-r--r--   0 dchaffey   (501) staff       (20)        1 2017-08-24 15:39:31.000000 nipyapi-0.9.1/nipyapi.egg-info/not-zip-safe
+-rw-r--r--   0 dchaffey   (501) staff       (20)    16586 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 dchaffey   (501) staff       (20)       73 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/requires.txt
+-rw-r--r--   0 dchaffey   (501) staff       (20)        8 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/top_level.txt
+-rw-r--r--   0 dchaffey   (501) staff       (20)        1 2018-05-18 12:20:36.000000 nipyapi-0.9.1/nipyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 dchaffey   (501) staff       (20)     2339 2018-05-18 12:14:01.000000 nipyapi-0.9.1/setup.py
+-rw-r--r--   0 dchaffey   (501) staff       (20)      418 2018-05-18 12:20:36.000000 nipyapi-0.9.1/setup.cfg
+-rw-r--r--   0 dchaffey   (501) staff       (20)     4454 2018-05-16 06:55:09.000000 nipyapi-0.9.1/README.rst
```

### Comparing `nipyapi-0.9.0/PKG-INFO` & `nipyapi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: nipyapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Nifi-Python-Api: A convenient Python wrapper for the Apache NiFi Rest API
 Home-page: https://github.com/Chaffelson/nipyapi
 Author: Daniel Chaffelson
 Author-email: chaffelson@gmail.com
 License: Apache Software License 2.0
-Download-URL: https://github.com/Chaffelson/nipyapi/archive/0.9.0.tar.gz
+Download-URL: https://github.com/Chaffelson/nipyapi/archive/0.9.1.tar.gz
 Description: =======
         NiPyApi
         =======
         
         Nifi-Python-Api: A rich Apache NiFi Python Client SDK
         
         .. image:: https://img.shields.io/pypi/v/nipyapi.svg
@@ -118,14 +118,24 @@
         | Outside of the standard Python modules, we make use of lxml, DeepDiff and ruamel.yaml
         
         
         =======
         History
         =======
         
+        0.9.1 (2018-05-18)
+        ------------------
+        
+        | Updated Demos for 0.9 release
+        
+        **New Features**
+        
+        * Added a new demo for Flow Development LifeCycle which illustrates the steps a user might automate to promote Versioned Flows between NiFi environments
+        * Check out nipyapi.demo.fdlc to see more details
+        
         0.9.0 (2018-05-16)
         ------------------
         
         | Updated NiFi client to 1.6.0 release
         
         **Potentially Breaking Changes**
```

### Comparing `nipyapi-0.9.0/LICENSE` & `nipyapi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/console.py` & `nipyapi-0.9.1/nipyapi/demo/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,19 @@
 log.info("Creating reg_client_0 as NiFi Registry Client")
 # If the secured environment demo setup has already run, then we just
 # want to reuse that client for NiFi <> Registry Comms
 reg_client_0 = nipyapi.versioning.get_registry_client(
     'nipyapi_secure_reg_client_0',
     'name'
 )
+try:
+    reg_client_0 = nipyapi.versioning.list_registry_clients().registries[0]
+except IndexError:
+    reg_client_0 = None
+
 if not reg_client_0:
     try:
         reg_client_0 = nipyapi.versioning.create_registry_client(
             name=_rc0,
             uri=_insecure_rc_endpoint,
             description='NiPyApi Demo Console'
         )
```

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ks.jks` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ks.jks`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.pem` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.pem`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.jks` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.jks`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/client-ks.p12` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/client-ks.p12`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/client-cert.pem` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/client-cert.pem`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/localhost-ts.p12` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/localhost-ts.p12`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/client-ks.jks` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/client-ks.jks`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/resources/keys/client-key.pem` & `nipyapi-0.9.1/nipyapi/demo/resources/keys/client-key.pem`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/demo/secure_connection.py` & `nipyapi-0.9.1/nipyapi/demo/secure_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,25 @@
     'LDAP_URL': 'ldap://ldap.forumsys.com:389',
 }
 
 d_containers = [
     DockerContainer(
         name='secure-nifi',
         image_name='apache/nifi',
-        image_tag='1.5.0',
+        image_tag='latest',
         ports={'8443/tcp': 8443},
         env=ldap_env_vars,
         volumes={
             host_certs_path: {'bind': '/opt/certs', 'mode': 'ro'}
         },
     ),
     DockerContainer(
         name='secure-registry',
-        image_name='chaffelson/nifi-registry',
-        image_tag='0.1.0',
+        image_name='apache/nifi-registry',
+        image_tag='latest',
         ports={'18443/tcp': 18443},
         env=tls_env_vars,
         volumes={
             host_certs_path: {'bind': '/opt/certs', 'mode': 'ro'}
         },
     ),
     # TODO update chaffelson/nifi-registry:0.1 image to fix LDAP configuration
```

### Comparing `nipyapi-0.9.0/nipyapi/demo/bbende_howdoideploymyflow.py` & `nipyapi-0.9.1/nipyapi/demo/bbende_howdoideploymyflow.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/system.py` & `nipyapi-0.9.1/nipyapi/system.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/config.py` & `nipyapi-0.9.1/nipyapi/config.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/configuration.py` & `nipyapi-0.9.1/nipyapi/nifi/configuration.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/flowfile_queues_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/flowfile_queues_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/policies_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/policies_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/templates_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/templates_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/connections_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/connections_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/input_ports_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/input_ports_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/labels_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/labels_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/data_transfer_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/data_transfer_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/process_groups_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/process_groups_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/processors_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/processors_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/provenance_events_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/provenance_events_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/provenance_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/provenance_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/counters_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/counters_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/controller_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/controller_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/__init__.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/reporting_tasks_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/reporting_tasks_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/controller_services_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/controller_services_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/output_ports_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/output_ports_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/funnel_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/funnel_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/flow_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/flow_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/snippets_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/snippets_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/resources_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/resources_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/tenants_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/tenants_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/system_diagnostics_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/system_diagnostics_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/remote_process_groups_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/remote_process_groups_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/versions_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/versions_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/access_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/access_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/apis/site_to_site_api.py` & `nipyapi-0.9.1/nipyapi/nifi/apis/site_to_site_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/rest.py` & `nipyapi-0.9.1/nipyapi/nifi/rest.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/__init__.py` & `nipyapi-0.9.1/nipyapi/nifi/__init__.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/link.py` & `nipyapi-0.9.1/nipyapi/nifi/models/link.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/user_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/user_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/explicit_restriction_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/explicit_restriction_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bulletin_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bulletin_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_funnel.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_funnel.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/create_template_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/create_template_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/uri_builder.py` & `nipyapi-0.9.1/nipyapi/nifi/models/uri_builder.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_comparison_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_comparison_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bulletin_board_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bulletin_board_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bundle.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bundle.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/drop_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/drop_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/status_descriptor_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/status_descriptor_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/version_info_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/version_info_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_state_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_state_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_configuration_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/lineage_results_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/lineage_results_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_label.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_label.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/registry_clients_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/registry_clients_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_difference_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_difference_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/action_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/action_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_configuration_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_configuration_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_results_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_results_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/previous_value_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/previous_value_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/affected_component_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/affected_component_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_remote_process_group.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_remote_process_group.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/start_version_control_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/start_version_control_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_reference_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_reference_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/tenant_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_breadcrumb_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_breadcrumb_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/cluster_search_results_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/cluster_search_results_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_restriction_permission_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_restriction_permission_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bucket.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bucket.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/template_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/template_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/queue_size_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/queue_size_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/peers_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/peers_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/transaction_result_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/transaction_result_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/dimensions_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/dimensions_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/counter_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/counter_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_reference_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_reference_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/version_control_information_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/version_control_information_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_component_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_component_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_counters_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_counters_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/create_active_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/create_active_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_status_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_status_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_details_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_details_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_contents_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_contents_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/snippet_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/snippet_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/labels_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/labels_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/peer_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/peer_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_history_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_history_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/drop_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/drop_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/counters_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/counters_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/cluste_summary_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/cluste_summary_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_file_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_file_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/listing_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/listing_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/user_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/input_ports_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/input_ports_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/about_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/about_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_options_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_options_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/counter_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/counter_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/template_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/template_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_bulletins_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_bulletins_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/reporting_tasks_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/reporting_tasks_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_policy_summary_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_policy_summary_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bulletin_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bulletin_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/allowable_value_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/allowable_value_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/garbage_collection_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/garbage_collection_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/output_ports_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/output_ports_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_coordinates.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_coordinates.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/resources_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/resources_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_configuration_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/banner_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/banner_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/streaming_output.py` & `nipyapi-0.9.1/nipyapi/nifi/models/streaming_output.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/funnels_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/funnels_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/tenants_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/tenants_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_services_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_services_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_policy_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_policy_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_metadata_set_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_metadata_set_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_file_summary_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_file_summary_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/history_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/history_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/banner_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/banner_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_link_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_link_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_port_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_port_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/templates_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/templates_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_file_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_file_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_types_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_types_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/documented_type_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/documented_type_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/reporting_task_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/reporting_task_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/required_permission_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/required_permission_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/attribute_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/attribute_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/listing_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/listing_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/__init__.py` & `nipyapi-0.9.1/nipyapi/nifi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/instantiate_template_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/instantiate_template_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_search_result_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_search_result_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/tenant_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/tenant_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/position_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/position_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/users_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/users_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/version_control_component_mapping_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/version_control_component_mapping_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/batch_settings_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/batch_settings_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/registry_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/registry_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_remote_process_group_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_remote_process_group_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/user_groups_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/user_groups_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/search_result_group_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/search_result_group_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_status_snapshots_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_status_snapshots_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_configuration_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_configuration_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_property_descriptor.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_property_descriptor.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_searchable_field_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_searchable_field_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_event_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_event_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_port.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_port.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_step_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_step_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_history_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_history_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/action_details_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/action_details_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/property_descriptor_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/property_descriptor_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/allowable_value_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/allowable_value_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_components_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_components_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/lineage_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/lineage_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/the_position_of_a_component_on_the_graph.py` & `nipyapi-0.9.1/nipyapi/nifi/models/the_position_of_a_component_on_the_graph.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/history_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/history_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connectable_component.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connectable_component.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_processor_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_processor_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/about_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/about_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_api.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/snippet_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/snippet_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_groups_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_groups_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/cluster_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/cluster_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_api_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_api_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_port_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_port_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/user_group_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/user_group_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bundle_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bundle_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/search_results_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/search_results_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connections_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connections_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/user_group_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/user_group_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/resource_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/resource_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_metadata_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_metadata_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/current_user_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/current_user_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/revision_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/revision_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/lineage_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/lineage_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connectable_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connectable_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_update_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_update_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_port_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_port_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/prioritizer_types_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/prioritizer_types_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/lineage_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/lineage_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_event_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_event_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/status_history_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/status_history_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_status_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_status_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_controller_service.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_controller_service.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_groups_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_groups_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_connection.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_connection.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/action_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/action_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_process_group_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_process_group_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_request_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_request_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_referencing_component_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_referencing_component_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/submit_replay_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/submit_replay_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/difference_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/difference_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_breadcrumb_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_breadcrumb_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_snippet_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_snippet_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/activate_controller_services_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/activate_controller_services_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_event_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_event_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/buckets_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/buckets_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_search_result_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_search_result_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bucket_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bucket_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/permissions.py` & `nipyapi-0.9.1/nipyapi/nifi/models/permissions.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/storage_usage_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/storage_usage_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_status_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_status_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/registry_client_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/registry_client_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/label_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/label_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_policy_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_policy_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/funnel_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/funnel_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_flow_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_flow_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_remote_group_port.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_remote_group_port.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_node_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_node_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/state_map_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/state_map_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/status_history_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/status_history_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/property_descriptor_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/property_descriptor_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/cluster_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/cluster_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_types_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_types_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/component_state_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/component_state_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/cluster_summary_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/cluster_summary_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_flow_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_flow_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bucket_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bucket_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/connection_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/connection_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/variable_registry_update_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/variable_registry_update_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_types_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_types_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_configuration_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/version_control_information_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/version_control_information_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/schedule_components_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/schedule_components_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/counters_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/counters_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/access_policy_summary_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/access_policy_summary_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_system_diagnostics_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_system_diagnostics_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/search_results_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/search_results_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_processor.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_processor.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/relationship_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/relationship_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/state_entry_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/state_entry_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/label_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/label_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/copy_snippet_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/copy_snippet_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processors_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processors_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/counters_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/counters_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_config_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_config_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/property_history_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/property_history_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/processor_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/processor_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/node_connection_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/node_connection_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/process_group_status_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/process_group_status_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flow_update_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flow_update_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_snapshot_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_snapshot_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/provenance_options_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/provenance_options_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/flow_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/flow_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/funnel_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/funnel_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/system_diagnostics_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/system_diagnostics_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_configuration_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_configuration_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/batch_size.py` & `nipyapi-0.9.1/nipyapi/nifi/models/batch_size.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/permissions_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/permissions_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/affected_component_dto.py` & `nipyapi-0.9.1/nipyapi/nifi/models/affected_component_dto.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/bulletin_board_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/bulletin_board_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/controller_service_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/controller_service_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_process_group.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_process_group.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/update_controller_service_reference_request_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/update_controller_service_reference_request_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/remote_process_group_status_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/remote_process_group_status_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/port_status_snapshot_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/port_status_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/models/versioned_flows_entity.py` & `nipyapi-0.9.1/nipyapi/nifi/models/versioned_flows_entity.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/nifi/api_client.py` & `nipyapi-0.9.1/nipyapi/nifi/api_client.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/security.py` & `nipyapi-0.9.1/nipyapi/security.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/templates.py` & `nipyapi-0.9.1/nipyapi/templates.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/utils.py` & `nipyapi-0.9.1/nipyapi/utils.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/versioning.py` & `nipyapi-0.9.1/nipyapi/versioning.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/configuration.py` & `nipyapi-0.9.1/nipyapi/registry/configuration.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/policies_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/policies_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/items_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/items_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/buckets_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/buckets_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/bucket_flows_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/bucket_flows_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/flows_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/flows_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/tenants_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/tenants_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/apis/access_api.py` & `nipyapi-0.9.1/nipyapi/registry/apis/access_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/rest.py` & `nipyapi-0.9.1/nipyapi/registry/rest.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/__init__.py` & `nipyapi-0.9.1/nipyapi/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/link.py` & `nipyapi-0.9.1/nipyapi/registry/models/link.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_funnel.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_funnel.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/uri_builder.py` & `nipyapi-0.9.1/nipyapi/registry/models/uri_builder.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/user_group.py` & `nipyapi-0.9.1/nipyapi/registry/models/user_group.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/bundle.py` & `nipyapi-0.9.1/nipyapi/registry/models/bundle.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/user.py` & `nipyapi-0.9.1/nipyapi/registry/models/user.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_flow.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_flow.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_label.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_label.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/current_user.py` & `nipyapi-0.9.1/nipyapi/registry/models/current_user.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_snapshot_metadata.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_snapshot_metadata.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_remote_process_group.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_remote_process_group.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/bucket.py` & `nipyapi-0.9.1/nipyapi/registry/models/bucket.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/tenant.py` & `nipyapi-0.9.1/nipyapi/registry/models/tenant.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/fields.py` & `nipyapi-0.9.1/nipyapi/registry/models/fields.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_coordinates.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_coordinates.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/resource_permissions.py` & `nipyapi-0.9.1/nipyapi/registry/models/resource_permissions.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/resource.py` & `nipyapi-0.9.1/nipyapi/registry/models/resource.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/__init__.py` & `nipyapi-0.9.1/nipyapi/registry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/access_policy_summary.py` & `nipyapi-0.9.1/nipyapi/registry/models/access_policy_summary.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_property_descriptor.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_property_descriptor.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_port.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_port.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/the_position_of_a_component_on_the_graph.py` & `nipyapi-0.9.1/nipyapi/registry/models/the_position_of_a_component_on_the_graph.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/connectable_component.py` & `nipyapi-0.9.1/nipyapi/registry/models/connectable_component.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/controller_service_api.py` & `nipyapi-0.9.1/nipyapi/registry/models/controller_service_api.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_flow_snapshot.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_flow_snapshot.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/bucket_item.py` & `nipyapi-0.9.1/nipyapi/registry/models/bucket_item.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_controller_service.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_controller_service.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_connection.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_connection.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/permissions.py` & `nipyapi-0.9.1/nipyapi/registry/models/permissions.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_remote_group_port.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_remote_group_port.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/access_policy.py` & `nipyapi-0.9.1/nipyapi/registry/models/access_policy.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_processor.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_processor.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/batch_size.py` & `nipyapi-0.9.1/nipyapi/registry/models/batch_size.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/models/versioned_process_group.py` & `nipyapi-0.9.1/nipyapi/registry/models/versioned_process_group.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/registry/api_client.py` & `nipyapi-0.9.1/nipyapi/registry/api_client.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi/canvas.py` & `nipyapi-0.9.1/nipyapi/canvas.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/tests/conftest.py` & `nipyapi-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/tests/test_templates.py` & `nipyapi-0.9.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/tests/test_canvas.py` & `nipyapi-0.9.1/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/tests/test_versioning.py` & `nipyapi-0.9.1/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/tests/test_system.py` & `nipyapi-0.9.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/contributing.rst` & `nipyapi-0.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/todo.rst` & `nipyapi-0.9.1/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/Makefile` & `nipyapi-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/devnotes.rst` & `nipyapi-0.9.1/docs/devnotes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,20 +15,15 @@
 
 
 Docker Test Environment
 -----------------------
 
 There is an Apache NiFi image available on Dockerhub::
 
-    docker pull apache/nifi:1.5.0
-
-However this is released with the official Apache cadence; for development convenience I keep slightly upstream versions of the NiFi & NiFi-Registry docker images on::
-
-    docker pull chaffelson/nifi:latest
-    docker pull chaffelson/nifi-registry:latest
+    docker pull apache/nifi:latest
 
 There are a couple of configuration files for launching various Docker environment configurations in ./test_env_config for convenience.
 
 Testing on OSX
 --------------
 
 There is a known issue with testing newer versions of Python on OSX.
```

### Comparing `nipyapi-0.9.0/docs/conf.py` & `nipyapi-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/make.bat` & `nipyapi-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/history.rst` & `nipyapi-0.9.1/docs/history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =======
 History
 =======
 
+0.9.1 (2018-05-18)
+------------------
+
+| Updated Demos for 0.9 release
+
+**New Features**
+
+* Added a new demo for Flow Development LifeCycle which illustrates the steps a user might automate to promote Versioned Flows between NiFi environments
+* Check out nipyapi.demo.fdlc to see more details
+
 0.9.0 (2018-05-16)
 ------------------
 
 | Updated NiFi client to 1.6.0 release
 
 **Potentially Breaking Changes**
```

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.models.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.models.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.apis.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.apis.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.registry.models.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.registry.models.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.nifi.apis.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.nifi.apis.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/nipyapi-docs/nipyapi.demo.rst` & `nipyapi-0.9.1/docs/nipyapi-docs/nipyapi.demo.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+FDLC
+----
+
+Importing this module provides further instructions for it's use.
+It will guide you through the steps involved in flow promotion.
+
+Note that it makes extensive use of Docker Containers.
+
+Usage::
+
+    from nipyapi.demo.fdlc import *
+
 Console
 -------
 
 Importing this module will run a script which populates the NiFi canvas with a
 Process Group containing a processor, and creates a sequence of Versioned
 Flow Objects from it, along with a Template and various export versions.
 
@@ -18,14 +30,16 @@
 them in a secured configuration, and prepare the environment for access via
 TLS in NiFi-Registry's case, and public LDAP username/password for NiFi.
 
 This is intended to give the user an example of a secured environment.
 May be combined with the Console to produce a secured environment with demo
 objects.
 
+Note that this demo makes extensive use of Docker Containers.
+
 Usage::
 
     from nipyapi.demo.secured_connection import *
 
 
 bbende How Do I Deploy My Flow
 ------------------------------
```

### Comparing `nipyapi-0.9.0/docs/installation.rst` & `nipyapi-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/docs/authors.rst` & `nipyapi-0.9.1/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `nipyapi-0.9.0/nipyapi.egg-info/PKG-INFO` & `nipyapi-0.9.1/nipyapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: nipyapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Nifi-Python-Api: A convenient Python wrapper for the Apache NiFi Rest API
 Home-page: https://github.com/Chaffelson/nipyapi
 Author: Daniel Chaffelson
 Author-email: chaffelson@gmail.com
 License: Apache Software License 2.0
-Download-URL: https://github.com/Chaffelson/nipyapi/archive/0.9.0.tar.gz
+Download-URL: https://github.com/Chaffelson/nipyapi/archive/0.9.1.tar.gz
 Description: =======
         NiPyApi
         =======
         
         Nifi-Python-Api: A rich Apache NiFi Python Client SDK
         
         .. image:: https://img.shields.io/pypi/v/nipyapi.svg
@@ -118,14 +118,24 @@
         | Outside of the standard Python modules, we make use of lxml, DeepDiff and ruamel.yaml
         
         
         =======
         History
         =======
         
+        0.9.1 (2018-05-18)
+        ------------------
+        
+        | Updated Demos for 0.9 release
+        
+        **New Features**
+        
+        * Added a new demo for Flow Development LifeCycle which illustrates the steps a user might automate to promote Versioned Flows between NiFi environments
+        * Check out nipyapi.demo.fdlc to see more details
+        
         0.9.0 (2018-05-16)
         ------------------
         
         | Updated NiFi client to 1.6.0 release
         
         **Potentially Breaking Changes**
```

### Comparing `nipyapi-0.9.0/nipyapi.egg-info/SOURCES.txt` & `nipyapi-0.9.1/nipyapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 nipyapi.egg-info/dependency_links.txt
 nipyapi.egg-info/not-zip-safe
 nipyapi.egg-info/requires.txt
 nipyapi.egg-info/top_level.txt
 nipyapi/demo/__init__.py
 nipyapi/demo/bbende_howdoideploymyflow.py
 nipyapi/demo/console.py
+nipyapi/demo/fdlc.py
 nipyapi/demo/secure_connection.py
 nipyapi/demo/resources/keys/client-cert.pem
 nipyapi/demo/resources/keys/client-key.pem
 nipyapi/demo/resources/keys/client-ks.jks
 nipyapi/demo/resources/keys/client-ks.p12
 nipyapi/demo/resources/keys/localhost-ks.jks
 nipyapi/demo/resources/keys/localhost-ts.jks
```

### Comparing `nipyapi-0.9.0/setup.py` & `nipyapi-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('docs/history.rst') as history_file:
     history = history_file.read()
 
-proj_version = '0.9.0'
+proj_version = '0.9.1'
 
 requirements = [
     'urllib3',  # Required for timeouts during security tests
     'lxml',  # Required for parsing NiFi Templates
     'deepdiff',  # Required for comparing configurations
     'six',  # Required for managing Python version compatibility
     'ruamel.yaml==0.14.12',  # Required for parsing Json/Yaml consistently
```

### Comparing `nipyapi-0.9.0/README.rst` & `nipyapi-0.9.1/README.rst`

 * *Files identical despite different names*

