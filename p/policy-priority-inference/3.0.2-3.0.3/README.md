# Comparing `tmp/policy_priority_inference-3.0.2.tar.gz` & `tmp/policy_priority_inference-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policy_priority_inference-3.0.2.tar", last modified: Fri Feb 24 09:47:50 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `policy_priority_inference-3.0.2.tar` & `policy_priority_inference-3.0.3.tar`

### file list

```diff
@@ -1,11 +1,5 @@
-drwxr-xr-x   0 tequilamambo   (501) staff       (20)        0 2023-02-24 09:47:50.443448 policy_priority_inference-3.0.2/
--rw-r--r--   0 tequilamambo   (501) staff       (20)    22778 2023-02-24 09:47:50.443132 policy_priority_inference-3.0.2/PKG-INFO
--rw-r--r--   0 tequilamambo   (501) staff       (20)    22128 2023-02-22 12:19:09.000000 policy_priority_inference-3.0.2/README.md
-drwxr-xr-x   0 tequilamambo   (501) staff       (20)        0 2023-02-24 09:47:50.442692 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/
--rw-r--r--   0 tequilamambo   (501) staff       (20)    22778 2023-02-24 09:47:50.000000 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/PKG-INFO
--rw-r--r--   0 tequilamambo   (501) staff       (20)      262 2023-02-24 09:47:50.000000 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/SOURCES.txt
--rw-r--r--   0 tequilamambo   (501) staff       (20)        1 2023-02-24 09:47:50.000000 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/dependency_links.txt
--rw-r--r--   0 tequilamambo   (501) staff       (20)       13 2023-02-24 09:47:50.000000 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/requires.txt
--rw-r--r--   0 tequilamambo   (501) staff       (20)        1 2023-02-24 09:47:50.000000 policy_priority_inference-3.0.2/policy_priority_inference.egg-info/top_level.txt
--rw-r--r--   0 tequilamambo   (501) staff       (20)       38 2023-02-24 09:47:50.443524 policy_priority_inference-3.0.2/setup.cfg
--rw-r--r--   0 tequilamambo   (501) staff       (20)     7684 2023-02-24 09:40:20.000000 policy_priority_inference-3.0.2/setup.py
+-rw-r--r--   0        0        0    41044 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.3/src/policy_priority_inference/policy_priority_inference.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.3/LICENSE
+-rw-r--r--   0        0        0    22098 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.3/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 policy_priority_inference-3.0.3/PKG-INFO
```

### Comparing `policy_priority_inference-3.0.2/PKG-INFO` & `policy_priority_inference-3.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: policy_priority_inference
-Version: 3.0.2
-Summary: Library to run the agent-computing model of the Policy Priority Inference research programme.
-Home-page: https://github.com/oguerrer/ppi
-Author: Omar A. Guerrero
-Author-email: oguerrer@gmail.com
-Keywords: ppi,policy priority inference,SDGs
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-
 # Policy Priority Inference
 
-This package contains all the code of PPI's agent-computing model, as well as helper functions to parallelise the Monte Carlo simulations, and the calibration algorithm.
+The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm
 
 
 FUNCTIONS:
 
 
     calibrate(I0, IF, success_rates, A=None, R=None, bs=None, qm=None, rl=None, Bs=None, B_dict=None, T=None, threshold=0.8, parallel_processes=None, verbose=False, low_precision_counts=101, increment=1000)
         Function to calibrate the model parameters.
@@ -234,15 +218,15 @@
                 for that indicator and it will grow indefinitely. If not provided,
                 no indicator will have upper bound.
             Imin: numpy array (optional)
                 Vector with the theoretical lower bound of the indicators. If an entry
                 contains a missing value (NaN), then there is no lower bound defined
                 for that indicator and it will decrease indefinitely. If not provided,
                 no indicator will have lower bound.
-            Bs: numpy ndarray
+            Bs: numpy ndarray (optional)
                 Disbursement schedule across expenditure programs. There are three 
                 options to specify Bs:
                     - A matrix: this is a disaggregated specification of the 
                     disbursement schedule across expenditure programs and time. 
                     The rows correspond to expenditure programs and the columns
                     to simulation periods. Since there may be more or less expenditure 
                     programs than indicators, the number of rows in Bs should be
```

### Comparing `policy_priority_inference-3.0.2/README.md` & `policy_priority_inference-3.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.3
+Name: policy_priority_inference
+Version: 3.0.3
+Summary: The model of the Policy Priority Inference impact-evaluation toolkit and its calibration algorithm.
+Project-URL: Homepage, https://policypriority.org
+Project-URL: Issues, https://github.com/oguerrer/ppi
+Author-email: "Omar A. Guerrero" <oguerrer@gmail.com>
+License-File: LICENSE
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
 # Policy Priority Inference
 
-This package contains all the code of PPI's agent-computing model, as well as helper functions to parallelise the Monte Carlo simulations, and the calibration algorithm.
+The model of the [Policy Priority Inference](https://policypriority.org) impact-evaluation toolkit and its calibration algorithm
 
 
 FUNCTIONS:
 
 
     calibrate(I0, IF, success_rates, A=None, R=None, bs=None, qm=None, rl=None, Bs=None, B_dict=None, T=None, threshold=0.8, parallel_processes=None, verbose=False, low_precision_counts=101, increment=1000)
         Function to calibrate the model parameters.
@@ -218,15 +234,15 @@
                 for that indicator and it will grow indefinitely. If not provided,
                 no indicator will have upper bound.
             Imin: numpy array (optional)
                 Vector with the theoretical lower bound of the indicators. If an entry
                 contains a missing value (NaN), then there is no lower bound defined
                 for that indicator and it will decrease indefinitely. If not provided,
                 no indicator will have lower bound.
-            Bs: numpy ndarray
+            Bs: numpy ndarray (optional)
                 Disbursement schedule across expenditure programs. There are three 
                 options to specify Bs:
                     - A matrix: this is a disaggregated specification of the 
                     disbursement schedule across expenditure programs and time. 
                     The rows correspond to expenditure programs and the columns
                     to simulation periods. Since there may be more or less expenditure 
                     programs than indicators, the number of rows in Bs should be
```

