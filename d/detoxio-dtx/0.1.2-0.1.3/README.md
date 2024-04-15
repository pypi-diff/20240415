# Comparing `tmp/detoxio_dtx-0.1.2.tar.gz` & `tmp/detoxio_dtx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detoxio_dtx-0.1.2.tar", max compression
+gzip compressed data, was "detoxio_dtx-0.1.3.tar", max compression
```

## Comparing `detoxio_dtx-0.1.2.tar` & `detoxio_dtx-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      597 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/README.md
--rw-r--r--   0        0        0      948 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/src/dtx/__init__.py
--rw-r--r--   0        0        0     5408 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/src/dtx/cli/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/src/dtx/cli/console.py
--rw-r--r--   0        0        0     3180 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/src/dtx/cli/inferencing.py
--rw-r--r--   0        0        0      714 2024-04-03 10:55:43.775988 detoxio_dtx-0.1.2/src/dtx/cli/utils.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 detoxio_dtx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      695 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/README.md
+-rw-r--r--   0        0        0      948 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/__init__.py
+-rw-r--r--   0        0        0     5631 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/console.py
+-rw-r--r--   0        0        0     3180 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/inferencing.py
+-rw-r--r--   0        0        0      714 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/utils.py
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 detoxio_dtx-0.1.3/PKG-INFO
```

### Comparing `detoxio_dtx-0.1.2/pyproject.toml` & `detoxio_dtx-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "detoxio-dtx"
-version = "0.1.2"
+version = "0.1.3"
 description = "detoxio.ai - API first LLM security testing and red team automation"
 authors = ["detoxio.ai <hello@detoxio.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://detoxio.ai"
 documentation = "https://docs.detoxio.ai"
 classifiers = [
@@ -22,15 +22,15 @@
 [[tool.poetry.source]]
 name = "buf"
 url = "https://buf.build/gen/python"
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-detoxio = "^0.1.15"
+detoxio = "^0.1.18"
 click = "^8.1.7"
 tenacity = "^8.2.3"
 transformers = "^4.38.2"
 tqdm = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
```

### Comparing `detoxio_dtx-0.1.2/src/dtx/cli/__init__.py` & `detoxio_dtx-0.1.3/src/dtx/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import traceback
 import click
 import tqdm
 import detoxio.config as config
 import detoxio.adapters.exceptions as exceptions
 
 from detoxio.scanner import LLMScanner, LLMPrompt, LLMResponse
-from detoxio.reporting import JSONLinesLLMScanReport
+from detoxio.reporting import JSONLinesLLMScanReport, MarkdownLLMScanReport
 from detoxio.adapters.grpc import get_secure_channel_with_token
 from detoxio.adapters.prompts import get_prompts_service
 
 from dtx.cli.utils import print_info, print_error, print_success, print_verbose, is_verbose
 from dtx.cli.inferencing import TransformersAdapter
 from dtx.cli.console import ConsoleReporter
 
@@ -61,17 +61,18 @@
         prompt = prompt_service.generate_prompt(count=1)
         print_info(f"Prompt {i + 1}: {prompt.prompts[0].data.content}")
 
 @click.command("scan", help="Scan a model from Hugging Face for security vulnerablities")
 @click.option("--model", type=str, required=True, help="The model to scan")
 @click.option("--count", type=int, help="The number prompts to generate for scanning", default=10)
 @click.option("--jsonl", type=str, help="Output the results in JSONL format")
+@click.option("--markdown", type=str, help="Output the results in Markdown format")
 @click.option("--fast", is_flag=True, help="Use fast evaluation mode which is less accurate")
 @click.option("--verbose", is_flag=True, help="Enable verbose mode")
-def scan(model, count, jsonl, fast, verbose, *extra):
+def scan(model, count, jsonl, markdown, fast, verbose, *extra):
     """
     Scan a model from Hugging Face for security vulnerabilities.
     """
     key = config.load_key_from_env()
     scanner = LLMScanner(count=count, key=key)
 
     if fast:
@@ -81,14 +82,17 @@
     print_info(f"Initializing model adapter for: {model} using Transformers")
     inference_adapter = TransformersAdapter(model_name=model)
 
     reporters = []
     if jsonl:
         file = open(jsonl, "w")
         reporters.append(JSONLinesLLMScanReport(file=file))
+    if markdown:
+        file = open(markdown, "w")
+        reporters.append(MarkdownLLMScanReport(file))
 
     print_info(f"Initializing scanner for testing with {count} prompt(s)")
 
     # We will manually handle the progress bar
     if not is_verbose():
         progress = tqdm.tqdm(total=count, desc="Scanning model", unit="prompt")
     else:
```

### Comparing `detoxio_dtx-0.1.2/src/dtx/cli/console.py` & `detoxio_dtx-0.1.3/src/dtx/cli/console.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 import proto.dtx.messages.common.threat_pb2 as dtx_threat_pb2
 
 from detoxio.reporting import LLMScanReport
 from detoxio.models import LLMScanResult
-
-def dtx_get_threat_name(tid):
-    return dtx_threat_pb2.ThreatCategory.DESCRIPTOR.values_by_number[tid].name
-
-def dtx_get_threat_class_name(tid):
-    return dtx_threat_pb2.ThreatClass.DESCRIPTOR.values_by_number[tid].name
+from detoxio.utils import get_threat_class_human_name, get_threat_category_human_name
 
 threat_classes = [value.name for value in dtx_threat_pb2.ThreatClass.DESCRIPTOR.values]
 threat_categories = [value.name for value in dtx_threat_pb2.ThreatCategory.DESCRIPTOR.values]
 
 class ConsoleReporter(LLMScanReport):
     def render(self, results: LLMScanResult):
         metrics = {
             'prompt_count': len(results.results),
             'vulnerabilities': {}
         }
 
         for r in results:
             for response in r.responses:
                 for result in response.results:
-                    threat_class = dtx_get_threat_class_name(result.threat.threat_class)
-                    threat_name = dtx_get_threat_name(result.threat.threat_category)
+                    threat_class = get_threat_class_human_name(result.threat.threat_class)
+                    threat_name = get_threat_category_human_name(result.threat.threat_category)
 
                     metrics['vulnerabilities'][threat_class] = metrics['vulnerabilities'].get(threat_class, {})
                     metrics['vulnerabilities'][threat_class][threat_name] = metrics['vulnerabilities'][threat_class].get(threat_name, 0)
 
                     if result.status == dtx_threat_pb2.THREAT_EVALUATION_STATUS_UNSAFE:
                         metrics['vulnerabilities'][threat_class][threat_name] += 1
 
         # TODO: Enhance the rendering with a better visualization library
         for tk, tv in metrics['vulnerabilities'].items():
             for vk, vv in tv.items():
-                print("{0:<20} {1:<20}: {2}".format(tk, vk, vv))
+                print("{0:<20} > {1:<20}: {2}".format(tk, vk, vv))
```

### Comparing `detoxio_dtx-0.1.2/src/dtx/cli/inferencing.py` & `detoxio_dtx-0.1.3/src/dtx/cli/inferencing.py`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.2/src/dtx/cli/utils.py` & `detoxio_dtx-0.1.3/src/dtx/cli/utils.py`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.2/PKG-INFO` & `detoxio_dtx-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detoxio-dtx
-Version: 0.1.2
+Version: 0.1.3
 Summary: detoxio.ai - API first LLM security testing and red team automation
 Home-page: https://detoxio.ai
 License: Apache-2.0
 Author: detoxio.ai
 Author-email: hello@detoxio.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,27 +13,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Security
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: detoxio (>=0.1.15,<0.2.0)
+Requires-Dist: detoxio (>=0.1.18,<0.2.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Project-URL: Documentation, https://docs.detoxio.ai
 Description-Content-Type: text/markdown
 
 # detoxio.ai Command Line Tool
 
 ## Installation
 
 ```bash
-python3 -m pip install detoxio-dtx \
+python3 -m pip install detoxio-dtx --upgrade
+```
+
+Install protocol buffers client libraries from BSR
+
+```bash
+python3 -m pip install \
     detoxio-api-protocolbuffers-python detoxio-api-grpc-python \
     --upgrade --extra-index-url https://buf.build/gen/python
 ```
 
 > **Note:** We need to install additional packages because as per PEP-440, we
 > cannot have a package with direct dependencies outside the public index
```

