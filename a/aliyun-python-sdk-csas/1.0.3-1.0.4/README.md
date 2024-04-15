# Comparing `tmp/aliyun-python-sdk-csas-1.0.3.tar.gz` & `tmp/aliyun-python-sdk-csas-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-csas-1.0.3.tar", last modified: Thu Nov 16 02:30:33 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-csas-1.0.4.tar", last modified: Mon Apr 15 03:00:13 2024, max compression
```

## Comparing `aliyun-python-sdk-csas-1.0.3.tar` & `aliyun-python-sdk-csas-1.0.4.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      575 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3890 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/
--rw-r--r--   0 root         (0) root         (0)       21 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/
--rw-r--r--   0 root         (0) root         (0)     1457 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1233 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1181 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1293 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1016 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4910 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3475 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2885 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-11-16 02:30:33.000000 aliyun-python-sdk-csas-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4069 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/setup.py
```

### Comparing `aliyun-python-sdk-csas-1.0.3/LICENSE` & `aliyun-python-sdk-csas-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/PKG-INFO` & `aliyun-python-sdk-csas-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-csas
-Version: 1.0.3
+Version: 1.0.4
 Summary: The csas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-csas
```

### Comparing `aliyun-python-sdk-csas-1.0.3/README.rst` & `aliyun-python-sdk-csas-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/PKG-INFO` & `aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-csas
-Version: 1.0.3
+Version: 1.0.4
 Summary: The csas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-csas
```

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyun_python_sdk_csas.egg-info/SOURCES.txt` & `aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,33 @@
 aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
 aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
 aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
 aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
+aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py
 aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py
 aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py
 aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py
 aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
+aliyunsdkcsas/request/v20230120/ListUsersRequest.py
 aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
 aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
+aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py
 aliyunsdkcsas/request/v20230120/__init__.py
```

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,19 @@
 				self.add_body_params('CustomUserAttributes.' + str(index1 + 1) + '.Relation', value1.get('Relation'))
 	def get_TagIds(self): # Array
 		return self.get_body_params().get('TagIds')
 
 	def set_TagIds(self, TagIds):  # Array
 		for index1, value1 in enumerate(TagIds):
 			self.add_body_params('TagIds.' + str(index1 + 1), value1)
+	def get_DeviceAttributeId(self): # String
+		return self.get_body_params().get('DeviceAttributeId')
+
+	def set_DeviceAttributeId(self, DeviceAttributeId):  # String
+		self.add_body_params('DeviceAttributeId', DeviceAttributeId)
 	def get_UserGroupIds(self): # Array
 		return self.get_body_params().get('UserGroupIds')
 
 	def set_UserGroupIds(self, UserGroupIds):  # Array
 		for index1, value1 in enumerate(UserGroupIds):
 			self.add_body_params('UserGroupIds.' + str(index1 + 1), value1)
 	def get_PolicyAction(self): # String
```

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 
 	def get_PolicyIds(self): # Array
 		return self.get_query_params().get('PolicyIds')
 
 	def set_PolicyIds(self, PolicyIds):  # Array
 		for index1, value1 in enumerate(PolicyIds):
 			self.add_query_param('PolicyIds.' + str(index1 + 1), value1)
+	def get_TagName(self): # String
+		return self.get_query_params().get('TagName')
+
+	def set_TagName(self, TagName):  # String
+		self.add_query_param('TagName', TagName)
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_ApplicationId(self): # String
 		return self.get_query_params().get('ApplicationId')
@@ -57,14 +62,19 @@
 	def set_CurrentPage(self, CurrentPage):  # Integer
 		self.add_query_param('CurrentPage', CurrentPage)
 	def get_PolicyAction(self): # String
 		return self.get_query_params().get('PolicyAction')
 
 	def set_PolicyAction(self, PolicyAction):  # String
 		self.add_query_param('PolicyAction', PolicyAction)
+	def get_ApplicationName(self): # String
+		return self.get_query_params().get('ApplicationName')
+
+	def set_ApplicationName(self, ApplicationName):  # String
+		self.add_query_param('ApplicationName', ApplicationName)
 	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
 	def set_Name(self, Name):  # String
 		self.add_query_param('Name', Name)
 	def get_Status(self): # String
 		return self.get_query_params().get('Status')
```

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 				self.add_body_params('CustomUserAttributes.' + str(index1 + 1) + '.Relation', value1.get('Relation'))
 	def get_TagIds(self): # Array
 		return self.get_body_params().get('TagIds')
 
 	def set_TagIds(self, TagIds):  # Array
 		for index1, value1 in enumerate(TagIds):
 			self.add_body_params('TagIds.' + str(index1 + 1), value1)
+	def get_DeviceAttributeId(self): # String
+		return self.get_body_params().get('DeviceAttributeId')
+
+	def set_DeviceAttributeId(self, DeviceAttributeId):  # String
+		self.add_body_params('DeviceAttributeId', DeviceAttributeId)
 	def get_UserGroupIds(self): # Array
 		return self.get_body_params().get('UserGroupIds')
 
 	def set_UserGroupIds(self, UserGroupIds):  # Array
 		for index1, value1 in enumerate(UserGroupIds):
 			self.add_body_params('UserGroupIds.' + str(index1 + 1), value1)
 	def get_PolicyAction(self): # String
```

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.3/setup.py` & `aliyun-python-sdk-csas-1.0.4/setup.py`

 * *Files identical despite different names*

