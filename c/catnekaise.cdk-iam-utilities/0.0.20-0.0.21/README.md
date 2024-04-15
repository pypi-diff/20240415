# Comparing `tmp/catnekaise.cdk-iam-utilities-0.0.20.tar.gz` & `tmp/catnekaise.cdk-iam-utilities-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.cdk-iam-utilities-0.0.20.tar", last modified: Tue Apr  2 06:56:20 2024, max compression
+gzip compressed data, was "catnekaise.cdk-iam-utilities-0.0.21.tar", last modified: Mon Apr 15 07:26:55 2024, max compression
```

## Comparing `catnekaise.cdk-iam-utilities-0.0.20.tar` & `catnekaise.cdk-iam-utilities-0.0.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:20.040109 catnekaise.cdk-iam-utilities-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-02 06:56:20.040109 catnekaise.cdk-iam-utilities-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:56:20.040109 catnekaise.cdk-iam-utilities-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:20.036109 catnekaise.cdk-iam-utilities-0.0.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:20.036109 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-02 06:56:20.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 06:56:20.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:56:20.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 06:56:20.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 06:56:20.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:20.036109 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)   175274 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:20.036109 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95916 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.20.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:56:09.000000 catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:26:55.001972 catnekaise.cdk-iam-utilities-0.0.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-15 07:26:54.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-15 07:26:54.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:26:54.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:26:54.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:26:54.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)   175274 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:26:55.005972 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95917 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.21.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:26:44.000000 catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/py.typed
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/LICENSE` & `catnekaise.cdk-iam-utilities-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/PKG-INFO` & `catnekaise.cdk-iam-utilities-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.cdk-iam-utilities
-Version: 0.0.20
+Version: 0.0.21
 Summary: Experimental utilities intended for AWS CDK IAM
 Home-page: https://github.com/catnekaise/cdk-iam-utilities.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/cdk-iam-utilities.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/setup.py` & `catnekaise.cdk-iam-utilities-0.0.21/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.cdk-iam-utilities",
-    "version": "0.0.20",
+    "version": "0.0.21",
     "description": "Experimental utilities intended for AWS CDK IAM",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/cdk-iam-utilities.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "catnekaise_cdk_iam_utilities",
         "catnekaise_cdk_iam_utilities._jsii"
     ],
     "package_data": {
         "catnekaise_cdk_iam_utilities._jsii": [
-            "cdk-iam-utilities@0.0.20.jsii.tgz"
+            "cdk-iam-utilities@0.0.21.jsii.tgz"
         ],
         "catnekaise_cdk_iam_utilities": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO` & `catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.cdk-iam-utilities
-Version: 0.0.20
+Version: 0.0.21
 Summary: Experimental utilities intended for AWS CDK IAM
 Home-page: https://github.com/catnekaise/cdk-iam-utilities.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/cdk-iam-utilities.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt` & `catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
 src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
 src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
 src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
 src/catnekaise_cdk_iam_utilities/__init__.py
 src/catnekaise_cdk_iam_utilities/py.typed
 src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
-src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.20.jsii.tgz
+src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.21.jsii.tgz
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.20/src/catnekaise_cdk_iam_utilities/__init__.py` & `catnekaise.cdk-iam-utilities-0.0.21/src/catnekaise_cdk_iam_utilities/__init__.py`

 * *Files identical despite different names*

