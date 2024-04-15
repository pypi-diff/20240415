# Comparing `tmp/guardian_client-0.2.1.dev0.tar.gz` & `tmp/guardian_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardian_client-0.2.1.dev0.tar", max compression
+gzip compressed data, was "guardian_client-0.2.2.tar", max compression
```

## Comparing `guardian_client-0.2.1.dev0.tar` & `guardian_client-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4628 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/README.md
--rw-r--r--   0        0        0      105 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/__init__.py
--rw-r--r--   0        0        0       27 2024-04-05 21:32:32.135271 guardian_client-0.2.1.dev0/guardian_client/_version.py
--rw-r--r--   0        0        0        0 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/__init__.py
--rw-r--r--   0        0        0     5384 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/api.py
--rw-r--r--   0        0        0     4644 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/credentials.py
--rw-r--r--   0        0        0     3949 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/guardian.py
--rw-r--r--   0        0        0      757 2024-04-05 21:32:32.479273 guardian_client-0.2.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 guardian_client-0.2.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     5762 2024-04-15 18:28:28.142296 guardian_client-0.2.2/README.md
+-rw-r--r--   0        0        0      105 2024-04-15 18:28:28.142296 guardian_client-0.2.2/guardian_client/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-15 18:28:48.954415 guardian_client-0.2.2/guardian_client/_version.py
+-rw-r--r--   0        0        0        0 2024-04-15 18:28:28.142296 guardian_client-0.2.2/guardian_client/python/__init__.py
+-rw-r--r--   0        0        0     7113 2024-04-15 18:28:28.142296 guardian_client-0.2.2/guardian_client/python/api.py
+-rw-r--r--   0        0        0     4644 2024-04-15 18:28:28.142296 guardian_client-0.2.2/guardian_client/python/credentials.py
+-rw-r--r--   0        0        0     4262 2024-04-15 18:28:28.142296 guardian_client-0.2.2/guardian_client/python/guardian.py
+-rw-r--r--   0        0        0      752 2024-04-15 18:28:49.302417 guardian_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 guardian_client-0.2.2/PKG-INFO
```

### Comparing `guardian_client-0.2.1.dev0/README.md` & `guardian_client-0.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -31,50 +31,53 @@
 ## Running Your Scans
 
 That's it!. Now you should be all set to start scanning your models.
 
 ``` shell
 
 guardian-client <base_url> <model_uri> \
+       [--threshold <threshold>] \
        [--block-on-errors] \
        [--log-level <log-level>] \
        [--silent] || echo $?
 ```
 
 ### Arguments
 
 - `base_url` The API URL (required)
 
 - `model_uri` The Path where the model is stored e.g. S3 bucket (required)
 
+- `--threshold` The minimum threshold at which a model should be blocked. Take following values: low, medium, high, critical. Default is critical
+
 - `--block-on-errors` A boolean flag indicating the error in scanning should also lead to a block. These errors are only specific to model scanning.
 
 - `--log-level` Can be set to any of the following: error, info, or debug
 
 - `--silent` Disable all logging / reporting
 
 - `--report-only` Print out the scan report and skip evaluating it for blocking.
 
 - `--poll-interval-secs` The interval in seconds to wait before polling the server for scan status. Default is 5.
 
 ### Exit Codes
 The CLI returns following exit codes that can be used by the downstream applications to block a deployment.
 
-- **0** Successful scan without violating any of your organization's policies
+- **0** Successful scan without issues at or above the threshold (default is CRITICAL)
 
-- **1** Successful scan with issues violating your organization's policies
+- **1** Successful scan with issues at or above the threshold (default is CRITICAL)
 
 - **2** Scan failed for any reason
 
 ## Examples
 
-### To get a block decision for a model in S3
+### To get a block decision for model vulnerability at or higher than "MEDIUM"
 
 ``` shell
-guardian-client https://protectai.dev/guardian s3://a-bucket/path/ || echo $?
+guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --threshold MEDIUM || echo $?
 ```
 ### To only see the report from scanning the model.
 
 ```
 guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --report-only
 
 ```
@@ -96,21 +99,23 @@
 # Initiate the client
 guardian = GuardianAPIClient(base_url=base_url)
 
 # Scan the model
 response = guardian.scan(model_uri=model_uri)
 
 
-# Retrieve the pass/fail decision from Guardian
+# Evaluate the scan response against a threshold
 assert response.get("http_status_code") == 200
 assert response.get("scan_status_json") != None
-assert response.get("scan_status_json").get("aggregate_eval_outcome") != "ERROR"
+assert response.get("scan_status_json").get("status") == "FINISHED"
+
+reason, should_block = guardian.evaluate(response.get("scan_status_json"))
   
-if response.get("scan_status_json").get("aggregate_eval_outcome") == "FAIL":
-  print(f"Model {model_uri} was blocked because it failed your organization's security policies")
+if should_block:
+  print(f"Model {model_uri} was blocked with reason: {reason}")
 ```
 
 ## Reference
 
 ### Class GuardianAPIClient
 
 ``` python
@@ -151,7 +156,31 @@
       Returns:
           dict: A dictionary containing the HTTP status code and the scan status JSON.
                 If an error occurs during the scan submission or polling, the dictionary
                 will also contain the error details.
 
       """
 ```
+
+#### GuardianAPIClient.evaluate
+``` python
+  def evaluate(
+      self,
+      status_json: Dict[str, Any],
+      threshold: str = "CRITICAL",
+      block_on_scan_errors: bool = False,
+  ) -> Tuple[str, bool]:
+      """
+      Evaluates the status of a scan based on the provided status JSON.
+
+      Args:
+          status_json (object): The status JSON object containing scan information obtained from scan method.
+          threshold (str, optional): The threshold level to consider for blocking. Defaults to "CRITICAL".
+          block_on_scan_errors (bool, optional): Whether to block if there are errors in scanning. Defaults to False.
+
+      Returns:
+          Tuple[str, bool]: A tuple containing the evaluation result message and a boolean indicating if blocking is required.
+
+          Raises:
+              ValueError: If the threshold is not one of "LOW", "MEDIUM", "HIGH", or "CRITICAL".
+      """
+```
```

### Comparing `guardian_client-0.2.1.dev0/guardian_client/python/credentials.py` & `guardian_client-0.2.2/guardian_client/python/credentials.py`

 * *Files identical despite different names*

### Comparing `guardian_client-0.2.1.dev0/pyproject.toml` & `guardian_client-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guardian-client"
-version = "0.2.1.dev0"
+version = "0.2.2"
 license = "Apache License 2.0"
 description = "Python SDK for Protect AI Guardian"
 authors = ["ProtectAI <community@protectai.com>"]
 readme = "README.md"
 packages = [
     { include = "guardian_client" },
 ]
```

### Comparing `guardian_client-0.2.1.dev0/PKG-INFO` & `guardian_client-0.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardian-client
-Version: 0.2.1.dev0
+Version: 0.2.2
 Summary: Python SDK for Protect AI Guardian
 License: Apache-2.0
 Author: ProtectAI
 Author-email: community@protectai.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -49,50 +49,53 @@
 ## Running Your Scans
 
 That's it!. Now you should be all set to start scanning your models.
 
 ``` shell
 
 guardian-client <base_url> <model_uri> \
+       [--threshold <threshold>] \
        [--block-on-errors] \
        [--log-level <log-level>] \
        [--silent] || echo $?
 ```
 
 ### Arguments
 
 - `base_url` The API URL (required)
 
 - `model_uri` The Path where the model is stored e.g. S3 bucket (required)
 
+- `--threshold` The minimum threshold at which a model should be blocked. Take following values: low, medium, high, critical. Default is critical
+
 - `--block-on-errors` A boolean flag indicating the error in scanning should also lead to a block. These errors are only specific to model scanning.
 
 - `--log-level` Can be set to any of the following: error, info, or debug
 
 - `--silent` Disable all logging / reporting
 
 - `--report-only` Print out the scan report and skip evaluating it for blocking.
 
 - `--poll-interval-secs` The interval in seconds to wait before polling the server for scan status. Default is 5.
 
 ### Exit Codes
 The CLI returns following exit codes that can be used by the downstream applications to block a deployment.
 
-- **0** Successful scan without violating any of your organization's policies
+- **0** Successful scan without issues at or above the threshold (default is CRITICAL)
 
-- **1** Successful scan with issues violating your organization's policies
+- **1** Successful scan with issues at or above the threshold (default is CRITICAL)
 
 - **2** Scan failed for any reason
 
 ## Examples
 
-### To get a block decision for a model in S3
+### To get a block decision for model vulnerability at or higher than "MEDIUM"
 
 ``` shell
-guardian-client https://protectai.dev/guardian s3://a-bucket/path/ || echo $?
+guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --threshold MEDIUM || echo $?
 ```
 ### To only see the report from scanning the model.
 
 ```
 guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --report-only
 
 ```
@@ -114,21 +117,23 @@
 # Initiate the client
 guardian = GuardianAPIClient(base_url=base_url)
 
 # Scan the model
 response = guardian.scan(model_uri=model_uri)
 
 
-# Retrieve the pass/fail decision from Guardian
+# Evaluate the scan response against a threshold
 assert response.get("http_status_code") == 200
 assert response.get("scan_status_json") != None
-assert response.get("scan_status_json").get("aggregate_eval_outcome") != "ERROR"
+assert response.get("scan_status_json").get("status") == "FINISHED"
+
+reason, should_block = guardian.evaluate(response.get("scan_status_json"))
   
-if response.get("scan_status_json").get("aggregate_eval_outcome") == "FAIL":
-  print(f"Model {model_uri} was blocked because it failed your organization's security policies")
+if should_block:
+  print(f"Model {model_uri} was blocked with reason: {reason}")
 ```
 
 ## Reference
 
 ### Class GuardianAPIClient
 
 ``` python
@@ -170,7 +175,31 @@
           dict: A dictionary containing the HTTP status code and the scan status JSON.
                 If an error occurs during the scan submission or polling, the dictionary
                 will also contain the error details.
 
       """
 ```
 
+#### GuardianAPIClient.evaluate
+``` python
+  def evaluate(
+      self,
+      status_json: Dict[str, Any],
+      threshold: str = "CRITICAL",
+      block_on_scan_errors: bool = False,
+  ) -> Tuple[str, bool]:
+      """
+      Evaluates the status of a scan based on the provided status JSON.
+
+      Args:
+          status_json (object): The status JSON object containing scan information obtained from scan method.
+          threshold (str, optional): The threshold level to consider for blocking. Defaults to "CRITICAL".
+          block_on_scan_errors (bool, optional): Whether to block if there are errors in scanning. Defaults to False.
+
+      Returns:
+          Tuple[str, bool]: A tuple containing the evaluation result message and a boolean indicating if blocking is required.
+
+          Raises:
+              ValueError: If the threshold is not one of "LOW", "MEDIUM", "HIGH", or "CRITICAL".
+      """
+```
+
```

