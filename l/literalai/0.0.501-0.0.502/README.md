# Comparing `tmp/literalai-0.0.501.tar.gz` & `tmp/literalai-0.0.502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.501.tar", last modified: Mon Apr  8 10:41:56 2024, max compression
+gzip compressed data, was "literalai-0.0.502.tar", last modified: Mon Apr 15 11:49:13 2024, max compression
```

## Comparing `literalai-0.0.501.tar` & `literalai-0.0.502.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.363604 literalai-0.0.501/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 10:41:44.000000 literalai-0.0.501/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 10:41:56.363604 literalai-0.0.501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 10:41:44.000000 literalai-0.0.501/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.359604 literalai-0.0.501/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.363604 literalai-0.0.501/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    36330 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.363604 literalai-0.0.501/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.363604 literalai-0.0.501/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 10:41:44.000000 literalai-0.0.501/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.359604 literalai-0.0.501/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 10:41:56.000000 literalai-0.0.501/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 10:41:56.000000 literalai-0.0.501/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:41:56.000000 literalai-0.0.501/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 10:41:56.000000 literalai-0.0.501/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 10:41:56.000000 literalai-0.0.501/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:41:56.363604 literalai-0.0.501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 10:41:44.000000 literalai-0.0.501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:56.363604 literalai-0.0.501/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:41:44.000000 literalai-0.0.501/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.827803 literalai-0.0.502/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 11:49:03.000000 literalai-0.0.502/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 11:49:13.823803 literalai-0.0.502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 11:49:03.000000 literalai-0.0.502/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-15 11:49:03.000000 literalai-0.0.502/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 11:49:13.000000 literalai-0.0.502/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 11:49:13.000000 literalai-0.0.502/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:49:13.000000 literalai-0.0.502/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 11:49:13.000000 literalai-0.0.502/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 11:49:13.000000 literalai-0.0.502/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:49:13.827803 literalai-0.0.502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 11:49:03.000000 literalai-0.0.502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:13.823803 literalai-0.0.502/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:49:03.000000 literalai-0.0.502/tests/__init__.py
```

### Comparing `literalai-0.0.501/LICENSE` & `literalai-0.0.502/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/README.md` & `literalai-0.0.502/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/api/__init__.py` & `literalai-0.0.502/literalai/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Literal,
     Optional,
     TypeVar,
     Union,
 )
 
 from literalai.dataset import DatasetType
+from literalai.dataset_experiment import DatasetExperiment, DatasetExperimentItem
 from literalai.filter import (
     generations_filters,
     generations_order_by,
     scores_filters,
     scores_order_by,
     threads_filters,
     threads_order_by,
@@ -29,14 +30,16 @@
     delete_attachment_helper,
     get_attachment_helper,
     update_attachment_helper,
 )
 from .dataset_helpers import (
     add_generation_to_dataset_helper,
     add_step_to_dataset_helper,
+    create_experiment_helper,
+    create_experiment_item_helper,
     create_dataset_helper,
     create_dataset_item_helper,
     delete_dataset_helper,
     delete_dataset_item_helper,
     get_dataset_helper,
     get_dataset_item_helper,
     update_dataset_helper,
@@ -45,15 +48,17 @@
 from .prompt_helpers import (
     create_prompt_helper,
     create_prompt_lineage_helper,
     get_prompt_helper,
 )
 from .score_helpers import (
     ScoreUpdate,
+    check_scores_finite,
     create_score_helper,
+    create_scores_query_builder,
     delete_score_helper,
     get_scores_helper,
     update_score_helper,
 )
 from .step_helpers import (
     create_step_helper,
     delete_step_helper,
@@ -84,14 +89,16 @@
 import httpx
 
 from literalai.my_types import (
     Attachment,
     ChatGeneration,
     CompletionGeneration,
     GenerationMessage,
+    Score,
+    ScoreDict,
     ScoreType,
 )
 from literalai.step import Step, StepDict, StepType
 
 logger = logging.getLogger(__name__)
 
 
@@ -299,25 +306,41 @@
         filters: Optional[scores_filters] = None,
         order_by: Optional[scores_order_by] = None,
     ):
         return self.gql_helper(
             *get_scores_helper(first, after, before, filters, order_by)
         )
 
+    def create_scores(self, scores: List[ScoreDict]):
+        check_scores_finite(scores)
+
+        query = create_scores_query_builder(scores)
+        variables = {}
+        for id, score in enumerate(scores):
+            for k, v in score.items():
+                variables[f"{k}_{id}"] = v
+
+        def process_response(response):
+            return [Score.from_dict(x) for x in response["data"].values()]
+
+        return self.gql_helper(query, "create scores", variables, process_response)
+
     def create_score(
         self,
         name: str,
-        value: int,
+        value: float,
         type: ScoreType,
         step_id: Optional[str] = None,
         generation_id: Optional[str] = None,
         dataset_experiment_item_id: Optional[str] = None,
         comment: Optional[str] = None,
         tags: Optional[List[str]] = None,
     ):
+        check_scores_finite([{"name": name, "value": value}])
+
         return self.gql_helper(
             *create_score_helper(
                 name,
                 value,
                 type,
                 step_id,
                 generation_id,
@@ -372,28 +395,29 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = (
-            {}
-        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
         with httpx.Client() as client:
             if upload_type == "raw":
                 upload_response = client.request(
-                    url=url, headers=headers, method=method, data=content  # type: ignore
+                    url=url,
+                    headers=headers,
+                    method=method,
+                    data=content,  # type: ignore
                 )
             else:
                 upload_response = client.request(
                     url=url,
                     headers=headers,
                     method=method,
                     files=form_data,
@@ -562,16 +586,18 @@
         metadata: Optional[Dict] = None,
         type: DatasetType = "key_value",
     ):
         return self.gql_helper(
             *create_dataset_helper(self, name, description, metadata, type)
         )
 
-    def get_dataset(self, id: str):
-        subpath, _, variables, process_response = get_dataset_helper(self, id)
+    def get_dataset(self, id: Optional[str] = None, name: Optional[str] = None):
+        subpath, _, variables, process_response = get_dataset_helper(
+            self, id=id, name=name
+        )
         response = self.make_rest_call(subpath, variables)
         return process_response(response)
 
     def update_dataset(
         self,
         id: str,
         name: Optional[str] = None,
@@ -581,14 +607,48 @@
         return self.gql_helper(
             *update_dataset_helper(self, id, name, description, metadata)
         )
 
     def delete_dataset(self, id: str):
         return self.gql_helper(*delete_dataset_helper(self, id))
 
+    # Dataset Experiment APIs
+
+    def create_experiment(
+        self,
+        dataset_id: str,
+        name: str,
+        prompt_id: Optional[str] = None,
+        params: Optional[Dict] = None,
+    ) -> "DatasetExperiment":
+        return self.gql_helper(
+            *create_experiment_helper(self, dataset_id, name, prompt_id, params)
+        )
+
+    def create_experiment_item(
+        self, experiment_item: DatasetExperimentItem
+    ) -> DatasetExperimentItem:
+        # Create the dataset experiment item
+        result = self.gql_helper(
+            *create_experiment_item_helper(
+                dataset_experiment_id=experiment_item.dataset_experiment_id,
+                dataset_item_id=experiment_item.dataset_item_id,
+                input=experiment_item.input,
+                output=experiment_item.output,
+            )
+        )
+
+        for score in experiment_item.scores:
+            score["datasetExperimentItemId"] = result.id
+
+        # Create the scores and add to experiment item.
+        result.scores = self.create_scores(experiment_item.scores)
+
+        return result
+
     # Dataset Item API
 
     def create_dataset_item(
         self,
         dataset_id: str,
         input: Dict,
         expected_output: Optional[Dict] = None,
@@ -819,25 +879,44 @@
         filters: Optional[scores_filters] = None,
         order_by: Optional[scores_order_by] = None,
     ):
         return await self.gql_helper(
             *get_scores_helper(first, after, before, filters, order_by)
         )
 
+    async def create_scores(self, scores: List[ScoreDict]):
+        check_scores_finite(scores)
+
+        query = create_scores_query_builder(scores)
+        variables = {}
+
+        for id, score in enumerate(scores):
+            for k, v in score.items():
+                variables[f"{k}_{id}"] = v
+
+        def process_response(response):
+            return [Score.from_dict(x) for x in response["data"].values()]
+
+        return await self.gql_helper(
+            query, "create scores", variables, process_response
+        )
+
     async def create_score(
         self,
         name: str,
-        value: int,
+        value: float,
         type: ScoreType,
         step_id: Optional[str] = None,
         generation_id: Optional[str] = None,
         dataset_experiment_item_id: Optional[str] = None,
         comment: Optional[str] = None,
         tags: Optional[List[str]] = None,
     ):
+        check_scores_finite([{"name": name, "value": value}])
+
         return await self.gql_helper(
             *create_score_helper(
                 name,
                 value,
                 type,
                 step_id,
                 generation_id,
@@ -892,28 +971,29 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = (
-            {}
-        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
         async with httpx.AsyncClient() as client:
             if upload_type == "raw":
                 upload_response = await client.request(
-                    url=url, headers=headers, method=method, data=content  # type: ignore
+                    url=url,
+                    headers=headers,
+                    method=method,
+                    data=content,  # type: ignore
                 )
             else:
                 upload_response = await client.request(
                     url=url,
                     headers=headers,
                     method=method,
                     files=form_data,
@@ -1085,17 +1165,19 @@
         type: DatasetType = "key_value",
     ):
         sync_api = LiteralAPI(self.api_key, self.url)
         return await self.gql_helper(
             *create_dataset_helper(sync_api, name, description, metadata, type)
         )
 
-    async def get_dataset(self, id: str):
+    async def get_dataset(self, id: Optional[str] = None, name: Optional[str] = None):
         sync_api = LiteralAPI(self.api_key, self.url)
-        subpath, _, variables, process_response = get_dataset_helper(sync_api, id)
+        subpath, _, variables, process_response = get_dataset_helper(
+            sync_api, id=id, name=name
+        )
         response = await self.make_rest_call(subpath, variables)
         return process_response(response)
 
     async def update_dataset(
         self,
         id: str,
         name: Optional[str] = None,
@@ -1107,14 +1189,54 @@
             *update_dataset_helper(sync_api, id, name, description, metadata)
         )
 
     async def delete_dataset(self, id: str):
         sync_api = LiteralAPI(self.api_key, self.url)
         return await self.gql_helper(*delete_dataset_helper(sync_api, id))
 
+    # Dataset Experiment APIs
+
+    async def create_experiment(
+        self,
+        dataset_id: str,
+        name: str,
+        prompt_id: Optional[str] = None,
+        params: Optional[Dict] = None,
+    ) -> "DatasetExperiment":
+        sync_api = LiteralAPI(self.api_key, self.url)
+
+        return await self.gql_helper(
+            *create_experiment_helper(
+                sync_api, dataset_id, name, prompt_id, params
+            )
+        )
+
+    async def create_experiment_item(
+        self, experiment_item: DatasetExperimentItem
+    ) -> DatasetExperimentItem:
+        check_scores_finite(experiment_item.scores)
+
+        # Create the dataset experiment item
+        result = await self.gql_helper(
+            *create_experiment_item_helper(
+                dataset_experiment_id=experiment_item.dataset_experiment_id,
+                dataset_item_id=experiment_item.dataset_item_id,
+                input=experiment_item.input,
+                output=experiment_item.output,
+            )
+        )
+
+        for score in experiment_item.scores:
+            score["datasetExperimentItemId"] = result.id
+
+        # Create the scores and add to experiment item.
+        result.scores = await self.create_scores(experiment_item.scores)
+
+        return result
+
     # DatasetItem API
 
     async def create_dataset_item(
         self,
         dataset_id: str,
         input: Dict,
         expected_output: Optional[Dict] = None,
```

### Comparing `literalai-0.0.501/literalai/api/attachment_helpers.py` & `literalai-0.0.502/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/api/dataset_helpers.py` & `literalai-0.0.502/literalai/api/dataset_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING, Dict, Optional
 
 from literalai.dataset import Dataset, DatasetType
+from literalai.dataset_experiment import DatasetExperiment, DatasetExperimentItem
 from literalai.dataset_item import DatasetItem
 
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
 
 from . import gql
 
@@ -27,16 +28,26 @@
         return Dataset.from_dict(api, response["data"]["createDataset"])
 
     description = "create dataset"
 
     return gql.CREATE_DATASET, description, variables, process_response
 
 
-def get_dataset_helper(api: "LiteralAPI", id: str):
-    body = {"id": id}
+def get_dataset_helper(
+    api: "LiteralAPI", id: Optional[str] = None, name: Optional[str] = None
+):
+    if not id and not name:
+        raise ValueError("id or name must be provided")
+
+    body = {}
+
+    if id:
+        body["id"] = id
+    if name:
+        body["name"] = name
 
     def process_response(response):
         dataset_dict = response.get("data")
         if dataset_dict is None:
             return None
         return Dataset.from_dict(api, dataset_dict)
 
@@ -78,14 +89,61 @@
         return Dataset.from_dict(api, response["data"]["deleteDataset"])
 
     description = "delete dataset"
 
     return gql.DELETE_DATASET, description, variables, process_response
 
 
+def create_experiment_helper(
+    api: "LiteralAPI",
+    dataset_id: str,
+    name: str,
+    prompt_id: Optional[str] = None,
+    params: Optional[Dict] = None,
+):
+    variables = {
+        "datasetId": dataset_id,
+        "name": name,
+        "promptId": prompt_id,
+        "params": params,
+    }
+
+    def process_response(response):
+        return DatasetExperiment.from_dict(
+            api, response["data"]["createDatasetExperiment"]
+        )
+
+    description = "create dataset experiment"
+
+    return gql.CREATE_EXPERIMENT, description, variables, process_response
+
+
+def create_experiment_item_helper(
+    dataset_experiment_id: str,
+    dataset_item_id: str,
+    input: Optional[Dict] = None,
+    output: Optional[Dict] = None,
+):
+    variables = {
+        "datasetExperimentId": dataset_experiment_id,
+        "datasetItemId": dataset_item_id,
+        "input": input,
+        "output": output,
+    }
+
+    def process_response(response):
+        return DatasetExperimentItem.from_dict(
+            response["data"]["createDatasetExperimentItem"]
+        )
+
+    description = "create dataset experiment item"
+
+    return gql.CREATE_EXPERIMENT_ITEM, description, variables, process_response
+
+
 def create_dataset_item_helper(
     dataset_id: str,
     input: Dict,
     expected_output: Optional[Dict] = None,
     metadata: Optional[Dict] = None,
 ):
     variables = {
```

### Comparing `literalai-0.0.501/literalai/api/generation_helpers.py` & `literalai-0.0.502/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/api/gql.py` & `literalai-0.0.502/literalai/api/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,14 +785,55 @@
             description
             metadata
             type
         }
     }
 """
 
+CREATE_EXPERIMENT = """
+    mutation CreateDatasetExperiment(
+        $name: String! 
+        $datasetId: String!
+        $promptId: String
+        $params: Json!
+    ) {
+        createDatasetExperiment(
+            name: $name
+            datasetId: $datasetId
+            promptId: $promptId
+            params: $params
+        ) {
+          id
+          name
+          datasetId
+          params
+        }
+    }
+"""
+
+CREATE_EXPERIMENT_ITEM = """
+    mutation CreateDatasetExperimentItem(
+        $datasetExperimentId: String!
+        $datasetItemId: String!
+        $input: Json
+        $output: Json
+    ) {
+        createDatasetExperimentItem(
+            datasetExperimentId: $datasetExperimentId
+            datasetItemId: $datasetItemId
+            input: $input
+            output: $output
+        ) {
+          id
+          input
+          output
+        }
+      }
+"""
+
 CREATE_DATASET_ITEM = """
 mutation CreateDatasetItem(
     $datasetId: String!
     $input: Json!
     $expectedOutput: Json
     $metadata: Json
 ) {
```

### Comparing `literalai-0.0.501/literalai/api/prompt_helpers.py` & `literalai-0.0.502/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/api/score_helpers.py` & `literalai-0.0.502/literalai/api/user_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,89 @@
-from typing import Any, Dict, List, Optional, TypedDict
+from typing import Any, Dict, Optional
 
-from literalai.filter import scores_filters, scores_order_by
-from literalai.my_types import PaginatedResponse, Score, ScoreType
+from literalai.filter import users_filters
+from literalai.my_types import PaginatedResponse, User
 
 from . import gql
 
 
-def get_scores_helper(
+def get_users_helper(
     first: Optional[int] = None,
     after: Optional[str] = None,
     before: Optional[str] = None,
-    filters: Optional[scores_filters] = None,
-    order_by: Optional[scores_order_by] = None,
+    filters: Optional[users_filters] = None,
 ):
     variables: Dict[str, Any] = {}
 
     if first:
         variables["first"] = first
     if after:
         variables["after"] = after
     if before:
         variables["before"] = before
     if filters:
         variables["filters"] = filters
-    if order_by:
-        variables["orderBy"] = order_by
 
     def process_response(response):
-        response_data = response["data"]["scores"]
-        response_data["data"] = list(map(lambda x: x["node"], response_data["edges"]))
-        del response_data["edges"]
-        return PaginatedResponse[Score].from_dict(response_data, Score)  # type: ignore
-
-    description = "get scores"
-
-    return gql.GET_SCORES, description, variables, process_response
-
-
-def create_score_helper(
-    name: str,
-    value: int,
-    type: ScoreType,
-    step_id: Optional[str] = None,
-    generation_id: Optional[str] = None,
-    dataset_experiment_item_id: Optional[str] = None,
-    comment: Optional[str] = None,
-    tags: Optional[List[str]] = None,
+        paginated_response = response["data"]["participants"]
+        response["data"] = list(map(lambda x: x["node"], paginated_response["edges"]))
+        return PaginatedResponse[User].from_dict(response, User)
+
+    description = "get users"
+
+    return gql.GET_PARTICIPANTS, description, variables, process_response
+
+
+def create_user_helper(identifier: str, metadata: Optional[Dict] = None):
+    variables = {"identifier": identifier, "metadata": metadata}
+
+    def process_response(response):
+        return User.from_dict(response["data"]["createParticipant"])
+
+    description = "create user"
+
+    return gql.CREATE_PARTICIPANT, description, variables, process_response
+
+
+def update_user_helper(
+    id: str, identifier: Optional[str] = None, metadata: Optional[Dict] = None
 ):
-    variables = {
-        "name": name,
-        "type": type,
-        "value": value,
-        "stepId": step_id,
-        "generationId": generation_id,
-        "datasetExperimentItemId": dataset_experiment_item_id,
-        "comment": comment,
-        "tags": tags,
-    }
+    variables = {"id": id, "identifier": identifier, "metadata": metadata}
+
+    # remove None values to prevent the API from removing existing values
+    variables = {k: v for k, v in variables.items() if v is not None}
 
     def process_response(response):
-        return Score.from_dict(response["data"]["createScore"])
+        return User.from_dict(response["data"]["updateParticipant"])
 
-    description = "create score"
+    description = "update user"
 
-    return gql.CREATE_SCORE, description, variables, process_response
+    return gql.UPDATE_PARTICIPANT, description, variables, process_response
 
 
-class ScoreUpdate(TypedDict, total=False):
-    comment: Optional[str]
-    value: float
+def get_user_helper(id: Optional[str] = None, identifier: Optional[str] = None):
+    if id is None and identifier is None:
+        raise Exception("Either id or identifier must be provided")
 
+    if id is not None and identifier is not None:
+        raise Exception("Only one of id or identifier must be provided")
 
-def update_score_helper(
-    id: str,
-    update_params: ScoreUpdate,
-):
-    variables = {"id": id, **update_params}
+    variables = {"id": id, "identifier": identifier}
 
     def process_response(response):
-        return Score.from_dict(response["data"]["updateScore"])
+        user = response["data"]["participant"]
+        return User.from_dict(user) if user else None
 
-    description = "update score"
+    description = "get user"
 
-    return gql.UPDATE_SCORE, description, variables, process_response
+    return gql.GET_PARTICIPANT, description, variables, process_response
 
 
-def delete_score_helper(id: str):
+def delete_user_helper(id: str):
     variables = {"id": id}
 
     def process_response(response):
-        return response["data"]["deleteScore"]
+        return response["data"]["deleteParticipant"]["id"]
 
-    description = "delete score"
+    description = "delete user"
 
-    return gql.DELETE_SCORE, description, variables, process_response
+    return gql.DELETE_PARTICIPANT, description, variables, process_response
```

### Comparing `literalai-0.0.501/literalai/api/step_helpers.py` & `literalai-0.0.502/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/api/thread_helpers.py` & `literalai-0.0.502/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/callback/langchain_callback.py` & `literalai-0.0.502/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/client.py` & `literalai-0.0.502/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/dataset.py` & `literalai-0.0.502/literalai/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
 
-from literalai.dataset_item import DatasetItemDict
+from literalai.dataset_experiment import DatasetExperiment
+from literalai.dataset_item import DatasetItem, DatasetItemDict
 
 DatasetType = Literal["key_value", "generation"]
 
 
 class DatasetDict(TypedDict, total=False):
     id: str
     createdAt: str
@@ -29,38 +30,42 @@
 class Dataset:
     api: "LiteralAPI"
     id: str
     created_at: str
     metadata: Dict
     name: Optional[str] = None
     description: Optional[str] = None
-    items: List[DatasetItemDict] = field(default_factory=lambda: [])
+    items: List[DatasetItem] = field(default_factory=lambda: [])
     type: DatasetType = "key_value"
 
     def to_dict(self):
         return {
             "id": self.id,
             "createdAt": self.created_at,
             "metadata": self.metadata,
             "name": self.name,
             "description": self.description,
-            "items": self.items,
+            "items": [item.to_dict() for item in self.items],
             "type": self.type,
         }
 
     @classmethod
     def from_dict(cls, api: "LiteralAPI", dataset: DatasetDict) -> "Dataset":
+        items = dataset.get("items", [])
+        if not isinstance(items, list):
+            raise Exception("Dataset items should be an array")
+
         return cls(
             api=api,
             id=dataset.get("id", ""),
             created_at=dataset.get("createdAt", ""),
             metadata=dataset.get("metadata", {}),
             name=dataset.get("name"),
             description=dataset.get("description"),
-            items=dataset.get("items") or [],
+            items=[DatasetItem.from_dict(item) for item in items],
             type=dataset.get("type", "key_value"),
         )
 
     def update(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
@@ -77,70 +82,82 @@
         self.api.delete_dataset(self.id)
 
     def create_item(
         self,
         input: Dict,
         expected_output: Optional[Dict] = None,
         metadata: Optional[Dict] = None,
-    ) -> DatasetItemDict:
+    ) -> DatasetItem:
         """
         Create a new dataset item and add it to this dataset.
         :param input: The input data for the dataset item.
         :param expected_output: The output data for the dataset item (optional).
         :param metadata: Metadata for the dataset item (optional).
         :return: The created DatasetItem instance.
         """
         dataset_item = self.api.create_dataset_item(
             self.id, input, expected_output, metadata
         )
         if self.items is None:
             self.items = []
-        dataset_item_dict = dataset_item.to_dict()
-        self.items.append(dataset_item_dict)
-        return dataset_item_dict
+        self.items.append(dataset_item)
+        return dataset_item
+
+    def create_experiment(
+        self, name: str, prompt_id: Optional[str] = None, params: Optional[Dict] = None
+    ) -> DatasetExperiment:
+        """
+        Creates a new dataset experiment based on this dataset.
+        :param name: The name of the experiment .
+        :param prompt_id: The Prompt ID used on LLM calls (optional).
+        :param params: The params used on the experiment.
+        :return: The created DatasetExperiment instance as a dictionary.
+        """
+        experiment = self.api.create_experiment(
+            self.id, name, prompt_id, params
+        )
+        return experiment
 
     def delete_item(self, item_id: str):
         """
         Delete a dataset item from this dataset.
         :param api: An instance of the DatasetAPI to make the call.
         :param item_id: The ID of the dataset item to delete.
         """
         self.api.delete_dataset_item(item_id)
         if self.items is not None:
-            self.items = [item for item in self.items if item["id"] != item_id]
+            self.items = [item for item in self.items if item.id != item_id]
 
     def add_step(
         self, step_id: str, metadata: Optional[Dict] = None
-    ) -> DatasetItemDict:
+    ) -> DatasetItem:
         """
         Create a new dataset item based on a step and add it to this dataset.
         :param step_id: The id of the step to add to the dataset.
         :param metadata: Metadata for the dataset item (optional).
         :return: The created DatasetItem instance.
         """
         if self.type == "generation":
             raise ValueError("Cannot add a step to a generation dataset")
 
         dataset_item = self.api.add_step_to_dataset(self.id, step_id, metadata)
         if self.items is None:
             self.items = []
-        dataset_item_dict = dataset_item.to_dict()
-        self.items.append(dataset_item_dict)
-        return dataset_item_dict
+        self.items.append(dataset_item)
+        return dataset_item
 
     def add_generation(
         self, generation_id: str, metadata: Optional[Dict] = None
-    ) -> DatasetItemDict:
+    ) -> DatasetItem:
         """
         Create a new dataset item based on a generation and add it to this dataset.
         :param generation_id: The id of the generation to add to the dataset.
         :param metadata: Metadata for the dataset item (optional).
         :return: The created DatasetItem instance.
         """
         dataset_item = self.api.add_generation_to_dataset(
             self.id, generation_id, metadata
         )
         if self.items is None:
             self.items = []
-        dataset_item_dict = dataset_item.to_dict()
-        self.items.append(dataset_item_dict)
-        return dataset_item_dict
+        self.items.append(dataset_item)
+        return dataset_item
```

### Comparing `literalai-0.0.501/literalai/dataset_item.py` & `literalai-0.0.502/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/event_processor.py` & `literalai-0.0.502/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/filter.py` & `literalai-0.0.502/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/helper.py` & `literalai-0.0.502/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/instrumentation/openai.py` & `literalai-0.0.502/literalai/instrumentation/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
             if isinstance(generation, ChatGeneration):
                 step.output = generation.message_completion  # type: ignore
             else:
                 step.output = {"content": generation.completion}
             step.generation = generation
             step.end()
         else:
-            await client.api.create_generation(generation)
+            client.api.create_generation(generation)
 
     def async_after_wrapper(metadata: Dict):
         async def after(result, context: AfterContext, *args, **kwargs):
             step = context.get("step")
             generation = context.get("generation")
 
             if not generation:
@@ -478,15 +478,15 @@
                 if isinstance(generation, ChatGeneration):
                     step.output = generation.message_completion  # type: ignore
                 else:
                     step.output = {"content": generation.completion}
                 step.generation = generation
                 step.end()
             else:
-                await client.api.create_generation(generation)
+                client.api.create_generation(generation)
             return result
 
         return after
 
     wrap_all(
         TO_WRAP,
         before_wrapper,
```

### Comparing `literalai-0.0.501/literalai/message.py` & `literalai-0.0.502/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/my_types.py` & `literalai-0.0.502/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/prompt.py` & `literalai-0.0.502/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/requirements.py` & `literalai-0.0.502/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/step.py` & `literalai-0.0.502/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/thread.py` & `literalai-0.0.502/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai/wrappers.py` & `literalai-0.0.502/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.501/literalai.egg-info/SOURCES.txt` & `literalai-0.0.502/literalai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 literalai/__init__.py
 literalai/client.py
 literalai/context.py
 literalai/dataset.py
+literalai/dataset_experiment.py
 literalai/dataset_item.py
 literalai/event_processor.py
 literalai/filter.py
 literalai/helper.py
 literalai/message.py
 literalai/my_types.py
 literalai/prompt.py
```

