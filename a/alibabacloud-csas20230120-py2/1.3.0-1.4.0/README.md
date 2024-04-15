# Comparing `tmp/alibabacloud_csas20230120_py2-1.3.0.tar.gz` & `tmp/alibabacloud_csas20230120_py2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.3.0.tar", last modified: Thu Jan 25 17:09:32 2024, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.4.0.tar", last modified: Mon Apr 15 03:01:33 2024, max compression
```

## Comparing `alibabacloud_csas20230120_py2-1.3.0.tar` & `alibabacloud_csas20230120_py2-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      494 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66659 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   389127 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2024-01-25 17:09:32.000000 alibabacloud_csas20230120_py2-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68633 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   398633 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/setup.py
```

### Comparing `alibabacloud_csas20230120_py2-1.3.0/LICENSE` & `alibabacloud_csas20230120_py2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.3.0/PKG-INFO` & `alibabacloud_csas20230120_py2-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120_py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.3.0/README-CN.md` & `alibabacloud_csas20230120_py2-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.3.0/README.md` & `alibabacloud_csas20230120_py2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1308,14 +1308,40 @@
             self.call_api(params, req, runtime)
         )
 
     def list_user_groups_for_registration_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_user_groups_for_registration_policy_with_options(request, runtime)
 
+    def list_users_with_options(self, request, runtime):
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
+    def list_users(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_users_with_options(request, runtime)
+
     def update_dynamic_route_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
@@ -1655,7 +1681,37 @@
             csas_20230120_models.UpdateUserGroupResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_user_group_with_options(request, runtime)
+
+    def update_users_status_with_options(self, request, runtime):
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
+    def update_users_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_users_status_with_options(request, runtime)
```

### Comparing `alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8605,14 +8605,202 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUserGroupsForRegistrationPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListUsersRequest(TeaModel):
+    def __init__(self, current_page=None, department=None, fuzzy_username=None, page_size=None,
+                 precise_username=None, sase_user_ids=None, status=None):
+        self.current_page = current_page  # type: long
+        self.department = department  # type: str
+        self.fuzzy_username = fuzzy_username  # type: str
+        self.page_size = page_size  # type: long
+        self.precise_username = precise_username  # type: str
+        self.sase_user_ids = sase_user_ids  # type: list[str]
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListUsersRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, department=None, email=None, idp_name=None, phone=None, sase_user_id=None, status=None,
+                 username=None):
+        self.department = department  # type: str
+        self.email = email  # type: str
+        self.idp_name = idp_name  # type: str
+        self.phone = phone  # type: str
+        self.sase_user_id = sase_user_id  # type: str
+        self.status = status  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListUsersResponseBodyUsers, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, total_num=None, users=None):
+        self.request_id = request_id  # type: str
+        self.total_num = total_num  # type: str
+        self.users = users  # type: list[ListUsersResponseBodyUsers]
+
+    def validate(self):
+        if self.users:
+            for k in self.users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListUsersResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListUsersResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListUsersResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, application_ids=None, application_type=None, description=None, dynamic_route_id=None,
                  dynamic_route_type=None, modify_type=None, name=None, next_hop=None, priority=None, region_ids=None, status=None,
                  tag_ids=None):
         self.application_ids = application_ids  # type: list[str]
         self.application_type = application_type  # type: str
         self.description = description  # type: str
@@ -10378,7 +10566,96 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateUsersStatusRequest(TeaModel):
+    def __init__(self, sase_user_ids=None, status=None):
+        self.sase_user_ids = sase_user_ids  # type: list[str]
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUsersStatusRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SaseUserIds') is not None:
+            self.sase_user_ids = m.get('SaseUserIds')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class UpdateUsersStatusResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUsersStatusResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateUsersStatusResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateUsersStatusResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateUsersStatusResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_csas20230120_py2-1.3.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO` & `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120-py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.3.0/setup.py` & `alibabacloud_csas20230120_py2-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120_py2.
 
-Created on 25/01/2024
+Created on 15/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python2"
```

