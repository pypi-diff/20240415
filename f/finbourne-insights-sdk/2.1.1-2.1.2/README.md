# Comparing `tmp/finbourne_insights_sdk-2.1.1.tar.gz` & `tmp/finbourne_insights_sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_insights_sdk-2.1.1.tar", max compression
+gzip compressed data, was "finbourne_insights_sdk-2.1.2.tar", max compression
```

## Comparing `finbourne_insights_sdk-2.1.1.tar` & `finbourne_insights_sdk-2.1.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    10629 2024-04-10 10:43:04.484893 finbourne_insights_sdk-2.1.1/README.md
--rw-r--r--   0        0        0     5228 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/__init__.py
--rw-r--r--   0        0        0      526 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/__init__.py
--rw-r--r--   0        0        0    24459 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/access_evaluations_api.py
--rw-r--r--   0        0        0     7550 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/application_metadata_api.py
--rw-r--r--   0        0        0    24169 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/auditing_api.py
--rw-r--r--   0        0        0    35948 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/requests_api.py
--rw-r--r--   0        0        0    36148 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/vendor_logs_api.py
--rw-r--r--   0        0        0    30813 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api_client.py
--rw-r--r--   0        0        0      852 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api_response.py
--rw-r--r--   0        0        0    14459 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/configuration.py
--rw-r--r--   0        0        0     5339 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/__init__.py
--rw-r--r--   0        0        0    30684 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client.py
--rw-r--r--   0        0        0     9902 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3641 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/__init__.py
--rw-r--r--   0        0        0     3915 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_action.py
--rw-r--r--   0        0        0     4858 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_resource.py
--rw-r--r--   0        0        0    11915 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_evaluation_log.py
--rw-r--r--   0        0        0     2070 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/action_id.py
--rw-r--r--   0        0        0     3756 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data.py
--rw-r--r--   0        0        0     2219 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data_summary.py
--rw-r--r--   0        0        0     3451 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry.py
--rw-r--r--   0        0        0     2096 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry_note.py
--rw-r--r--   0        0        0     2779 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process.py
--rw-r--r--   0        0        0     3039 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process_summary.py
--rw-r--r--   0        0        0     2119 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/bucket.py
--rw-r--r--   0        0        0     2519 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/create_audit_entry.py
--rw-r--r--   0        0        0     2597 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/histogram.py
--rw-r--r--   0        0        0     3184 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/id_selector_definition.py
--rw-r--r--   0        0        0     3109 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2262 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/link.py
--rw-r--r--   0        0        0     3857 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4693 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3212 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/problem_details.py
--rw-r--r--   0        0        0     5510 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/request.py
--rw-r--r--   0        0        0     8268 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/request_log.py
--rw-r--r--   0        0        0     2374 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource.py
--rw-r--r--   0        0        0     4263 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4203 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_audit_process_summary.py
--rw-r--r--   0        0        0     4738 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
--rw-r--r--   0        0        0     4638 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
--rw-r--r--   0        0        0     4627 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
--rw-r--r--   0        0        0     5048 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/response.py
--rw-r--r--   0        0        0     2913 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/scrollable_collection_of_audit_entry.py
--rw-r--r--   0        0        0     4520 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_log.py
--rw-r--r--   0        0        0     2797 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_request.py
--rw-r--r--   0        0        0     2823 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_response.py
--rw-r--r--   0        0        0        0 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/py.typed
--rw-r--r--   0        0        0    10164 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/rest.py
--rw-r--r--   0        0        0      871 2024-04-10 10:43:04.484893 finbourne_insights_sdk-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11682 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10554 2024-04-15 09:55:54.189774 finbourne_insights_sdk-2.1.2/README.md
+-rw-r--r--   0        0        0     5228 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/__init__.py
+-rw-r--r--   0        0        0    24459 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/access_evaluations_api.py
+-rw-r--r--   0        0        0     7520 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/application_metadata_api.py
+-rw-r--r--   0        0        0    24169 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/auditing_api.py
+-rw-r--r--   0        0        0    35828 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/requests_api.py
+-rw-r--r--   0        0        0    36148 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api/vendor_logs_api.py
+-rw-r--r--   0        0        0    30813 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/api_response.py
+-rw-r--r--   0        0        0    14459 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/configuration.py
+-rw-r--r--   0        0        0     5339 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/__init__.py
+-rw-r--r--   0        0        0    30684 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3641 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/__init__.py
+-rw-r--r--   0        0        0     3915 2024-04-15 09:55:54.184774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4858 2024-04-15 09:55:54.184774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_controlled_resource.py
+-rw-r--r--   0        0        0    11915 2024-04-15 09:55:54.184774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_evaluation_log.py
+-rw-r--r--   0        0        0     2070 2024-04-15 09:55:54.184774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/action_id.py
+-rw-r--r--   0        0        0     3756 2024-04-15 09:55:54.184774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_data.py
+-rw-r--r--   0        0        0     2219 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_data_summary.py
+-rw-r--r--   0        0        0     3451 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_entry.py
+-rw-r--r--   0        0        0     2096 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_entry_note.py
+-rw-r--r--   0        0        0     2779 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_process.py
+-rw-r--r--   0        0        0     3039 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_process_summary.py
+-rw-r--r--   0        0        0     2119 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/bucket.py
+-rw-r--r--   0        0        0     2519 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/create_audit_entry.py
+-rw-r--r--   0        0        0     2597 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/histogram.py
+-rw-r--r--   0        0        0     3184 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3109 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2262 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/link.py
+-rw-r--r--   0        0        0     3857 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3212 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/problem_details.py
+-rw-r--r--   0        0        0     5510 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/request.py
+-rw-r--r--   0        0        0     8268 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/request_log.py
+-rw-r--r--   0        0        0     2374 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource.py
+-rw-r--r--   0        0        0     4263 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4203 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_of_audit_process_summary.py
+-rw-r--r--   0        0        0     4738 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
+-rw-r--r--   0        0        0     4638 2024-04-15 09:55:54.185774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
+-rw-r--r--   0        0        0     4627 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
+-rw-r--r--   0        0        0     5048 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/response.py
+-rw-r--r--   0        0        0     2913 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/scrollable_collection_of_audit_entry.py
+-rw-r--r--   0        0        0     4520 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_log.py
+-rw-r--r--   0        0        0     2797 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_request.py
+-rw-r--r--   0        0        0     2823 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_response.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:55:54.186774 finbourne_insights_sdk-2.1.2/finbourne_insights/py.typed
+-rw-r--r--   0        0        0    10164 2024-04-15 09:55:54.187774 finbourne_insights_sdk-2.1.2/finbourne_insights/rest.py
+-rw-r--r--   0        0        0      871 2024-04-15 09:55:54.189774 finbourne_insights_sdk-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11607 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.1.2/PKG-INFO
```

### Comparing `finbourne_insights_sdk-2.1.1/README.md` & `finbourne_insights_sdk-2.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.764
-- Package version: 2.1.1
+- API version: 0.0.765
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -187,22 +187,22 @@
 
 All URIs are relative to *https://fbn-prd.lusid.com/insights*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AccessEvaluationsApi* | [**get_access_evaluation_log**](docs/AccessEvaluationsApi.md#get_access_evaluation_log) | **GET** /api/access/{id} | [EARLY ACCESS] GetAccessEvaluationLog: Get the log for a specific access evaluation.  This endpoint will be deprecated in the near future.
 *AccessEvaluationsApi* | [**list_access_evaluation_logs**](docs/AccessEvaluationsApi.md#list_access_evaluation_logs) | **GET** /api/access | [EARLY ACCESS] ListAccessEvaluationLogs: List the logs for access evaluations.
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
 *AuditingApi* | [**create_entry**](docs/AuditingApi.md#create_entry) | **POST** /api/auditing/entries | [EARLY ACCESS] CreateEntry: Create (persist) and audit entry..
 *AuditingApi* | [**get_processes**](docs/AuditingApi.md#get_processes) | **GET** /api/auditing/processes | [EARLY ACCESS] GetProcesses: Get the latest audit entry for each process.
 *AuditingApi* | [**list_entries**](docs/AuditingApi.md#list_entries) | **GET** /api/auditing/entries | [EARLY ACCESS] ListEntries: Get the audit entries.
-*RequestsApi* | [**get_request**](docs/RequestsApi.md#get_request) | **GET** /api/requests/{id}/request | [EARLY ACCESS] GetRequest: Get the request content for a specific API request.
-*RequestsApi* | [**get_request_log**](docs/RequestsApi.md#get_request_log) | **GET** /api/requests/{id} | [EARLY ACCESS] GetRequestLog: Get the log for a specific API request.
-*RequestsApi* | [**get_response**](docs/RequestsApi.md#get_response) | **GET** /api/requests/{id}/response | [EARLY ACCESS] GetResponse: Get the response for a specific API request.
-*RequestsApi* | [**list_request_logs**](docs/RequestsApi.md#list_request_logs) | **GET** /api/requests | [EARLY ACCESS] ListRequestLogs: Get the logs for API requests.
+*RequestsApi* | [**get_request**](docs/RequestsApi.md#get_request) | **GET** /api/requests/{id}/request | GetRequest: Get the request content for a specific API request.
+*RequestsApi* | [**get_request_log**](docs/RequestsApi.md#get_request_log) | **GET** /api/requests/{id} | GetRequestLog: Get the log for a specific API request.
+*RequestsApi* | [**get_response**](docs/RequestsApi.md#get_response) | **GET** /api/requests/{id}/response | GetResponse: Get the response for a specific API request.
+*RequestsApi* | [**list_request_logs**](docs/RequestsApi.md#list_request_logs) | **GET** /api/requests | ListRequestLogs: Get the logs for API requests.
 *VendorLogsApi* | [**get_vendor_log**](docs/VendorLogsApi.md#get_vendor_log) | **GET** /api/vendor/{id} | [EXPERIMENTAL] GetVendorLog: Get the log for a specific vendor request.
 *VendorLogsApi* | [**get_vendor_request**](docs/VendorLogsApi.md#get_vendor_request) | **GET** /api/vendor/{id}/request | [EXPERIMENTAL] GetVendorRequest: Get the request body for a vendor request.
 *VendorLogsApi* | [**get_vendor_response**](docs/VendorLogsApi.md#get_vendor_response) | **GET** /api/vendor/{id}/response | [EXPERIMENTAL] GetVendorResponse: Get the response from a vendor request.
 *VendorLogsApi* | [**list_vendor_logs**](docs/VendorLogsApi.md#list_vendor_logs) | **GET** /api/vendor | [EXPERIMENTAL] ListVendorLogs: List the logs for vendor requests.
 
 
 ## Documentation For Models
```

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/__init__.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/__init__.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/access_evaluations_api.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/access_evaluations_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/application_metadata_api.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/application_metadata_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     @overload
     def list_access_controlled_resources(self, async_req: Optional[bool]=True, **kwargs) -> ResourceListOfAccessControlledResource:  # noqa: E501
         ...
 
     @validate_arguments
     def list_access_controlled_resources(self, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListOfAccessControlledResource, Awaitable[ResourceListOfAccessControlledResource]]:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources(async_req=True)
         >>> result = thread.get()
@@ -77,15 +77,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_access_controlled_resources_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def list_access_controlled_resources_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/auditing_api.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/auditing_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/requests_api.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/requests_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     @overload
     def get_request(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the content for.")], async_req: Optional[bool]=True, **kwargs) -> Request:  # noqa: E501
         ...
 
     @validate_arguments
     def get_request(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the content for.")], async_req: Optional[bool]=None, **kwargs) -> Union[Request, Awaitable[Request]]:  # noqa: E501
-        """[EARLY ACCESS] GetRequest: Get the request content for a specific API request.  # noqa: E501
+        """GetRequest: Get the request content for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_request(id, async_req=True)
         >>> result = thread.get()
 
@@ -86,15 +86,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_request_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_request_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the content for.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetRequest: Get the request content for a specific API request.  # noqa: E501
+        """GetRequest: Get the request content for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_request_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
@@ -204,15 +204,15 @@
 
     @overload
     def get_request_log(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the log for.")], async_req: Optional[bool]=True, **kwargs) -> RequestLog:  # noqa: E501
         ...
 
     @validate_arguments
     def get_request_log(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the log for.")], async_req: Optional[bool]=None, **kwargs) -> Union[RequestLog, Awaitable[RequestLog]]:  # noqa: E501
-        """[EARLY ACCESS] GetRequestLog: Get the log for a specific API request.  # noqa: E501
+        """GetRequestLog: Get the log for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_request_log(id, async_req=True)
         >>> result = thread.get()
 
@@ -235,15 +235,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_request_log_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_request_log_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the log for.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetRequestLog: Get the log for a specific API request.  # noqa: E501
+        """GetRequestLog: Get the log for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_request_log_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
@@ -353,15 +353,15 @@
 
     @overload
     def get_response(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the response for.")], async_req: Optional[bool]=True, **kwargs) -> Response:  # noqa: E501
         ...
 
     @validate_arguments
     def get_response(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the response for.")], async_req: Optional[bool]=None, **kwargs) -> Union[Response, Awaitable[Response]]:  # noqa: E501
-        """[EARLY ACCESS] GetResponse: Get the response for a specific API request.  # noqa: E501
+        """GetResponse: Get the response for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_response(id, async_req=True)
         >>> result = thread.get()
 
@@ -384,15 +384,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_response_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_response_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The identifier of the request to obtain the response for.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetResponse: Get the response for a specific API request.  # noqa: E501
+        """GetResponse: Get the response for a specific API request.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_response_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
@@ -502,15 +502,15 @@
 
     @overload
     def list_request_logs(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Expression to filter the result set. Read more about <see href=\"https://support.lusid.com/filtering-results-from-lusid\"> filtering results from LUSID</see>.")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName. Multiple fields can be denoted by a comma e.g. -MyFieldName,AnotherFieldName,-AFurtherFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=10000, ge=0)], Field(description="When paginating, only return this number of records. The minimum value is 0 and the maximum is 10000.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Encoded page string returned from a previous search result that will retrieve the next page of data. When this field is supplied, filter and sortby fields should not be supplied.")] = None, histogram_interval : Annotated[Optional[StrictStr], Field(description="Optional interval to use in a histogram of the returned values. If not provided, no histogram will be generated.")] = None, async_req: Optional[bool]=True, **kwargs) -> ResourceListWithHistogramOfRequestLog:  # noqa: E501
         ...
 
     @validate_arguments
     def list_request_logs(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Expression to filter the result set. Read more about <see href=\"https://support.lusid.com/filtering-results-from-lusid\"> filtering results from LUSID</see>.")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName. Multiple fields can be denoted by a comma e.g. -MyFieldName,AnotherFieldName,-AFurtherFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=10000, ge=0)], Field(description="When paginating, only return this number of records. The minimum value is 0 and the maximum is 10000.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Encoded page string returned from a previous search result that will retrieve the next page of data. When this field is supplied, filter and sortby fields should not be supplied.")] = None, histogram_interval : Annotated[Optional[StrictStr], Field(description="Optional interval to use in a histogram of the returned values. If not provided, no histogram will be generated.")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListWithHistogramOfRequestLog, Awaitable[ResourceListWithHistogramOfRequestLog]]:  # noqa: E501
-        """[EARLY ACCESS] ListRequestLogs: Get the logs for API requests.  # noqa: E501
+        """ListRequestLogs: Get the logs for API requests.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_request_logs(filter, sort_by, limit, page, histogram_interval, async_req=True)
         >>> result = thread.get()
 
@@ -541,15 +541,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_request_logs_with_http_info(filter, sort_by, limit, page, histogram_interval, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_request_logs_with_http_info(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Expression to filter the result set. Read more about <see href=\"https://support.lusid.com/filtering-results-from-lusid\"> filtering results from LUSID</see>.")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName. Multiple fields can be denoted by a comma e.g. -MyFieldName,AnotherFieldName,-AFurtherFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=10000, ge=0)], Field(description="When paginating, only return this number of records. The minimum value is 0 and the maximum is 10000.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Encoded page string returned from a previous search result that will retrieve the next page of data. When this field is supplied, filter and sortby fields should not be supplied.")] = None, histogram_interval : Annotated[Optional[StrictStr], Field(description="Optional interval to use in a histogram of the returned values. If not provided, no histogram will be generated.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListRequestLogs: Get the logs for API requests.  # noqa: E501
+        """ListRequestLogs: Get the logs for API requests.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_request_logs_with_http_info(filter, sort_by, limit, page, histogram_interval, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api/vendor_logs_api.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api/vendor_logs_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api_client.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/api_response.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/configuration.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_insights-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.764\n"\
+               "Version of the API: 0.0.765\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/exceptions.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/__init__.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client_factory.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_configuration.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/configuration_loaders.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/proxy_config.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/refreshing_token.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/rest.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/retry.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/socket_keep_alive.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/tcp_keep_alive_connector.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/__init__.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_action.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_resource.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_evaluation_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/action_id.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_data.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data_summary.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_data_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry_note.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_entry_note.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_process.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process_summary.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/bucket.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/bucket.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/create_audit_entry.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/create_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/histogram.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/histogram.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/id_selector_definition.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/identifier_part_schema.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/link.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_problem_details.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_validation_problem_details.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/problem_details.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/request.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/request_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_access_controlled_resource.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_audit_process_summary.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_of_audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_request_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/response.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/scrollable_collection_of_audit_entry.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/scrollable_collection_of_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_log.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_request.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_response.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/models/vendor_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/finbourne_insights/rest.py` & `finbourne_insights_sdk-2.1.2/finbourne_insights/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.1/pyproject.toml` & `finbourne_insights_sdk-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-insights-sdk"
-version = "2.1.1"
+version = "2.1.2"
 description = "FINBOURNE Insights API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/insights-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Insights API", "finbourne-insights-sdk"]
 packages = [
```

### Comparing `finbourne_insights_sdk-2.1.1/PKG-INFO` & `finbourne_insights_sdk-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-insights-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: FINBOURNE Insights API
 Home-page: https://github.com/finbourne/insights-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Insights API,finbourne-insights-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.764
-- Package version: 2.1.1
+- API version: 0.0.765
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -213,22 +213,22 @@
 
 All URIs are relative to *https://fbn-prd.lusid.com/insights*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AccessEvaluationsApi* | [**get_access_evaluation_log**](docs/AccessEvaluationsApi.md#get_access_evaluation_log) | **GET** /api/access/{id} | [EARLY ACCESS] GetAccessEvaluationLog: Get the log for a specific access evaluation.  This endpoint will be deprecated in the near future.
 *AccessEvaluationsApi* | [**list_access_evaluation_logs**](docs/AccessEvaluationsApi.md#list_access_evaluation_logs) | **GET** /api/access | [EARLY ACCESS] ListAccessEvaluationLogs: List the logs for access evaluations.
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
 *AuditingApi* | [**create_entry**](docs/AuditingApi.md#create_entry) | **POST** /api/auditing/entries | [EARLY ACCESS] CreateEntry: Create (persist) and audit entry..
 *AuditingApi* | [**get_processes**](docs/AuditingApi.md#get_processes) | **GET** /api/auditing/processes | [EARLY ACCESS] GetProcesses: Get the latest audit entry for each process.
 *AuditingApi* | [**list_entries**](docs/AuditingApi.md#list_entries) | **GET** /api/auditing/entries | [EARLY ACCESS] ListEntries: Get the audit entries.
-*RequestsApi* | [**get_request**](docs/RequestsApi.md#get_request) | **GET** /api/requests/{id}/request | [EARLY ACCESS] GetRequest: Get the request content for a specific API request.
-*RequestsApi* | [**get_request_log**](docs/RequestsApi.md#get_request_log) | **GET** /api/requests/{id} | [EARLY ACCESS] GetRequestLog: Get the log for a specific API request.
-*RequestsApi* | [**get_response**](docs/RequestsApi.md#get_response) | **GET** /api/requests/{id}/response | [EARLY ACCESS] GetResponse: Get the response for a specific API request.
-*RequestsApi* | [**list_request_logs**](docs/RequestsApi.md#list_request_logs) | **GET** /api/requests | [EARLY ACCESS] ListRequestLogs: Get the logs for API requests.
+*RequestsApi* | [**get_request**](docs/RequestsApi.md#get_request) | **GET** /api/requests/{id}/request | GetRequest: Get the request content for a specific API request.
+*RequestsApi* | [**get_request_log**](docs/RequestsApi.md#get_request_log) | **GET** /api/requests/{id} | GetRequestLog: Get the log for a specific API request.
+*RequestsApi* | [**get_response**](docs/RequestsApi.md#get_response) | **GET** /api/requests/{id}/response | GetResponse: Get the response for a specific API request.
+*RequestsApi* | [**list_request_logs**](docs/RequestsApi.md#list_request_logs) | **GET** /api/requests | ListRequestLogs: Get the logs for API requests.
 *VendorLogsApi* | [**get_vendor_log**](docs/VendorLogsApi.md#get_vendor_log) | **GET** /api/vendor/{id} | [EXPERIMENTAL] GetVendorLog: Get the log for a specific vendor request.
 *VendorLogsApi* | [**get_vendor_request**](docs/VendorLogsApi.md#get_vendor_request) | **GET** /api/vendor/{id}/request | [EXPERIMENTAL] GetVendorRequest: Get the request body for a vendor request.
 *VendorLogsApi* | [**get_vendor_response**](docs/VendorLogsApi.md#get_vendor_response) | **GET** /api/vendor/{id}/response | [EXPERIMENTAL] GetVendorResponse: Get the response from a vendor request.
 *VendorLogsApi* | [**list_vendor_logs**](docs/VendorLogsApi.md#list_vendor_logs) | **GET** /api/vendor | [EXPERIMENTAL] ListVendorLogs: List the logs for vendor requests.
 
 
 ## Documentation For Models
```

