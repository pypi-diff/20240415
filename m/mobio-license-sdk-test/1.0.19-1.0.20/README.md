# Comparing `tmp/mobio-license-sdk-test-1.0.19.tar.gz` & `tmp/mobio-license-sdk-test-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-license-sdk-test-1.0.19.tar", last modified: Fri Mar 15 09:55:13 2024, max compression
+gzip compressed data, was "mobio-license-sdk-test-1.0.20.tar", last modified: Mon Apr 15 07:27:25 2024, max compression
```

## Comparing `mobio-license-sdk-test-1.0.19.tar` & `mobio-license-sdk-test-1.0.20.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 09:55:13.389185 mobio-license-sdk-test-1.0.19/
--rw-r--r--   0 root         (0) root         (0)     2116 2024-03-15 09:55:13.388184 mobio-license-sdk-test-1.0.19/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2023-12-18 16:06:14.000000 mobio-license-sdk-test-1.0.19/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 09:55:13.359184 mobio-license-sdk-test-1.0.19/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 09:55:13.360184 mobio-license-sdk-test-1.0.19/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 09:55:13.373184 mobio-license-sdk-test-1.0.19/mobio/sdks/license/
--rw-r--r--   0 root         (0) root         (0)      256 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/call_api.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/config.py
--rw-r--r--   0 root         (0) root         (0)    13599 2024-03-15 09:54:44.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/crypt_utils.py
--rw-r--r--   0 root         (0) root         (0)    10108 2024-01-25 09:39:05.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/date_utils.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_detail_mess_used.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_history_mess_used.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_mess_used.py
--rw-r--r--   0 root         (0) root         (0)     9269 2024-03-15 09:54:44.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_sdk.py
--rw-r--r--   0 root         (0) root         (0)      841 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/mongo_connection.py
--rw-r--r--   0 root         (0) root         (0)    23992 2024-03-15 09:54:44.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/package_utils.py
--rw-r--r--   0 root         (0) root         (0)    33688 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/mobio/sdks/license/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 09:55:13.387184 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2116 2024-03-15 09:55:13.000000 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      692 2024-03-15 09:55:13.000000 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 09:55:13.000000 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-15 09:55:13.000000 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-15 09:55:13.000000 mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.19/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-15 09:55:13.390184 mobio-license-sdk-test-1.0.19/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9439 2024-03-15 09:55:12.000000 mobio-license-sdk-test-1.0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:27:25.459357 mobio-license-sdk-test-1.0.20/
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-15 07:27:25.458357 mobio-license-sdk-test-1.0.20/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-12-18 16:06:14.000000 mobio-license-sdk-test-1.0.20/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:27:25.436356 mobio-license-sdk-test-1.0.20/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:27:25.437356 mobio-license-sdk-test-1.0.20/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:27:25.451357 mobio-license-sdk-test-1.0.20/mobio/sdks/license/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/config.py
+-rw-r--r--   0 root         (0) root         (0)    13599 2024-03-15 09:54:44.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/crypt_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10108 2024-01-25 09:39:05.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/date_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_detail_mess_used.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_history_mess_used.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_mess_used.py
+-rw-r--r--   0 root         (0) root         (0)     9269 2024-03-15 09:54:44.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_sdk.py
+-rw-r--r--   0 root         (0) root         (0)      841 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/mongo_connection.py
+-rw-r--r--   0 root         (0) root         (0)    24709 2024-04-15 07:26:41.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/package_utils.py
+-rw-r--r--   0 root         (0) root         (0)    33688 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/mobio/sdks/license/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:27:25.457357 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-15 07:27:25.000000 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      692 2024-04-15 07:27:25.000000 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 07:27:25.000000 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-15 07:27:25.000000 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-15 07:27:25.000000 mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-12-18 16:06:15.000000 mobio-license-sdk-test-1.0.20/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 07:27:25.459357 mobio-license-sdk-test-1.0.20/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9439 2024-04-15 07:27:24.000000 mobio-license-sdk-test-1.0.20/setup.py
```

### Comparing `mobio-license-sdk-test-1.0.19/PKG-INFO` & `mobio-license-sdk-test-1.0.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-license-sdk-test
-Version: 1.0.19
+Version: 1.0.20
 Summary: Mobio license SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-license
```

### Comparing `mobio-license-sdk-test-1.0.19/README.md` & `mobio-license-sdk-test-1.0.20/README.md`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/call_api.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/call_api.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/config.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/config.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/crypt_utils.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/date_utils.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/date_utils.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_detail_mess_used.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_detail_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_history_mess_used.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_history_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_mess_used.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/license_sdk.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/license_sdk.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/mongo_connection.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/mongo_connection.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/package_utils.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/package_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         merchant_id = "merchant_id"
         version = "version"
         created_time = "created_time"
         api_key = "api_key"
         alert_merchant = "alert_merchant"
         packages = "packages"
         field_map_module = "field_map_module"
+        field_merge_values = "field_merge_values"
         # start_time = "start_time"
         # expire_time = "expire_time"
         config_constant = "config_constant"
         coefficient_message = "coefficient_message"
         config_expire = "config_expire"
 
     class LicenseMerchant:
@@ -66,17 +67,20 @@
 
     def __init__(self, json_license):
         self.json_license = json_license
         self.package_current = {}
         self.uncheck_license = False
 
         self.field_map_module = {}
+        self.field_merge_values = {}
         if json_license and isinstance(json_license, dict):
             if json_license.get(self.LicenseJson.field_map_module):
                 self.field_map_module = json_license.get(self.LicenseJson.field_map_module)
+            if json_license.get(self.LicenseJson.field_merge_values):
+                self.field_merge_values = json_license.get(self.LicenseJson.field_merge_values)
 
         """
         {
             "config_constant": {
                 "coefficient_message":{ # he so x mtp = so message duoc phep trong thang
                     "free": 5,
                     "growth": 5,
@@ -290,23 +294,31 @@
             return self.get_attribute_quantity(
                 module=module, attribute=attribute
             )
 
     def pre_check_allow_attribute_feature(self, module: str, attribute: str):
         if attribute in self.field_map_module:
             data_default = {"is_allowed": False}
+            values_merge = []
             for m in self.field_map_module.get(attribute):
                 data_package = self.check_allow_attribute_feature(
                     module=m, attribute=attribute
                 )
                 if data_package:
-                    if data_package.get("is_allowed"):
-                        return data_package
+                    if self.field_merge_values.get(attribute):
+                        if data_package.get("is_allowed"):
+                            values_merge.extend(data_package.get("values", []))
+                            data_default.update(data_package)
                     else:
-                        data_default.update(data_package)
+                        if data_package.get("is_allowed"):
+                            return data_package
+                        else:
+                            data_default.update(data_package)
+            if self.field_merge_values.get(attribute):
+                data_default.update({"values": list(set(values_merge))})
             return data_default
         else:
             return self.check_allow_attribute_feature(
                 module=module, attribute=attribute
             )
 
     def calculate_limit_number(self, number_mtp, package_code):
```

### Comparing `mobio-license-sdk-test-1.0.19/mobio/sdks/license/utils.py` & `mobio-license-sdk-test-1.0.20/mobio/sdks/license/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/PKG-INFO` & `mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-license-sdk-test
-Version: 1.0.19
+Version: 1.0.20
 Summary: Mobio license SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-license
```

### Comparing `mobio-license-sdk-test-1.0.19/mobio_license_sdk_test.egg-info/SOURCES.txt` & `mobio-license-sdk-test-1.0.20/mobio_license_sdk_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-test-1.0.19/setup.py` & `mobio-license-sdk-test-1.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         # with open(Requirements.__requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 
-version_dev='1.0.19'
-version_prod='1.0.17'
+version_dev='1.0.20'
+version_prod='1.0.18'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -66,15 +66,15 @@
     name="mobio-license-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.19',  # Required
+    version='1.0.20',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio license SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

