# Comparing `tmp/dexus-vault-0.2.0.tar.gz` & `tmp/dexus_vault-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexus-vault-0.2.0.tar", last modified: Thu Apr 11 17:21:58 2024, max compression
+gzip compressed data, was "dexus_vault-0.2.1.tar", last modified: Mon Apr 15 20:55:33 2024, max compression
```

## Comparing `dexus-vault-0.2.0.tar` & `dexus_vault-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/dex_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/vault_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/dexus_vault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/client_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/dexus_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.139352 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/dex_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/src/vault_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/client_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/dexus_vault/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/dexus_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 20:55:33.000000 dexus_vault-0.2.1/dexus_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:55:33.143352 dexus_vault-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-15 20:55:26.000000 dexus_vault-0.2.1/setup.py
```

### Comparing `dexus-vault-0.2.0/LICENSE` & `dexus_vault-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/PKG-INFO` & `dexus_vault-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.0
+Version: 0.2.1
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -52,16 +52,14 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
-> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
-
 ### How it works
 
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
@@ -122,27 +120,29 @@
 | DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
 | VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
 | VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
 | VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
 | VAULT_TOKEN | - | - | used to auth to Vault via token |
 | VAULT_CERT | - | - | Vault client certificate path |
 | VAULT_CERT_KEY | - | - | Vault client certificate key path |
 | VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
 | VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
 | VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
 | VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
 | VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_APPROLE_SECRET_PATH | - | - | Vault approle secret path used to gain secret created by agent |
+| VAULT_KUBERNETES_ROLE | - | - | Vault role, used for kube app |
+| VAULT_KUBERNETES_JWT_PATH | - | /var/run/secrets/kubernetes.io/serviceaccount/token | Path to jwt mounted by Vault agent |
+| VAULT_KUBERNETES_MOUNT_POINT | - | kubernetes | Mount point for role "/auth/{mount_point}/role" |
 | VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
 | VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
```

### Comparing `dexus-vault-0.2.0/README.md` & `dexus_vault-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
-> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
-
 ### How it works
 
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
@@ -94,27 +92,29 @@
 | DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
 | VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
 | VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
 | VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
 | VAULT_TOKEN | - | - | used to auth to Vault via token |
 | VAULT_CERT | - | - | Vault client certificate path |
 | VAULT_CERT_KEY | - | - | Vault client certificate key path |
 | VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
 | VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
 | VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
 | VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
 | VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_APPROLE_SECRET_PATH | - | - | Vault approle secret path used to gain secret created by agent |
+| VAULT_KUBERNETES_ROLE | - | - | Vault role, used for kube app |
+| VAULT_KUBERNETES_JWT_PATH | - | /var/run/secrets/kubernetes.io/serviceaccount/token | Path to jwt mounted by Vault agent |
+| VAULT_KUBERNETES_MOUNT_POINT | - | kubernetes | Mount point for role "/auth/{mount_point}/role" |
 | VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
 | VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
```

### Comparing `dexus-vault-0.2.0/dexus_vault/__main__.py` & `dexus_vault-0.2.1/dexus_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/client.py` & `dexus_vault-0.2.1/dexus_vault/client.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py` & `dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py` & `dexus_vault-0.2.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/src/dex_processor.py` & `dexus_vault-0.2.1/dexus_vault/src/dex_processor.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/src/vault_processor.py` & `dexus_vault-0.2.1/dexus_vault/src/vault_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sys
 import time
 import requests
+
+from hvac.api.auth_methods import Kubernetes
 import hvac
 
 from dexus_vault.utils.client_parser import normalize_config
 from dexus_vault.utils.logger import logger
 from dexus_vault.utils.metrics import vault_client_secret
 
 
@@ -60,34 +62,41 @@
     def login_to_client(self) -> object:
         """
         Define auth method for Vault and authenticate
         """
         client = hvac.Client(url=self.config["VAULT_ADDR"])
         self._check_vault_status(client)
 
-        if self.config["VAULT_APPROLE"] is not None:
+        if self.config["VAULT_APPROLE_ROLE_ID"] is not None:
             auth_method = "approle"
-            client.sys.enable_auth_method(
-                method_type=self.auth_method,
-            )
 
-            if self.config["VAULT_APPROLE_ROLE_ID"]:
+            if self.config["VAULT_APPROLE_SECRET_PATH"] is not None:
+                client.auth.approle.login_by_approle_path(
+                    role_id=self.config["VAULT_APPROLE_ROLE_ID"],
+                    secret_id=self.config["VAULT_APPROLE_SECRET_PATH"],
+                )
+            else:
                 client.auth.approle.login(
                     role_id=self.config["VAULT_APPROLE_ROLE_ID"],
                     secret_id=self.config["VAULT_APPROLE_SECRET_ID"],
                 )
 
-            elif self.config["VAULT_APPROLE_PATH"]:
-                client.sys.enable_auth_method(
-                    method_type=self.auth_method,
-                    path=self.config["VAULT_APPROLE_PATH"],
+        elif self.config["VAULT_KUBERNETES_ROLE"] is not None:
+            # POST /auth/{mount_point}/login
+            auth_method = "kubernetes"
+
+            with open(self.config["VAULT_KUBERNETES_JWT_PATH"], "r") as jwt:
+                Kubernetes(client.adapter).login(
+                    role=self.config["VAULT_KUBERNETES_ROLE"],
+                    jwt=jwt,
+                    mount_point=self.config["VAULT_KUBERNETES_MOUNT_POINT"],
                 )
 
         elif self.config["VAULT_LDAP_USERNAME"] is not None:
-            auth_method = "LDAP"
+            auth_method = "ldap"
             client.auth.ldap.login(
                 username=self.config["VAULT_LDAP_USERNAME"],
                 password=self.config["VAULT_LDAP_PASSWORD"],
             )
 
         elif self.config["VAULT_CERT"] is not None:
             auth_method = "Client cert"
@@ -99,15 +108,15 @@
             )
 
         elif self.config["VAULT_TOKEN"] is not None:
             auth_method = "Vault token"
             client.token = self.config["VAULT_TOKEN"]
 
         else:
-            raise KeyError(f"Vault auth method is not specified!")
+            raise KeyError(f"Vault auth method is not specified, or not supported")
 
         self._check_if_vault_auth(client, auth_method)
         return client
 
     def vault_list_secrets(self) -> list:
         """
         List secrets from Vault by path
```

### Comparing `dexus-vault-0.2.0/dexus_vault/utils/client_parser.py` & `dexus_vault-0.2.1/dexus_vault/utils/client_parser.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/utils/config.py` & `dexus_vault-0.2.1/dexus_vault/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,25 @@
     Get the configuration value for the given key, cast it to the specified target type,
     and return the default value if the environment variable is not set.
     """
     env_value = os.getenv(key, default)
     return check_var_type(env_value, target_type)
 
 
+def get_metrics_config() -> Dict[str, Any]:
+    """
+    Get the configuration as a dictionary, with type-checked values.
+    """
+    return {
+        "METRICS_ENABLE": _get_config_value("METRICS_ENABLE", bool, True),
+        "METRICS_PORT": _get_config_value("METRICS_PORT", int, 8000),
+        "INTERNAL_METRICS": _get_config_value("INTERNAL_METRICS", bool, False),
+    }
+
+
 def get_dex_config() -> Dict[str, Any]:
     """
     Get the configuration as a dictionary, with type-checked values.
     """
     config = {
         "CLIENT_CRT": load_file(_get_config_value("CLIENT_CRT", str)),
         "CLIENT_KEY": load_file(_get_config_value("CLIENT_KEY", str)),
@@ -27,36 +38,35 @@
         "DEX_GRPC_URL": _get_config_value("DEX_GRPC_URL", str, "127.0.0.1:5557"),
         "DEX_MAX_RETRIES": _get_config_value("DEX_MAX_RETRIES", int, 20),
         "DEX_RETRY_WAIT": _get_config_value("DEX_RETRY_WAIT", int, 3),
     }
     return config
 
 
-def get_metrics_config() -> Dict[str, Any]:
-    """
-    Get the configuration as a dictionary, with type-checked values.
-    """
-    return {
-        "METRICS_ENABLE": _get_config_value("METRICS_ENABLE", bool, True),
-        "METRICS_PORT": _get_config_value("METRICS_PORT", int, 8000),
-        "INTERNAL_METRICS": _get_config_value("INTERNAL_METRICS", bool, False),
-    }
-
-
 def get_vault_config() -> Dict[str, Any]:
     """
     Get the configuration as a dictionary, with type-checked values.
     """
     # TODO: Check if it really need assignment
     config = {
         "VAULT_ADDR": _get_config_value("VAULT_ADDR", str, "http://127.0.0.1:8200"),
-        "VAULT_APPROLE": _get_config_value("VAULT_APPROLE", str),
         "VAULT_APPROLE_ROLE_ID": _get_config_value("VAULT_APPROLE_ROLE_ID", str),
         "VAULT_APPROLE_SECRET_ID": _get_config_value("VAULT_APPROLE_SECRET_ID", str),
-        "VAULT_APPROLE_PATH": _get_config_value("VAULT_APPROLE_PATH", str),
+        "VAULT_APPROLE_SECRET_PATH": load_file(
+            _get_config_value("VAULT_APPROLE_SECRET_PATH", str)
+        ),
+        "VAULT_KUBERNETES_ROLE": _get_config_value("VAULT_KUBERNETES_ROLE", str),
+        "VAULT_KUBERNETES_JWT_PATH": _get_config_value(
+            "VAULT_KUBERNETES_JWT_PATH",
+            str,
+            "/var/run/secrets/kubernetes.io/serviceaccount/token",
+        ),
+        "VAULT_KUBERNETES_MOUNT_POINT": _get_config_value(
+            "VAULT_KUBERNETES_MOUNT_POINT", str, "kubernetes"
+        ),
         "VAULT_TOKEN": _get_config_value("VAULT_TOKEN", str),
         "VAULT_CERT": _get_config_value("VAULT_CERT", str),
         "VAULT_CERT_KEY": _get_config_value("VAULT_CERT_KEY", str),
         "VAULT_CERT_CA": _get_config_value("VAULT_CERT_CA", bool | str, False),
         "VAULT_LDAP_USERNAME": _get_config_value("VAULT_LDAP_USERNAME", str),
         "VAULT_LDAP_PASSWORD": _get_config_value("VAULT_LDAP_PASSWORD", str),
         "VAULT_REQUEST_TIMEOUT": _get_config_value("VAULT_REQUEST_TIMEOUT", int, 5),
```

### Comparing `dexus-vault-0.2.0/dexus_vault/utils/logger.py` & `dexus_vault-0.2.1/dexus_vault/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault/utils/metrics.py` & `dexus_vault-0.2.1/dexus_vault/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/dexus_vault.egg-info/PKG-INFO` & `dexus_vault-0.2.1/dexus_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.0
+Version: 0.2.1
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -52,16 +52,14 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
-> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
-
 ### How it works
 
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
@@ -122,27 +120,29 @@
 | DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
 | VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
 | VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
 | VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
 | VAULT_TOKEN | - | - | used to auth to Vault via token |
 | VAULT_CERT | - | - | Vault client certificate path |
 | VAULT_CERT_KEY | - | - | Vault client certificate key path |
 | VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
 | VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
 | VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
 | VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
 | VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_APPROLE_SECRET_PATH | - | - | Vault approle secret path used to gain secret created by agent |
+| VAULT_KUBERNETES_ROLE | - | - | Vault role, used for kube app |
+| VAULT_KUBERNETES_JWT_PATH | - | /var/run/secrets/kubernetes.io/serviceaccount/token | Path to jwt mounted by Vault agent |
+| VAULT_KUBERNETES_MOUNT_POINT | - | kubernetes | Mount point for role "/auth/{mount_point}/role" |
 | VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
 | VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
```

### Comparing `dexus-vault-0.2.0/dexus_vault.egg-info/SOURCES.txt` & `dexus_vault-0.2.1/dexus_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.2.0/setup.py` & `dexus_vault-0.2.1/setup.py`

 * *Files identical despite different names*

