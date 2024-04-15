# Comparing `tmp/oteltest-0.6.1.tar.gz` & `tmp/oteltest-0.7.0.tar.gz`

## Comparing `oteltest-0.6.1.tar` & `oteltest-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oteltest-0.6.1/_v/.gitignore
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.6.1/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1484 2020-02-02 00:00:00.000000 oteltest-0.6.1/example_scripts/simple_loop.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/main.py
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/private.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/version.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/sink/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.6.1/src/oteltest/sink/private.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.6.1/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 oteltest-0.6.1/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 oteltest-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1484 2020-02-02 00:00:00.000000 oteltest-0.7.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/private.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/version.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/sink/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.7.0/src/oteltest/sink/private.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oteltest-0.7.0/tests/test_oteltest.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.7.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 oteltest-0.7.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 oteltest-0.7.0/PKG-INFO
```

### Comparing `oteltest-0.6.1/example_scripts/simple_loop.py` & `oteltest-0.7.0/example_scripts/simple_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 import time
 
 from opentelemetry import trace
 from oteltest import OtelTest, Telemetry
 
-SERVICE_NAME = "integration-test"
+SERVICE_NAME = "my-otel-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
             print(f"simple_loop.py: {i+1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
-class MyTest(OtelTest):
+class MyOtelTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
     def environment_variables(self):
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
     def wrapper_script(self):
```

### Comparing `oteltest-0.6.1/src/oteltest/__init__.py` & `oteltest-0.7.0/src/oteltest/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,47 +19,49 @@
 from typing import List, Mapping, Optional, Sequence
 
 
 @dataclasses.dataclass
 class Request:
     request: dict
     headers: dict
+    test_elapsed_ms: int
 
     def get_header(self, name):
         return self.headers.get(name)
 
     def to_json(self):
         return json.dumps(self.to_dict())
 
     def to_dict(self):
         return {
             "request": self.request,
             "headers": self.headers,
+            "test_elapsed_ms": self.test_elapsed_ms,
         }
 
 
 class Telemetry:
     def __init__(
         self,
         log_reqs: Optional[List[Request]] = None,
         metric_reqs: Optional[List[Request]] = None,
         trace_reqs: Optional[List[Request]] = None,
     ):
         self.log_reqs: List[Request] = log_reqs or []
         self.metric_reqs: List[Request] = metric_reqs or []
         self.trace_reqs: List[Request] = trace_reqs or []
 
-    def add_log(self, log: dict, headers: dict):
-        self.log_reqs.append(Request(log, headers))
+    def add_log(self, log: dict, headers: dict, test_elapsed_ms: int):
+        self.log_reqs.append(Request(log, headers, test_elapsed_ms))
 
-    def add_metric(self, metric: dict, headers: dict):
-        self.metric_reqs.append(Request(metric, headers))
+    def add_metric(self, metric: dict, headers: dict, test_elapsed_ms: int):
+        self.metric_reqs.append(Request(metric, headers, test_elapsed_ms))
 
-    def add_trace(self, trace: dict, headers: dict):
-        self.trace_reqs.append(Request(trace, headers))
+    def add_trace(self, trace: dict, headers: dict, test_elapsed_ms: int):
+        self.trace_reqs.append(Request(trace, headers, test_elapsed_ms))
 
     def get_trace_requests(self) -> List[Request]:
         return self.trace_reqs
 
     def num_metrics(self) -> int:
         out = 0
         for req in self.metric_reqs:
```

### Comparing `oteltest-0.6.1/src/oteltest/main.py` & `oteltest-0.7.0/src/oteltest/main.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/src/oteltest/private.py` & `oteltest-0.7.0/src/oteltest/private.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import importlib
 import inspect
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
+import time
 import typing
 import venv
 from pathlib import Path
 
 from google.protobuf.json_format import MessageToDict
 
 from opentelemetry.proto.collector.logs.v1.logs_service_pb2 import (
@@ -64,23 +65,37 @@
         print(f"- Will install requirement: '{req}'")
         run_subprocess([pip_path, "install", req])
 
     run_python_script(script, script_dir, oteltest_instance, v)
 
     v.rm()
 
-    save_telemetry_json(script_dir, module_name, handler.telemetry_to_json())
+    filename = get_next_json_file(script_dir, module_name)
+    print(f"- Will save telemetry to {filename}")
+    save_telemetry_json(script_dir, filename, handler.telemetry_to_json())
 
     oteltest_instance.on_shutdown(handler.telemetry)
     print(f"- {script} PASSED")
 
 
-def save_telemetry_json(script_dir, module_name, json_str):
-    path_str = str(Path(script_dir) / f"{module_name}.json")
-    with open(path_str, "w") as file:
+def get_next_json_file(path_to_dir: str, module_name: str):
+    p = Path(path_to_dir)
+    max_index = -1
+    for file in p.glob(f"{module_name}.*.json"):
+        parts = file.stem.split(".")
+        if parts[-1].isdigit():  # Ensure the last part is an integer
+            index = int(parts[-1])
+            if index > max_index:
+                max_index = index
+    return f"{module_name}.{max_index+1}.json"
+
+
+def save_telemetry_json(script_dir: str, file_name: str, json_str: str):
+    path = Path(script_dir) / file_name
+    with open(str(path), "w") as file:
         file.write(json_str)
 
 
 def run_python_script(script, script_dir, oteltest_instance: OtelTest, v):
     python_script_cmd = [
         v.path_to_executable("python"),
         str(Path(script_dir) / script),
@@ -178,37 +193,47 @@
 
     def rm(self):
         shutil.rmtree(self.venv_dir)
 
 
 class AccumulatingHandler(RequestHandler):
     def __init__(self):
+        self.start_time = time.time_ns()
         self.telemetry = Telemetry()
 
     def handle_logs(
         self, request: ExportLogsServiceRequest, context
     ):  # noqa: ARG002
         self.telemetry.add_log(
-            MessageToDict(request), get_context_headers(context)
+            MessageToDict(request),
+            get_context_headers(context),
+            self.get_millis_since_test_start(),
         )
 
     def handle_metrics(
         self, request: ExportMetricsServiceRequest, context
     ):  # noqa: ARG002
         self.telemetry.add_metric(
-            MessageToDict(request), get_context_headers(context)
+            MessageToDict(request),
+            get_context_headers(context),
+            self.get_millis_since_test_start(),
         )
 
     def handle_trace(
         self, request: ExportTraceServiceRequest, context
     ):  # noqa: ARG002
         self.telemetry.add_trace(
-            MessageToDict(request), get_context_headers(context)
+            MessageToDict(request),
+            get_context_headers(context),
+            self.get_millis_since_test_start(),
         )
 
+    def get_millis_since_test_start(self):
+        return time.time_ns() - self.start_time
+
     def telemetry_to_json(self):
         return self.telemetry.to_json()
 
 
 def get_context_headers(context):
     return pbmetadata_to_dict(context.invocation_metadata())
```

### Comparing `oteltest-0.6.1/src/oteltest/version.py` & `oteltest-0.7.0/src/oteltest/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `oteltest-0.6.1/src/oteltest/sink/__init__.py` & `oteltest-0.7.0/src/oteltest/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/src/oteltest/sink/private.py` & `oteltest-0.7.0/src/oteltest/sink/private.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/tests/__init__.py` & `oteltest-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/.gitignore` & `oteltest-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/LICENSE.txt` & `oteltest-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/README.md` & `oteltest-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/pyproject.toml` & `oteltest-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.6.1/PKG-INFO` & `oteltest-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.6.1
+Version: 0.7.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

