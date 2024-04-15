# Comparing `tmp/vantage6-algorithm-tools-4.3.4rc3.tar.gz` & `tmp/vantage6-algorithm-tools-4.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-tools-4.3.4rc3.tar", last modified: Mon Mar 25 11:01:59 2024, max compression
+gzip compressed data, was "vantage6-algorithm-tools-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:18 2024, max compression
```

## Comparing `vantage6-algorithm-tools-4.3.4rc3.tar` & `vantage6-algorithm-tools-4.4.0rc3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/
--rw-r--r--   0 runner    (1001) docker     (127)    23645 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.671503 vantage6-algorithm-tools-4.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-15 13:15:18.671503 vantage6-algorithm-tools-4.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:18.671503 vantage6-algorithm-tools-4.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    23881 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/preprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-15 13:15:06.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:18.667503 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-15 13:15:18.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 13:15:18.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:18.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 13:15:18.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 13:15:18.000000 vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/PKG-INFO` & `vantage6-algorithm-tools-4.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.4.0rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/setup.py` & `vantage6-algorithm-tools-4.4.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/tests/test_docker_wrapper.py` & `vantage6-algorithm-tools-4.4.0rc3/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/tests/test_serialization.py` & `vantage6-algorithm-tools-4.4.0rc3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/__init__.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,17 +254,21 @@
             response = self.parent.request(f"result/{id_}")
 
             # Encryption is not done at the client level for the container. The
             # algorithm developer is responsible for decrypting the results.
             self.parent.log.info("--> Attempting to decode results!")
             result = None
             if response.get("result"):
-                result = json_lib.loads(
-                    base64s_to_bytes(response.get("result")).decode()
-                )
+                try:
+                    result = json_lib.loads(
+                        base64s_to_bytes(response.get("result")).decode()
+                    )
+                except Exception as e:
+                    self.parent.log.error("Unable to load results")
+                    self.parent.log.debug(e)
             return result
 
         def from_task(self, task_id: int) -> list[Any]:
             """
             Obtain results from a specific task at the server.
 
             Containers are allowed to obtain the results of their children
@@ -368,26 +372,29 @@
             # serializing input. Note that the input is not encrypted here, but
             # in the proxy server (self.parent.request())
             serialized_input = bytes_to_base64s(serialize(input_))
             organization_json_list = []
             for org_id in organizations:
                 organization_json_list.append({"id": org_id, "input": serialized_input})
 
+            json_body = {
+                "name": name,
+                "image": self.parent.image,
+                "collaboration_id": self.parent.collaboration_id,
+                "description": description,
+                "organizations": organization_json_list,
+                "databases": self.parent.databases,
+            }
+            if self.parent.study_id:
+                json_body["study_id"] = self.parent.study_id
+
             return self.parent.request(
                 "task",
                 method="post",
-                json={
-                    "name": name,
-                    "image": self.parent.image,
-                    "collaboration_id": self.parent.collaboration_id,
-                    "study_id": self.parent.study_id,
-                    "description": description,
-                    "organizations": organization_json_list,
-                    "databases": self.parent.databases,
-                },
+                json=json_body,
             )
 
     class VPN(ClientBase.SubClient):
         """
         A VPN client for the algorithm container.
 
         It provides functions to obtain the IP addresses of other containers.
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/_version.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/client/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 3, 4, "candidate", __build__, 0)
+version_info = (4, 4, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/decorators.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import wraps
 from dataclasses import dataclass
 
 import pandas as pd
 
 from vantage6.algorithm.client import AlgorithmClient
 from vantage6.algorithm.tools.mock_client import MockAlgorithmClient
-from vantage6.algorithm.tools.util import info, error, warn, get_env_var
+from vantage6.algorithm.tools.util import info, error, warn
 from vantage6.algorithm.tools.wrappers import load_data
 from vantage6.algorithm.tools.preprocessing import preprocess_data
 
 OHDSI_AVAILABLE = True
 try:
     from ohdsi.database_connector import connect as connect_to_omop
 except ImportError:
@@ -89,20 +89,20 @@
             ----------
             mock_client : MockAlgorithmClient
                 Mock client to use instead of the regular client
             """
             if mock_client is not None:
                 return func(mock_client, *args, **kwargs)
             # read server address from the environment
-            host = get_env_var("HOST")
-            port = get_env_var("PORT")
-            api_path = get_env_var("API_PATH")
+            host = os.environ["HOST"]
+            port = os.environ["PORT"]
+            api_path = os.environ["API_PATH"]
 
             # read token from the environment
-            token_file = get_env_var("TOKEN_FILE")
+            token_file = os.environ["TOKEN_FILE"]
             info("Reading token")
             with open(token_file) as fp:
                 token = fp.read().strip()
 
             client = AlgorithmClient(token=token, host=host, port=port, path=api_path)
             return func(client, *args, **kwargs)
 
@@ -191,15 +191,15 @@
                 label = labels[i]
                 # read the data from the database
                 info("Reading data from database")
                 data_ = _get_data_from_label(label)
 
                 # do any data preprocessing here
                 info(f"Applying preprocessing for database '{label}'")
-                env_prepro = get_env_var(f"{label.upper()}_PREPROCESSING")
+                env_prepro = os.environ.get(f"{label.upper()}_PREPROCESSING")
                 if env_prepro is not None:
                     preprocess = json.loads(env_prepro)
                     data_ = preprocess_data(data_, preprocess)
 
                 # add the data to the arguments
                 args = (data_, *args)
 
@@ -305,31 +305,31 @@
 
         Example
         -------
         >>> @metadata
         >>> def my_algorithm(metadata: RunMetaData, <other arguments>):
         >>>     pass
         """
-        token_file = get_env_var("TOKEN_FILE")
+        token_file = os.environ["TOKEN_FILE"]
         info("Reading token")
         with open(token_file) as fp:
             token = fp.read().strip()
 
         info("Extracting payload from token")
         payload = _extract_token_payload(token)
 
         metadata = RunMetaData(
             task_id=payload["task_id"],
             node_id=payload["node_id"],
             collaboration_id=payload["collaboration_id"],
             organization_id=payload["organization_id"],
-            temporary_directory=Path(get_env_var("TEMPORARY_FOLDER")),
-            output_file=Path(get_env_var("OUTPUT_FILE")),
-            input_file=Path(get_env_var("INPUT_FILE")),
-            token_file=Path(get_env_var("TOKEN_FILE")),
+            temporary_directory=Path(os.environ["TEMPORARY_FOLDER"]),
+            output_file=Path(os.environ["OUTPUT_FILE"]),
+            input_file=Path(os.environ["INPUT_FILE"]),
+            token_file=Path(os.environ["TOKEN_FILE"]),
         )
         return func(metadata, *args, **kwargs)
 
     return decorator
 
 
 def get_ohdsi_metadata(label: str) -> OHDSIMetaData:
@@ -351,19 +351,19 @@
     """
     # check that all node environment variables are set
     expected_env_vars = ["CDM_DATABASE", "CDM_SCHEMA", "RESULTS_SCHEMA"]
     label_ = label.upper()
     for var in expected_env_vars:
         _check_environment_var_exists_or_exit(f"{label_}_DB_PARAM_{var}")
 
-    tmp = Path(get_env_var("TEMPORARY_FOLDER"))
+    tmp = Path(os.environ["TEMPORARY_FOLDER"])
     metadata = OHDSIMetaData(
-        database=get_env_var(f"{label_}_DB_PARAM_CDM_DATABASE"),
-        cdm_schema=get_env_var(f"{label_}_DB_PARAM_CDM_SCHEMA"),
-        results_schema=get_env_var(f"{label_}_DB_PARAM_RESULTS_SCHEMA"),
+        database=os.environ[f"{label_}_DB_PARAM_CDM_DATABASE"],
+        cdm_schema=os.environ[f"{label_}_DB_PARAM_CDM_SCHEMA"],
+        results_schema=os.environ[f"{label_}_DB_PARAM_RESULTS_SCHEMA"],
         incremental_folder=tmp / "incremental",
         cohort_statistics_folder=tmp / "cohort_statistics",
         export_folder=tmp / "export",
     )
     return metadata
 
 
@@ -413,18 +413,18 @@
     label_ = label.upper()
 
     # check that the required environment variables are set
     for var in ("DBMS", "USER", "PASSWORD"):
         _check_environment_var_exists_or_exit(f"{label_}_DB_PARAM_{var}")
 
     info("Reading OHDSI environment variables")
-    dbms = get_env_var(f"{label_}_DB_PARAM_DBMS")
-    uri = get_env_var(f"{label_}_DATABASE_URI")
-    user = get_env_var(f"{label_}_DB_PARAM_USER")
-    password = get_env_var(f"{label_}_DB_PARAM_PASSWORD")
+    dbms = os.environ[f"{label_}_DB_PARAM_DBMS"]
+    uri = os.environ[f"{label_}_DATABASE_URI"]
+    user = os.environ[f"{label_}_DB_PARAM_USER"]
+    password = os.environ[f"{label_}_DB_PARAM_PASSWORD"]
     info(f" - dbms: {dbms}")
     info(f" - uri: {uri}")
     info(f" - user: {user}")
 
     info("Creating OHDSI database connection")
     return connect_to_omop(
         dbms=dbms, connection_string=uri, password=password, user=user
@@ -456,43 +456,43 @@
 
     Returns
     -------
     pd.DataFrame
         Data from the database
     """
     # Load the input data from the input file - this may e.g. include the
-    database_uri = get_env_var(f"{label.upper()}_DATABASE_URI")
+    database_uri = os.environ[f"{label.upper()}_DATABASE_URI"]
     info(f"Using '{database_uri}' with label '{label}' as database")
 
     # Get the database type from the environment variable, this variable is
     # set by the vantage6 node based on its configuration file.
-    database_type = get_env_var(f"{label.upper()}_DATABASE_TYPE", "csv").lower()
+    database_type = os.environ.get(f"{label.upper()}_DATABASE_TYPE", "csv").lower()
 
     # Load the data based on the database type. Try to provide environment
     # variables that should be available for some data types.
     return load_data(
         database_uri,
         database_type,
-        query=get_env_var(f"{label.upper()}_QUERY"),
-        sheet_name=get_env_var(f"{label.upper()}_SHEET_NAME"),
+        query=os.environ.get(f"{label.upper()}_QUERY"),
+        sheet_name=os.environ.get(f"{label.upper()}_SHEET_NAME"),
     )
 
 
 def _get_user_database_labels() -> list[str]:
     """
     Get the database labels from the environment
 
     Returns
     -------
     list[str]
         List of database labels
     """
     # read the labels that the user requested, which is a comma
     # separated list of labels.
-    labels = get_env_var("USER_REQUESTED_DATABASE_LABELS")
+    labels = os.environ["USER_REQUESTED_DATABASE_LABELS"]
     return labels.split(",")
 
 
 def _extract_token_payload(token: str) -> dict:
     """
     Extract the payload from the token.
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/mock_client.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/mock_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/__init__.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/functions.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/preprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/util.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sys
 import os
 import base64
+import binascii
+
 from vantage6.common.globals import STRING_ENCODING, ENV_VAR_EQUALS_REPLACEMENT
 
 
 def info(msg: str) -> None:
     """
     Print an info message to stdout.
 
@@ -36,14 +38,17 @@
     ----------
     msg : str
         Error message to be printed
     """
     sys.stdout.write(f"error > {msg}\n")
 
 
+# TODO v5+ move this function to wrap.py and no longer expose it to be used by
+# algorithms but as part of _decode_env_vars. It is kept here for backwards
+# compatibility with 4.2/4.3 algorithms
 def get_env_var(var_name: str, default: str | None = None) -> str:
     """
     Get the value of an environment variable. Environment variables are encoded
     by the node so they need to be decoded here.
 
     Note that this decoding follows the reverse of the encoding in the node:
     first replace '=' back and then decode the base32 string.
@@ -65,7 +70,10 @@
             os.environ[var_name]
             .replace(ENV_VAR_EQUALS_REPLACEMENT, "=")
             .encode(STRING_ENCODING)
         )
         return base64.b32decode(encoded_env_var_value).decode(STRING_ENCODING)
     except KeyError:
         return default
+    except binascii.Error:
+        # If the decoding fails, return the original value
+        return os.environ[var_name]
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrap.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/wrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import traceback
 
 from typing import Any
 
 from vantage6.common.client import deserialization
 from vantage6.common import serialization
 from vantage6.algorithm.tools.util import info, error, get_env_var
-from vantage6.algorithm.tools.exceptions import DeserializationException
+from vantage6.algorithm.tools.exceptions import DeserializationError
 
 
 def wrap_algorithm(log_traceback: bool = True) -> None:
     """
     Wrap an algorithm module to provide input and output handling for the
     vantage6 infrastructure.
 
@@ -48,26 +48,29 @@
         error(
             "No PKG_NAME specified! Make sure that the PKG_NAME environment "
             "variable is specified in the Dockerfile. Exiting..."
         )
         exit(1)
     info(f"wrapper for {module}")
 
+    # Decode environment variables that are encoded by the node.
+    _decode_env_vars()
+
     # read input from the mounted input file.
-    input_file = get_env_var("INPUT_FILE")
+    input_file = os.environ["INPUT_FILE"]
     info(f"Reading input file {input_file}")
     input_data = load_input(input_file)
 
     # make the actual call to the method/function
     info("Dispatching ...")
     output = _run_algorithm_method(input_data, module, log_traceback)
 
     # write output from the method to mounted output file. Which will be
     # transferred back to the server by the node-instance.
-    output_file = get_env_var("OUTPUT_FILE")
+    output_file = os.environ["OUTPUT_FILE"]
     info(f"Writing output to {output_file}")
 
     _write_output(output, output_file)
 
 
 def _run_algorithm_method(
     input_data: dict, module: str, log_traceback: bool = True
@@ -141,22 +144,22 @@
     Returns
     -------
     input_data : Any
         Input data for the algorithm
 
     Raises
     ------
-    DeserializationException
+    DeserializationError
         Failed to deserialize input data
     """
     with open(input_file, "rb") as fp:
         try:
             input_data = deserialization.deserialize(fp)
-        except DeserializationException:
-            raise DeserializationException("Could not deserialize input")
+        except DeserializationError:
+            raise DeserializationError("Could not deserialize input")
     return input_data
 
 
 def _write_output(output: Any, output_file: str) -> None:
     """
     Write output to output file using JSON serialization.
 
@@ -166,7 +169,20 @@
         Output of the algorithm
     output_file : str
         Path to the output file
     """
     with open(output_file, "wb") as fp:
         serialized = serialization.serialize(output)
         fp.write(serialized)
+
+
+def _decode_env_vars() -> None:
+    """
+    Decode environment variables that are encoded by the node
+
+    Note that environment variables may be present that are not specific to vantage6,
+    such as HOME, PATH, etc. These are not encoded by the node and should not be
+    decoded here. The `get_env_var` function handles these properly so that the
+    original value is returned if the environment variable is not encoded.
+    """
+    for env_var in os.environ:
+        os.environ[env_var] = get_env_var(env_var)
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrappers.py` & `vantage6-algorithm-tools-4.4.0rc3/vantage6/algorithm/tools/wrappers.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/PKG-INFO` & `vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.4.0rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt` & `vantage6-algorithm-tools-4.4.0rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

