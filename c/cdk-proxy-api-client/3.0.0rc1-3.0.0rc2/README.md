# Comparing `tmp/cdk_proxy_api_client-3.0.0rc1.tar.gz` & `tmp/cdk_proxy_api_client-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-3.0.0rc1.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-3.0.0rc2.tar", max compression
```

## Comparing `cdk_proxy_api_client-3.0.0rc1.tar` & `cdk_proxy_api_client-3.0.0rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-3.0.0rc1/LICENSE
--rw-r--r--   0        0        0      222 2023-10-03 07:30:35.881560 cdk_proxy_api_client-3.0.0rc1/README.md
--rw-r--r--   0        0        0      185 2024-04-09 06:04:25.917364 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     5889 2024-04-08 16:25:03.929937 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0       93 2024-04-08 14:50:57.285009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1937 2023-10-03 07:41:27.578445 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     3012 2024-04-08 14:50:57.281009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0      426 2024-04-08 14:50:57.287009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/exceptions.py
--rw-r--r--   0        0        0     8629 2024-04-08 17:43:00.455397 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/interceptors/__init__.py
--rw-r--r--   0        0        0     1040 2024-04-08 16:25:03.927937 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/plugins/__init__.py
--rw-r--r--   0        0        0      890 2024-04-08 14:50:57.289009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0     4635 2024-04-08 21:50:09.929832 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/user_mappings/__init__.py
--rw-r--r--   0        0        0     8138 2024-04-08 22:17:53.442884 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/vclusters/__init__.py
--rw-r--r--   0        0        0     2072 2024-04-09 06:04:25.917364 cdk_proxy_api_client-3.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 cdk_proxy_api_client-3.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-3.0.0rc2/LICENSE
+-rw-r--r--   0        0        0      222 2023-10-03 07:30:35.881560 cdk_proxy_api_client-3.0.0rc2/README.md
+-rw-r--r--   0        0        0      185 2024-04-09 22:26:32.183177 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     5889 2024-04-08 16:25:03.929937 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0       93 2024-04-08 14:50:57.285009 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1937 2023-10-03 07:41:27.578445 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     3012 2024-04-08 14:50:57.281009 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0      426 2024-04-08 14:50:57.287009 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/exceptions.py
+-rw-r--r--   0        0        0     8629 2024-04-08 17:43:00.455397 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/interceptors/__init__.py
+-rw-r--r--   0        0        0     1040 2024-04-08 16:25:03.927937 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/plugins/__init__.py
+-rw-r--r--   0        0        0      890 2024-04-08 14:50:57.289009 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0     5185 2024-04-09 20:00:54.000656 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/user_mappings/__init__.py
+-rw-r--r--   0        0        0     8138 2024-04-08 22:17:53.442884 cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/vclusters/__init__.py
+-rw-r--r--   0        0        0     2066 2024-04-09 22:26:32.183177 cdk_proxy_api_client-3.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 cdk_proxy_api_client-3.0.0rc2/PKG-INFO
```

### Comparing `cdk_proxy_api_client-3.0.0rc1/LICENSE` & `cdk_proxy_api_client-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/interceptors/__init__.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/plugins/__init__.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/proxy_api.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/user_mappings/__init__.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/user_mappings/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,7 +127,19 @@
         """
         if vcluster_name:
             _path: str = f"{self.base_path}/vcluster/{vcluster_name}"
         else:
             _path: str = self.base_path
         req = self.proxy.client.get(_path)
         return req
+
+    def list_mappings_detailed(self, vcluster_name: str = None) -> list[dict]:
+        """
+        Given the list of mappings only returns the usernames, we might want the full picture
+        about the identity.
+        For each username, retrieve the whole identity.
+        """
+        usernames: list[str] = self.list_mappings(vcluster_name=vcluster_name).json()
+        identities: list[dict] = []
+        for username in usernames:
+            identities.append(self.get_user_mapping(username, vcluster_name).json())
+        return identities
```

### Comparing `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/vclusters/__init__.py` & `cdk_proxy_api_client-3.0.0rc2/cdk_proxy_api_client/vclusters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-3.0.0rc1/pyproject.toml` & `cdk_proxy_api_client-3.0.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "3.0.0-rc1"
+version = "3.0.0-rc2"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{ include = "cdk_proxy_api_client" }]
 keywords = ["conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -39,23 +39,23 @@
 pydantic = "^1.10.5"
 tbump = "^6.9.0"
 
 [tool.poetry.group.testing.dependencies]
 coverage = "^7.4.4"
 pytest = "^8.1.1"
 testcontainers = "^4.3.2"
-confluent-kafka = "^3.0.0-rc1"
+confluent-kafka = "^2.3"
 pytest-timeout = "^2.3.1"
 
 
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "3.0.0-rc1"
+current = "3.0.0-rc2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-3.0.0rc1/PKG-INFO` & `cdk_proxy_api_client-3.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-proxy-api-client
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

