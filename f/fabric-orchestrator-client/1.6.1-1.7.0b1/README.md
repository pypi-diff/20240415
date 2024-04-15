# Comparing `tmp/fabric-orchestrator-client-1.6.1.tar.gz` & `tmp/fabric-orchestrator-client-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.6.1.tar", last modified: Fri Jan 12 03:43:10 2024, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.7.0b1.tar", last modified: Mon Apr 15 21:31:29 2024, max compression
```

## Comparing `fabric-orchestrator-client-1.6.1.tar` & `fabric-orchestrator-client-1.7.0b1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.6.1/.gitignore
--rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.6.1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2024-01-12 03:42:46.102318 fabric-orchestrator-client-1.6.1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.6.1/.travis.yml
--rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.6.1/CODEGEN.md
--rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.6.1/LICENSE
--rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.6.1/MANIFEST.in
--rw-r--r--   0        0        0     9867 2024-01-12 03:42:46.104165 fabric-orchestrator-client-1.6.1/README.md
--rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.6.1/docs/Poa.md
--rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.6.1/docs/PoaData.md
--rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.6.1/docs/PoaPost.md
--rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.6.1/docs/PoaPostData.md
--rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.6.1/docs/PoaPostDataKeys.md
--rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.6.1/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.6.1/docs/PoasApi.md
--rw-r--r--   0        0        0     4263 2024-01-12 03:42:46.105517 fabric-orchestrator-client-1.6.1/docs/ResourcesApi.md
--rw-r--r--   0        0        0    20667 2024-01-12 03:42:46.105687 fabric-orchestrator-client-1.6.1/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.6.1/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.6.1/docs/Success.md
--rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.6.1/docs/Version.md
--rw-r--r--   0        0        0       22 2024-01-12 03:43:04.214903 fabric-orchestrator-client-1.6.1/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    21973 2024-01-12 03:42:46.106541 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3649 2024-01-12 03:42:46.106764 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2024-01-12 03:42:46.106916 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0     9597 2024-01-12 03:42:46.107306 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    43978 2024-01-12 03:42:46.107525 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2978 2024-01-12 03:42:46.108309 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2024-01-12 03:42:46.108447 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
--rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2024-01-12 03:42:46.109662 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2024-01-12 03:42:46.109991 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    10905 2024-01-12 03:42:46.110449 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2024-01-12 03:42:46.112630 fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.6.1/git_push.sh
--rw-r--r--   0        0        0     1024 2024-01-12 03:42:58.584905 fabric-orchestrator-client-1.6.1/pyproject.toml
--rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.6.1/test/__init__.py
--rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.6.1/test/test_poa.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.6.1/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.6.1/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.6.1/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.6.1/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.6.1/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.6.1/test/test_resource.py
--rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.6.1/test/test_resources.py
--rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.6.1/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.6.1/test/test_slice.py
--rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.6.1/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.6.1/test/test_slices.py
--rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.6.1/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.6.1/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.6.1/test/test_sliver.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.6.1/test/test_slivers.py
--rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.6.1/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.6.1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.6.1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.6.1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.6.1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.6.1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.6.1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.6.1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.6.1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.6.1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.6.1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.6.1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.6.1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.6.1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.6.1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.6.1/test/test_version.py
--rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.6.1/test/test_version_api.py
--rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.6.1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.6.1/tox.ini
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.7.0b1/.gitignore
+-rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.7.0b1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2024-04-05 22:19:27.031216 fabric-orchestrator-client-1.7.0b1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.7.0b1/.travis.yml
+-rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.7.0b1/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.7.0b1/LICENSE
+-rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.7.0b1/MANIFEST.in
+-rw-r--r--   0        0        0    10034 2024-04-05 22:21:50.264153 fabric-orchestrator-client-1.7.0b1/README.md
+-rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.7.0b1/docs/Poa.md
+-rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.7.0b1/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.7.0b1/docs/PoaPost.md
+-rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.7.0b1/docs/PoaPostData.md
+-rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.7.0b1/docs/PoaPostDataKeys.md
+-rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.7.0b1/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.7.0b1/docs/PoasApi.md
+-rw-r--r--   0        0        0     5067 2024-04-15 15:10:09.775273 fabric-orchestrator-client-1.7.0b1/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    21005 2024-04-05 22:21:01.694717 fabric-orchestrator-client-1.7.0b1/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.7.0b1/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.7.0b1/docs/Success.md
+-rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.7.0b1/docs/Version.md
+-rw-r--r--   0        0        0       24 2024-04-15 21:30:48.912389 fabric-orchestrator-client-1.7.0b1/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    23053 2024-04-15 15:14:36.619887 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3649 2024-01-12 03:42:46.106764 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2024-01-12 03:42:46.106916 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0    10809 2024-04-15 15:11:50.036544 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    44836 2024-04-05 22:26:59.835003 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     3070 2024-04-05 22:28:49.311561 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2024-01-12 03:42:46.108447 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
+-rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     9914 2024-04-05 22:29:14.527230 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2024-01-12 03:42:46.109991 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    12331 2024-04-05 22:29:46.008920 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12985 2024-04-05 22:30:18.293171 fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.7.0b1/git_push.sh
+-rw-r--r--   0        0        0     1024 2024-04-05 22:18:00.458232 fabric-orchestrator-client-1.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.7.0b1/test/__init__.py
+-rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.7.0b1/test/test_poa.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.7.0b1/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.7.0b1/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.7.0b1/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.7.0b1/test/test_resource.py
+-rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.7.0b1/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.7.0b1/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.7.0b1/test/test_slice.py
+-rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.7.0b1/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.7.0b1/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.7.0b1/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.7.0b1/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.7.0b1/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.7.0b1/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.7.0b1/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.7.0b1/test/test_version.py
+-rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.7.0b1/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.7.0b1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.7.0b1/tox.ini
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.7.0b1/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.6.1/.gitignore` & `fabric-orchestrator-client-1.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.7.0b1/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/CODEGEN.md` & `fabric-orchestrator-client-1.7.0b1/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/LICENSE` & `fabric-orchestrator-client-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/README.md` & `fabric-orchestrator-client-1.7.0b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 ------------ | ------------- | ------------- | -------------
 *PoasApi* | [**poas_create_sliver_id_post**](docs/PoasApi.md#poas_create_sliver_id_post) | **POST** /poas/create/{sliver_id} | Perform an operational action on a sliver.
 *PoasApi* | [**poas_get**](docs/PoasApi.md#poas_get) | **GET** /poas/ | Request get the status of the POAs.
 *PoasApi* | [**poas_poa_id_get**](docs/PoasApi.md#poas_poa_id_get) | **GET** /poas/{poa_id} | Perform an operational action on a sliver.
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
 *ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
+*SlicesApi* | [**slices_creates_post**](docs/SlicesApi.md#slices_creates_post) | **POST** /slices/creates | Create slice
 *SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 *SlicesApi* | [**slices_modify_slice_id_put**](docs/SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 *SlicesApi* | [**slices_renew_slice_id_post**](docs/SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
@@ -124,14 +125,15 @@
 
 ## Documentation For Models
 
  - [Poa](docs/Poa.md)
  - [PoaData](docs/PoaData.md)
  - [PoaPost](docs/PoaPost.md)
  - [PoaPostData](docs/PoaPostData.md)
+ - [PoaPostDataKeys](docs/PoaPostDataKeys.md)
  - [PoaPostDataVcpuCpuMap](docs/PoaPostDataVcpuCpuMap.md)
  - [Resource](docs/Resource.md)
  - [Resources](docs/Resources.md)
  - [Slice](docs/Slice.md)
  - [SliceDetails](docs/SliceDetails.md)
  - [Slices](docs/Slices.md)
  - [SlicesPost](docs/SlicesPost.md)
```

### Comparing `fabric-orchestrator-client-1.6.1/docs/PoaData.md` & `fabric-orchestrator-client-1.7.0b1/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/docs/PoasApi.md` & `fabric-orchestrator-client-1.7.0b1/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.7.0b1/docs/ResourcesApi.md`

 * *Files 22% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **resources_get**
-> Resources resources_get(level, force_refresh)
+> Resources resources_get(level, force_refresh, start_date=start_date, end_date=end_date, includes=includes, excludes=excludes)
 
 Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 
 Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 
 ### Example
 ```python
@@ -76,29 +76,37 @@
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = ResourcesApi(ApiClient(configuration))
 level = 1 # int | Level of details (default to 1)
 force_refresh = False # bool | Force to retrieve current available resource information. (default to false)
+start_date = 'start_date_example' # str | starting date to check availability from (optional)
+end_date = 'end_date_example' # str | end date to check availability until (optional)
+includes = 'includes_example' # str | comma separated lists of sites to include (optional)
+excludes = 'excludes_example' # str | comma separated lists of sites to exclude (optional)
 
 try:
     # Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
-    api_response = api_instance.resources_get(level, force_refresh)
+    api_response = api_instance.resources_get(level, force_refresh, start_date=start_date, end_date=end_date)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling ResourcesApi->resources_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **level** | **int**| Level of details | [default to 1]
  **force_refresh** | **bool**| Force to retrieve current available resource information. | [default to false]
+ **start_date** | **str**| starting date to check availability from | [optional] 
+ **end_date** | **str**| end date to check availability until | [optional] 
+ **includes** | **str**| comma separated lists of sites to include | [optional] 
+ **excludes** | **str**| comma separated lists of sites to exclude | [optional] 
 
 ### Return type
 
 [**Resources**](Resources.md)
 
 ### Authorization
```

### Comparing `fabric-orchestrator-client-1.6.1/docs/SlicesApi.md` & `fabric-orchestrator-client-1.7.0b1/docs/SlicesApi.md`

 * *Files 2% similar despite different names*

```diff
@@ -259,32 +259,36 @@
 configuration.api_key['Authorization'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
 name = 'name_example' # str | Search for Slices with the name (optional)
+search = 'search_example' # str | search term applied (optional)
+exact_match = false # bool | Exact Match for Search term (optional) (default to false)
 as_self = true # bool | GET object as Self (optional) (default to true)
 states = ['states_example'] # list[str] | Search for Slices in the specified states (optional)
 limit = 5 # int | maximum number of results to return per page (1 or more) (optional) (default to 5)
 offset = 0 # int | number of items to skip before starting to collect the result set (optional) (default to 0)
 
 try:
     # Retrieve a listing of user slices
-    api_response = api_instance.slices_get(name=name, as_self=as_self, states=states, limit=limit, offset=offset)
+    api_response = api_instance.slices_get(name=name, search=search, exact_match=exact_match, as_self=as_self, states=states, limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **name** | **str**| Search for Slices with the name | [optional] 
+ **search** | **str**| search term applied | [optional] 
+ **exact_match** | **bool**| Exact Match for Search term | [optional] [default to false]
  **as_self** | **bool**| GET object as Self | [optional] [default to true]
  **states** | [**list[str]**](str.md)| Search for Slices in the specified states | [optional] 
  **limit** | **int**| maximum number of results to return per page (1 or more) | [optional] [default to 5]
  **offset** | **int**| number of items to skip before starting to collect the result set | [optional] [default to 0]
 
 ### Return type
```

### Comparing `fabric-orchestrator-client-1.6.1/docs/SliversApi.md` & `fabric-orchestrator-client-1.7.0b1/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -274,25 +274,27 @@
 
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
 
     def slices(self, *, token: str, includes: List[SliceState] = None, excludes: List[SliceState] = None,
                name: str = None, limit: int = 20, offset: int = 0, slice_id: str = None,
-               as_self: bool = True) -> Tuple[Status, Union[Exception, List[Slice]]]:
+               as_self: bool = True, search: str = None, exact_match: bool = False) -> Tuple[Status, Union[Exception, List[Slice]]]:
         """
         Get slices
         @param token fabric token
         @param includes list of the slice state used to include the slices in the output
         @param excludes list of the slice state used to exclude the slices from the output
         @param name name of the slice
         @param limit maximum number of slices to return
         @param offset offset of the first slice to return
         @param slice_id Slice Id
-        @param as_self
+        @param as_self query as self
+        @param search search term
+        @param exact_match true if exact match
         @return Tuple containing Status and Exception/Json containing slices
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
@@ -310,18 +312,20 @@
                         states.remove(x)
 
             if slice_id is not None:
                 slices = self.slices_api.slices_slice_id_get(slice_id=slice_id, graph_format=GraphFormat.GRAPHML.name,
                                                              as_self=as_self)
             elif name is not None:
                 slices = self.slices_api.slices_get(states=SliceState.state_list_to_str_list(states), name=name,
-                                                    limit=limit, offset=offset, as_self=as_self)
+                                                    limit=limit, offset=offset, as_self=as_self,
+                                                    search=search, exact_match=exact_match)
             else:
                 slices = self.slices_api.slices_get(states=SliceState.state_list_to_str_list(states), limit=limit,
-                                                    offset=offset, as_self=as_self)
+                                                    offset=offset, as_self=as_self, search=search,
+                                                    exact_match=exact_match)
 
             return Status.OK, slices.data if slices.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
     def get_slice(self, *, token: str, slice_id: str = None,
                   graph_format: GraphFormat = GraphFormat.GRAPHML,
@@ -384,32 +388,41 @@
                 slivers = self.slivers_api.slivers_sliver_id_get(slice_id=slice_id, sliver_id=sliver_id,
                                                                  as_self=as_self)
 
             return Status.OK, slivers.data if slivers.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
-    def resources(self, *, token: str, level: int = 1,
-                  force_refresh: bool = False) -> Tuple[Status, Union[Exception, AdvertizedTopology]]:
+    def resources(self, *, token: str, level: int = 1, force_refresh: bool = False,
+                  start: datetime = None, end: datetime = None,
+                  includes: List[str] = None, excludes: List[str] = None) -> Tuple[Status, Union[Exception, AdvertizedTopology]]:
         """
         Get resources; by default cached resource information is returned. Cache is refreshed every 5 minutes.
         @param token fabric token
         @param level level
         @param force_refresh force current available resources
+        @param start start time
+        @param end end time
+        @param includes list of sites to include
+        @param excludes list of sites to exclude
         @return Tuple containing Status and Exception/Json containing Resources
         """
-
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
-            resources = self.resources_api.resources_get(level=level, force_refresh=force_refresh)
+            start_date = start.strftime('%Y-%m-%d %H:%M:%S %z') if start else None
+            end_date = end.strftime('%Y-%m-%d %H:%M:%S %z') if end else None
+            resources = self.resources_api.resources_get(level=level, force_refresh=force_refresh,
+                                                         start_date=start_date, end_date=end_date,
+                                                         includes=', '.join(includes) if includes else None,
+                                                         excludes=', '.join(excludes) if excludes else None)
             graph_string = resources.data[0].model
             substrate = None
             if graph_string is not None:
                 substrate = AdvertizedTopology()
                 substrate.load(graph_string=graph_string)
 
             return Status.OK, substrate
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,18 +126,24 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.resources_get(level, force_refresh, async_req=True)
         >>> result = thread.get()
         :param async_req bool
         :param int level: Level of details (required)
         :param bool force_refresh: Force to retrieve current available resource information. (required)
+        :param str start_date: starting date to check availability from
+        :param str end_date: end date to check availability until
+        :param str includes: comma separated lists of sites to include
+        :param str excludes: comma separated lists of sites to exclude
         :return: Resources
                  If the method is called asynchronously,
                  returns the request thread.
         """
+        # Remove all arguments with None value from kwargs
+        kwargs = {key: value for key, value in kwargs.items() if value is not None}
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.resources_get_with_http_info(level, force_refresh, **kwargs)  # noqa: E501
         else:
             (data) = self.resources_get_with_http_info(level, force_refresh, **kwargs)  # noqa: E501
             return data
 
@@ -147,20 +153,24 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.resources_get_with_http_info(level, force_refresh, async_req=True)
         >>> result = thread.get()
         :param async_req bool
         :param int level: Level of details (required)
         :param bool force_refresh: Force to retrieve current available resource information. (required)
+        :param str start_date: starting date to check availability from
+        :param str end_date: end date to check availability until
+        :param str includes: comma separated lists of sites to include
+        :param str excludes: comma separated lists of sites to exclude
         :return: Resources
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['level', 'force_refresh']  # noqa: E501
+        all_params = ['level', 'force_refresh', 'start_date', 'end_date', 'includes', 'excludes']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -185,14 +195,22 @@
         path_params = {}
 
         query_params = []
         if 'level' in params:
             query_params.append(('level', params['level']))  # noqa: E501
         if 'force_refresh' in params:
             query_params.append(('force_refresh', params['force_refresh']))  # noqa: E501
+        if 'start_date' in params:
+            query_params.append(('start_date', params['start_date']))  # noqa: E501
+        if 'end_date' in params:
+            query_params.append(('end_date', params['end_date']))  # noqa: E501
+        if 'includes' in params:
+            query_params.append(('includes', params['includes']))  # noqa: E501
+        if 'excludes' in params:
+            query_params.append(('excludes', params['excludes']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -213,8 +231,8 @@
             files=local_var_files,
             response_type='Resources',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
+            collection_formats=collection_formats)
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,59 +25,59 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def slices_create_post(self, body, name, **kwargs):  # noqa: E501
+    def slices_create_post(self, body, name, ssh_key, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
 
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_create_post(body, name, async_req=True)
+        >>> thread = api.slices_create_post(body, name, ssh_key, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param SlicesPost body: Create new Slice (required)
+        :param str body: (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.slices_create_post_with_http_info(body, name, **kwargs)  # noqa: E501
+            return self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
         else:
-            (data) = self.slices_create_post_with_http_info(body, name, **kwargs)  # noqa: E501
+            (data) = self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
             return data
 
-    def slices_create_post_with_http_info(self, body, name, **kwargs):  # noqa: E501
+    def slices_create_post_with_http_info(self, body, name, ssh_key, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
 
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_create_post_with_http_info(body, name, async_req=True)
+        >>> thread = api.slices_create_post_with_http_info(body, name, ssh_key, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param SlicesPost body: Create new Slice (required)
+        :param str body: (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'name', 'lease_end_time']  # noqa: E501
+        all_params = ['body', 'name', 'ssh_key', 'lease_end_time']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -92,22 +92,28 @@
         if ('body' not in params or
                 params['body'] is None):
             raise ValueError("Missing the required parameter `body` when calling `slices_create_post`")  # noqa: E501
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
             raise ValueError("Missing the required parameter `name` when calling `slices_create_post`")  # noqa: E501
+        # verify the required parameter 'ssh_key' is set
+        if ('ssh_key' not in params or
+                params['ssh_key'] is None):
+            raise ValueError("Missing the required parameter `ssh_key` when calling `slices_create_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
+        if 'ssh_key' in params:
+            query_params.append(('ssh_key', params['ssh_key']))  # noqa: E501
         if 'lease_end_time' in params:
             query_params.append(('lease_end_time', params['lease_end_time']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -442,14 +448,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Search for Slices with the name
+        :param str search: search term applied
+        :param bool exact_match: Exact Match for Search term
         :param bool as_self: GET object as Self
         :param list[str] states: Search for Slices in the specified states
         :param int limit: maximum number of results to return per page (1 or more)
         :param int offset: number of items to skip before starting to collect the result set
         :return: Slices
                  If the method is called asynchronously,
                  returns the request thread.
@@ -468,24 +476,26 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: Search for Slices with the name
+        :param str search: search term applied
+        :param bool exact_match: Exact Match for Search term
         :param bool as_self: GET object as Self
         :param list[str] states: Search for Slices in the specified states
         :param int limit: maximum number of results to return per page (1 or more)
         :param int offset: number of items to skip before starting to collect the result set
         :return: Slices
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'as_self', 'states', 'limit', 'offset']  # noqa: E501
+        all_params = ['name', 'search', 'exact_match', 'as_self', 'states', 'limit', 'offset']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -500,14 +510,18 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
+        if 'search' in params:
+            query_params.append(('search', params['search']))  # noqa: E501
+        if 'exact_match' in params:
+            query_params.append(('exact_match', params['exact_match']))  # noqa: E501
         if 'as_self' in params:
             query_params.append(('as_self', params['as_self']))  # noqa: E501
         if 'states' in params:
             query_params.append(('states', params['states']))  # noqa: E501
             collection_formats['states'] = 'multi'  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from __future__ import absolute_import
 
 # import models into model package
 from fabric_cf.orchestrator.swagger_client.models.poa import Poa
 from fabric_cf.orchestrator.swagger_client.models.poa_data import PoaData
 from fabric_cf.orchestrator.swagger_client.models.poa_post import PoaPost
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data import PoaPostData
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data_keys import PoaPostDataKeys
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_client.models.resource import Resource
 from fabric_cf.orchestrator.swagger_client.models.resources import Resources
 from fabric_cf.orchestrator.swagger_client.models.slice import Slice
 from fabric_cf.orchestrator.swagger_client.models.slice_details import SliceDetails
 from fabric_cf.orchestrator.swagger_client.models.slices import Slices
 from fabric_cf.orchestrator.swagger_client.models.slices_post import SlicesPost
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,40 +32,46 @@
         'lease_start_time': 'str',
         'lease_end_time': 'str',
         'state': 'str',
         'project_id': 'str',
         'project_name': 'str',
         'graph_id': 'str',
         'name': 'str',
-        'slice_id': 'str'
+        'slice_id': 'str',
+        'owner_user_id': 'str',
+        'owner_email': 'str'
     }
 
     attribute_map = {
         'model': 'model',
         'lease_start_time': 'lease_start_time',
         'lease_end_time': 'lease_end_time',
         'state': 'state',
         'project_id': 'project_id',
         'project_name': 'project_name',
         'graph_id': 'graph_id',
         'name': 'name',
-        'slice_id': 'slice_id'
+        'slice_id': 'slice_id',
+        'owner_user_id': 'owner_user_id',
+        'owner_email': 'owner_email'
     }
 
-    def __init__(self, model=None, lease_start_time=None, lease_end_time=None, state=None, project_id=None, project_name=None, graph_id=None, name=None, slice_id=None):  # noqa: E501
+    def __init__(self, model=None, lease_start_time=None, lease_end_time=None, state=None, project_id=None, project_name=None, graph_id=None, name=None, slice_id=None, owner_user_id=None, owner_email=None):  # noqa: E501
         """Slice - a model defined in Swagger"""  # noqa: E501
         self._model = None
         self._lease_start_time = None
         self._lease_end_time = None
         self._state = None
         self._project_id = None
         self._project_name = None
         self._graph_id = None
         self._name = None
         self._slice_id = None
+        self._owner_user_id = None
+        self._owner_email = None
         self.discriminator = None
         if model is not None:
             self.model = model
         if lease_start_time is not None:
             self.lease_start_time = lease_start_time
         if lease_end_time is not None:
             self.lease_end_time = lease_end_time
@@ -74,14 +80,18 @@
         if project_id is not None:
             self.project_id = project_id
         if project_name is not None:
             self.project_name = project_name
         self.graph_id = graph_id
         self.name = name
         self.slice_id = slice_id
+        if owner_user_id is not None:
+            self.owner_user_id = owner_user_id
+        if owner_email is not None:
+            self.owner_email = owner_email
 
     @property
     def model(self):
         """Gets the model of this Slice.  # noqa: E501
 
 
         :return: The model of this Slice.  # noqa: E501
@@ -270,14 +280,56 @@
         :type: str
         """
         if slice_id is None:
             raise ValueError("Invalid value for `slice_id`, must not be `None`")  # noqa: E501
 
         self._slice_id = slice_id
 
+    @property
+    def owner_user_id(self):
+        """Gets the owner_user_id of this Slice.  # noqa: E501
+
+
+        :return: The owner_user_id of this Slice.  # noqa: E501
+        :rtype: str
+        """
+        return self._owner_user_id
+
+    @owner_user_id.setter
+    def owner_user_id(self, owner_user_id):
+        """Sets the owner_user_id of this Slice.
+
+
+        :param owner_user_id: The owner_user_id of this Slice.  # noqa: E501
+        :type: str
+        """
+
+        self._owner_user_id = owner_user_id
+
+    @property
+    def owner_email(self):
+        """Gets the owner_email of this Slice.  # noqa: E501
+
+
+        :return: The owner_email of this Slice.  # noqa: E501
+        :rtype: str
+        """
+        return self._owner_email
+
+    @owner_email.setter
+    def owner_email(self, owner_email):
+        """Sets the owner_email of this Slice.
+
+
+        :param owner_email: The owner_email of this Slice.  # noqa: E501
+        :type: str
+        """
+
+        self._owner_email = owner_email
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,44 +39,50 @@
         'lease_start_time': 'str',
         'lease_end_time': 'str',
         'state': 'str',
         'pending_state': 'str',
         'join_state': 'str',
         'graph_node_id': 'str',
         'slice_id': 'str',
-        'sliver_id': 'str'
+        'sliver_id': 'str',
+        'owner_user_id': 'str',
+        'owner_email': 'str'
     }
 
     attribute_map = {
         'notice': 'notice',
         'sliver_type': 'sliver_type',
         'sliver': 'sliver',
         'lease_start_time': 'lease_start_time',
         'lease_end_time': 'lease_end_time',
         'state': 'state',
         'pending_state': 'pending_state',
         'join_state': 'join_state',
         'graph_node_id': 'graph_node_id',
         'slice_id': 'slice_id',
-        'sliver_id': 'sliver_id'
+        'sliver_id': 'sliver_id',
+        'owner_user_id': 'owner_user_id',
+        'owner_email': 'owner_email'
     }
 
-    def __init__(self, notice=None, sliver_type=None, sliver=None, lease_start_time=None, lease_end_time=None, state=None, pending_state=None, join_state=None, graph_node_id=None, slice_id=None, sliver_id=None):  # noqa: E501
+    def __init__(self, notice=None, sliver_type=None, sliver=None, lease_start_time=None, lease_end_time=None, state=None, pending_state=None, join_state=None, graph_node_id=None, slice_id=None, sliver_id=None, owner_user_id=None, owner_email=None):  # noqa: E501
         """Sliver - a model defined in Swagger"""  # noqa: E501
         self._notice = None
         self._sliver_type = None
         self._sliver = None
         self._lease_start_time = None
         self._lease_end_time = None
         self._state = None
         self._pending_state = None
         self._join_state = None
         self._graph_node_id = None
         self._slice_id = None
         self._sliver_id = None
+        self._owner_user_id = None
+        self._owner_email = None
         self.discriminator = None
         if notice is not None:
             self.notice = notice
         if sliver_type is not None:
             self.sliver_type = sliver_type
         if sliver is not None:
             self.sliver = sliver
@@ -89,14 +95,18 @@
         if pending_state is not None:
             self.pending_state = pending_state
         if join_state is not None:
             self.join_state = join_state
         self.graph_node_id = graph_node_id
         self.slice_id = slice_id
         self.sliver_id = sliver_id
+        if owner_user_id is not None:
+            self.owner_user_id = owner_user_id
+        if owner_email is not None:
+            self.owner_email = owner_email
 
     @property
     def notice(self):
         """Gets the notice of this Sliver.  # noqa: E501
 
 
         :return: The notice of this Sliver.  # noqa: E501
@@ -327,14 +337,56 @@
         :type: str
         """
         if sliver_id is None:
             raise ValueError("Invalid value for `sliver_id`, must not be `None`")  # noqa: E501
 
         self._sliver_id = sliver_id
 
+    @property
+    def owner_user_id(self):
+        """Gets the owner_user_id of this Sliver.  # noqa: E501
+
+
+        :return: The owner_user_id of this Sliver.  # noqa: E501
+        :rtype: str
+        """
+        return self._owner_user_id
+
+    @owner_user_id.setter
+    def owner_user_id(self, owner_user_id):
+        """Sets the owner_user_id of this Sliver.
+
+
+        :param owner_user_id: The owner_user_id of this Sliver.  # noqa: E501
+        :type: str
+        """
+
+        self._owner_user_id = owner_user_id
+
+    @property
+    def owner_email(self):
+        """Gets the owner_email of this Sliver.  # noqa: E501
+
+
+        :return: The owner_email of this Sliver.  # noqa: E501
+        :rtype: str
+        """
+        return self._owner_email
+
+    @owner_email.setter
+    def owner_email(self, owner_email):
+        """Sets the owner_email of this Sliver.
+
+
+        :param owner_email: The owner_email of this Sliver.  # noqa: E501
+        :type: str
+        """
+
+        self._owner_email = owner_email
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.7.0b1/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.6.1/git_push.sh` & `fabric-orchestrator-client-1.7.0b1/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/pyproject.toml` & `fabric-orchestrator-client-1.7.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poa.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poa_data.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poa_post.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_poas_api.py` & `fabric-orchestrator-client-1.7.0b1/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_resource.py` & `fabric-orchestrator-client-1.7.0b1/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_resources.py` & `fabric-orchestrator-client-1.7.0b1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_resources_api.py` & `fabric-orchestrator-client-1.7.0b1/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slice.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slice_details.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slices.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slices_api.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slices_post.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_sliver.py` & `fabric-orchestrator-client-1.7.0b1/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slivers.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.7.0b1/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_version.py` & `fabric-orchestrator-client-1.7.0b1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_version_api.py` & `fabric-orchestrator-client-1.7.0b1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/test/test_version_data.py` & `fabric-orchestrator-client-1.7.0b1/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.1/PKG-INFO` & `fabric-orchestrator-client-1.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.6.1
+Version: 1.7.0b1
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -132,14 +132,15 @@
 ------------ | ------------- | ------------- | -------------
 *PoasApi* | [**poas_create_sliver_id_post**](docs/PoasApi.md#poas_create_sliver_id_post) | **POST** /poas/create/{sliver_id} | Perform an operational action on a sliver.
 *PoasApi* | [**poas_get**](docs/PoasApi.md#poas_get) | **GET** /poas/ | Request get the status of the POAs.
 *PoasApi* | [**poas_poa_id_get**](docs/PoasApi.md#poas_poa_id_get) | **GET** /poas/{poa_id} | Perform an operational action on a sliver.
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
 *ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
+*SlicesApi* | [**slices_creates_post**](docs/SlicesApi.md#slices_creates_post) | **POST** /slices/creates | Create slice
 *SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 *SlicesApi* | [**slices_modify_slice_id_put**](docs/SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 *SlicesApi* | [**slices_renew_slice_id_post**](docs/SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
@@ -149,14 +150,15 @@
 
 ## Documentation For Models
 
  - [Poa](docs/Poa.md)
  - [PoaData](docs/PoaData.md)
  - [PoaPost](docs/PoaPost.md)
  - [PoaPostData](docs/PoaPostData.md)
+ - [PoaPostDataKeys](docs/PoaPostDataKeys.md)
  - [PoaPostDataVcpuCpuMap](docs/PoaPostDataVcpuCpuMap.md)
  - [Resource](docs/Resource.md)
  - [Resources](docs/Resources.md)
  - [Slice](docs/Slice.md)
  - [SliceDetails](docs/SliceDetails.md)
  - [Slices](docs/Slices.md)
  - [SlicesPost](docs/SlicesPost.md)
```

