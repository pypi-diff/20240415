# Comparing `tmp/wiliot-api-4.8.2.tar.gz` & `tmp/wiliot-api-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.8.2.tar", last modified: Wed Apr 10 06:56:06 2024, max compression
+gzip compressed data, was "wiliot-api-4.8.3.tar", last modified: Mon Apr 15 10:17:53 2024, max compression
```

## Comparing `wiliot-api-4.8.2.tar` & `wiliot-api-4.8.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    11293 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10787 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.382493 wiliot-api-4.8.2/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20618 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52463 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11293 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.622357 wiliot-api-4.8.3/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11555 2024-04-15 10:17:53.622357 wiliot-api-4.8.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11049 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-15 10:17:53.622357 wiliot-api-4.8.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20618 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23479 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52466 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.622357 wiliot-api-4.8.3/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.622357 wiliot-api-4.8.3/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-15 10:17:38.000000 wiliot-api-4.8.3/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 10:17:53.618357 wiliot-api-4.8.3/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11555 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-15 10:17:53.000000 wiliot-api-4.8.3/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.8.2/LICENSE` & `wiliot-api-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/PKG-INFO` & `wiliot-api-4.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.2
+Version: 4.8.3
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.3:
+
+* Added a function to get all key values for an entity types
+
 ### Version 4.8.2:
 
 * Fixed a bug in updating bridge configuration
 
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
@@ -234,14 +238,18 @@
 # * GATEWAY
 
 # Get a specific key:value for a zone
 platform.get_entity_keys_values(entity_type=EntityType.ZONE,
                                 entity_id="my-zone-id",
                                 key="special_zone")
 
+# Get all key values for a specific key and all bridges
+platform.get_entity_type_keys_values(entity_type=EntityType.BRIDGE,
+                                     key='autoUpdate')
+
 # Set one or more key:value pairs for one or more entities (of the same type)
 platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
                                       entity_ids=["gateway-id-1", "gateway-id-2"],
                                       keys_values={"special_gateway": "True"})
 
 # The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
 # To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
```

### Comparing `wiliot-api-4.8.2/README.md` & `wiliot-api-4.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.3:
+
+* Added a function to get all key values for an entity types
+
 ### Version 4.8.2:
 
 * Fixed a bug in updating bridge configuration
 
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
@@ -217,14 +221,18 @@
 # * GATEWAY
 
 # Get a specific key:value for a zone
 platform.get_entity_keys_values(entity_type=EntityType.ZONE,
                                 entity_id="my-zone-id",
                                 key="special_zone")
 
+# Get all key values for a specific key and all bridges
+platform.get_entity_type_keys_values(entity_type=EntityType.BRIDGE,
+                                     key='autoUpdate')
+
 # Set one or more key:value pairs for one or more entities (of the same type)
 platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
                                       entity_ids=["gateway-id-1", "gateway-id-2"],
                                       keys_values={"special_gateway": "True"})
 
 # The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
 # To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
```

### Comparing `wiliot-api-4.8.2/bitbucket-pipelines.yml` & `wiliot-api-4.8.3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/setup.py` & `wiliot-api-4.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/__init__.py` & `wiliot-api-4.8.3/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/api_client.py` & `wiliot-api-4.8.3/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/edge/edge.py` & `wiliot-api-4.8.3/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.8.3/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.8.3/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.8.3/wiliot_api/manufacturing/manufacturing.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,18 +300,19 @@
         """
         Resolve a tag's payload
         :param payload: valid Wiliot tag payload starting with the manufacturer ID
         :param owner_id: String - The ID of the owner to resolve this payload for
         :param verbose: Bool
         :return: A dictionary from the returned JSON
         """
+        allowed_roles_to_resolve = ['manufacturing', 'resolve', 'asset-creator']
         now_ts = int(datetime.datetime.now().timestamp())
         decoded_token = jwt.decode(self.auth_obj.token['access_token'], options={"verify_signature": False})
         # Make sure the roles included in the token include "manufacturing"
-        if "manufacturing" not in decoded_token['roles'] and "resolve" not in decoded_token['roles']:
+        if not any([allowed in decoded_token['roles'] for allowed in allowed_roles_to_resolve]):
             raise Exception("The provided API key is not a manufacturing API key. Please use the appropriate key")
         # Make sure that the generated token allows access to the requested owner
         if owner_id not in decoded_token['owners'].keys() and owner_id != 'wiliot_cloud-ops':
             raise Exception(f"The provided API key does not belong to the requested owner ID: {owner_id}")
         payload = {
             'timestamp': now_ts,
             'packets': [
```

### Comparing `wiliot-api-4.8.2/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.8.3/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/platform/platform.py` & `wiliot-api-4.8.3/wiliot_api/platform/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,23 +1096,23 @@
         payload = [{
             'entityId': entity_id,
             'labelIds': labels
         } for entity_id in entity_ids]
         res = self._delete(path, payload)
         return res['status_code'] == 200
 
-    def get_entity_labels(self, entity_type: EntityType, entity_id: str=None, key: str=None):
+    def get_entity_type_keys_values(self, entity_type: EntityType, entity_id: str = None, key: str = None):
         """
-        Get all labels and values either for a specific entity or for all entities of a certain type
+        Get multiple key value pairs for an entity type. Filterable by entity ID and by key
         :param entity_type: EntityType - required - the type of entity to return labels and values for
         :param entity_id: String - Optional - If provided returns only label and value pairs for the entity with the
         specified entity_id
         :param key: String - optional - filter only labels with the specified key
         """
-        if entity_type is None:
+        if entity_id is None:
             path = f"entity/{entity_type.value}/label"
         else:
             path = f"entity/{entity_type.value}/{entity_id}/label"
         params = {}
         if key is not None:
             params['key'] = key
         return self._get(path, params=params).get('data',[])
```

### Comparing `wiliot-api-4.8.2/wiliot_api/platform/platform_models.py` & `wiliot-api-4.8.3/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/security/security.py` & `wiliot-api-4.8.3/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api/utils/get_version.py` & `wiliot-api-4.8.3/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.2/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.8.3/wiliot_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.2
+Version: 4.8.3
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.3:
+
+* Added a function to get all key values for an entity types
+
 ### Version 4.8.2:
 
 * Fixed a bug in updating bridge configuration
 
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
@@ -234,14 +238,18 @@
 # * GATEWAY
 
 # Get a specific key:value for a zone
 platform.get_entity_keys_values(entity_type=EntityType.ZONE,
                                 entity_id="my-zone-id",
                                 key="special_zone")
 
+# Get all key values for a specific key and all bridges
+platform.get_entity_type_keys_values(entity_type=EntityType.BRIDGE,
+                                     key='autoUpdate')
+
 # Set one or more key:value pairs for one or more entities (of the same type)
 platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
                                       entity_ids=["gateway-id-1", "gateway-id-2"],
                                       keys_values={"special_gateway": "True"})
 
 # The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
 # To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
```

### Comparing `wiliot-api-4.8.2/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.8.3/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

