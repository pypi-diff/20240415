# Comparing `tmp/policy_priority_inference-3.0.4.tar.gz` & `tmp/policy_priority_inference-3.0.5.tar.gz`

## Comparing `policy_priority_inference-3.0.4.tar` & `policy_priority_inference-3.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/pypi token.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/src/policy_priority_inference/__init__.py
--rw-r--r--   0        0        0    41044 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/src/policy_priority_inference/policy_priority_inference.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/LICENSE
--rw-r--r--   0        0        0    22098 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/pypi token.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/src/policy_priority_inference/__init__.py
+-rw-r--r--   0        0        0    41044 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/src/policy_priority_inference/policy_priority_inference.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/LICENSE
+-rw-r--r--   0        0        0    22099 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0    22788 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.5/PKG-INFO
```

### Comparing `policy_priority_inference-3.0.4/src/policy_priority_inference/policy_priority_inference.py` & `policy_priority_inference-3.0.5/src/policy_priority_inference/policy_priority_inference.py`

 * *Files identical despite different names*

### Comparing `policy_priority_inference-3.0.4/LICENSE` & `policy_priority_inference-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `policy_priority_inference-3.0.4/README.md` & `policy_priority_inference-3.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Policy Priority Inference
 
-The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm
+The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm.
 
 
 FUNCTIONS:
 
 
     calibrate(I0, IF, success_rates, A=None, R=None, bs=None, qm=None, rl=None, Bs=None, B_dict=None, T=None, threshold=0.8, parallel_processes=None, verbose=False, low_precision_counts=101, increment=1000)
         Function to calibrate the model parameters.
```

### Comparing `policy_priority_inference-3.0.4/pyproject.toml` & `policy_priority_inference-3.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "policy_priority_inference"
-version = "3.0.4"
+version = "3.0.5"
 authors = [
   { name="Omar A. Guerrero", email="oguerrer@gmail.com" },
 ]
 description = "The model of the Policy Priority Inference impact-evaluation toolkit and its calibration algorithm."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `policy_priority_inference-3.0.4/PKG-INFO` & `policy_priority_inference-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: policy_priority_inference
-Version: 3.0.4
+Version: 3.0.5
 Summary: The model of the Policy Priority Inference impact-evaluation toolkit and its calibration algorithm.
 Project-URL: Homepage, https://policypriority.org
 Project-URL: Issues, https://github.com/oguerrer/ppi
 Author-email: "Omar A. Guerrero" <oguerrer@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Policy Priority Inference
 
-The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm
+The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm.
 
 
 FUNCTIONS:
 
 
     calibrate(I0, IF, success_rates, A=None, R=None, bs=None, qm=None, rl=None, Bs=None, B_dict=None, T=None, threshold=0.8, parallel_processes=None, verbose=False, low_precision_counts=101, increment=1000)
         Function to calibrate the model parameters.
```

