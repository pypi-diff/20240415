# Comparing `tmp/openshift_operator_utilities-1.0.5.tar.gz` & `tmp/openshift_operator_utilities-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_operator_utilities-1.0.5.tar", max compression
+gzip compressed data, was "openshift_operator_utilities-1.0.6.tar", max compression
```

## Comparing `openshift_operator_utilities-1.0.5.tar` & `openshift_operator_utilities-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-01-17 15:15:55.659009 openshift_operator_utilities-1.0.5/LICENSE
--rw-r--r--   0        0        0       86 2024-01-17 15:15:55.659009 openshift_operator_utilities-1.0.5/README.md
--rw-r--r--   0        0        0      711 2024-01-17 15:16:00.314965 openshift_operator_utilities-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-17 15:15:55.664009 openshift_operator_utilities-1.0.5/utilities/__init__.py
--rw-r--r--   0        0        0      364 2024-01-17 15:15:55.664009 openshift_operator_utilities-1.0.5/utilities/infra.py
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 openshift_operator_utilities-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 19:17:42.596719 openshift_operator_utilities-1.0.6/LICENSE
+-rw-r--r--   0        0        0       86 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/constants.py
+-rw-r--r--   0        0        0      340 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/exceptions.py
+-rw-r--r--   0        0        0     3492 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/hyperconverged.py
+-rw-r--r--   0        0        0     4650 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/infra.py
+-rw-r--r--   0        0        0     2937 2024-04-15 19:17:42.597719 openshift_operator_utilities-1.0.6/operator_utilities/olm.py
+-rw-r--r--   0        0        0     1153 2024-04-15 19:17:46.428693 openshift_operator_utilities-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 openshift_operator_utilities-1.0.6/PKG-INFO
```

### Comparing `openshift_operator_utilities-1.0.5/LICENSE` & `openshift_operator_utilities-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_operator_utilities-1.0.5/PKG-INFO` & `openshift_operator_utilities-1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: openshift-operator-utilities
-Version: 1.0.5
+Version: 1.0.6
 Summary: Utilities to interact with openshift operators
+Home-page: https://github.com/RedHatQE/openshift-operator-utilities
 License: Apache License
 Author: dbasunag
 Author-email: dbasunag@redhat.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: openshift-python-utilities (>=5.0.16,<6.0.0)
 Requires-Dist: openshift-python-wrapper (>=10.0.0,<11.0.0)
+Project-URL: Documentation, https://github.com/RedHatQE/openshift-operator-utilities/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # openshift-operator-utilities
 Utilities to interact with various openshift operators
```

