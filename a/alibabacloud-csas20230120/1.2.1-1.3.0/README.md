# Comparing `tmp/alibabacloud_csas20230120-1.2.1.tar.gz` & `tmp/alibabacloud_csas20230120-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120-1.2.1.tar", last modified: Wed Nov 15 17:18:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120-1.3.0.tar", last modified: Mon Apr 15 03:02:10 2024, max compression
```

## Comparing `alibabacloud_csas20230120-1.2.1.tar` & `alibabacloud_csas20230120-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      422 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)   163506 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   383182 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-11-15 17:18:32.000000 alibabacloud_csas20230120-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2023-11-15 17:18:31.000000 alibabacloud_csas20230120-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171706 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   393460 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/setup.py
```

### Comparing `alibabacloud_csas20230120-1.2.1/LICENSE` & `alibabacloud_csas20230120-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.2.1/PKG-INFO` & `alibabacloud_csas20230120-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120
-Version: 1.2.1
+Version: 1.3.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/csas-20230120/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_csas20230120-1.2.1/README-CN.md` & `alibabacloud_csas20230120-1.3.0/README-CN.md`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/csas-20230120/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_csas20230120-1.2.1/README.md` & `alibabacloud_csas20230120-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/csas-20230120/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,16 @@
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
         if not UtilClient.is_unset(request.custom_user_attributes):
             body_flat['CustomUserAttributes'] = request.custom_user_attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.device_attribute_id):
+            body['DeviceAttributeId'] = request.device_attribute_id
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.policy_action):
             body['PolicyAction'] = request.policy_action
         if not UtilClient.is_unset(request.priority):
             body['Priority'] = request.priority
         if not UtilClient.is_unset(request.status):
@@ -398,14 +400,16 @@
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
         if not UtilClient.is_unset(request.custom_user_attributes):
             body_flat['CustomUserAttributes'] = request.custom_user_attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.device_attribute_id):
+            body['DeviceAttributeId'] = request.device_attribute_id
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.policy_action):
             body['PolicyAction'] = request.policy_action
         if not UtilClient.is_unset(request.priority):
             body['Priority'] = request.priority
         if not UtilClient.is_unset(request.status):
@@ -2215,14 +2219,80 @@
     async def list_polices_for_user_group_async(
         self,
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_user_group_with_options_async(request, runtime)
 
+    def list_pop_traffic_statistics_with_options(
+        self,
+        request: csas_20230120_models.ListPopTrafficStatisticsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListPopTrafficStatistics',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListPopTrafficStatisticsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_pop_traffic_statistics_with_options_async(
+        self,
+        request: csas_20230120_models.ListPopTrafficStatisticsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListPopTrafficStatistics',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListPopTrafficStatisticsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_pop_traffic_statistics(
+        self,
+        request: csas_20230120_models.ListPopTrafficStatisticsRequest,
+    ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_pop_traffic_statistics_with_options(request, runtime)
+
+    async def list_pop_traffic_statistics_async(
+        self,
+        request: csas_20230120_models.ListPopTrafficStatisticsRequest,
+    ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_pop_traffic_statistics_with_options_async(request, runtime)
+
     def list_private_access_applications_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -3139,14 +3209,80 @@
     async def list_user_groups_for_registration_policy_async(
         self,
         request: csas_20230120_models.ListUserGroupsForRegistrationPolicyRequest,
     ) -> csas_20230120_models.ListUserGroupsForRegistrationPolicyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_user_groups_for_registration_policy_with_options_async(request, runtime)
 
+    def list_users_with_options(
+        self,
+        request: csas_20230120_models.ListUsersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListUsersResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListUsers',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListUsersResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_users_with_options_async(
+        self,
+        request: csas_20230120_models.ListUsersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListUsersResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListUsers',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListUsersResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_users(
+        self,
+        request: csas_20230120_models.ListUsersRequest,
+    ) -> csas_20230120_models.ListUsersResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_users_with_options(request, runtime)
+
+    async def list_users_async(
+        self,
+        request: csas_20230120_models.ListUsersRequest,
+    ) -> csas_20230120_models.ListUsersResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_users_with_options_async(request, runtime)
+
     def update_dynamic_route_with_options(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -3459,14 +3595,16 @@
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
         if not UtilClient.is_unset(request.custom_user_attributes):
             body_flat['CustomUserAttributes'] = request.custom_user_attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.device_attribute_id):
+            body['DeviceAttributeId'] = request.device_attribute_id
         if not UtilClient.is_unset(request.modify_type):
             body['ModifyType'] = request.modify_type
         if not UtilClient.is_unset(request.policy_action):
             body['PolicyAction'] = request.policy_action
         if not UtilClient.is_unset(request.policy_id):
             body['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.priority):
@@ -3512,14 +3650,16 @@
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
         if not UtilClient.is_unset(request.custom_user_attributes):
             body_flat['CustomUserAttributes'] = request.custom_user_attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.device_attribute_id):
+            body['DeviceAttributeId'] = request.device_attribute_id
         if not UtilClient.is_unset(request.modify_type):
             body['ModifyType'] = request.modify_type
         if not UtilClient.is_unset(request.policy_action):
             body['PolicyAction'] = request.policy_action
         if not UtilClient.is_unset(request.policy_id):
             body['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.priority):
@@ -3942,7 +4082,81 @@
 
     async def update_user_group_async(
         self,
         request: csas_20230120_models.UpdateUserGroupRequest,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.update_user_group_with_options_async(request, runtime)
+
+    def update_users_status_with_options(
+        self,
+        request: csas_20230120_models.UpdateUsersStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.sase_user_ids):
+            query['SaseUserIds'] = request.sase_user_ids
+        if not UtilClient.is_unset(request.status):
+            query['Status'] = request.status
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateUsersStatus',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateUsersStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_users_status_with_options_async(
+        self,
+        request: csas_20230120_models.UpdateUsersStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.sase_user_ids):
+            query['SaseUserIds'] = request.sase_user_ids
+        if not UtilClient.is_unset(request.status):
+            query['Status'] = request.status
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateUsersStatus',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateUsersStatusResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_users_status(
+        self,
+        request: csas_20230120_models.UpdateUsersStatusRequest,
+    ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_users_status_with_options(request, runtime)
+
+    async def update_users_status_async(
+        self,
+        request: csas_20230120_models.UpdateUsersStatusRequest,
+    ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_users_status_with_options_async(request, runtime)
```

### Comparing `alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,14 @@
         body: AttachApplication2ConnectorResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -265,17 +262,14 @@
         body: CreateDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -446,17 +440,14 @@
         body: CreatePrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -530,26 +521,28 @@
 class CreatePrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         custom_user_attributes: List[CreatePrivateAccessPolicyRequestCustomUserAttributes] = None,
         description: str = None,
+        device_attribute_id: str = None,
         name: str = None,
         policy_action: str = None,
         priority: int = None,
         status: str = None,
         tag_ids: List[str] = None,
         user_group_ids: List[str] = None,
         user_group_mode: str = None,
     ):
         self.application_ids = application_ids
         self.application_type = application_type
         self.custom_user_attributes = custom_user_attributes
         self.description = description
+        self.device_attribute_id = device_attribute_id
         self.name = name
         self.policy_action = policy_action
         self.priority = priority
         self.status = status
         # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
@@ -576,14 +569,16 @@
             result['ApplicationType'] = self.application_type
         result['CustomUserAttributes'] = []
         if self.custom_user_attributes is not None:
             for k in self.custom_user_attributes:
                 result['CustomUserAttributes'].append(k.to_map() if k else None)
         if self.description is not None:
             result['Description'] = self.description
+        if self.device_attribute_id is not None:
+            result['DeviceAttributeId'] = self.device_attribute_id
         if self.name is not None:
             result['Name'] = self.name
         if self.policy_action is not None:
             result['PolicyAction'] = self.policy_action
         if self.priority is not None:
             result['Priority'] = self.priority
         if self.status is not None:
@@ -605,14 +600,16 @@
         self.custom_user_attributes = []
         if m.get('CustomUserAttributes') is not None:
             for k in m.get('CustomUserAttributes'):
                 temp_model = CreatePrivateAccessPolicyRequestCustomUserAttributes()
                 self.custom_user_attributes.append(temp_model.from_map(k))
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('DeviceAttributeId') is not None:
+            self.device_attribute_id = m.get('DeviceAttributeId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PolicyAction') is not None:
             self.policy_action = m.get('PolicyAction')
         if m.get('Priority') is not None:
             self.priority = m.get('Priority')
         if m.get('Status') is not None:
@@ -667,17 +664,14 @@
         body: CreatePrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -777,17 +771,14 @@
         body: CreatePrivateAccessTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1282,17 +1273,14 @@
         body: CreateRegistrationPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1451,17 +1439,14 @@
         body: CreateUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1549,17 +1534,14 @@
         body: DeleteDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1647,17 +1629,14 @@
         body: DeletePrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1745,17 +1724,14 @@
         body: DeletePrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1843,17 +1819,14 @@
         body: DeletePrivateAccessTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1941,17 +1914,14 @@
         body: DeleteRegistrationPoliciesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2039,17 +2009,14 @@
         body: DeleteUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2178,17 +2145,14 @@
         body: DetachApplication2ConnectorResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2377,17 +2341,14 @@
         body: GetDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2611,17 +2572,14 @@
         body: GetPrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2723,28 +2681,30 @@
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         create_time: str = None,
         custom_user_attributes: List[GetPrivateAccessPolicyResponseBodyPolicyCustomUserAttributes] = None,
         description: str = None,
+        device_attribute_id: str = None,
         name: str = None,
         policy_action: str = None,
         policy_id: str = None,
         priority: int = None,
         status: str = None,
         tag_ids: List[str] = None,
         user_group_ids: List[str] = None,
         user_group_mode: str = None,
     ):
         self.application_ids = application_ids
         self.application_type = application_type
         self.create_time = create_time
         self.custom_user_attributes = custom_user_attributes
         self.description = description
+        self.device_attribute_id = device_attribute_id
         self.name = name
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
@@ -2770,14 +2730,16 @@
             result['CreateTime'] = self.create_time
         result['CustomUserAttributes'] = []
         if self.custom_user_attributes is not None:
             for k in self.custom_user_attributes:
                 result['CustomUserAttributes'].append(k.to_map() if k else None)
         if self.description is not None:
             result['Description'] = self.description
+        if self.device_attribute_id is not None:
+            result['DeviceAttributeId'] = self.device_attribute_id
         if self.name is not None:
             result['Name'] = self.name
         if self.policy_action is not None:
             result['PolicyAction'] = self.policy_action
         if self.policy_id is not None:
             result['PolicyId'] = self.policy_id
         if self.priority is not None:
@@ -2803,14 +2765,16 @@
         self.custom_user_attributes = []
         if m.get('CustomUserAttributes') is not None:
             for k in m.get('CustomUserAttributes'):
                 temp_model = GetPrivateAccessPolicyResponseBodyPolicyCustomUserAttributes()
                 self.custom_user_attributes.append(temp_model.from_map(k))
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('DeviceAttributeId') is not None:
+            self.device_attribute_id = m.get('DeviceAttributeId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PolicyAction') is not None:
             self.policy_action = m.get('PolicyAction')
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         if m.get('Priority') is not None:
@@ -2869,17 +2833,14 @@
         body: GetPrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3115,17 +3076,14 @@
         body: GetRegistrationPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3439,17 +3397,14 @@
         body: GetUserDeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3649,17 +3604,14 @@
         body: GetUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3912,17 +3864,14 @@
         body: ListApplicationsForPrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4176,17 +4125,14 @@
         body: ListApplicationsForPrivateAccessTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4531,17 +4477,14 @@
         body: ListConnectorsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4614,17 +4557,14 @@
         body: ListDynamicRouteRegionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4873,17 +4813,14 @@
         body: ListDynamicRoutesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5138,17 +5075,14 @@
         body: ListExcessiveDeviceRegistrationApplicationsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5425,17 +5359,14 @@
         body: ListPolicesForPrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5728,17 +5659,14 @@
         body: ListPolicesForPrivateAccessTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5920,17 +5848,14 @@
         body: ListPolicesForUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5952,14 +5877,210 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListPolicesForUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListPopTrafficStatisticsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        region: str = None,
+        start_time: str = None,
+    ):
+        self.end_time = end_time
+        self.region = region
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class ListPopTrafficStatisticsResponseBodyTrafficDataDatapoints(TeaModel):
+    def __init__(
+        self,
+        average: float = None,
+        date_time: str = None,
+    ):
+        self.average = average
+        self.date_time = date_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.average is not None:
+            result['Average'] = self.average
+        if self.date_time is not None:
+            result['DateTime'] = self.date_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Average') is not None:
+            self.average = m.get('Average')
+        if m.get('DateTime') is not None:
+            self.date_time = m.get('DateTime')
+        return self
+
+
+class ListPopTrafficStatisticsResponseBodyTrafficData(TeaModel):
+    def __init__(
+        self,
+        datapoints: List[ListPopTrafficStatisticsResponseBodyTrafficDataDatapoints] = None,
+        metric_name: str = None,
+    ):
+        self.datapoints = datapoints
+        self.metric_name = metric_name
+
+    def validate(self):
+        if self.datapoints:
+            for k in self.datapoints:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Datapoints'] = []
+        if self.datapoints is not None:
+            for k in self.datapoints:
+                result['Datapoints'].append(k.to_map() if k else None)
+        if self.metric_name is not None:
+            result['MetricName'] = self.metric_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.datapoints = []
+        if m.get('Datapoints') is not None:
+            for k in m.get('Datapoints'):
+                temp_model = ListPopTrafficStatisticsResponseBodyTrafficDataDatapoints()
+                self.datapoints.append(temp_model.from_map(k))
+        if m.get('MetricName') is not None:
+            self.metric_name = m.get('MetricName')
+        return self
+
+
+class ListPopTrafficStatisticsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        traffic_data: List[ListPopTrafficStatisticsResponseBodyTrafficData] = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+        self.traffic_data = traffic_data
+
+    def validate(self):
+        if self.traffic_data:
+            for k in self.traffic_data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['TrafficData'] = []
+        if self.traffic_data is not None:
+            for k in self.traffic_data:
+                result['TrafficData'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.traffic_data = []
+        if m.get('TrafficData') is not None:
+            for k in m.get('TrafficData'):
+                temp_model = ListPopTrafficStatisticsResponseBodyTrafficData()
+                self.traffic_data.append(temp_model.from_map(k))
+        return self
+
+
+class ListPopTrafficStatisticsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListPopTrafficStatisticsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListPopTrafficStatisticsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListPrivateAccessApplicationsRequest(TeaModel):
     def __init__(
         self,
         address: str = None,
         application_ids: List[str] = None,
         connector_id: str = None,
         current_page: int = None,
@@ -6214,17 +6335,14 @@
         body: ListPrivateAccessApplicationsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6477,17 +6595,14 @@
         body: ListPrivateAccessApplicationsForDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6513,31 +6628,35 @@
         return self
 
 
 class ListPrivateAccessPolicesRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
+        application_name: str = None,
         current_page: int = None,
         name: str = None,
         page_size: int = None,
         policy_action: str = None,
         policy_ids: List[str] = None,
         status: str = None,
         tag_id: str = None,
+        tag_name: str = None,
         user_group_id: str = None,
     ):
         self.application_id = application_id
+        self.application_name = application_name
         self.current_page = current_page
         self.name = name
         self.page_size = page_size
         self.policy_action = policy_action
         self.policy_ids = policy_ids
         self.status = status
         self.tag_id = tag_id
+        self.tag_name = tag_name
         # 用户组ID。取值来源：
         # - [ListUserGroups](~~ListUserGroups~~)：批量查询用户组。
         # - [CreateUserGroup](~~CreateUserGroup~~)：创建用户组。
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
@@ -6546,50 +6665,58 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.application_id is not None:
             result['ApplicationId'] = self.application_id
+        if self.application_name is not None:
+            result['ApplicationName'] = self.application_name
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.name is not None:
             result['Name'] = self.name
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.policy_action is not None:
             result['PolicyAction'] = self.policy_action
         if self.policy_ids is not None:
             result['PolicyIds'] = self.policy_ids
         if self.status is not None:
             result['Status'] = self.status
         if self.tag_id is not None:
             result['TagId'] = self.tag_id
+        if self.tag_name is not None:
+            result['TagName'] = self.tag_name
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApplicationId') is not None:
             self.application_id = m.get('ApplicationId')
+        if m.get('ApplicationName') is not None:
+            self.application_name = m.get('ApplicationName')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PolicyAction') is not None:
             self.policy_action = m.get('PolicyAction')
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
+        if m.get('TagName') is not None:
+            self.tag_name = m.get('TagName')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
 
 
 class ListPrivateAccessPolicesResponseBodyPolicesCustomUserAttributes(TeaModel):
     def __init__(
@@ -6640,28 +6767,30 @@
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         create_time: str = None,
         custom_user_attributes: List[ListPrivateAccessPolicesResponseBodyPolicesCustomUserAttributes] = None,
         description: str = None,
+        device_attribute_id: str = None,
         name: str = None,
         policy_action: str = None,
         policy_id: str = None,
         priority: int = None,
         status: str = None,
         tag_ids: List[str] = None,
         user_group_ids: List[str] = None,
         user_group_mode: str = None,
     ):
         self.application_ids = application_ids
         self.application_type = application_type
         self.create_time = create_time
         self.custom_user_attributes = custom_user_attributes
         self.description = description
+        self.device_attribute_id = device_attribute_id
         self.name = name
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
@@ -6687,14 +6816,16 @@
             result['CreateTime'] = self.create_time
         result['CustomUserAttributes'] = []
         if self.custom_user_attributes is not None:
             for k in self.custom_user_attributes:
                 result['CustomUserAttributes'].append(k.to_map() if k else None)
         if self.description is not None:
             result['Description'] = self.description
+        if self.device_attribute_id is not None:
+            result['DeviceAttributeId'] = self.device_attribute_id
         if self.name is not None:
             result['Name'] = self.name
         if self.policy_action is not None:
             result['PolicyAction'] = self.policy_action
         if self.policy_id is not None:
             result['PolicyId'] = self.policy_id
         if self.priority is not None:
@@ -6720,14 +6851,16 @@
         self.custom_user_attributes = []
         if m.get('CustomUserAttributes') is not None:
             for k in m.get('CustomUserAttributes'):
                 temp_model = ListPrivateAccessPolicesResponseBodyPolicesCustomUserAttributes()
                 self.custom_user_attributes.append(temp_model.from_map(k))
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('DeviceAttributeId') is not None:
+            self.device_attribute_id = m.get('DeviceAttributeId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PolicyAction') is not None:
             self.policy_action = m.get('PolicyAction')
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         if m.get('Priority') is not None:
@@ -6798,17 +6931,14 @@
         body: ListPrivateAccessPolicesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6841,20 +6971,33 @@
         current_page: int = None,
         name: str = None,
         page_size: int = None,
         policy_id: str = None,
         simple_mode: bool = None,
         tag_ids: List[str] = None,
     ):
+        # The ID of the internal access application. You can obtain the application ID by calling the following operations:
+        # 
+        # *   [ListPrivateAccessApplications](~~ListPrivateAccessApplications~~): queries all internal access applications.
+        # *   [CreatePrivateAccessApplication](~~CreatePrivateAccessApplication~~): creates an internal access application.
         self.application_id = application_id
+        # The page number. Valid values: 1 to 10000.
         self.current_page = current_page
+        # The name of the internal access tag. The name must be 1 to 128 characters in length and can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
         self.name = name
+        # The number of entries per page. Valid values: 1 to 1000.
         self.page_size = page_size
+        # The ID of the internal access policy. You can obtain the policy ID by calling the following operations:
+        # 
+        # *   [ListPrivateAccessPolices](~~ListPrivateAccessPolices~~): queries all internal access policies.
+        # *   [CreatePrivateAccessPolicy](~~CreatePrivateAccessPolicy~~): creates an internal access policy.
         self.policy_id = policy_id
+        # Specifies whether to enable the simple query mode. A value of true specifies that policy IDs are not queried.
         self.simple_mode = simple_mode
+        # The IDs of internal access tags. You can specify up to 100 tag IDs.
         self.tag_ids = tag_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6904,20 +7047,30 @@
         create_time: str = None,
         description: str = None,
         name: str = None,
         policy_ids: List[str] = None,
         tag_id: str = None,
         tag_type: str = None,
     ):
+        # The IDs of the internal access applications.
         self.application_ids = application_ids
+        # The time when the internal access tag was created.
         self.create_time = create_time
+        # The description of the internal access tag.
         self.description = description
+        # The name of the internal access tag.
         self.name = name
+        # The IDs of the internal access policies.
         self.policy_ids = policy_ids
+        # The ID of the internal access tag.
         self.tag_id = tag_id
+        # The type of the internal access tag. Valid values:
+        # 
+        # *   **Default**\
+        # *   **Custom**\
         self.tag_type = tag_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6963,16 +7116,19 @@
 class ListPrivateAccessTagsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tags: List[ListPrivateAccessTagsResponseBodyTags] = None,
         total_num: int = None,
     ):
+        # The request ID.
         self.request_id = request_id
+        # The internal access tags.
         self.tags = tags
+        # The total number of internal access tags.
         self.total_num = total_num
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -7015,17 +7171,14 @@
         body: ListPrivateAccessTagsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7219,17 +7372,14 @@
         body: ListPrivateAccessTagsForDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7554,17 +7704,14 @@
         body: ListRegistrationPoliciesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7870,17 +8017,14 @@
         body: ListRegistrationPoliciesForUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8045,17 +8189,14 @@
         body: ListSoftwareForUserDeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8249,17 +8390,14 @@
         body: ListTagsForPrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8454,17 +8592,14 @@
         body: ListTagsForPrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8845,17 +8980,14 @@
         body: ListUserDevicesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9098,17 +9230,14 @@
         body: ListUserGroupsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9356,17 +9485,14 @@
         body: ListUserGroupsForPrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9613,17 +9739,14 @@
         body: ListUserGroupsForRegistrationPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9645,14 +9768,228 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUserGroupsForRegistrationPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListUsersRequest(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        department: str = None,
+        fuzzy_username: str = None,
+        page_size: int = None,
+        precise_username: str = None,
+        sase_user_ids: List[str] = None,
+        status: str = None,
+    ):
+        self.current_page = current_page
+        self.department = department
+        self.fuzzy_username = fuzzy_username
+        self.page_size = page_size
+        self.precise_username = precise_username
+        self.sase_user_ids = sase_user_ids
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.department is not None:
+            result['Department'] = self.department
+        if self.fuzzy_username is not None:
+            result['FuzzyUsername'] = self.fuzzy_username
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.precise_username is not None:
+            result['PreciseUsername'] = self.precise_username
+        if self.sase_user_ids is not None:
+            result['SaseUserIds'] = self.sase_user_ids
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('Department') is not None:
+            self.department = m.get('Department')
+        if m.get('FuzzyUsername') is not None:
+            self.fuzzy_username = m.get('FuzzyUsername')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('PreciseUsername') is not None:
+            self.precise_username = m.get('PreciseUsername')
+        if m.get('SaseUserIds') is not None:
+            self.sase_user_ids = m.get('SaseUserIds')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class ListUsersResponseBodyUsers(TeaModel):
+    def __init__(
+        self,
+        department: str = None,
+        email: str = None,
+        idp_name: str = None,
+        phone: str = None,
+        sase_user_id: str = None,
+        status: str = None,
+        username: str = None,
+    ):
+        self.department = department
+        self.email = email
+        self.idp_name = idp_name
+        self.phone = phone
+        self.sase_user_id = sase_user_id
+        self.status = status
+        self.username = username
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department is not None:
+            result['Department'] = self.department
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.idp_name is not None:
+            result['IdpName'] = self.idp_name
+        if self.phone is not None:
+            result['Phone'] = self.phone
+        if self.sase_user_id is not None:
+            result['SaseUserId'] = self.sase_user_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Department') is not None:
+            self.department = m.get('Department')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('IdpName') is not None:
+            self.idp_name = m.get('IdpName')
+        if m.get('Phone') is not None:
+            self.phone = m.get('Phone')
+        if m.get('SaseUserId') is not None:
+            self.sase_user_id = m.get('SaseUserId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class ListUsersResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        total_num: str = None,
+        users: List[ListUsersResponseBodyUsers] = None,
+    ):
+        self.request_id = request_id
+        self.total_num = total_num
+        self.users = users
+
+    def validate(self):
+        if self.users:
+            for k in self.users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_num is not None:
+            result['TotalNum'] = self.total_num
+        result['Users'] = []
+        if self.users is not None:
+            for k in self.users:
+                result['Users'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalNum') is not None:
+            self.total_num = m.get('TotalNum')
+        self.users = []
+        if m.get('Users') is not None:
+            for k in m.get('Users'):
+                temp_model = ListUsersResponseBodyUsers()
+                self.users.append(temp_model.from_map(k))
+        return self
+
+
+class ListUsersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListUsersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListUsersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateDynamicRouteRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         description: str = None,
         dynamic_route_id: str = None,
@@ -9777,17 +10114,14 @@
         body: UpdateDynamicRouteResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9988,17 +10322,14 @@
         body: UpdateExcessiveDeviceRegistrationApplicationsStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10169,17 +10500,14 @@
         body: UpdatePrivateAccessApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10253,27 +10581,29 @@
 class UpdatePrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         custom_user_attributes: List[UpdatePrivateAccessPolicyRequestCustomUserAttributes] = None,
         description: str = None,
+        device_attribute_id: str = None,
         modify_type: str = None,
         policy_action: str = None,
         policy_id: str = None,
         priority: int = None,
         status: str = None,
         tag_ids: List[str] = None,
         user_group_ids: List[str] = None,
         user_group_mode: str = None,
     ):
         self.application_ids = application_ids
         self.application_type = application_type
         self.custom_user_attributes = custom_user_attributes
         self.description = description
+        self.device_attribute_id = device_attribute_id
         self.modify_type = modify_type
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids = tag_ids
@@ -10301,14 +10631,16 @@
             result['ApplicationType'] = self.application_type
         result['CustomUserAttributes'] = []
         if self.custom_user_attributes is not None:
             for k in self.custom_user_attributes:
                 result['CustomUserAttributes'].append(k.to_map() if k else None)
         if self.description is not None:
             result['Description'] = self.description
+        if self.device_attribute_id is not None:
+            result['DeviceAttributeId'] = self.device_attribute_id
         if self.modify_type is not None:
             result['ModifyType'] = self.modify_type
         if self.policy_action is not None:
             result['PolicyAction'] = self.policy_action
         if self.policy_id is not None:
             result['PolicyId'] = self.policy_id
         if self.priority is not None:
@@ -10332,14 +10664,16 @@
         self.custom_user_attributes = []
         if m.get('CustomUserAttributes') is not None:
             for k in m.get('CustomUserAttributes'):
                 temp_model = UpdatePrivateAccessPolicyRequestCustomUserAttributes()
                 self.custom_user_attributes.append(temp_model.from_map(k))
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('DeviceAttributeId') is not None:
+            self.device_attribute_id = m.get('DeviceAttributeId')
         if m.get('ModifyType') is not None:
             self.modify_type = m.get('ModifyType')
         if m.get('PolicyAction') is not None:
             self.policy_action = m.get('PolicyAction')
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         if m.get('Priority') is not None:
@@ -10390,17 +10724,14 @@
         body: UpdatePrivateAccessPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10907,17 +11238,14 @@
         body: UpdateRegistrationPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11196,17 +11524,14 @@
         body: UpdateUserDevicesSharingStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11485,17 +11810,14 @@
         body: UpdateUserDevicesStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11654,17 +11976,14 @@
         body: UpdateUserGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11686,7 +12005,108 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateUsersStatusRequest(TeaModel):
+    def __init__(
+        self,
+        sase_user_ids: List[str] = None,
+        status: str = None,
+    ):
+        self.sase_user_ids = sase_user_ids
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.sase_user_ids is not None:
+            result['SaseUserIds'] = self.sase_user_ids
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SaseUserIds') is not None:
+            self.sase_user_ids = m.get('SaseUserIds')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class UpdateUsersStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateUsersStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateUsersStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateUsersStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_csas20230120-1.2.1/alibabacloud_csas20230120.egg-info/PKG-INFO` & `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120
-Version: 1.2.1
+Version: 1.3.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/csas-20230120/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_csas20230120-1.2.1/setup.py` & `alibabacloud_csas20230120-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120.
 
-Created on 15/11/2023
+Created on 15/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

