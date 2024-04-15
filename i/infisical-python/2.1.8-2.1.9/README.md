# Comparing `tmp/infisical_python-2.1.8.tar.gz` & `tmp/infisical_python-2.1.9.tar.gz`

## Comparing `infisical_python-2.1.8.tar` & `infisical_python-2.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 infisical_python-2.1.8/local_dependencies/infisical/Cargo.toml
--rw-r--r--   0     1001      127     1702 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/access_token.rs
--rw-r--r--   0     1001      127     1951 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/mod.rs
--rw-r--r--   0     1001      127     2311 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/create_secret.rs
--rw-r--r--   0     1001      127     1907 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/delete_secret.rs
--rw-r--r--   0     1001      127     2590 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/get_secret.rs
--rw-r--r--   0     1001      127     2904 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/list_secrets.rs
--rw-r--r--   0     1001      127      111 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/mod.rs
--rw-r--r--   0     1001      127     1733 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/update_secret.rs
--rw-r--r--   0     1001      127      806 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/auth/authenticate.rs
--rw-r--r--   0     1001      127      133 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/auth/mod.rs
--rw-r--r--   0     1001      127     4966 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/cache.rs
--rw-r--r--   0     1001      127     1658 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/client/client.rs
--rw-r--r--   0     1001      127     1032 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/client/client_settings.rs
--rw-r--r--   0     1001      127       61 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/client/mod.rs
--rw-r--r--   0     1001      127     4621 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/error.rs
--rw-r--r--   0     1001      127     2935 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/helper.rs
--rw-r--r--   0     1001      127      167 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/lib.rs
--rw-r--r--   0     1001      127     1144 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/client_cryptography.rs
--rw-r--r--   0     1001      127     1894 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/client_secrets.rs
--rw-r--r--   0     1001      127      708 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
--rw-r--r--   0     1001      127     2519 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
--rw-r--r--   0     1001      127     2405 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
--rw-r--r--   0     1001      127      335 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/mod.rs
--rw-r--r--   0     1001      127       93 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/mod.rs
--rw-r--r--   0     1001      127     1365 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/create.rs
--rw-r--r--   0     1001      127     1092 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/delete.rs
--rw-r--r--   0     1001      127      985 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/get.rs
--rw-r--r--   0     1001      127      990 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/list.rs
--rw-r--r--   0     1001      127      979 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/mod.rs
--rw-r--r--   0     1001      127     1201 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/update.rs
--rw-r--r--   0     1001      127     3791 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/tests/cryptography.rs
--rw-r--r--   0     1001      127    10538 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical/tests/secrets.rs
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.1.8/local_dependencies/infisical-json/Cargo.toml
--rw-r--r--   0     1001      127     2314 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical-json/src/client.rs
--rw-r--r--   0     1001      127     1122 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical-json/src/command.rs
--rw-r--r--   0     1001      127       51 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical-json/src/lib.rs
--rw-r--r--   0     1001      127     1788 2024-02-01 21:53:53.000000 infisical_python-2.1.8/local_dependencies/infisical-json/src/response.rs
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.1.8/Cargo.toml
--rw-r--r--   0     1001      127     1053 2024-02-01 21:53:53.000000 infisical_python-2.1.8/LICENSE
--rw-r--r--   0     1001      127       43 2024-02-01 21:53:53.000000 infisical_python-2.1.8/MANIFEST.in
--rw-r--r--   0     1001      127      502 2024-02-01 21:53:53.000000 infisical_python-2.1.8/README.md
--rw-r--r--   0     1001      127      894 2024-02-01 21:53:53.000000 infisical_python-2.1.8/example.py
--rw-r--r--   0     1001      127      866 2024-02-01 21:53:58.000000 infisical_python-2.1.8/infisical_client/__init__.py
--rw-r--r--   0     1001      127     3643 2024-02-01 21:53:53.000000 infisical_python-2.1.8/infisical_client/infisical_client.py
--rw-r--r--   0     1001      127     2123 2024-02-01 21:53:57.000000 infisical_python-2.1.8/pyproject.toml
--rw-r--r--   0     1001      127      938 2024-02-01 21:53:53.000000 infisical_python-2.1.8/src/client.rs
--rw-r--r--   0     1001      127      104 2024-02-01 21:53:53.000000 infisical_python-2.1.8/src/lib.rs
--rw-r--r--   0     1001      127      189 2024-02-01 21:53:53.000000 infisical_python-2.1.8/src/python_module.rs
--rw-r--r--   0        0        0    62986 2024-02-01 21:54:46.000000 infisical_python-2.1.8/Cargo.lock
--rw-r--r--   0     1001      127    40201 2024-02-01 21:53:59.000000 infisical_python-2.1.8/infisical_client/schemas.py
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.1.9/local_dependencies/infisical-json/Cargo.toml
+-rw-r--r--   0     1001      127     2314 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/client.rs
+-rw-r--r--   0     1001      127     1122 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/command.rs
+-rw-r--r--   0     1001      127       51 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/lib.rs
+-rw-r--r--   0     1001      127     1788 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/response.rs
+-rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 infisical_python-2.1.9/local_dependencies/infisical/Cargo.toml
+-rw-r--r--   0     1001      127     1625 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/access_token.rs
+-rw-r--r--   0     1001      127     1951 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/mod.rs
+-rw-r--r--   0     1001      127     2311 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/create_secret.rs
+-rw-r--r--   0     1001      127     1907 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/delete_secret.rs
+-rw-r--r--   0     1001      127     2590 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/get_secret.rs
+-rw-r--r--   0     1001      127     2904 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/list_secrets.rs
+-rw-r--r--   0     1001      127      111 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/mod.rs
+-rw-r--r--   0     1001      127     1733 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/update_secret.rs
+-rw-r--r--   0     1001      127      806 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/auth/authenticate.rs
+-rw-r--r--   0     1001      127      133 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/auth/mod.rs
+-rw-r--r--   0     1001      127     4966 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/cache.rs
+-rw-r--r--   0     1001      127     1658 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/client.rs
+-rw-r--r--   0     1001      127     1032 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/client_settings.rs
+-rw-r--r--   0     1001      127       61 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/mod.rs
+-rw-r--r--   0     1001      127     4621 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/error.rs
+-rw-r--r--   0     1001      127     2935 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/helper.rs
+-rw-r--r--   0     1001      127      167 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/lib.rs
+-rw-r--r--   0     1001      127     1144 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_cryptography.rs
+-rw-r--r--   0     1001      127     1894 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_secrets.rs
+-rw-r--r--   0     1001      127      708 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
+-rw-r--r--   0     1001      127     2519 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
+-rw-r--r--   0     1001      127     2405 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
+-rw-r--r--   0     1001      127      335 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/mod.rs
+-rw-r--r--   0     1001      127       93 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/mod.rs
+-rw-r--r--   0     1001      127     1365 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/create.rs
+-rw-r--r--   0     1001      127     1092 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/delete.rs
+-rw-r--r--   0     1001      127      985 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/get.rs
+-rw-r--r--   0     1001      127      990 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/list.rs
+-rw-r--r--   0     1001      127      979 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/mod.rs
+-rw-r--r--   0     1001      127     1201 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/update.rs
+-rw-r--r--   0     1001      127     3791 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/tests/cryptography.rs
+-rw-r--r--   0     1001      127    10538 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/tests/secrets.rs
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.1.9/Cargo.toml
+-rw-r--r--   0     1001      127     1053 2024-04-15 11:50:35.000000 infisical_python-2.1.9/LICENSE
+-rw-r--r--   0     1001      127       43 2024-04-15 11:50:35.000000 infisical_python-2.1.9/MANIFEST.in
+-rw-r--r--   0     1001      127      502 2024-04-15 11:50:35.000000 infisical_python-2.1.9/README.md
+-rw-r--r--   0     1001      127      894 2024-04-15 11:50:35.000000 infisical_python-2.1.9/example.py
+-rw-r--r--   0     1001      127      866 2024-04-15 11:50:44.000000 infisical_python-2.1.9/infisical_client/__init__.py
+-rw-r--r--   0     1001      127     3643 2024-04-15 11:50:35.000000 infisical_python-2.1.9/infisical_client/infisical_client.py
+-rw-r--r--   0     1001      127     2123 2024-04-15 11:50:44.000000 infisical_python-2.1.9/pyproject.toml
+-rw-r--r--   0     1001      127      938 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/client.rs
+-rw-r--r--   0     1001      127      104 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/lib.rs
+-rw-r--r--   0     1001      127      189 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/python_module.rs
+-rw-r--r--   0        0        0    62705 2024-04-15 11:51:30.000000 infisical_python-2.1.9/Cargo.lock
+-rw-r--r--   0     1001      127    40201 2024-04-15 11:50:45.000000 infisical_python-2.1.9/infisical_client/schemas.py
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.1.9/PKG-INFO
```

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/Cargo.toml` & `infisical_python-2.1.9/local_dependencies/infisical/Cargo.toml`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/access_token.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/access_token.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 use crate::{
     error::{api_error_handler, Result},
     Client,
 };
 use log::debug;
-use reqwest::StatusCode;
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 
 #[derive(Serialize, Deserialize, Debug, JsonSchema)]
 #[serde(rename_all = "camelCase")]
 pub struct AccessTokenSuccessResponse {
     pub access_token: String,
 }
 
 pub async fn access_token_request(client: &mut Client) -> Result<AccessTokenSuccessResponse> {
     let mut body = HashMap::new();
     body.insert(
         "clientId",
-        client.auth.client_id.clone().to_string().to_owned(),
+        client.auth.client_id.clone(),
     );
     body.insert(
         "clientSecret",
-        client.auth.client_secret.clone().to_string().to_owned(),
+        client.auth.client_secret.clone(),
     );
 
     let object = serde_json::to_string(&body).unwrap();
 
     let url = format!(
         "{}/api/v1/auth/universal-auth/login",
         client.site_url.clone()
@@ -45,16 +44,15 @@
 
     let response = request.body(object).send().await?;
 
     debug!("access_token_request status: {}", response.status());
 
     let status = response.status();
 
-    if status == StatusCode::OK {
+    if status.is_success() {
         let response = response.json::<AccessTokenSuccessResponse>().await?;
-
         Ok(response)
     } else {
         let err = api_error_handler(status, response, None, true).await?;
         Err(err)
     }
 }
```

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/mod.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/mod.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/create_secret.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/create_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/delete_secret.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/delete_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/get_secret.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/get_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/list_secrets.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/list_secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/api/secrets/update_secret.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/update_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/auth/authenticate.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/auth/authenticate.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/cache.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/cache.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/client/client.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/client/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/client/client_settings.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/client/client_settings.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/error.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/error.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/helper.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/helper.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/client_cryptography.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_cryptography.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/client_secrets.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/create.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/create.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/delete.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/delete.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/get.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/get.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/list.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/list.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/mod.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/mod.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/src/manager/secrets/update.rs` & `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/update.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/tests/cryptography.rs` & `infisical_python-2.1.9/local_dependencies/infisical/tests/cryptography.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical/tests/secrets.rs` & `infisical_python-2.1.9/local_dependencies/infisical/tests/secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical-json/src/client.rs` & `infisical_python-2.1.9/local_dependencies/infisical-json/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical-json/src/command.rs` & `infisical_python-2.1.9/local_dependencies/infisical-json/src/command.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/local_dependencies/infisical-json/src/response.rs` & `infisical_python-2.1.9/local_dependencies/infisical-json/src/response.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/Cargo.toml` & `infisical_python-2.1.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "infisical-py"
-version = "2.1.8"
+version = "2.1.9"
 edition = "2021"
 rust-version = "1.57"
 
 [lib]
 name = "infisical_py"
 crate-type = ["cdylib"]
```

### Comparing `infisical_python-2.1.8/LICENSE` & `infisical_python-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/example.py` & `infisical_python-2.1.9/example.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/infisical_client/__init__.py` & `infisical_python-2.1.9/infisical_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 
 from .infisical_client import InfisicalClient as InfisicalClient
 
 from .infisical_py import InfisicalClient as RustInfisicalClient
 
 from .schemas import GetSecretOptions as GetSecretOptions
 from .schemas import UpdateSecretOptions as UpdateSecretOptions
```

### Comparing `infisical_python-2.1.8/infisical_client/infisical_client.py` & `infisical_python-2.1.9/infisical_client/infisical_client.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/pyproject.toml` & `infisical_python-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [tool.poetry]
 name = "infisical-python"
-version = "2.1.8"
+version = "2.1.9"
 description = 'Official Infisical SDK for Python (New)'
 authors = ["Daniel Hougaard <daniel@infisical.com>"]
 
 [tool.poetry_bumpversion.file."infisical_client/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
```

### Comparing `infisical_python-2.1.8/src/client.rs` & `infisical_python-2.1.9/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/Cargo.lock` & `infisical_python-2.1.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 dependencies = [
  "crypto-common",
  "generic-array",
 ]
 
 [[package]]
 name = "aes"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1f845298e95f983ff1944b728ae08b8cebab80d684f0a832ed0fc74dfa27e2"
+checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
@@ -50,26 +50,26 @@
  "ctr",
  "ghash",
  "subtle",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "argon2"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c3610892ee6e0cbce8ae2700349fcf8f98adb0dbfbee85aec3c9179d29cc072"
 dependencies = [
@@ -94,23 +94,23 @@
  "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -133,17 +133,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
@@ -166,47 +166,44 @@
 checksum = "a8894febbff9f758034a5b8e12d87918f56dfc64a8e1fe757d65e29041538d93"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cbc"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
 
@@ -214,17 +211,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.33"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f13690e35a5e4ace198e7beea2895d29f3a9cc55015fcebe6336bd2010af9eb"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "cipher"
@@ -234,17 +231,17 @@
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "combine"
-version = "4.6.6"
+version = "4.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
+checksum = "ba5a308b75df32fe02788e748662718f03fde005016435c444eea572398219fd"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "console_error_panic_hook"
@@ -316,20 +313,20 @@
  "generic-array",
  "rand_core",
  "typenum",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30d2b3721e861707777e3195b0158f950ae6dc4a27e4d02ff9f67e3eb3de199e"
+checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
 dependencies = [
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "ctr"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
@@ -348,17 +345,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "der"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fffa369a668c8af7dbf8b5e56c9f744fbd399949ed171606040001947de40b1c"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
@@ -377,29 +374,29 @@
 name = "dotenv"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77c90badedccf4105eca100756a0b1289e191f6fcbdadd3cee1d2f614f97da8f"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.9.3"
@@ -429,24 +426,14 @@
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
-dependencies = [
- "libc",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
@@ -509,15 +496,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -554,54 +541,54 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghash"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d930750de5717d2dd0b8c0d42c076c0e884c81a73e6cab859bbd2339c71e3e40"
+checksum = "f0d8a4362ccb29cb0b265253fb0a2728f592895ee6854fd9bc13f2ffda266ff1"
 dependencies = [
  "opaque-debug",
  "polyval",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 2.2.2",
+ "indexmap 2.2.6",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -629,17 +616,17 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.4"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hkdf"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5f8eb2ad728638ea2c7d47a21db23b7b58a72ed6a38256b8a1849f15fbbdf7"
 dependencies = [
@@ -653,17 +640,17 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -752,27 +739,27 @@
  "autocfg",
  "hashbrown 0.12.3",
  "serde",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "824b2ae422412366ba479e8111fd301f7b5faece8149317bb81925979a53f520"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "infisical"
 version = "0.1.0"
 dependencies = [
  "aes",
  "aes-gcm",
@@ -841,15 +828,15 @@
  "napi",
  "napi-build",
  "napi-derive",
 ]
 
 [[package]]
 name = "infisical-py"
-version = "2.1.8"
+version = "2.1.9"
 dependencies = [
  "env_logger 0.9.3",
  "infisical-json",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config",
@@ -885,37 +872,37 @@
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.10"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bad00257d07be169d870ab665980b06cdb366d792ad690bf2e76876dc503455"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "hermit-abi 0.3.4",
- "rustix",
+ "hermit-abi 0.3.9",
+ "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jni"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6df18c2e3db7e453d3c6ac5b3e9d5182664d28788126d39b91f2d1e22b017ec"
 dependencies = [
@@ -955,145 +942,139 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
-name = "linux-raw-sys"
-version = "0.4.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
-
-[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "napi"
-version = "2.15.1"
+version = "2.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43792514b0c95c5beec42996da0c1b39265b02b75c97baa82d163d3ef55cbfa7"
+checksum = "70d04890ef4ec001fad791be785b8b920e2a3f5a6b1188e7a81dfa6197c0dee4"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "napi-build"
-version = "2.1.0"
+version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4b4532cf86bfef556348ac65e561e3123879f0e7566cca6d43a6ff5326f13df"
+checksum = "e1c0f5d67ee408a4685b61f5ab7e58605c8ae3f2b4189f0127d804ff13d5560a"
 
 [[package]]
 name = "napi-derive"
-version = "2.15.0"
+version = "2.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7622f0dbe0968af2dacdd64870eee6dee94f93c989c841f1ad8f300cf1abd514"
+checksum = "aff4a63f26a7aa9fa25df6ea36675890115972b207ae516e86bd0c47e31eba39"
 dependencies = [
  "cfg-if",
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.59"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ec514d65fce18a959be55e7f683ac89c6cb850fb59b09e25ab777fd5a4a8d9e"
+checksum = "e5e76afe642e2424ebe465406e328e4316d82af1f79256231d4b0f184c67550a"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "napi-sys"
-version = "2.3.0"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2503fa6af34dc83fb74888df8b22afe933b58d37daf7d80424b1c60c68196b8b"
+checksum = "427802e8ec3a734331fec1035594a210ce1ff4dc5bc1950530920ab717964ea3"
 dependencies = [
  "libloading",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.4"
@@ -1120,50 +1101,49 @@
  "rand",
  "smallvec",
  "zeroize",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.43"
+version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.3.4",
+ "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1176,17 +1156,17 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "opaque-debug"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
+checksum = "c08d65885ee38876c4f86fa503fb49d7b507c2b62552df7c70b2fce627e06381"
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
@@ -1246,17 +1226,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1279,50 +1259,57 @@
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "polyval"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52cff9d1d4dee5fe6d03729099f4a310a41179e0a10dbf542039873f2e826fb"
+checksum = "9d1fe60d06143b2430aa532c94cfe9e29783047f06c0d7fd359a9a51b729fa25"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "opaque-debug",
  "universal-hash",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
@@ -1348,61 +1335,62 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1440,46 +1428,46 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.11.24"
+version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
+checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -1509,24 +1497,25 @@
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "ring"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "688c63d65483050968b2a8937f7995f443e27041a0f7700aa59b0822aedebb74"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
+ "cfg-if",
  "getrandom",
  "libc",
  "spin 0.9.8",
  "untrusted",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rsa"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d0e5124fcb30e76a7e79bfee683a2746db83784b86289f6251b54b7950a0dfc"
@@ -1548,27 +1537,14 @@
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
-name = "rustix"
-version = "0.38.31"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
-dependencies = [
- "bitflags 2.4.2",
- "errno",
- "libc",
- "linux-raw-sys",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "rustls"
 version = "0.21.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
 dependencies = [
  "log",
  "ring",
@@ -1632,17 +1608,17 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1717,31 +1693,31 @@
  "itertools",
  "schemars",
  "serde_json",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "num-bigint",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "seeded-random"
@@ -1752,36 +1728,36 @@
  "parking_lot",
  "rand",
  "rand_chacha",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.21"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -1789,17 +1765,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1811,21 +1787,21 @@
  "percent-encoding",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -1854,15 +1830,15 @@
 name = "serial_test_derive"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "sha1"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
@@ -1909,26 +1885,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
@@ -1964,17 +1940,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2002,45 +1978,45 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -2052,17 +2028,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.35.1"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c89b4efa943be685f629b149f53829423f8f5531ea21249408e8e2f8671ec104"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -2077,15 +2053,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -2155,26 +2131,26 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
@@ -2203,32 +2179,32 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
@@ -2264,15 +2240,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2298,15 +2274,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.59",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2345,17 +2321,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.25.3"
+version = "0.25.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1778a42e8b3b90bff8d0f5032bf22250792889a5cdc752aa0020c84abe3aaf10"
+checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -2395,15 +2371,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2415,110 +2391,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
```

### Comparing `infisical_python-2.1.8/infisical_client/schemas.py` & `infisical_python-2.1.9/infisical_client/schemas.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.8/PKG-INFO` & `infisical_python-2.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infisical-python
-Version: 2.1.8
+Version: 2.1.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Official Infisical SDK for Python (New)
 Maintainer-email: Daniel Hougaard <daniel@infisical.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source, https://github.com/infisical/sdk
 Project-URL: Documentation, https://github.com/Infisical/sdk/tree/main/crates/infisical-py#readme
 Project-URL: Issues, https://github.com/infisical/sdk/issues
+Project-URL: Source, https://github.com/infisical/sdk
 
 <h1 align="center">
     <a href="https://github.com/Infisical/infisical">
         <img width="300" src="https://raw.githubusercontent.com/Infisical/infisical-node/main/img/logoname-white.svg#gh-dark-mode-only" alt="infisical">
     </a>
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: infisical-python Version: 2.1.8 Classifier:
+Metadata-Version: 2.1 Name: infisical-python Version: 2.1.9 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -11,16 +11,16 @@
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy License-File: LICENSE Summary: Official Infisical SDK
 for Python (New) Maintainer-email: Daniel Hougaard
 infisical.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Source, https://github.com/infisical/
-sdk Project-URL: Documentation, https://github.com/Infisical/sdk/tree/main/
-crates/infisical-py#readme Project-URL: Issues, https://github.com/infisical/
-sdk/issues
+charset=UTF-8; variant=GFM Project-URL: Documentation, https://github.com/
+Infisical/sdk/tree/main/crates/infisical-py#readme Project-URL: Issues, https:/
+/github.com/infisical/sdk/issues Project-URL: Source, https://github.com/
+infisical/sdk
                            ************ _[[_ii_nn_ff_ii_ss_ii_cc_aa_ll_]] ************
   Open-source, end-to-end encrypted tool to manage secrets and configs across
                          your team and infrastructure.
 # Documentation [You can find the documentation here](https://infisical.com/
 docs/sdks/languages/python)
```

