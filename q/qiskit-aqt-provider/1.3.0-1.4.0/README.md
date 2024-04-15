# Comparing `tmp/qiskit_aqt_provider-1.3.0.tar.gz` & `tmp/qiskit_aqt_provider-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_aqt_provider-1.3.0.tar", max compression
+gzip compressed data, was "qiskit_aqt_provider-1.4.0.tar", max compression
```

## Comparing `qiskit_aqt_provider-1.3.0.tar` & `qiskit_aqt_provider-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     3214 2024-02-20 17:48:54.619542 qiskit_aqt_provider-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    14035 2024-02-20 17:48:54.619542 qiskit_aqt_provider-1.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11416 2024-02-20 17:48:54.619542 qiskit_aqt_provider-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1579 2024-02-20 17:48:54.619542 qiskit_aqt_provider-1.3.0/README.md
--rw-r--r--   0        0        0     7067 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      562 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/__init__.py
--rw-r--r--   0        0        0     9111 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/api_models.py
--rw-r--r--   0        0        0    17787 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/api_models_generated.py
--rw-r--r--   0        0        0    20864 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_job.py
--rw-r--r--   0        0        0     4004 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_options.py
--rw-r--r--   0        0        0     9826 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_provider.py
--rw-r--r--   0        0        0    14357 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_resource.py
--rw-r--r--   0        0        0     5096 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/circuit_to_aqt.py
--rw-r--r--   0        0        0     5802 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/persistence.py
--rw-r--r--   0        0        0      616 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/__init__.py
--rw-r--r--   0        0        0     2659 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/estimator.py
--rw-r--r--   0        0        0     2459 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/sampler.py
--rw-r--r--   0        0        0        0 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/py.typed
--rw-r--r--   0        0        0      587 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/__init__.py
--rw-r--r--   0        0        0     2747 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/circuits.py
--rw-r--r--   0        0        0     2334 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/fixtures.py
--rw-r--r--   0        0        0     7204 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/resources.py
--rw-r--r--   0        0        0     1268 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/timeout.py
--rw-r--r--   0        0        0     2147 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/utils.py
--rw-r--r--   0        0        0     7831 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/transpiler_plugin.py
--rw-r--r--   0        0        0     1825 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/utils.py
--rw-r--r--   0        0        0     1013 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/versions.py
--rw-r--r--   0        0        0        0 2024-02-20 17:48:54.623542 qiskit_aqt_provider-1.3.0/test/__init__.py
--rw-r--r--   0        0        0     3790 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_api_models.py
--rw-r--r--   0        0        0     7772 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_circuit_to_aqt.py
--rw-r--r--   0        0        0    13668 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_execution.py
--rw-r--r--   0        0        0     9114 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_job_persistence.py
--rw-r--r--   0        0        0     2159 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_options.py
--rw-r--r--   0        0        0     6627 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_primitives.py
--rw-r--r--   0        0        0     8422 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_provider.py
--rw-r--r--   0        0        0    15445 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_resource.py
--rw-r--r--   0        0        0     8668 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_transpilation.py
--rw-r--r--   0        0        0     1102 2024-02-20 17:48:54.627542 qiskit_aqt_provider-1.3.0/test/test_utils.py
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 qiskit_aqt_provider-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3214 2024-04-15 07:48:30.174040 qiskit_aqt_provider-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    14035 2024-04-15 07:48:30.174040 qiskit_aqt_provider-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11416 2024-04-15 07:48:30.174040 qiskit_aqt_provider-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1579 2024-04-15 07:48:30.174040 qiskit_aqt_provider-1.4.0/README.md
+-rw-r--r--   0        0        0     7046 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/__init__.py
+-rw-r--r--   0        0        0     9111 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/api_models.py
+-rw-r--r--   0        0        0    18547 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/api_models_generated.py
+-rw-r--r--   0        0        0    20864 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_job.py
+-rw-r--r--   0        0        0     4074 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_options.py
+-rw-r--r--   0        0        0     9826 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_provider.py
+-rw-r--r--   0        0        0    14357 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_resource.py
+-rw-r--r--   0        0        0     5096 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/circuit_to_aqt.py
+-rw-r--r--   0        0        0     5802 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/persistence.py
+-rw-r--r--   0        0        0      616 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/estimator.py
+-rw-r--r--   0        0        0     2471 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/sampler.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/py.typed
+-rw-r--r--   0        0        0      587 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/__init__.py
+-rw-r--r--   0        0        0     2747 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/circuits.py
+-rw-r--r--   0        0        0     2334 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/fixtures.py
+-rw-r--r--   0        0        0     7204 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/resources.py
+-rw-r--r--   0        0        0     1268 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/timeout.py
+-rw-r--r--   0        0        0     2147 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/utils.py
+-rw-r--r--   0        0        0     8081 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/transpiler_plugin.py
+-rw-r--r--   0        0        0     1825 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/utils.py
+-rw-r--r--   0        0        0     1013 2024-04-15 07:48:30.178040 qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/versions.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/__init__.py
+-rw-r--r--   0        0        0     3790 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_api_models.py
+-rw-r--r--   0        0        0     7772 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_circuit_to_aqt.py
+-rw-r--r--   0        0        0    13668 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_execution.py
+-rw-r--r--   0        0        0     9114 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_job_persistence.py
+-rw-r--r--   0        0        0     2159 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_options.py
+-rw-r--r--   0        0        0     6392 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_primitives.py
+-rw-r--r--   0        0        0     8422 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_provider.py
+-rw-r--r--   0        0        0    15445 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_resource.py
+-rw-r--r--   0        0        0     9776 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_transpilation.py
+-rw-r--r--   0        0        0     1102 2024-04-15 07:48:30.182040 qiskit_aqt_provider-1.4.0/test/test_utils.py
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 qiskit_aqt_provider-1.4.0/PKG-INFO
```

### Comparing `qiskit_aqt_provider-1.3.0/CODE_OF_CONDUCT.md` & `qiskit_aqt_provider-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/CONTRIBUTING.md` & `qiskit_aqt_provider-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/LICENSE.txt` & `qiskit_aqt_provider-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/README.md` & `qiskit_aqt_provider-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/pyproject.toml` & `qiskit_aqt_provider-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qiskit-aqt-provider"
-version = "1.3.0"
+version = "1.4.0"
 description = "Qiskit provider for AQT backends"
 authors = ["Qiskit Development Team", "Alpine Quantum Technologies GmbH"]
 repository = "https://github.com/qiskit-community/qiskit-aqt-provider"
 documentation = "https://qiskit-community.github.io/qiskit-aqt-provider"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers=[
@@ -45,15 +45,15 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 
 httpx = ">=0.24.0"
 platformdirs = ">=3"
 pydantic = ">=2.5.0"
 python-dotenv = ">=1"
-qiskit = ">=0.45.1,<1"
+qiskit = "^1"
 qiskit-aer = ">=0.13.2"
 qiskit-algorithms = { version = ">=0.2.1", optional = true }
 qiskit-optimization = { version = ">=0.6.0", optional = true }
 tabulate = ">=0.9.0"
 tqdm = ">=4"
 typing-extensions = ">=4.0.0"
 
@@ -71,17 +71,17 @@
 polyfactory = "^2.0.0"
 pre-commit = "^3.1.1"
 pyproject-fmt = "^1.7.0"
 pytest = ">=7"
 pytest-httpx = "^0.22.0"
 pytest-mock = "^3.11.1"
 pytest-sugar = "^0.9.6"
-qiskit-experiments = "^0.5.4"
+qiskit-experiments = "^0.6.0"
 qiskit-sphinx-theme = ">=1.16.0"
-qiskit-terra = {version = ">=0.23.2", extras = ["visualization"]}
+qiskit = {version = "^1", extras = ["visualization"]}
 rich = "^13.5.3"
 ruff = "^0.2.0"
 sphinx = "^7"
 tomlkit = "^0.12.1"
 typer = "^0.7.0"
 types-requests = "^2.28.11"
 types-setuptools = "^65.7.0"
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/__init__.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/api_models.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/api_models_generated.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/api_models_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,20 +211,22 @@
 
     model_config = ConfigDict(
         frozen=True,
     )
     root: Annotated[
         List[OperationModel],
         Field(
-            examples=[[
-                {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                {"operation": "R", "phi": 0.25, "qubit": 1, "theta": 0.5},
-                {"operation": "RXX", "qubits": [0, 1], "theta": 0.5},
-                {"operation": "MEASURE"},
-            ]],
+            examples=[
+                [
+                    {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                    {"operation": "R", "phi": 0.25, "qubit": 1, "theta": 0.5},
+                    {"operation": "RXX", "qubits": [0, 1], "theta": 0.5},
+                    {"operation": "MEASURE"},
+                ]
+            ],
             max_length=10000,
             min_length=1,
             title="Circuit",
         ),
     ]
     """
     Json encoding of a quantum circuit.
@@ -336,33 +338,35 @@
                     "summary": "Queued Job",
                     "value": {
                         "job": {
                             "job_id": "ccaa39de-d0f3-4c8b-bdb1-4d74f0c2f450",
                             "job_type": "quantum_circuit",
                             "label": "Example computation",
                             "payload": {
-                                "circuits": [{
-                                    "number_of_qubits": 2,
-                                    "quantum_circuit": [
-                                        {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                                        {
-                                            "operation": "R",
-                                            "phi": 0.25,
-                                            "qubit": 1,
-                                            "theta": 0.5,
-                                        },
-                                        {
-                                            "operation": "RXX",
-                                            "qubits": [0, 1],
-                                            "theta": 0.5,
-                                        },
-                                        {"operation": "MEASURE"},
-                                    ],
-                                    "repetitions": 5,
-                                }]
+                                "circuits": [
+                                    {
+                                        "number_of_qubits": 2,
+                                        "quantum_circuit": [
+                                            {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                                            {
+                                                "operation": "R",
+                                                "phi": 0.25,
+                                                "qubit": 1,
+                                                "theta": 0.5,
+                                            },
+                                            {
+                                                "operation": "RXX",
+                                                "qubits": [0, 1],
+                                                "theta": 0.5,
+                                            },
+                                            {"operation": "MEASURE"},
+                                        ],
+                                        "repetitions": 5,
+                                    }
+                                ]
                             },
                         },
                         "response": {"status": "queued"},
                     },
                 },
                 {
                     "description": (
@@ -371,33 +375,35 @@
                     "summary": "Ongoing Job",
                     "value": {
                         "job": {
                             "job_id": "ccaa39de-d0f3-4c8b-bdb1-4d74f0c2f450",
                             "job_type": "quantum_circuit",
                             "label": "Example computation",
                             "payload": {
-                                "circuits": [{
-                                    "number_of_qubits": 2,
-                                    "quantum_circuit": [
-                                        {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                                        {
-                                            "operation": "R",
-                                            "phi": 0.25,
-                                            "qubit": 1,
-                                            "theta": 0.5,
-                                        },
-                                        {
-                                            "operation": "RXX",
-                                            "qubits": [0, 1],
-                                            "theta": 0.5,
-                                        },
-                                        {"operation": "MEASURE"},
-                                    ],
-                                    "repetitions": 5,
-                                }]
+                                "circuits": [
+                                    {
+                                        "number_of_qubits": 2,
+                                        "quantum_circuit": [
+                                            {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                                            {
+                                                "operation": "R",
+                                                "phi": 0.25,
+                                                "qubit": 1,
+                                                "theta": 0.5,
+                                            },
+                                            {
+                                                "operation": "RXX",
+                                                "qubits": [0, 1],
+                                                "theta": 0.5,
+                                            },
+                                            {"operation": "MEASURE"},
+                                        ],
+                                        "repetitions": 5,
+                                    }
+                                ]
                             },
                         },
                         "response": {"finished_count": 0, "status": "ongoing"},
                     },
                 },
                 {
                     "description": (
@@ -407,33 +413,35 @@
                     "summary": "Failed Job",
                     "value": {
                         "job": {
                             "job_id": "ccaa39de-d0f3-4c8b-bdb1-4d74f0c2f450",
                             "job_type": "quantum_circuit",
                             "label": "Example computation",
                             "payload": {
-                                "circuits": [{
-                                    "number_of_qubits": 2,
-                                    "quantum_circuit": [
-                                        {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                                        {
-                                            "operation": "R",
-                                            "phi": 0.25,
-                                            "qubit": 1,
-                                            "theta": 0.5,
-                                        },
-                                        {
-                                            "operation": "RXX",
-                                            "qubits": [0, 1],
-                                            "theta": 0.5,
-                                        },
-                                        {"operation": "MEASURE"},
-                                    ],
-                                    "repetitions": 5,
-                                }]
+                                "circuits": [
+                                    {
+                                        "number_of_qubits": 2,
+                                        "quantum_circuit": [
+                                            {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                                            {
+                                                "operation": "R",
+                                                "phi": 0.25,
+                                                "qubit": 1,
+                                                "theta": 0.5,
+                                            },
+                                            {
+                                                "operation": "RXX",
+                                                "qubits": [0, 1],
+                                                "theta": 0.5,
+                                            },
+                                            {"operation": "MEASURE"},
+                                        ],
+                                        "repetitions": 5,
+                                    }
+                                ]
                             },
                         },
                         "response": {
                             "message": "detailed error message",
                             "status": "error",
                         },
                     },
@@ -446,33 +454,35 @@
                     "summary": "Cancelled Job",
                     "value": {
                         "job": {
                             "job_id": "ccaa39de-d0f3-4c8b-bdb1-4d74f0c2f450",
                             "job_type": "quantum_circuit",
                             "label": "Example computation",
                             "payload": {
-                                "circuits": [{
-                                    "number_of_qubits": 2,
-                                    "quantum_circuit": [
-                                        {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                                        {
-                                            "operation": "R",
-                                            "phi": 0.25,
-                                            "qubit": 1,
-                                            "theta": 0.5,
-                                        },
-                                        {
-                                            "operation": "RXX",
-                                            "qubits": [0, 1],
-                                            "theta": 0.5,
-                                        },
-                                        {"operation": "MEASURE"},
-                                    ],
-                                    "repetitions": 5,
-                                }]
+                                "circuits": [
+                                    {
+                                        "number_of_qubits": 2,
+                                        "quantum_circuit": [
+                                            {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                                            {
+                                                "operation": "R",
+                                                "phi": 0.25,
+                                                "qubit": 1,
+                                                "theta": 0.5,
+                                            },
+                                            {
+                                                "operation": "RXX",
+                                                "qubits": [0, 1],
+                                                "theta": 0.5,
+                                            },
+                                            {"operation": "MEASURE"},
+                                        ],
+                                        "repetitions": 5,
+                                    }
+                                ]
                             },
                         },
                         "response": {"status": "cancelled"},
                     },
                 },
                 {
                     "description": (
@@ -482,33 +492,35 @@
                     "summary": "Finished Job",
                     "value": {
                         "job": {
                             "job_id": "ccaa39de-d0f3-4c8b-bdb1-4d74f0c2f450",
                             "job_type": "quantum_circuit",
                             "label": "Example computation",
                             "payload": {
-                                "circuits": [{
-                                    "number_of_qubits": 2,
-                                    "quantum_circuit": [
-                                        {"operation": "RZ", "phi": 0.5, "qubit": 0},
-                                        {
-                                            "operation": "R",
-                                            "phi": 0.25,
-                                            "qubit": 1,
-                                            "theta": 0.5,
-                                        },
-                                        {
-                                            "operation": "RXX",
-                                            "qubits": [0, 1],
-                                            "theta": 0.5,
-                                        },
-                                        {"operation": "MEASURE"},
-                                    ],
-                                    "repetitions": 5,
-                                }]
+                                "circuits": [
+                                    {
+                                        "number_of_qubits": 2,
+                                        "quantum_circuit": [
+                                            {"operation": "RZ", "phi": 0.5, "qubit": 0},
+                                            {
+                                                "operation": "R",
+                                                "phi": 0.25,
+                                                "qubit": 1,
+                                                "theta": 0.5,
+                                            },
+                                            {
+                                                "operation": "RXX",
+                                                "qubits": [0, 1],
+                                                "theta": 0.5,
+                                            },
+                                            {"operation": "MEASURE"},
+                                        ],
+                                        "repetitions": 5,
+                                    }
+                                ]
                             },
                         },
                         "response": {
                             "result": {"0": [[1, 0], [1, 1], [0, 0], [1, 1], [1, 1]]},
                             "status": "finished",
                         },
                     },
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_job.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_options.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     """Whether to display a progress bar when waiting for results from a single job.
 
     When enabled, the progress bar is written to :data:`sys.stderr`."""
 
     @pdt.field_validator("query_timeout_seconds")
     @classmethod
     def validate_timeout(cls, value: Optional[float], info: pdt.ValidationInfo) -> Optional[float]:
+        """Enforce that the timeout, if set, is strictly positive."""
         if value is not None and value <= 0.0:
             raise ValueError(f"{info.field_name} must be None or > 0.")
 
         return value
 
     def update_options(self, **kwargs: Any) -> Self:
         """Update options by name.
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_provider.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/aqt_resource.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/aqt_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/circuit_to_aqt.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/persistence.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/persistence.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/__init__.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/estimator.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from qiskit.primitives import BackendEstimator
 
 from qiskit_aqt_provider import transpiler_plugin
 from qiskit_aqt_provider.aqt_resource import AQTResource, make_transpiler_target
 
 
 class AQTEstimator(BackendEstimator):
-    """:class:`Estimator <qiskit.primitives.Estimator>` primitive for AQT backends."""
+    """:class:`BaseEstimatorV1 <qiskit.primitives.BaseEstimatorV1>` primitive for AQT backends."""
 
     _backend: AQTResource
 
     def __init__(
         self,
         backend: AQTResource,
         options: Optional[dict[str, Any]] = None,
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/primitives/sampler.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/primitives/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from qiskit.primitives import BackendSampler
 
 from qiskit_aqt_provider import transpiler_plugin
 from qiskit_aqt_provider.aqt_resource import AQTResource, make_transpiler_target
 
 
 class AQTSampler(BackendSampler):
-    """:class:`Sampler <qiskit.primitives.Sampler>` primitive for AQT backends."""
+    """:class:`BaseSamplerV1 <qiskit.primitives.BaseSamplerV1>` primitive for AQT backends."""
 
     _backend: AQTResource
 
     def __init__(
         self,
         backend: AQTResource,
         options: Optional[dict[str, Any]] = None,
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/__init__.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/circuits.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/fixtures.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/resources.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/resources.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/timeout.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/timeout.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/test/utils.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/transpiler_plugin.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/transpiler_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 import math
+from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import Final, Optional
 
 import numpy as np
 from qiskit import QuantumCircuit
 from qiskit.circuit import Gate, Instruction
 from qiskit.circuit.library import RGate, RXGate, RXXGate, RZGate
@@ -193,15 +194,15 @@
     register a :class:`WrapRxxAngles` pass after the preset pass irrespective
     of the optimization level.
     """
 
     def pass_manager(
         self,
         pass_manager_config: PassManagerConfig,
-        optimization_level: Optional[int] = None,  # noqa: ARG002
+        optimization_level: Optional[int] = None,
     ) -> PassManager:
         translation_pm = common.generate_translation_passmanager(
             target=pass_manager_config.target,
             basis_gates=pass_manager_config.basis_gates,
             approximation_degree=pass_manager_config.approximation_degree,
             coupling_map=pass_manager_config.coupling_map,
             backend_props=pass_manager_config.backend_properties,
@@ -209,10 +210,18 @@
             unitary_synthesis_plugin_config=pass_manager_config.unitary_synthesis_plugin_config,
             hls_config=pass_manager_config.hls_config,
         )
 
         if isinstance(pass_manager_config.target, UnboundParametersTarget):
             return translation_pm
 
-        passes: list[BasePass] = [WrapRxxAngles()]
+        passes: Sequence[BasePass] = [
+            WrapRxxAngles(),
+        ] + (
+            [
+                Decompose([f"{WrapRxxAngles.SUBSTITUTE_GATE_NAME}*"]),
+            ]
+            if optimization_level is None or optimization_level == 0
+            else []
+        )
 
         return translation_pm + PassManager(passes)
```

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/utils.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/qiskit_aqt_provider/versions.py` & `qiskit_aqt_provider-1.4.0/qiskit_aqt_provider/versions.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_api_models.py` & `qiskit_aqt_provider-1.4.0/test/test_api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_circuit_to_aqt.py` & `qiskit_aqt_provider-1.4.0/test/test_circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_execution.py` & `qiskit_aqt_provider-1.4.0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_job_persistence.py` & `qiskit_aqt_provider-1.4.0/test/test_job_persistence.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_options.py` & `qiskit_aqt_provider-1.4.0/test/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_primitives.py` & `qiskit_aqt_provider-1.4.0/test/test_primitives.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,59 +6,50 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-import importlib.metadata
 from math import isclose, pi
 from typing import Callable
 
 import pytest
 import qiskit
 from qiskit.circuit import Parameter, QuantumCircuit
-from qiskit.primitives import BackendSampler, BaseSampler, Sampler
+from qiskit.primitives import (
+    BackendEstimator,
+    BackendSampler,
+    BaseEstimatorV1,
+    BaseSamplerV1,
+    Sampler,
+)
 from qiskit.providers import Backend
 from qiskit.quantum_info import SparsePauliOp
 from qiskit.transpiler.exceptions import TranspilerError
 
 from qiskit_aqt_provider.aqt_resource import AQTResource
 from qiskit_aqt_provider.primitives import AQTSampler
 from qiskit_aqt_provider.primitives.estimator import AQTEstimator
 from qiskit_aqt_provider.test.circuits import assert_circuits_equal
 from qiskit_aqt_provider.test.fixtures import MockSimulator
 
 
-@pytest.mark.skipif(
-    importlib.metadata.version("qiskit-terra") >= "0.24.0",
-    reason="qiskit.opflow is deprecated in qiskit-terra>=0.24",
-)
-def test_circuit_sampling_opflow(
-    offline_simulator_no_noise: AQTResource,
-) -> None:  # pragma: no cover
-    """Check that an `AQTResource` can be used as backend for the legacy
-    `opflow.CircuitSampler` with parametric circuits.
-    """
-    from qiskit.opflow import CircuitSampler, StateFn
-
-    theta = Parameter("θ")
-
-    qc = QuantumCircuit(2)
-    qc.rx(theta, 0)
-    qc.ry(theta, 0)
-    qc.rz(theta, 0)
-    qc.rxx(theta, 0, 1)
+def test_backend_primitives_are_v1() -> None:
+    """Check that `BackendSampler` and `BackendEstimator` have primitives V1 interfaces.
 
-    assert qc.num_parameters > 0
+    As of 2024-02-20, there are no backend primitives that provide V2 interfaces.
 
-    sampler = CircuitSampler(offline_simulator_no_noise)
+    If this test fails, the `AQTSampler` and `AQTEstimator` docs as well as the user
+    guide must be updated.
 
-    sampled = sampler.convert(StateFn(qc), params={theta: pi}).eval()
-    assert sampled.to_matrix().tolist() == [[0.0, 0.0, 0.0, 1.0]]
+    An interface mismatch may be detected at other spots. This makes the detection explicit.
+    """
+    assert issubclass(BackendSampler, BaseSamplerV1)
+    assert issubclass(BackendEstimator, BaseEstimatorV1)
 
 
 @pytest.mark.parametrize(
     "get_sampler",
     [
         # Reference implementation
         lambda _: Sampler(),
@@ -71,15 +62,15 @@
         ),
         # The specialized implementation of the Sampler primitive for AQT backends delays the
         # transpilation passes that require bound parameters.
         lambda backend: AQTSampler(backend),
     ],
 )
 def test_circuit_sampling_primitive(
-    get_sampler: Callable[[Backend], BaseSampler],
+    get_sampler: Callable[[Backend], BaseSamplerV1],
     offline_simulator_no_noise: AQTResource,
 ) -> None:
     """Check that a `Sampler` primitive using an AQT backend can sample parametric circuits."""
     theta = Parameter("θ")
 
     qc = QuantumCircuit(2)
     qc.rx(theta, 0)
```

### Comparing `qiskit_aqt_provider-1.3.0/test/test_provider.py` & `qiskit_aqt_provider-1.4.0/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_resource.py` & `qiskit_aqt_provider-1.4.0/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/test/test_transpilation.py` & `qiskit_aqt_provider-1.4.0/test/test_transpilation.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # that they have been altered from the originals.
 
 
 from math import pi
 from typing import Union
 
 import pytest
-from hypothesis import assume, given
+from hypothesis import assume, example, given
 from hypothesis import strategies as st
 from qiskit import QuantumCircuit, transpile
 from qiskit.circuit.library import RXGate, RYGate
 
 from qiskit_aqt_provider.aqt_resource import AQTResource
 from qiskit_aqt_provider.test.circuits import (
     assert_circuits_equal,
@@ -56,15 +56,15 @@
     reference.rx(input_theta, 0)
 
     assert_circuits_equal(result, expected)
     assert_circuits_equivalent(result, reference)
 
 
 @given(theta=st.floats(allow_nan=False, min_value=-1000 * pi, max_value=1000 * pi))
-@pytest.mark.parametrize("optimization_level", [1, 2, 3])
+@pytest.mark.parametrize("optimization_level", [0, 1, 2, 3])
 @pytest.mark.parametrize("test_gate", [RXGate, RYGate])
 def test_rx_ry_rewrite_transpile(
     theta: float,
     optimization_level: int,
     test_gate: Union[RXGate, RYGate],
 ) -> None:
     """Test the rewrite rule: Rx(θ), Ry(θ) → R(θ, φ), θ ∈ [0, π], φ ∈ [0, 2π]."""
@@ -198,15 +198,15 @@
         allow_nan=False,
         allow_infinity=False,
         min_value=-1000 * pi,
         max_value=1000 * pi,
     )
 )
 @pytest.mark.parametrize("qubits", [3])
-@pytest.mark.parametrize("optimization_level", [1, 2, 3])
+@pytest.mark.parametrize("optimization_level", [0, 1, 2, 3])
 def test_rxx_wrap_angle_transpile(angle: float, qubits: int, optimization_level: int) -> None:
     """Check that Rxx angles are wrapped by the transpiler."""
     assume(abs(angle) > pi / 200)
 
     qc = QuantumCircuit(qubits)
     qc.rxx(angle, 0, 1)
 
@@ -214,33 +214,67 @@
     backend = MockSimulator(noisy=False)
     trans_qc = transpile(qc, backend, optimization_level=optimization_level)
     assert isinstance(trans_qc, QuantumCircuit)
 
     assert_circuits_equivalent(trans_qc, qc)
 
     assert set(trans_qc.count_ops()) <= set(backend.configuration().basis_gates)
-    num_rxx = trans_qc.count_ops().get("rxx")
+    num_rxx = trans_qc.count_ops().get("rxx", 0)
 
-    # in high optimization levels, the gate might be dropped
-    assume(num_rxx is not None)
-    assert num_rxx == 1
+    # Higher optimization levels can optimize e.g. Rxx(2n*π) = Identity away.
+    assert num_rxx <= 1
 
-    # check that all Rxx have angles in [0, π/2]
+    # check that the Rxx gate has angle in [0, π/2]
     for operation in trans_qc.data:
         instruction = operation[0]
         if instruction.name == "rxx":
             (theta,) = instruction.params
             assert 0 <= float(theta) <= pi / 2
-            break  # there's only one Rxx gate in the circuit
+            break
     else:  # pragma: no cover
-        pytest.fail("Transpiled circuit contains no Rxx gate.")
+        if num_rxx > 0:
+            pytest.fail("Transpiled circuit contains no Rxx gate.")
+
+
+@example(angles_pi=[-582.16 / pi])
+@given(
+    angles_pi=st.lists(
+        st.floats(min_value=-1000.0, max_value=1000.0, allow_nan=False),
+        min_size=1,
+        max_size=4,
+    )
+)
+@pytest.mark.parametrize("optimization_level", [0, 1, 2, 3])
+def test_transpilation_preserves_or_decreases_number_of_rxx_gates(
+    angles_pi: list[float], optimization_level: int
+) -> None:
+    """Check that transpilation at least preserves the number of RXX gates."""
+    if optimization_level > 1:
+        # FIXME: remove once https://github.com/Qiskit/qiskit/issues/12051 is fixed.
+        assume(len(angles_pi) == 1)
+
+    qc = QuantumCircuit(2)
+
+    for angle_pi in angles_pi:
+        qc.rxx(angle_pi * pi, 0, 1)
+
+    # we only need the backend's transpilation target for this test
+    backend = MockSimulator(noisy=False)
+    tr_qc = transpile(qc, backend, optimization_level=optimization_level)
+
+    tr_qc_ops = tr_qc.count_ops()
+    assert set(tr_qc_ops) <= set(backend.configuration().basis_gates)
+
+    qc_rxx = qc.count_ops()["rxx"]
+    assert qc_rxx == len(angles_pi)
+    assert tr_qc_ops.get("rxx", 0) <= qc_rxx
 
 
 @pytest.mark.parametrize("qubits", [1, 5, 10])
-@pytest.mark.parametrize("optimization_level", [1, 2, 3])
+@pytest.mark.parametrize("optimization_level", [0, 1, 2, 3])
 def test_qft_circuit_transpilation(
     qubits: int, optimization_level: int, offline_simulator_no_noise: AQTResource
 ) -> None:
     """Transpile a N-qubit QFT circuit for an AQT backend. Check that the angles are properly
     wrapped.
     """
     qc = qft_circuit(qubits)
```

### Comparing `qiskit_aqt_provider-1.3.0/test/test_utils.py` & `qiskit_aqt_provider-1.4.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider-1.3.0/PKG-INFO` & `qiskit_aqt_provider-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-aqt-provider
-Version: 1.3.0
+Version: 1.4.0
 Summary: Qiskit provider for AQT backends
 Home-page: https://github.com/qiskit-community/qiskit-aqt-provider
 License: Apache-2.0
 Keywords: qiskit,sdk,quantum
 Author: Qiskit Development Team
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: examples
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: platformdirs (>=3)
 Requires-Dist: pydantic (>=2.5.0)
 Requires-Dist: python-dotenv (>=1)
-Requires-Dist: qiskit (>=0.45.1,<1)
+Requires-Dist: qiskit (>=1,<2)
 Requires-Dist: qiskit-aer (>=0.13.2)
 Requires-Dist: qiskit-algorithms (>=0.2.1) ; extra == "examples"
 Requires-Dist: qiskit-optimization (>=0.6.0) ; extra == "examples"
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: tqdm (>=4)
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Documentation, https://qiskit-community.github.io/qiskit-aqt-provider
```

