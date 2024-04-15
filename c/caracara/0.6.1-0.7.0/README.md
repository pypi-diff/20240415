# Comparing `tmp/caracara-0.6.1.tar.gz` & `tmp/caracara-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caracara-0.6.1.tar", max compression
+gzip compressed data, was "caracara-0.7.0.tar", max compression
```

## Comparing `caracara-0.6.1.tar` & `caracara-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0     1068 2024-03-04 18:46:48.886943 caracara-0.6.1/LICENSE
--rw-r--r--   0        0        0     8994 2024-03-04 18:46:48.886943 caracara-0.6.1/README.md
--rw-r--r--   0        0        0     2314 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/__init__.py
--rw-r--r--   0        0        0     6860 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/client.py
--rw-r--r--   0        0        0      417 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/__init__.py
--rw-r--r--   0        0        0     4212 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/batching.py
--rw-r--r--   0        0        0     1664 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/constants.py
--rw-r--r--   0        0        0     3493 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/csdialog.py
--rw-r--r--   0        0        0     2062 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/decorators.py
--rw-r--r--   0        0        0     4111 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/exceptions.py
--rw-r--r--   0        0        0     3402 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/interpolation.py
--rw-r--r--   0        0        0      560 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/meta.py
--rw-r--r--   0        0        0     1110 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/module.py
--rw-r--r--   0        0        0    12581 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/pagination.py
--rw-r--r--   0        0        0    15403 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/policy_wrapper.py
--rw-r--r--   0        0        0      152 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/common/sorting.py
--rw-r--r--   0        0        0      211 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/filters/__init__.py
--rw-r--r--   0        0        0     2353 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/filters/decorators.py
--rw-r--r--   0        0        0      792 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/__init__.py
--rw-r--r--   0        0        0      282 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/custom_ioa/__init__.py
--rw-r--r--   0        0        0    11860 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/custom_ioa/custom_ioa.py
--rw-r--r--   0        0        0     6045 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/custom_ioa/rule_types.py
--rw-r--r--   0        0        0    25066 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/custom_ioa/rules.py
--rw-r--r--   0        0        0      166 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/flight_control/__init__.py
--rw-r--r--   0        0        0     3811 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/flight_control/flight_control.py
--rw-r--r--   0        0        0      124 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/__init__.py
--rw-r--r--   0        0        0     1840 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_containment.py
--rw-r--r--   0        0        0     2877 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_data_history.py
--rw-r--r--   0        0        0    16077 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_groups.py
--rw-r--r--   0        0        0     3567 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_hiding.py
--rw-r--r--   0        0        0     2953 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_online_state.py
--rw-r--r--   0        0        0     2776 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/_tagging.py
--rw-r--r--   0        0        0     7849 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/hosts/hosts.py
--rw-r--r--   0        0        0      191 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/prevention_policies/__init__.py
--rw-r--r--   0        0        0     3440 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/prevention_policies/prevention_policies.py
--rw-r--r--   0        0        0    25782 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/prevention_policies/template.py
--rw-r--r--   0        0        0      173 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/response_policies/__init__.py
--rw-r--r--   0        0        0     5495 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/response_policies/response_policies.py
--rw-r--r--   0        0        0     4817 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/response_policies/template.py
--rw-r--r--   0        0        0      397 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/rtr/__init__.py
--rw-r--r--   0        0        0    18711 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/rtr/batch_session.py
--rw-r--r--   0        0        0     1792 2024-03-04 18:46:48.886943 caracara-0.6.1/caracara/modules/rtr/constants.py
--rw-r--r--   0        0        0     3413 2024-03-04 18:46:48.890943 caracara-0.6.1/caracara/modules/rtr/get_file.py
--rw-r--r--   0        0        0     9219 2024-03-04 18:46:48.890943 caracara-0.6.1/caracara/modules/rtr/rtr.py
--rw-r--r--   0        0        0      131 2024-03-04 18:46:48.890943 caracara-0.6.1/caracara/modules/users/__init__.py
--rw-r--r--   0        0        0     4921 2024-03-04 18:46:48.890943 caracara-0.6.1/caracara/modules/users/users.py
--rw-r--r--   0        0        0     3856 2024-03-04 18:46:48.890943 caracara-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     9655 1970-01-01 00:00:00.000000 caracara-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-15 14:31:07.410333 caracara-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8994 2024-04-15 14:31:07.410333 caracara-0.7.0/README.md
+-rw-r--r--   0        0        0     2314 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/__init__.py
+-rw-r--r--   0        0        0     7062 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/client.py
+-rw-r--r--   0        0        0      417 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/__init__.py
+-rw-r--r--   0        0        0     4212 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/batching.py
+-rw-r--r--   0        0        0     1664 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/constants.py
+-rw-r--r--   0        0        0     3493 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/csdialog.py
+-rw-r--r--   0        0        0     2062 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/decorators.py
+-rw-r--r--   0        0        0     4111 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/exceptions.py
+-rw-r--r--   0        0        0     3402 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/interpolation.py
+-rw-r--r--   0        0        0      560 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/meta.py
+-rw-r--r--   0        0        0     1110 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/module.py
+-rw-r--r--   0        0        0    12581 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/pagination.py
+-rw-r--r--   0        0        0    15403 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/policy_wrapper.py
+-rw-r--r--   0        0        0      152 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/common/sorting.py
+-rw-r--r--   0        0        0      211 2024-04-15 14:31:07.410333 caracara-0.7.0/caracara/filters/__init__.py
+-rw-r--r--   0        0        0     2353 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/filters/decorators.py
+-rw-r--r--   0        0        0      911 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/__init__.py
+-rw-r--r--   0        0        0      282 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/custom_ioa/__init__.py
+-rw-r--r--   0        0        0    11860 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/custom_ioa/custom_ioa.py
+-rw-r--r--   0        0        0     6045 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/custom_ioa/rule_types.py
+-rw-r--r--   0        0        0    25066 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/custom_ioa/rules.py
+-rw-r--r--   0        0        0      166 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/flight_control/__init__.py
+-rw-r--r--   0        0        0     3811 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/flight_control/flight_control.py
+-rw-r--r--   0        0        0      124 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_containment.py
+-rw-r--r--   0        0        0     2877 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_data_history.py
+-rw-r--r--   0        0        0    16077 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_groups.py
+-rw-r--r--   0        0        0     3567 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_hiding.py
+-rw-r--r--   0        0        0     2953 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_online_state.py
+-rw-r--r--   0        0        0     2776 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/_tagging.py
+-rw-r--r--   0        0        0     7849 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/hosts/hosts.py
+-rw-r--r--   0        0        0      191 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/prevention_policies/__init__.py
+-rw-r--r--   0        0        0     3440 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/prevention_policies/prevention_policies.py
+-rw-r--r--   0        0        0    25782 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/prevention_policies/template.py
+-rw-r--r--   0        0        0      173 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/response_policies/__init__.py
+-rw-r--r--   0        0        0     5495 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/response_policies/response_policies.py
+-rw-r--r--   0        0        0     4817 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/response_policies/template.py
+-rw-r--r--   0        0        0      397 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/rtr/__init__.py
+-rw-r--r--   0        0        0    18711 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/rtr/batch_session.py
+-rw-r--r--   0        0        0     1792 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/rtr/constants.py
+-rw-r--r--   0        0        0     3413 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/rtr/get_file.py
+-rw-r--r--   0        0        0     9219 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/rtr/rtr.py
+-rw-r--r--   0        0        0      206 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/sensor_update_policies/__init__.py
+-rw-r--r--   0        0        0     2973 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/sensor_update_policies/sensor_update_policies.py
+-rw-r--r--   0        0        0      131 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/users/__init__.py
+-rw-r--r--   0        0        0     4921 2024-04-15 14:31:07.414334 caracara-0.7.0/caracara/modules/users/users.py
+-rw-r--r--   0        0        0     3990 2024-04-15 14:31:07.418334 caracara-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9655 1970-01-01 00:00:00.000000 caracara-0.7.0/PKG-INFO
```

### Comparing `caracara-0.6.1/LICENSE` & `caracara-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/README.md` & `caracara-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/__init__.py` & `caracara-0.7.0/caracara/__init__.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/client.py` & `caracara-0.7.0/caracara/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from caracara.modules import (
     CustomIoaApiModule,
     FlightControlApiModule,
     HostsApiModule,
     PreventionPoliciesApiModule,
     ResponsePoliciesApiModule,
     RTRApiModule,
+    SensorUpdatePoliciesApiModule,
     UsersApiModule,
 )
 
 
 class Client:
     """Falcon API client.
 
@@ -154,14 +155,16 @@
         self.hosts = HostsApiModule(self.api_authentication)
         self.logger.debug("Setting up the Prevention Policies module")
         self.prevention_policies = PreventionPoliciesApiModule(self.api_authentication)
         self.logger.debug("Setting up the Response Policies module")
         self.response_policies = ResponsePoliciesApiModule(self.api_authentication)
         self.logger.debug("Setting up the RTR module")
         self.rtr = RTRApiModule(self.api_authentication)
+        self.logger.debug("Setting up the Sensor Update Policies module")
+        self.sensor_update_policies = SensorUpdatePoliciesApiModule(self.api_authentication)
         self.logger.debug("Setting up the Users module")
         self.users = UsersApiModule(self.api_authentication)
 
         self.logger.info("Caracara client configured")
 
     def __enter__(self):
         """Allow for entry as a context manager."""
```

### Comparing `caracara-0.6.1/caracara/common/batching.py` & `caracara-0.7.0/caracara/common/batching.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/constants.py` & `caracara-0.7.0/caracara/common/constants.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/csdialog.py` & `caracara-0.7.0/caracara/common/csdialog.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/decorators.py` & `caracara-0.7.0/caracara/common/decorators.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/exceptions.py` & `caracara-0.7.0/caracara/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/interpolation.py` & `caracara-0.7.0/caracara/common/interpolation.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/meta.py` & `caracara-0.7.0/caracara/common/meta.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/module.py` & `caracara-0.7.0/caracara/common/module.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/pagination.py` & `caracara-0.7.0/caracara/common/pagination.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/common/policy_wrapper.py` & `caracara-0.7.0/caracara/common/policy_wrapper.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/filters/decorators.py` & `caracara-0.7.0/caracara/filters/decorators.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/__init__.py` & `caracara-0.7.0/caracara/modules/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 __all__ = [
     'CustomIoaApiModule',
     'FlightControlApiModule',
     'HostsApiModule',
     'PreventionPoliciesApiModule',
     'ResponsePoliciesApiModule',
     'RTRApiModule',
+    'SensorUpdatePoliciesApiModule',
     'UsersApiModule',
 ]
 
 from caracara.modules.custom_ioa import CustomIoaApiModule
 from caracara.modules.flight_control import FlightControlApiModule
 from caracara.modules.hosts import HostsApiModule
 from caracara.modules.prevention_policies import PreventionPoliciesApiModule
 from caracara.modules.response_policies import ResponsePoliciesApiModule
 from caracara.modules.rtr import RTRApiModule
+from caracara.modules.sensor_update_policies import SensorUpdatePoliciesApiModule
 from caracara.modules.users import UsersApiModule
```

### Comparing `caracara-0.6.1/caracara/modules/custom_ioa/custom_ioa.py` & `caracara-0.7.0/caracara/modules/custom_ioa/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/custom_ioa/rule_types.py` & `caracara-0.7.0/caracara/modules/custom_ioa/rule_types.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/custom_ioa/rules.py` & `caracara-0.7.0/caracara/modules/custom_ioa/rules.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/flight_control/flight_control.py` & `caracara-0.7.0/caracara/modules/flight_control/flight_control.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_containment.py` & `caracara-0.7.0/caracara/modules/hosts/_containment.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_data_history.py` & `caracara-0.7.0/caracara/modules/hosts/_data_history.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_groups.py` & `caracara-0.7.0/caracara/modules/hosts/_groups.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_hiding.py` & `caracara-0.7.0/caracara/modules/hosts/_hiding.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_online_state.py` & `caracara-0.7.0/caracara/modules/hosts/_online_state.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/_tagging.py` & `caracara-0.7.0/caracara/modules/hosts/_tagging.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/hosts/hosts.py` & `caracara-0.7.0/caracara/modules/hosts/hosts.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/prevention_policies/prevention_policies.py` & `caracara-0.7.0/caracara/modules/prevention_policies/prevention_policies.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/prevention_policies/template.py` & `caracara-0.7.0/caracara/modules/prevention_policies/template.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/response_policies/response_policies.py` & `caracara-0.7.0/caracara/modules/response_policies/response_policies.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/response_policies/template.py` & `caracara-0.7.0/caracara/modules/response_policies/template.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/rtr/batch_session.py` & `caracara-0.7.0/caracara/modules/rtr/batch_session.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/rtr/constants.py` & `caracara-0.7.0/caracara/modules/rtr/constants.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/rtr/get_file.py` & `caracara-0.7.0/caracara/modules/rtr/get_file.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/rtr/rtr.py` & `caracara-0.7.0/caracara/modules/rtr/rtr.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/caracara/modules/users/users.py` & `caracara-0.7.0/caracara/modules/users/users.py`

 * *Files identical despite different names*

### Comparing `caracara-0.6.1/pyproject.toml` & `caracara-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "caracara"
-version = "0.6.1"
+version = "0.7.0"
 description = "The CrowdStrike Falcon Developer Toolkit"
 authors = [ "CrowdStrike <falconpy@crowdstrike.com>" ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.2"
-py7zr = "^0.20"
+py7zr = ">=0.20,<0.22"
 crowdstrike-falconpy = "^1.4.0"
 caracara-filters = "^0.2"
 setuptools = "^69.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.7"
 coverage = "^7.4.0"
@@ -77,10 +77,12 @@
 # RTR
 clear-queued-sessions = "examples.rtr.clear_queued_sessions:clear_queued_sessions"
 describe-put-files = "examples.rtr.describe_put_files:describe_put_files"
 describe-queued-sessions = "examples.rtr.describe_queued_sessions:describe_queued_sessions"
 describe-scripts = "examples.rtr.describe_scripts:describe_scripts"
 download-event-log = "examples.rtr.download_event_log:download_event_log"
 queue-command = "examples.rtr.queue_command:queue_command"
+# Sensor Update Policies
+get-maintenance-token = "examples.sensor_update_policies.get_maintenance_token:get_maintenance_token"
 # Users
 describe-roles = "examples.users.describe_roles:describe_roles"
 describe-users = "examples.users.describe_users:describe_users"
```

### Comparing `caracara-0.6.1/PKG-INFO` & `caracara-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: caracara
-Version: 0.6.1
+Version: 0.7.0
 Summary: The CrowdStrike Falcon Developer Toolkit
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: caracara-filters (>=0.2,<0.3)
 Requires-Dist: crowdstrike-falconpy (>=1.4.0,<2.0.0)
-Requires-Dist: py7zr (>=0.20,<0.21)
+Requires-Dist: py7zr (>=0.20,<0.22)
 Requires-Dist: setuptools (>=69.0,<70.0)
 Description-Content-Type: text/markdown
 
 ![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png) [![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)<br/>
 
 # Caracara
```

