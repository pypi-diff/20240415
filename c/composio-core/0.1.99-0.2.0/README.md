# Comparing `tmp/composio_core-0.1.99.tar.gz` & `tmp/composio_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.99.tar", last modified: Fri Apr 12 15:24:16 2024, max compression
+gzip compressed data, was "composio_core-0.2.0.tar", last modified: Mon Apr 15 09:07:38 2024, max compression
```

## Comparing `composio_core-0.1.99.tar` & `composio_core-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:16.322215 composio_core-0.1.99/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.99/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:24:16.321994 composio_core-0.1.99/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.99/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:16.319837 composio_core-0.1.99/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.99/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21879 2024-04-12 13:27:15.000000 composio_core-0.1.99/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:16.320733 composio_core-0.1.99/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.99/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7042 2024-04-12 13:36:37.000000 composio_core-0.1.99/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.99/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    19094 2024-04-12 13:26:45.000000 composio_core-0.1.99/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.1.99/composio/sdk/shared.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.99/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.99/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:16.321745 composio_core-0.1.99/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 15:24:16.000000 composio_core-0.1.99/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.1.99/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.1.99/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:24:16.322263 composio_core-0.1.99/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 15:24:05.000000 composio_core-0.1.99/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.726396 composio_core-0.2.0/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.0/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-15 09:07:38.726193 composio_core-0.2.0/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.0/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.723155 composio_core-0.2.0/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    21879 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.725077 composio_core-0.2.0/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7042 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    19363 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/shared.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3328 2024-04-15 07:39:40.000000 composio_core-0.2.0/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:38.725966 composio_core-0.2.0/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-15 09:07:38.000000 composio_core-0.2.0/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.0/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.0/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-15 09:07:38.726438 composio_core-0.2.0/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-15 09:07:06.000000 composio_core-0.2.0/setup.py
```

### Comparing `composio_core-0.1.99/PKG-INFO` & `composio_core-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.99
+Version: 0.2.0
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.99/composio/composio_cli.py` & `composio_core-0.2.0/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/composio/sdk/core.py` & `composio_core-0.2.0/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/composio/sdk/enums.py` & `composio_core-0.2.0/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/composio/sdk/sdk.py` & `composio_core-0.2.0/composio/sdk/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 
     sdk_instance: "Composio" = None
 
     def __init__(self, sdk_instance: "Composio", **data):
         super().__init__(**data)
         self.sdk_instance = sdk_instance
 
-    def save_user_access_data(self, field_inputs: dict):
+    def save_user_access_data(self, field_inputs: dict, redirect_url: str = None):
         connected_account_id = self.sdk_instance.get_connected_account(self.connectedAccountId)
         resp = self.sdk_instance.http_client.post(f"{self.sdk_instance.base_url}/v1/connectedAccounts", json={
             "integrationId": connected_account_id.integrationId,
             "data": field_inputs,
+            "redirectUri": redirect_url,
         })
         return resp.json()
 
     def wait_until_active(
         self, timeout=60
     ) -> "ConnectedAccount":  # Timeout adjusted to seconds
         if not self.sdk_instance:
@@ -172,19 +173,26 @@
     sdk_instance: "Composio" = None  # type: ignore
 
     def __init__(self, sdk_instance: "Composio", **data):
         super().__init__(**data)
         self.sdk_instance = sdk_instance
 
     def initiate_connection(
-        self, entity_id: str = None, params: dict = {}
+        self, entity_id: str = None,
+        params: dict = {},
+        redirect_url: str = None
     ) -> ConnectionRequest:
         resp = self.sdk_instance.http_client.post(
             f"{self.sdk_instance.base_url}/v1/connectedAccounts",
-            json={"integrationId": self.id, "userUuid": entity_id, "data": params},
+            json={
+                "integrationId": self.id,
+                "userUuid": entity_id,
+                "data": params,
+                "redirectUri": redirect_url
+            },
         )
         if resp.status_code == 200:
             return ConnectionRequest(self.sdk_instance, **resp.json())
 
         raise Exception("Failed to create connection")
 
     def get_required_variables(self):
@@ -496,10 +504,10 @@
                 run_object = client.beta.threads.runs.retrieve(
                     thread_id=thread_object.id,
                     run_id=run_object.id,
                 )
                 time.sleep(0.5)
         return run_object
 
-    def initiate_connection(self, app_name: Union[str, App]):
+    def initiate_connection(self, app_name: Union[str, App], redirect_url: str = None):
         integration = self.client.get_default_integration(app_name)
-        return integration.initiate_connection(entity_id=self.entity_id)
+        return integration.initiate_connection(entity_id=self.entity_id, redirect_url=redirect_url)
```

### Comparing `composio_core-0.1.99/composio/sdk/storage.py` & `composio_core-0.2.0/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/composio/sdk/utils.py` & `composio_core-0.2.0/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.0/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.99
+Version: 0.2.0
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.99/pyproject.toml` & `composio_core-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.99/setup.py` & `composio_core-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.99",
+    version="0.2.0",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

