# Comparing `tmp/flojoy_cloud-0.1.3.tar.gz` & `tmp/flojoy_cloud-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy_cloud-0.1.3.tar", max compression
+gzip compressed data, was "flojoy_cloud-0.2.0.tar", max compression
```

## Comparing `flojoy_cloud-0.1.3.tar` & `flojoy_cloud-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-02-15 21:52:07.176756 flojoy_cloud-0.1.3/README.md
--rw-r--r--   0        0        0      205 2024-03-20 22:23:17.128704 flojoy_cloud-0.1.3/flojoy_cloud/__init__.py
--rw-r--r--   0        0        0    11450 2024-03-20 22:23:17.129166 flojoy_cloud-0.1.3/flojoy_cloud/client.py
--rw-r--r--   0        0        0     2100 2024-02-15 21:52:06.863260 flojoy_cloud-0.1.3/flojoy_cloud/dtypes.py
--rw-r--r--   0        0        0      757 2024-02-15 21:52:06.916326 flojoy_cloud-0.1.3/flojoy_cloud/measurement.py
--rw-r--r--   0        0        0     3600 2024-03-22 16:55:46.390698 flojoy_cloud-0.1.3/flojoy_cloud/test_sequencer.py
--rw-r--r--   0        0        0     2471 2024-02-15 21:52:06.961480 flojoy_cloud-0.1.3/flojoy_cloud/watch.py
--rw-r--r--   0        0        0      591 2024-03-22 16:56:00.471858 flojoy_cloud-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 flojoy_cloud-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 02:02:50.649483 flojoy_cloud-0.2.0/README.md
+-rw-r--r--   0        0        0      205 2024-04-05 02:02:50.649586 flojoy_cloud-0.2.0/flojoy_cloud/__init__.py
+-rw-r--r--   0        0        0    12842 2024-04-11 17:51:50.620763 flojoy_cloud-0.2.0/flojoy_cloud/client.py
+-rw-r--r--   0        0        0     2352 2024-04-15 21:19:38.258403 flojoy_cloud-0.2.0/flojoy_cloud/dtypes.py
+-rw-r--r--   0        0        0      757 2024-04-05 02:02:50.650153 flojoy_cloud-0.2.0/flojoy_cloud/measurement.py
+-rw-r--r--   0        0        0     5960 2024-04-15 21:19:38.258938 flojoy_cloud-0.2.0/flojoy_cloud/test_sequencer.py
+-rw-r--r--   0        0        0     2471 2024-04-05 02:02:50.650305 flojoy_cloud-0.2.0/flojoy_cloud/watch.py
+-rw-r--r--   0        0        0      607 2024-04-15 21:19:55.902198 flojoy_cloud-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 flojoy_cloud-0.2.0/PKG-INFO
```

### Comparing `flojoy_cloud-0.1.3/flojoy_cloud/client.py` & `flojoy_cloud-0.2.0/flojoy_cloud/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import json
 import os
-from typing import Any, Callable, Optional, ParamSpec, TypeVar, overload
+from typing import Any, Callable, List, Optional, ParamSpec, TypeVar, overload
 
 import httpx
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, TypeAdapter
 
 from flojoy_cloud.dtypes import (
@@ -16,14 +16,15 @@
     MeasurementCreateResult,
     Model,
     ModelComponent,
     ModelTree,
     Project,
     ProjectWithModel,
     Test,
+    SessionMeasurement,
 )
 from flojoy_cloud.measurement import MeasurementData, MeasurementType, make_payload
 
 
 class CloudEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, datetime.datetime) or isinstance(o, pd.Timestamp):
@@ -383,7 +384,53 @@
     @query(model=Measurement)
     def get_measurement(self, measurement_id: str):
         return self.client.get(f"/measurements/{measurement_id}")
 
     @query(model=None)
     def delete_measurement(self, measurement_id: str):
         return self.client.delete(f"/measurements/{measurement_id}")
+
+    @query(model=None)
+    def get_hardware_id(self, part_number: str, serial_number: str):
+        return "TODO"
+
+    @query(model=MeasurementCreateResult)
+    def upload_session(
+        self,
+        serial_number: str,
+        station_id: str,
+        integrity: bool,
+        aborted: bool,
+        notes: Optional[str],
+        commit_hash: Optional[str],
+        measurements: List[SessionMeasurement],
+    ):
+        m_list = []
+        for m in measurements:
+            # Find id of each part
+            m_list.append(
+                {
+                    "data": make_payload(m.data),
+                    "name": m.name,
+                    "pass": m.passed,
+                    "createdAt": m.created_at.isoformat() if m.created_at else None,
+                }
+            )
+        body = _make_params(
+            {
+                "serialNumber": serial_number,
+                "stationId": station_id,
+                "integrity": integrity,
+                "aborted": aborted,
+                "notes": notes,
+                "commitHash": commit_hash,
+                "measurements": m_list,
+            }
+        )
+
+        return self.client.post(
+            "/session/measurements",
+            content=json.dumps(body, cls=CloudEncoder),
+            headers={
+                "Content-Type": "application/json",
+            },
+        )
```

### Comparing `flojoy_cloud-0.1.3/flojoy_cloud/dtypes.py` & `flojoy_cloud-0.2.0/flojoy_cloud/dtypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
-import datetime
-from typing import ForwardRef, Literal, Optional
 
+import datetime
+from typing import Literal, Optional
 
 from pydantic import BaseModel, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 
-from flojoy_cloud.measurement import MeasurementType
+from flojoy_cloud.measurement import MeasurementData, MeasurementType
 
 
 class CamelModel(BaseModel):
     model_config = ConfigDict(alias_generator=to_camel, protected_namespaces=())
 
 
 class CloudModel(CamelModel):
@@ -109,7 +109,18 @@
 
 
 class Test(CloudModel):
     project_id: str
     name: str
     measurement_type: MeasurementType
     updated_at: Optional[datetime.datetime]
+
+
+class SessionMeasurement(BaseModel):
+    data: MeasurementData
+    test_id: str
+    name: str | None = None
+    passed: bool | None = None
+    created_at: datetime.datetime | None = None
+
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `flojoy_cloud-0.1.3/flojoy_cloud/measurement.py` & `flojoy_cloud-0.2.0/flojoy_cloud/measurement.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.1.3/flojoy_cloud/test_sequencer.py` & `flojoy_cloud-0.2.0/flojoy_cloud/test_sequencer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import logging
 import os
+import shutil
+from typing import Tuple
 import pandas as pd
 import tempfile
 from .measurement import MeasurementData
+from pydantic import BaseModel
+
+
+ExpectedMeasurementType = int | float
+
+
+class ExpectedMeasurement(BaseModel):
+    min: ExpectedMeasurementType | None = None
+    max: ExpectedMeasurementType | None = None
 
 
 # ------ Public ------
 
 __all__ = [
     "export",
     "_get_most_recent_data",
     "_set_output_loc",
 ]
 
 
 def export(data: MeasurementData):
     """Export data so it can be retrieved by the test sequencer"""
     output_dir, prefix_file = __get_location()
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
     if isinstance(data, pd.DataFrame):
         data.to_csv(os.path.join(output_dir, prefix_file + DATAFRAME))
     elif isinstance(data, bool):
         with open(os.path.join(output_dir, prefix_file + BOOLEAN), "w") as f:
             f.write(str(data))
     elif isinstance(data, int):
         with open(os.path.join(output_dir, prefix_file + INT), "w") as f:
@@ -30,17 +39,57 @@
     elif isinstance(data, float):
         with open(os.path.join(output_dir, prefix_file + FLOAT), "w") as f:
             f.write(str(data))
     else:
         raise TypeError(f"Unsupported data type: {type(data)}")
 
 
+def is_in_range(data: ExpectedMeasurementType):
+    """Assert that the data is within the min and max values"""
+    min, max = get_min_max()
+    if min is not None and max is not None:
+        return min <= data <= max
+    elif min is not None:
+        return min <= data
+    elif max is not None:
+        return data <= max
+    raise ValueError("Min and max values not set")
+
+
+def get_min_max() -> (
+    Tuple[ExpectedMeasurementType | None, ExpectedMeasurementType | None]
+):
+    output_dir, postfix_file = __get_location()
+    min_max_file = os.path.join(output_dir, f"min_max_{postfix_file}.json")
+    if os.path.exists(min_max_file):
+        with open(min_max_file, "r") as f:
+            data = ExpectedMeasurement.model_validate_json(f.read())
+            return data.min, data.max
+    logging.warn("Min and max values not found")
+    return None, None
+
+
 # ------ Protected ------
 
 
+def _set_min_max(
+    min_val: ExpectedMeasurementType | None, max_val: ExpectedMeasurementType | None
+):
+    """
+    Set the min and max values for a test from within the test sequencer.
+     - The use of `_set_output_loc` prior to calling this is highly recommended.
+    """
+    output_dir, postfix_file = __get_location()
+    min_max_file = os.path.join(output_dir, f"min_max_{postfix_file}.json")
+    data = {"min": min_val, "max": max_val}
+    with open(min_max_file, "w") as f:
+        f.write(ExpectedMeasurement(**data).model_dump_json())
+        logging.info(f"Min and max values set to {min_max_file}")
+
+
 def _get_most_recent_data(
     test_id: str | None, rm_file: bool = False
 ) -> MeasurementData | None:
     """
     Retrieves the most recent data produced in a test run from within the test sequencer.
     Parameters:
         - test_id (str | None): The prefix used to find the data files. If None, the default prefix is used.
@@ -57,20 +106,40 @@
 
     if rm_file:
         os.remove(output_dir + output_file)
 
     return __extract_data(output_dir + output_file)
 
 
-def _set_output_loc(prefix: str | None):
-    """Set the output location for the data when launching a test in the test sequencer."""
+def _set_output_loc(prefix: str | None, rm_existing_data: bool = False):
+    """
+    Set the output location for the data when launching a test in the test sequencer.
+    @prefix: The prefix to use for the data files and directory.
+    - If None, the default prefix is used.
+    @rm_existing_data: If True, all existing data in the output directory is deleted.
+    - Warning: If the prefixis None, everything is deleted.
+
+    """
     if prefix is not None:
         os.environ[OPTIONAL_NAME_ENV] = prefix
     else:
         os.environ.pop(OPTIONAL_NAME_ENV)
+    if rm_existing_data:
+        _nuke_output_loc()
+
+
+def _nuke_output_loc():
+    """
+    Delete data files in the output directory.
+    - Warning: If the output loc is not set, everything is deleted
+    """
+    output_dir, _ = __get_location()
+    if not os.path.exists(output_dir):
+        return
+    shutil.rmtree(output_dir)
 
 
 # ------ Private ------
 
 
 DEFAULT_PATH = os.path.join(tempfile.gettempdir(), "flojoy/")
 OPTIONAL_PATH_ENV = "FLOJOY_DATA_PATH"
@@ -82,27 +151,29 @@
 INT = "_int.txt"
 FLOAT = "_float.txt"
 
 
 def __get_location():
     output_dir = DEFAULT_PATH
     prefix_file = os.environ.get(OPTIONAL_NAME_ENV)
+    output_dir = os.path.join(output_dir, f"{prefix_file}/")
     if prefix_file is None:
         prefix_file = DEFAULT_NAME
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
 
     return output_dir, prefix_file
 
 
 def __get_most_recent_file(output_dir: str, prefix_file: str):
     most_recent_file = None
     most_recent_time = 0
     if not os.path.exists(output_dir):
         return None
     for file in os.listdir(output_dir):
-        logging.info(f"Available data: {file}")
         if file.startswith(prefix_file):
             file_path = os.path.join(output_dir, file)
             file_time = os.path.getmtime(file_path)
             if file_time > most_recent_time:
                 most_recent_time = file_time
                 most_recent_file = file
```

### Comparing `flojoy_cloud-0.1.3/flojoy_cloud/watch.py` & `flojoy_cloud-0.2.0/flojoy_cloud/watch.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.1.3/pyproject.toml` & `flojoy_cloud-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flojoy-cloud"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = ["Joey Yu <joey@flojoy.io>", "Jeff Zhang <jeff@flojoy.io>"]
 readme = "README.md"
 packages = [{ include = "flojoy_cloud" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -18,11 +18,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 ipykernel = "^6.29.0"
 python-dotenv = "^1.0.1"
 plotly = "^5.18.0"
 nbformat = "^5.9.2"
+ruff = "^0.3.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flojoy_cloud-0.1.3/PKG-INFO` & `flojoy_cloud-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy-cloud
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Author: Joey Yu
 Author-email: joey@flojoy.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

