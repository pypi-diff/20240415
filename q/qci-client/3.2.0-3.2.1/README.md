# Comparing `tmp/qci-client-3.2.0.tar.gz` & `tmp/qci_client-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qci-client-3.2.0.tar", last modified: Wed Apr 10 20:57:28 2024, max compression
+gzip compressed data, was "qci_client-3.2.1.tar", last modified: Mon Apr 15 14:31:03 2024, max compression
```

## Comparing `qci-client-3.2.0.tar` & `qci_client-3.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-10 20:54:33.000000 qci-client-3.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-10 20:54:33.000000 qci-client-3.2.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-10 20:54:33.000000 qci-client-3.2.0/.mega-linter.yml
--rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-10 20:54:33.000000 qci-client-3.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-10 20:54:33.000000 qci-client-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-10 20:57:28.920869 qci-client-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-10 20:54:33.000000 qci-client-3.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-10 20:54:33.000000 qci-client-3.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.916869 qci-client-3.2.0/qci_client/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/enum.py
--rw-rw-rw-   0 root         (0) root         (0)    27324 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)    13726 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/types.py
--rw-rw-rw-   0 root         (0) root         (0)    16845 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/qci_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 20:57:28.920869 qci-client-3.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9336 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    32556 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_remote_jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.319787 qci_client-3.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-15 14:27:48.000000 qci_client-3.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-15 14:27:48.000000 qci_client-3.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-15 14:27:48.000000 qci_client-3.2.1/.mega-linter.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-15 14:27:48.000000 qci_client-3.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-15 14:27:48.000000 qci_client-3.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-15 14:31:03.319787 qci_client-3.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-15 14:27:48.000000 qci_client-3.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-15 14:27:48.000000 qci_client-3.2.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/qci_client/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6253 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    27439 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    13726 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/types.py
+-rw-rw-rw-   0 root         (0) root         (0)    16845 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/qci_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 14:31:03.319787 qci_client-3.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9336 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    32560 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_remote_jobs.py
```

### Comparing `qci-client-3.2.0/.gitlab-ci.yml` & `qci_client-3.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/.mega-linter.yml` & `qci_client-3.2.1/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/LICENSE` & `qci_client-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/PKG-INFO` & `qci_client-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.2.0
+Version: 3.2.1
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `qci-client-3.2.0/README.md` & `qci_client-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/pyproject.toml` & `qci_client-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/qci_client/base.py` & `qci_client-3.2.1/qci_client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,23 +105,28 @@
     def headers_without_connection_close(self):
         """Headers with cached bearer token, but without connection closing."""
         headers = self.headers
         headers.pop("Connection", None)
 
         return headers
 
-    def _check_response_error(self, response: requests.Response) -> None:
+    @classmethod
+    def _check_response_error(cls, response: requests.Response) -> None:
         """
         Single place to update error check and message for API calls
         :param response: a response from any API call using the requests package
         """
-        if response.status_code >= 300:
-            raise AssertionError(
-                f"Error: {response.text}. Received error code {response.status_code}"
-            )
+        try:
+            # The requests package does special handling here, so build off of this.
+            response.raise_for_status()
+        except requests.HTTPError as err:
+            # Include response body in exception message to aid user understanding.
+            raise requests.HTTPError(
+                str(err) + f" with response body: {response.text}"
+            ) from err
 
     def get_bearer_token(self) -> requests.Response:
         """Request new bearer token. (Not cached here, see set_bearer_token.)"""
         payload = {"refresh_token": self.api_token}
 
         response = self.session.request(
             "POST",
```

### Comparing `qci-client-3.2.0/qci_client/data_converter.py` & `qci_client-3.2.1/qci_client/data_converter.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/qci_client/enum.py` & `qci_client-3.2.1/qci_client/enum.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/qci_client/qci_client.py` & `qci_client-3.2.1/qci_client/qci_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 json=utilities.get_post_request_body(file=file),
             )
 
             for response_future in concurrent.futures.as_completed(
                 [post_response_future], self.timeout
             ):
                 response = response_future.result()
-                response.raise_for_status()
+                self._check_response_error(response)
 
             file_id = response.json()["file_id"]
             file_part_generator = utilities.file_part_generator(
                 file=file, compress=self.compress
             )
             patch_response_futures = []
 
@@ -177,15 +177,15 @@
 
             # Due to timeout in underlying PATCH, this should not hang despite no
             # timeout.
             for response_future in concurrent.futures.as_completed(
                 patch_response_futures
             ):
                 response = response_future.result()
-                response.raise_for_status()
+                self._check_response_error(response)
 
         return {"file_id": file_id}
 
     @BaseApi.refresh_token
     def download_file(self, *, file_id: str) -> dict:
         """Download file (metadata and then parts concurrently)."""
         # Use session with maintained connection and multipart concurrency for
@@ -209,15 +209,15 @@
                 timeout=self.timeout,
             )
 
             for response_future in concurrent.futures.as_completed(
                 [get_response_future], self.timeout
             ):
                 response = response_future.result()
-                response.raise_for_status()
+                self._check_response_error(response)
 
             # File metadata is base for returned fully assembled file.
             file = {**response.json()}
 
             # Remove metadata fields that are not well-defined for fully assembled file.
             file.pop("last_accessed_rfc3339")
             file.pop("upload_date_rfc3339")
@@ -233,15 +233,15 @@
             ]
 
             # Due to timeout in underlying GET, this should not hang despite no timeout.
             for response_future in concurrent.futures.as_completed(
                 get_response_futures
             ):
                 response = response_future.result()
-                response.raise_for_status()
+                self._check_response_error(response)
 
             # Unpack in order.
             for response_future in get_response_futures:
                 file_part = response_future.result().json()
                 # Append to all array fields.
                 for file_type, file_type_config in file_part["file_config"].items():
                     if file_type not in file["file_config"]:
@@ -358,14 +358,15 @@
             job_type: one of _supported_job_types
             job_params: dict of params to be passed to job submission in "params" key
             qubo_file_id: file id from files API for uploaded qubo
             graph_file_id: file id from files API for uploaded graph
             hamiltonian_file_id: file id from files API for uploaded hamiltonian
             objective_file_id: file id from files API for uploaded objective
             constraints_file_id: file id from files API for uploaded constraints
+            polynomial_file_id: file id from files API for uploaded polynomial
             job_name: user specified name for job submission
             job_tags: user specified labels for classifying and filtering user jobs after submission
 
         Returns:
             None
         """
         # TODO: Need to add validation for job parameters
```

### Comparing `qci-client-3.2.0/qci_client/types.py` & `qci_client-3.2.1/qci_client/types.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/qci_client/utilities.py` & `qci_client-3.2.1/qci_client/utilities.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/qci_client.egg-info/PKG-INFO` & `qci_client-3.2.1/qci_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.2.0
+Version: 3.2.1
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `qci-client-3.2.0/qci_client.egg-info/SOURCES.txt` & `qci_client-3.2.1/qci_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/tests/test_data_converter.py` & `qci_client-3.2.1/tests/test_data_converter.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.2.0/tests/test_qci_client.py` & `qci_client-3.2.1/tests/test_qci_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -915,9 +915,9 @@
         self.assertEqual(
             self.qci_client.get_job_type_from_job_id(self.job_id), self.job_type
         )
 
         self.qci_client.session.request = unittest.mock.MagicMock(
             return_value=self.get_response_bad
         )
-        with self.assertRaises(AssertionError):
+        with self.assertRaises(requests.HTTPError):
             self.qci_client.get_job_type_from_job_id(self.job_id)
```

### Comparing `qci-client-3.2.0/tests/test_remote_jobs.py` & `qci_client-3.2.1/tests/test_remote_jobs.py`

 * *Files identical despite different names*

