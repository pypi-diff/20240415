# Comparing `tmp/whylabs_toolkit-0.0.8.dev0.tar.gz` & `tmp/whylabs_toolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs_toolkit-0.0.8.dev0.tar", max compression
+gzip compressed data, was "whylabs_toolkit-0.0.9.tar", max compression
```

## Comparing `whylabs_toolkit-0.0.8.dev0.tar` & `whylabs_toolkit-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-06-01 13:58:08.969547 whylabs_toolkit-0.0.8.dev0/LICENSE
--rw-r--r--   0        0        0     1409 2023-06-01 13:58:08.969547 whylabs_toolkit-0.0.8.dev0/README.md
--rw-r--r--   0        0        0      785 2023-06-01 13:58:08.969547 whylabs_toolkit-0.0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/cli/__init__.py
--rw-r--r--   0        0        0      559 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/container/config_types.py
--rw-r--r--   0        0        0        0 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/__init__.py
--rw-r--r--   0        0        0      362 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/client.py
--rw-r--r--   0        0        0     1600 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/config.py
--rw-r--r--   0        0        0      960 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/dataset_profiles.py
--rw-r--r--   0        0        0     1999 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/models.py
--rw-r--r--   0        0        0     3316 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/monitor_helpers.py
--rw-r--r--   0        0        0     6066 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/schema.py
--rw-r--r--   0        0        0      922 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/utils.py
--rw-r--r--   0        0        0      121 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/__init__.py
--rw-r--r--   0        0        0      178 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/__init__.py
--rw-r--r--   0        0        0      557 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/credentials.py
--rw-r--r--   0        0        0     5777 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/manager.py
--rw-r--r--   0        0        0     9557 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py
--rw-r--r--   0        0        0     1500 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/__init__.py
--rw-r--r--   0        0        0      841 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py
--rw-r--r--   0        0        0    12589 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py
--rw-r--r--   0        0        0     4597 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py
--rw-r--r--   0        0        0     3242 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py
--rw-r--r--   0        0        0     2071 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py
--rw-r--r--   0        0        0     4115 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/column_schema.py
--rw-r--r--   0        0        0     3363 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/commons.py
--rw-r--r--   0        0        0     2497 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/document.py
--rw-r--r--   0        0        0     9201 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/monitor.py
--rw-r--r--   0        0        0      574 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/segments.py
--rw-r--r--   0        0        0      961 2023-06-01 13:58:08.973547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/utils.py
--rw-r--r--   0        0        0    75902 2023-06-01 13:58:08.977547 whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/schema/schema.json
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.8.dev0/setup.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1409 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/README.md
+-rw-r--r--   0        0        0      780 2023-07-28 18:17:12.083372 whylabs_toolkit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/cli/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/container/config_types.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/client.py
+-rw-r--r--   0        0        0     2029 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/config.py
+-rw-r--r--   0        0        0     1982 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/dataset_profiles.py
+-rw-r--r--   0        0        0     2199 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/models.py
+-rw-r--r--   0        0        0     4639 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/monitor_helpers.py
+-rw-r--r--   0        0        0     5922 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/schema.py
+-rw-r--r--   0        0        0      922 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/utils.py
+-rw-r--r--   0        0        0      100 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/__init__.py
+-rw-r--r--   0        0        0      178 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/credentials.py
+-rw-r--r--   0        0        0     5777 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/manager.py
+-rw-r--r--   0        0        0    10796 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/monitor_setup.py
+-rw-r--r--   0        0        0     1702 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/__init__.py
+-rw-r--r--   0        0        0    14365 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/algorithms.py
+-rw-r--r--   0        0        0     4731 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3242 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/baseline.py
+-rw-r--r--   0        0        0     2071 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/targets.py
+-rw-r--r--   0        0        0     4115 2023-07-28 18:17:12.087372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/column_schema.py
+-rw-r--r--   0        0        0     3363 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/commons.py
+-rw-r--r--   0        0        0     2366 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/document.py
+-rw-r--r--   0        0        0     9201 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/monitor.py
+-rw-r--r--   0        0        0      574 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/segments.py
+-rw-r--r--   0        0        0      961 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/utils.py
+-rw-r--r--   0        0        0    75902 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/schema/schema.json
+-rw-r--r--   0        0        0        0 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-28 18:17:12.091372 whylabs_toolkit-0.0.9/whylabs_toolkit/utils/granularity.py
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.9/setup.py
+-rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.9/PKG-INFO
```

### Comparing `whylabs_toolkit-0.0.8.dev0/LICENSE` & `whylabs_toolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/README.md` & `whylabs_toolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/pyproject.toml` & `whylabs_toolkit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylabs-toolkit"
-version = "0.0.8-dev0"
+version = "0.0.9"
 description = "Whylabs CLI and Helpers package."
 authors = ["Anthony Naddeo <anthony.naddeo@gmail.com>", "Murilo Mendonca <murilommen@gmail.com>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 packages = [{include = "whylabs_toolkit/**/*.py"}]
 include = ["whylabs_toolkit/monitor/schema/schema.json"]
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/container/config_types.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/container/config_types.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/config.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import os
+import logging
 from enum import Enum
 
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
 
 class ConfigVars(Enum):
     ORG_ID = 1
     DATASET_ID = 2
     WHYLABS_API_KEY = 3
     WHYLABS_HOST = "https://api.whylabsapp.com"
+    WHYLABS_PRIVATE_API_ENDPOINT = 5
 
 
 class Config:
     def get_whylabs_api_key(self) -> str:
         return Validations.require(ConfigVars.WHYLABS_API_KEY)
 
     def get_whylabs_host(self) -> str:
+        _private_api_endpoint = Validations.get_or_default(ConfigVars.WHYLABS_PRIVATE_API_ENDPOINT)
+        if _private_api_endpoint and isinstance(_private_api_endpoint, str):
+            logger.debug(f"Using private API endpoint: {_private_api_endpoint}")
+            return _private_api_endpoint
         return Validations.get_or_default(ConfigVars.WHYLABS_HOST)
 
     def get_default_org_id(self) -> str:
         return Validations.require(ConfigVars.ORG_ID)
 
     def get_default_dataset_id(self) -> str:
         return Validations.require(ConfigVars.DATASET_ID)
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/models.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 from whylabs_toolkit.helpers.utils import get_models_api
 from whylabs_toolkit.helpers.config import Config
 
 logger = logging.getLogger(__name__)
 
 
 def update_model_metadata(
-    dataset_id: str,
+    dataset_id: Optional[str] = None,
     org_id: Optional[str] = None,
     time_period: Optional[str] = None,
     model_type: Optional[str] = None,
     config: Config = Config(),
 ) -> None:
     """
     Update model attributes like model type and period.
     """
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
+
     api = get_models_api(config=config)
 
     model_metadata = api.get_model(org_id=org_id, model_id=dataset_id)
     logger.debug(f"Updating dataset with current metadata: \n {model_metadata}")
 
     try:
         resp = api.update_model(
@@ -37,24 +40,25 @@
         )
         logger.debug(f"Updated sucessfully! Resp: {resp}")
     except ApiValueError as e:
         raise e
 
 
 def add_custom_metric(
-    dataset_id: str,
     label: str,
     column: str,
     default_metric: str,
     org_id: Optional[str] = None,
+    dataset_id: Optional[str] = None,
     config: Config = Config(),
 ) -> None:
 
-    if not org_id:
-        org_id = config.get_default_org_id()
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
+
     api = get_models_api(config=config)
     metric_schema = MetricSchema(label=label, column=column, default_metric=default_metric)
 
     try:
         api.put_entity_schema_metric(org_id, dataset_id, metric_schema)
         logger.info(f"Updated entity schema metric!")
     except ApiException as e:
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/monitor_helpers.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/monitor_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,121 @@
 import logging
 from typing import Any, List, Optional
 
 from whylabs_client.exceptions import ApiValueError
-from whylabs_client.exceptions import NotFoundException
+from whylabs_client.exceptions import NotFoundException, ForbiddenException
 
 from whylabs_toolkit.helpers.config import Config
 from whylabs_toolkit.helpers.utils import get_monitor_api, get_models_api
+from whylabs_toolkit.utils.granularity import Granularity
 
 
 BASE_ENDPOINT = "https://api.whylabsapp.com"
+logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 # TODO create deactivate_monitor
 
 
 def get_monitor_config(org_id: str, dataset_id: str, config: Config = Config()) -> Any:
     api = get_monitor_api(config=config)
-    monitor_config = api.get_monitor_config_v3(org_id=org_id, dataset_id=dataset_id)
-    return monitor_config
+    try:
+        monitor_config = api.get_monitor_config_v3(org_id=org_id, dataset_id=dataset_id)
+        return monitor_config
+    except NotFoundException:
+        logger.warning(f"Could not find a monitor config for {dataset_id}")
+        return None
 
 
 def get_monitor(
     monitor_id: str, org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
 ) -> Any:
-    if not org_id:
-        org_id = config.get_default_org_id()
-    if not dataset_id:
-        dataset_id = config.get_default_dataset_id()
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
+
     api = get_monitor_api(config=config)
-    return api.get_monitor(org_id=org_id, dataset_id=dataset_id, monitor_id=monitor_id)
+    try:
+        monitor = api.get_monitor(org_id=org_id, dataset_id=dataset_id, monitor_id=monitor_id)
+        return monitor
+    except (ForbiddenException, NotFoundException):
+        logger.warning(
+            f"Could not find a monitor with id {monitor_id} for {dataset_id}." "Did you set a correct WHYLABS_API_KEY?"
+        )
+        return None
 
 
-def get_analyzer_ids(org_id: str, dataset_id: str, monitor_id: str, config: Config = Config()) -> Any:
-    monitor_config = get_monitor_config(org_id=org_id, dataset_id=dataset_id, config=config)
-    for item in monitor_config["monitors"]:
-        if item["id"] == monitor_id:
-            resp = item["analyzerIds"]
-            return resp
+def get_analyzer_ids(
+    monitor_id: str, org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
+) -> Any:
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
+    try:
+        monitor_config = get_monitor_config(org_id=org_id, dataset_id=dataset_id, config=config)
+
+        if monitor_config:
+            for item in monitor_config.get("monitors"):
+                if item["id"] == monitor_id:
+                    resp = item["analyzerIds"]
+                    return resp
+    except ForbiddenException:
+        logger.warning(f"Could not find analyzer IDs for {org_id}, {dataset_id}, {monitor_id}")
+        return None
 
 
 def get_analyzers(
-    monitor_id: str, org_id: Optional[str], dataset_id: Optional[str], config: Config = Config()
-) -> List[Any]:
-    if not org_id:
-        org_id = config.get_default_org_id()
-    if not dataset_id:
-        dataset_id = config.get_default_dataset_id()
+    monitor_id: str, org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
+) -> Optional[List[Any]]:
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
     api = get_monitor_api(config=config)
     analyzers = []
     analyzer_ids = get_analyzer_ids(org_id=org_id, dataset_id=dataset_id, monitor_id=monitor_id, config=config)
     if analyzer_ids:
         for analyzer in analyzer_ids:
             analyzers.append(api.get_analyzer(org_id=org_id, dataset_id=dataset_id, analyzer_id=analyzer))
         return analyzers
     else:
-        raise NotFoundException
+        return None
+
 
+def get_model_granularity(
+    org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
+) -> Optional[Granularity]:
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
 
-def get_model_granularity(org_id: str, dataset_id: str, config: Config = Config()) -> Optional[str]:
     api = get_models_api(config=config)
     model_meta = api.get_model(org_id=org_id, model_id=dataset_id)
 
     time_period_to_gran = {
-        "H": "hourly",
-        "D": "daily",
-        "W": "weekly",
-        "M": "monthly",
+        "H": Granularity.hourly,
+        "D": Granularity.daily,
+        "W": Granularity.weekly,
+        "M": Granularity.monthly,
     }
-
-    for key, value in time_period_to_gran.items():
-        if key in model_meta["time_period"]:
-            return value
+    if model_meta:
+        for key, value in time_period_to_gran.items():
+            if key in model_meta["time_period"]:
+                return value
     return None
 
 
-def delete_monitor(org_id: str, dataset_id: str, monitor_id: str, config: Config = Config()) -> None:
+def delete_monitor(
+    monitor_id: str, org_id: Optional[str] = None, dataset_id: Optional[str] = None, config: Config = Config()
+) -> None:
+    org_id = org_id or config.get_default_org_id()
+    dataset_id = dataset_id or config.get_default_dataset_id()
+
     api = get_monitor_api(config=config)
     try:
         analyzer_ids = get_analyzer_ids(org_id=org_id, dataset_id=dataset_id, monitor_id=monitor_id, config=config)
         if analyzer_ids is None:
             return
         for analyzer_id in analyzer_ids:
             resp_analyzer = api.delete_analyzer(org_id=org_id, dataset_id=dataset_id, analyzer_id=analyzer_id)
             logger.debug(f"Deleted analyzer with Resp:{resp_analyzer}")
         resp_monitor = api.delete_monitor(org_id=org_id, dataset_id=dataset_id, monitor_id=monitor_id)
         logger.debug(f"Deleted monitor with Resp:{resp_monitor}")
     except ApiValueError as e:
+        logger.error(f"Error deleting monitor {monitor_id}: {e.msg}")
         raise e
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/schema.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,29 @@
 from whylabs_toolkit.helpers.config import Config
 from whylabs_toolkit.helpers.utils import get_models_api
 from whylabs_toolkit.monitor.models.column_schema import ColumnDataType
 
 BASE_ENDPOINT = "https://api.whylabsapp.com"
 
 
+@dataclass
+class ColumnsClassifiers:
+    inputs: List[str] = field(default_factory=list)  # type: ignore
+    outputs: List[str] = field(default_factory=list)  # type: ignore
+
+
+@dataclass
+class ColumnsDiscreteness:
+    discrete: List[str] = field(default_factory=list)  # type: ignore
+    continuous: List[str] = field(default_factory=list)  # type: ignore
+
+
 class UpdateEntity(ABC):
-    def __init__(self, dataset_id: str, org_id: Optional[str] = None, config: Config = Config()):
-        self.dataset_id = dataset_id
+    def __init__(self, dataset_id: Optional[str] = None, org_id: Optional[str] = None, config: Config = Config()):
+        self.dataset_id = dataset_id or Config().get_default_dataset_id()
         self.org_id = org_id or Config().get_default_org_id()
         self.api = get_models_api(config=config)
 
     def _get_entity_schema(self) -> Any:
         entity_schema = self.api.get_entity_schema(org_id=self.org_id, dataset_id=self.dataset_id)
         return entity_schema
 
@@ -44,28 +56,16 @@
     def update(self) -> None:
         self._validate_input()
         self._get_current_entity_schema()
         self._update_entity_schema()
         self._put_updated_entity_schema()
 
 
-@dataclass
-class ColumnsClassifiers:
-    inputs: List[str] = field(default=None)  # type: ignore
-    outputs: List[str] = field(default=None)  # type: ignore
-
-    def __post_init__(self) -> None:
-        if self.inputs is None:
-            self.inputs = []
-        if self.outputs is None:
-            self.outputs = []
-
-
 class UpdateColumnClassifiers(UpdateEntity):
-    def __init__(self, dataset_id: str, classifiers: ColumnsClassifiers, org_id: Optional[str] = None):
+    def __init__(self, classifiers: ColumnsClassifiers, org_id: Optional[str] = None, dataset_id: Optional[str] = None):
         super().__init__(dataset_id, org_id)
         self.classifiers = classifiers
 
     def _validate_input(self) -> None:
         if self.classifiers.inputs == [] and self.classifiers.outputs == []:
             raise ValueError("You must define either input or output features to use this function.")
         same_list = [item for item in self.classifiers.inputs if item in self.classifiers.outputs]
@@ -105,15 +105,17 @@
     - bool
     - string
     - unknown
     - null
     ---
     """
 
-    def __init__(self, dataset_id: str, columns_schema: Dict[str, ColumnDataType], org_id: Optional[str] = None):
+    def __init__(
+        self, columns_schema: Dict[str, ColumnDataType], org_id: Optional[str] = None, dataset_id: Optional[str] = None
+    ):
         super().__init__(dataset_id, org_id)
         self.columns_schema = columns_schema
 
     def _validate_input(self) -> None:
         for data_type in self.columns_schema.values():
             if not isinstance(data_type, ColumnDataType):
                 raise ValueError(
@@ -122,28 +124,21 @@
 
     def _update_entity_schema(self) -> None:
         for column, data_type in self.columns_schema.items():
             if column in self.columns_dict.keys() and self.columns_dict[column]["data_type"] != data_type.value:
                 self.columns_dict[column].data_type = self.columns_schema[column].value
 
 
-@dataclass
-class ColumnsDiscreteness:
-    discrete: List[str] = field(default=None)  # type: ignore
-    continuous: List[str] = field(default=None)  # type: ignore
-
-    def __post_init__(self) -> None:
-        if self.discrete is None:
-            self.discrete = []
-        if self.continuous is None:
-            self.continuous = []
-
-
 class UpdateColumnsDiscreteness(UpdateEntity):
-    def __init__(self, dataset_id: str, columns: ColumnsDiscreteness, org_id: Optional[str] = None):
+    def __init__(
+        self,
+        columns: ColumnsDiscreteness,
+        org_id: Optional[str] = None,
+        dataset_id: Optional[str] = None,
+    ):
         super().__init__(dataset_id, org_id)
         self.columns = columns
 
     def _validate_input(self) -> None:
         if self.columns.discrete == [] and self.columns.continuous == []:
             raise ValueError("You must define either discrete or continuous columns to use this.")
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/helpers/utils.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/credentials.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/credentials.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/manager.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/manager.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/manager/monitor_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,47 +32,50 @@
         self._target_matrix: Optional[Union[ColumnMatrix, DatasetMatrix]] = None
         self._analyzer_config: Optional[
             Union[
                 DiffConfig,
                 FixedThresholdsConfig,
                 StddevConfig,
                 DriftConfig,
+                ComparisonConfig,
                 SeasonalConfig,
+                FrequentStringComparisonConfig,
+                ListComparisonConfig,
             ]
         ] = None
         self._target_columns: Optional[List[str]] = []
         self._exclude_columns: Optional[List[str]] = []
         self._prefill_properties()
 
     def _check_if_monitor_exists(self) -> Any:
-        try:
-            existing_monitor = get_monitor(
-                org_id=self.credentials.org_id,
-                dataset_id=self.credentials.dataset_id,
-                monitor_id=self.credentials.monitor_id,
-                config=self._config,
-            )
+        existing_monitor = get_monitor(
+            org_id=self.credentials.org_id,
+            dataset_id=self.credentials.dataset_id,
+            monitor_id=self.credentials.monitor_id,
+            config=self._config,
+        )
+        if existing_monitor:
             existing_monitor = Monitor.parse_obj(existing_monitor)
             logger.info(f"Got existing {self.credentials.monitor_id} from WhyLabs!")
-        except NotFoundException:
+        else:
             logger.info(f"Did not find a monitor with {self.credentials.monitor_id}, creating a new one.")
             existing_monitor = None
         return existing_monitor
 
     def _check_if_analyzer_exists(self) -> Any:
-        try:
-            existing_analyzers = get_analyzers(
-                org_id=self.credentials.org_id,
-                dataset_id=self.credentials.dataset_id,
-                monitor_id=self.credentials.monitor_id,
-                config=self._config,
-            )
+        existing_analyzers = get_analyzers(
+            org_id=self.credentials.org_id,
+            dataset_id=self.credentials.dataset_id,
+            monitor_id=self.credentials.monitor_id,
+            config=self._config,
+        )
+        if existing_analyzers:
             existing_analyzer = Analyzer.parse_obj(existing_analyzers[0])  # enforcing 1:1 relationship
 
-        except NotFoundException:
+        else:
             existing_analyzer = None
         return existing_analyzer
 
     def _prefill_properties(self) -> None:
         if self.monitor:
             self._monitor_mode = self.monitor.mode
             self._monitor_actions = self.monitor.actions
@@ -96,26 +99,39 @@
     @target_matrix.setter
     def target_matrix(self, target: Union[ColumnMatrix, DatasetMatrix]) -> None:
         self._target_matrix = target
 
     @property
     def config(
         self,
-    ) -> Optional[Union[DiffConfig, FixedThresholdsConfig, StddevConfig, DriftConfig, SeasonalConfig,]]:
+    ) -> Optional[
+        Union[
+            DiffConfig,
+            FixedThresholdsConfig,
+            StddevConfig,
+            DriftConfig,
+            ComparisonConfig,
+            SeasonalConfig,
+            FrequentStringComparisonConfig,
+            ListComparisonConfig,
+        ]
+    ]:
         return self._analyzer_config
 
     @config.setter
     def config(
         self,
         config: Union[
             DiffConfig,
             FixedThresholdsConfig,
             StddevConfig,
             DriftConfig,
             SeasonalConfig,
+            FrequentStringComparisonConfig,
+            ListComparisonConfig,
         ],
     ) -> None:
         self._analyzer_config = config
 
     @property
     def actions(self) -> Optional[List[Union[GlobalAction, EmailRecipient, SlackWebhook]]]:
         return self._monitor_actions
@@ -162,20 +178,28 @@
         """
         Args:
             :columns: A list of the targeted columns to monitor against the reference profile.
             :type columns: List[str]
         """
         if self._validate_columns_input(columns=columns):
             self._target_columns = columns
-            self._target_matrix = ColumnMatrix(include=self._target_columns, exclude=self._exclude_columns, segments=[])
+            self._target_matrix = self._target_matrix or ColumnMatrix(
+                include=self._target_columns, exclude=self._exclude_columns, segments=[]
+            )
+            if isinstance(self._target_matrix, ColumnMatrix):
+                self._target_matrix.include = self._target_columns
 
     def exclude_target_columns(self, columns: List[str]) -> None:
         if self._validate_columns_input(columns=columns):
             self._exclude_columns = columns
-            self._target_matrix = ColumnMatrix(include=self._target_columns, exclude=self._exclude_columns, segments=[])
+            self._target_matrix = self._target_matrix or ColumnMatrix(
+                include=self._target_columns, exclude=self._exclude_columns, segments=[]
+            )
+            if isinstance(self._target_matrix, ColumnMatrix):
+                self._target_matrix.exclude = self._exclude_columns
 
     def set_fixed_dates_baseline(self, start_date: datetime, end_date: datetime) -> None:
         if not start_date.tzinfo:
             start_date = start_date.replace(tzinfo=timezone.utc)
         if not end_date.tzinfo:
             end_date = end_date.replace(tzinfo=timezone.utc)
         # TODO make baseline nullable and default baseline to be TrailingWindowBaseline(size=14)
@@ -217,22 +241,32 @@
         )
 
     def __set_dataset_matrix_for_dataset_metric(self) -> None:
         if self._analyzer_config:
             if isinstance(self._analyzer_config.metric, DatasetMetric) and isinstance(
                 self._target_matrix, ColumnMatrix
             ):
-                self._target_matrix = DatasetMatrix(segments=[])
+                logger.warning(
+                    "ColumnMatrix is not configurable with a DatasetMetric." "Changing it to DatasetMatrix instead"
+                )
+                self._target_matrix = DatasetMatrix(segments=self._target_matrix.segments)
                 return None
 
             elif isinstance(self._target_matrix, DatasetMatrix) and not isinstance(
                 self._analyzer_config.metric, DatasetMetric
             ):
-                self._target_matrix = None
-                self.__configure_target_matrix()
+                logger.warning(
+                    "Setting a DatasetMatrix requires a DatasetMetric to be used"
+                    "Changing it to an empty ColumnMatrix instead"
+                )
+                self._target_matrix = ColumnMatrix(
+                    include=self._target_columns or ["*"],
+                    exclude=self._exclude_columns,
+                    segments=self._target_matrix.segments,
+                )
                 return None
 
     def apply(self) -> None:
         monitor_mode = self._monitor_mode or DigestMode()
         actions = self._monitor_actions or []
         self._analyzer_schedule = self._analyzer_schedule or FixedCadenceSchedule(
             cadence=get_model_granularity(
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,25 @@
     "DiffConfig",
     "ComparisonConfig",
     "ComparisonOperator",
     "ExperimentalConfig",
     "FixedThresholdsConfig",
     "ColumnListChangeConfig",
     "SeasonalConfig",
+    "ListComparisonConfig",
+    "FrequentStringComparisonConfig",
     "StddevConfig",
     # enums
     "DiffMode",
     "ThresholdType",
     "AlgorithmType",
     "DatasetMetric",
     "SimpleColumnMetric",
     "ComplexMetrics",
+    "ListComparisonOperator",
+    "FrequentStringComparisonOperator",
     # targets
     "DatasetMatrix",
     "ColumnMatrix",
     "TargetLevel",
+    "ExpectedValue",
 ]
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 class AlgorithmType(str, Enum):
     """Specify the algorithm type."""
 
     expected = "expected"
     column_list = "column_list"
     comparison = "comparison"
+    list_comparison = "list_comparison"
+    frequent_string_comparison = "frequent_string_comparison"
     diff = "diff"
     drift = "drift"
     stddev = "stddev"
     seasonal = "seasonal"
     fixed = "fixed"
     experimental = "experimental"
 
@@ -144,21 +146,34 @@
     float: Optional[float]
 
 
 class ComparisonOperator(str, Enum):
     """Operators for performing a comparison."""
 
     eq = "eq"
+    # Not Yet Implemented:
+    # gt = "gt"
+    # lt = "lt"
+    # ge = "ge"
+    # le = "le"
 
 
-# Not Yet Implemented:
-# gt = "gt"
-# lt = "lt"
-# ge = "ge"
-# le = "le"
+class ListComparisonOperator(str, Enum):
+    """Operators for performing a comparison."""
+
+    in_list = "in"
+    not_in_list = "not_in"
+
+
+class FrequentStringComparisonOperator(str, Enum):
+    """Operators for performing a comparison."""
+
+    eq = "eq"
+    target_includes_all_baseline = "target_includes_all_baseline"
+    baseline_includes_all_target = "baseline_includes_all_target"
 
 
 class ComparisonConfig(AlgorithmConfig):
     """Compare whether the target against a value or against a baseline's metric.
 
     This is useful to detect data type change, for instance.
     """
@@ -244,17 +259,15 @@
 
     This will fall back to Poisson distribution if there is only 1 value in the baseline.
 
     This only works with TrailingWindow baseline (TODO: add backend validation)
     """
 
     type: Literal[AlgorithmType.seasonal] = AlgorithmType.seasonal
-    algorithm: Literal["arima", "rego", "stastforecast"] = Field(
-        "arima", description="The algorithm implementation for seasonal analysis"
-    )
+    algorithm: Literal["arima"] = Field("arima", description="The algorithm implementation for seasonal analysis")
     minBatchSize: Optional[int] = Field(
         30,
         title="MinBatchSize",
         description="Minimum number of batches that is required",
     )
     alpha: Optional[float] = Field(
         default=0.05,
@@ -283,15 +296,15 @@
     """An analyzer using stddev for a window of time range.
 
     This analysis will detect whether the data drifts or not. By default, we use hellinger distance with a threshold
     of 0.7.
     """
 
     type: Literal[AlgorithmType.drift] = AlgorithmType.drift
-    algorithm: Literal["hellinger", "ks_test", "kl_divergence", "variation_distance"] = Field(
+    algorithm: Literal["hellinger", "jensenshannon", "kl_divergence", "psi"] = Field(
         "hellinger", description="The algorithm to use when calculating drift."
     )
     metric: Literal[ComplexMetrics.histogram, ComplexMetrics.frequent_items]
     threshold: float = Field(
         0.7,
         description="The threshold for the distance algorithm. Depending on the algorithm, this threshold"
         "is used for greater than or less than comparison.",
@@ -310,14 +323,39 @@
 
     type: Literal[AlgorithmType.experimental] = AlgorithmType.experimental
     implementation: str = Field(description="The implementation of an experimental config", max_length=100)
     baseline: Union[TrailingWindowBaseline, ReferenceProfileId, TimeRangeBaseline, SingleBatchBaseline]
     stub: Optional[AlgorithmType] = Field(description="Stub field to flow algoirthm type into the schema. Do not use.")
 
 
+class ListComparisonConfig(AlgorithmConfig):
+    """Compare a target list of values against a baseline list of values."""
+
+    type: Literal[AlgorithmType.list_comparison] = AlgorithmType.list_comparison
+    operator: ListComparisonOperator = Field(
+        description="The operator for the comparison. The right hand side is the target batch's metric. The left hand"
+        "side is the expected value or a baseline's metric."
+    )
+    expected: Optional[List[ExpectedValue]] = Field(
+        None,
+        description="The expected values of the equality. If the value is not set we will extract the corresponding "
+        "metric from the baseline and perform the comparison",
+    )
+    baseline: Optional[Union[TrailingWindowBaseline, ReferenceProfileId, TimeRangeBaseline, SingleBatchBaseline]]
+
+
+class FrequentStringComparisonConfig(AlgorithmConfig):
+    """Compare whether target against a list of values."""
+
+    type: Literal[AlgorithmType.frequent_string_comparison] = AlgorithmType.frequent_string_comparison
+    metric: Literal[ComplexMetrics.frequent_items] = ComplexMetrics.frequent_items
+    operator: FrequentStringComparisonOperator = Field(description="The operator for the comparison.")
+    baseline: Union[TrailingWindowBaseline, ReferenceProfileId, TimeRangeBaseline, SingleBatchBaseline]
+
+
 class DiffMode(str, Enum):
     """Whether to use the absolute difference or the percentage to calculate the difference."""
 
     abs = "abs"
     pct = "pct"
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from whylabs_toolkit.monitor.models.commons import NoExtrasBaseModel
 
 from ..commons import CronSchedule, FixedCadenceSchedule, Metadata
 from ..utils import anyOf_to_oneOf, duration_field
 from .algorithms import (
     ColumnListChangeConfig,
     ComparisonConfig,
+    ListComparisonConfig,
+    FrequentStringComparisonConfig,
     DiffConfig,
     DriftConfig,
     ExperimentalConfig,
     FixedThresholdsConfig,
     SeasonalConfig,
     StddevConfig,
 )
@@ -86,23 +88,25 @@
         "we will only backfill batches not previously analyzed. If the batch was already analyzed, "
         "even with partial data, the backfill will ignore the new data unless you trigger an explicit "
         "backfill request. We support 48 hours for hourly data, 30 days for daily data, and 6 months for "
         "monthly data.",
     )
 
     # NOT YET IMPLEMENTED:
-    # ComparisonConfig,
     # ExperimentalConfig,
     # ColumnListChangeConfig,
 
     config: Union[
         DiffConfig,
         FixedThresholdsConfig,
+        ListComparisonConfig,
+        FrequentStringComparisonConfig,
         StddevConfig,
         DriftConfig,
+        ComparisonConfig,
         SeasonalConfig,
     ] = Field(description="The configuration map of the analyzer", discriminator="type")
 
     class Config:
         """Updates JSON schema anyOf to oneOf."""
 
         # noinspection PyUnusedLocal
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/baseline.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/analyzer/targets.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/column_schema.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/commons.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/commons.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/document.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/document.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 """The overall document for monitor."""
 import uuid
-from enum import Enum
 from typing import List, Literal, Optional
 
 from pydantic import Field
 
 from whylabs_toolkit.monitor.models.commons import NoExtrasBaseModel
 
 from .analyzer import Analyzer
 from .column_schema import EntitySchema, EntityWeights
 from .commons import DATASET_ID_DEF, Metadata
 from .monitor import Monitor
-
-
-class Granularity(str, Enum):
-    """Supported granularity."""
-
-    hourly = "hourly"
-    daily = "daily"
-    weekly = "weekly"
-    monthly = "monthly"
+from ...utils.granularity import Granularity
 
 
 class Document(NoExtrasBaseModel):
     """The main document that dictates how the monitor should be run. This document is managed by WhyLabs internally."""
 
     id: Optional[uuid.UUID] = Field(None, description="A unique ID for the document")
     schemaVersion: Literal[1] = Field(
```

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/monitor.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/monitor.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/segments.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/segments.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/models/utils.py` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/models/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/whylabs_toolkit/monitor/schema/schema.json` & `whylabs_toolkit-0.0.9/whylabs_toolkit/monitor/schema/schema.json`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.8.dev0/setup.py` & `whylabs_toolkit-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 ['whylabs_toolkit',
  'whylabs_toolkit.cli',
  'whylabs_toolkit.container',
  'whylabs_toolkit.helpers',
  'whylabs_toolkit.monitor',
  'whylabs_toolkit.monitor.manager',
  'whylabs_toolkit.monitor.models',
- 'whylabs_toolkit.monitor.models.analyzer']
+ 'whylabs_toolkit.monitor.models.analyzer',
+ 'whylabs_toolkit.utils']
 
 package_data = \
 {'': ['*'], 'whylabs_toolkit.monitor': ['schema/*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'whylabs-client>=0.5,<0.6',
  'whylogs>=1.1.26,<2.0.0']
 
 setup_kwargs = {
     'name': 'whylabs-toolkit',
-    'version': '0.0.8.dev0',
+    'version': '0.0.9',
     'description': 'Whylabs CLI and Helpers package.',
     'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package             | Usage                |\n|---------------------|----------------------|\n| [Monitor Manager](/whylabs_toolkit/monitor/manager/README.md) | Author and modify existing WhyLabs monitor with Python |\n| [WhyLabs Helpers](/whylabs_toolkit/helpers/README.md) | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
     'author': 'Anthony Naddeo',
     'author_email': 'anthony.naddeo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `whylabs_toolkit-0.0.8.dev0/PKG-INFO` & `whylabs_toolkit-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-toolkit
-Version: 0.0.8.dev0
+Version: 0.0.9
 Summary: Whylabs CLI and Helpers package.
 License: Apache-2.0 license
 Author: Anthony Naddeo
 Author-email: anthony.naddeo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

