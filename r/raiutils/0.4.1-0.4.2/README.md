# Comparing `tmp/raiutils-0.4.1.tar.gz` & `tmp/raiutils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raiutils-0.4.1.tar", last modified: Mon Aug 14 14:08:58 2023, max compression
+gzip compressed data, was "raiutils-0.4.2.tar", last modified: Mon Apr 15 21:13:39 2024, max compression
```

## Comparing `raiutils-0.4.1.tar` & `raiutils-0.4.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.931287 raiutils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-14 14:08:22.000000 raiutils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-14 14:08:22.000000 raiutils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-14 14:08:58.931287 raiutils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-14 14:08:22.000000 raiutils-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/cohort/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/cohort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/cohort/cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/cohort/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/common/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/common/retries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/data_processing/data_processing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.931287 raiutils-0.4.1/raiutils/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/sampling/random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.931287 raiutils-0.4.1/raiutils/webservice/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/webservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-14 14:08:22.000000 raiutils-0.4.1/raiutils/webservice/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.927287 raiutils-0.4.1/raiutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-14 14:08:58.000000 raiutils-0.4.1/raiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-14 14:08:58.000000 raiutils-0.4.1/raiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 14:08:58.000000 raiutils-0.4.1/raiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-14 14:08:58.000000 raiutils-0.4.1/raiutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-14 14:08:58.000000 raiutils-0.4.1/raiutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-14 14:08:22.000000 raiutils-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 14:08:58.931287 raiutils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-14 14:08:22.000000 raiutils-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:08:58.931287 raiutils-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26670 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_data_processing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-14 14:08:22.000000 raiutils-0.4.1/tests/test_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.205897 raiutils-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 21:13:09.000000 raiutils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 21:13:09.000000 raiutils-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-15 21:13:39.205897 raiutils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 21:13:09.000000 raiutils-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.197897 raiutils-0.4.2/raiutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.197897 raiutils-0.4.2/raiutils/cohort/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/cohort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/cohort/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/cohort/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.197897 raiutils-0.4.2/raiutils/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/common/retries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/raiutils/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/data_processing/data_processing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/raiutils/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/raiutils/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/raiutils/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/sampling/random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/raiutils/webservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/webservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 21:13:09.000000 raiutils-0.4.2/raiutils/webservice/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.205897 raiutils-0.4.2/raiutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-15 21:13:39.000000 raiutils-0.4.2/raiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 21:13:39.000000 raiutils-0.4.2/raiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:13:39.000000 raiutils-0.4.2/raiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 21:13:39.000000 raiutils-0.4.2/raiutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 21:13:39.000000 raiutils-0.4.2/raiutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 21:13:09.000000 raiutils-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:13:39.205897 raiutils-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 21:13:09.000000 raiutils-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:13:39.201897 raiutils-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_data_processing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_retry_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-15 21:13:09.000000 raiutils-0.4.2/tests/test_sampling.py
```

### Comparing `raiutils-0.4.1/LICENSE` & `raiutils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/PKG-INFO` & `raiutils-0.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: raiutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Common basic utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
 
 # Responsible AI Utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
+### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 The Responsible AI Utilities package contains common functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets and other packages, as well as notebook examples.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `raiutils-0.4.1/raiutils/cohort/__init__.py` & `raiutils-0.4.2/raiutils/cohort/__init__.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/cohort/cohort.py` & `raiutils-0.4.2/raiutils/cohort/cohort.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
 
 class Cohort:
     """Defines the cohort which will be injected from SDK into the Dashboard.
     :param name: Name of the cohort.
     :type name: str
     """
     def __init__(self, name: str):
-        """Defines the cohort which will be injected from SDK into the Dashboard.
+        """Defines the cohort to be injected from SDK into the Dashboard.
         :param name: Name of the cohort.
         :type name: str
         """
         if not isinstance(name, str):
             raise UserConfigValidationException(
                 "Got unexpected type {0} for cohort name. "
                 "Expected string type.".format(type(name))
```

### Comparing `raiutils-0.4.1/raiutils/cohort/constants.py` & `raiutils-0.4.2/raiutils/cohort/constants.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/common/retries.py` & `raiutils-0.4.2/raiutils/common/retries.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,13 +29,17 @@
             result = function()
             break
         except Exception as e:
             print("{0} attempt failed with exception:".format(action_name))
             print(e)
             if i + 1 != max_retries:
                 print("Will retry after {0} seconds".format(retry_delay))
-                time.sleep(retry_delay)
+                try:
+                    for _ in range(retry_delay):
+                        time.sleep(1)
+                except TypeError:
+                    time.sleep(retry_delay)
                 retry_delay = retry_delay * 2
     else:
         raise RuntimeError(err_msg)
 
     return result
```

### Comparing `raiutils-0.4.1/raiutils/data_processing/data_processing_utils.py` & `raiutils-0.4.2/raiutils/data_processing/data_processing_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             if np.isinf(o) or np.isnan(o):
                 return 0
         # need to escape double quoted string values
         # and other special characters for json
         if isinstance(o, str):
             return json.dumps(o)[1:-1]
         return o
-    elif isinstance(o, datetime.datetime):
+    elif isinstance(o, datetime.datetime) or isinstance(o, pd.Timestamp):
         return o.__str__()
     elif isinstance(o, dict):
         return {k: serialize_json_safe(v, ) for k, v in o.items()}
     elif isinstance(o, list):
         return [serialize_json_safe(v) for v in o]
     elif isinstance(o, tuple):
         return tuple(serialize_json_safe(v) for v in o)
```

### Comparing `raiutils-0.4.1/raiutils/dataset/dataset.py` & `raiutils-0.4.2/raiutils/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/exceptions.py` & `raiutils-0.4.2/raiutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/models/model_utils.py` & `raiutils-0.4.2/raiutils/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/sampling/random_sampling.py` & `raiutils-0.4.2/raiutils/sampling/random_sampling.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils/webservice/webservice.py` & `raiutils-0.4.2/raiutils/webservice/webservice.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/raiutils.egg-info/PKG-INFO` & `raiutils-0.4.2/raiutils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: raiutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Common basic utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
 
 # Responsible AI Utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
+### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 The Responsible AI Utilities package contains common functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets and other packages, as well as notebook examples.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `raiutils-0.4.1/raiutils.egg-info/SOURCES.txt` & `raiutils-0.4.2/raiutils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 raiutils/webservice/webservice.py
 tests/test_cohort.py
 tests/test_data_processing_utils.py
 tests/test_exceptions.py
 tests/test_fetch_dataset.py
 tests/test_model_utils.py
 tests/test_post.py
+tests/test_retry_func.py
 tests/test_sampling.py
```

### Comparing `raiutils-0.4.1/setup.py` & `raiutils-0.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     author="Roman Lutz, Ilya Matiach, Ke Xu",
     author_email="raiwidgets-maintain@microsoft.com",
     description="Common basic utilities used across various RAI tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/responsible-ai-widgets",
     packages=setuptools.find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=install_requires,
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ]
 )
```

### Comparing `raiutils-0.4.1/tests/test_cohort.py` & `raiutils-0.4.2/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/tests/test_data_processing_utils.py` & `raiutils-0.4.2/tests/test_data_processing_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,20 @@
 
     def test_serialize_timestamp(self):
         datetime_str = "2020-10-10"
         datetime_object = datetime.datetime.strptime(datetime_str, "%Y-%m-%d")
         result = serialize_json_safe(datetime_object)
         assert datetime_str in result
 
+    def test_serialize_pandas_timestamp(self):
+        datetime_str = "2020-10-10"
+        datetime_object = pd.Timestamp(datetime_str)
+        result = serialize_json_safe(datetime_object)
+        assert datetime_str in result
+
     def test_serialize_via_json_timestamp(self):
         timestamp_obj = pd.Timestamp(2020, 1, 1)
         assert isinstance(timestamp_obj, pd.Timestamp)
         result = json.dumps(serialize_json_safe(timestamp_obj))
         assert result is not None
         assert "2020" in result
```

### Comparing `raiutils-0.4.1/tests/test_exceptions.py` & `raiutils-0.4.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/tests/test_fetch_dataset.py` & `raiutils-0.4.2/tests/test_fetch_dataset.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/tests/test_model_utils.py` & `raiutils-0.4.2/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `raiutils-0.4.1/tests/test_sampling.py` & `raiutils-0.4.2/tests/test_sampling.py`

 * *Files identical despite different names*

