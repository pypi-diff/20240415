# Comparing `tmp/cdk8s-plus-29-2.0.0.tar.gz` & `tmp/cdk8s-plus-29-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-29-2.0.0.tar", last modified: Mon Apr 15 06:04:34 2024, max compression
+gzip compressed data, was "cdk8s-plus-29-2.0.1.tar", last modified: Mon Apr 15 06:35:33 2024, max compression
```

## Comparing `cdk8s-plus-29-2.0.0.tar` & `cdk8s-plus-29-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.619425 cdk8s-plus-29-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 06:04:34.619425 cdk8s-plus-29-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:04:34.619425 cdk8s-plus-29-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.611425 cdk8s-plus-29-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.615425 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/
--rw-r--r--   0 runner    (1001) docker     (127)  1167638 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.615425 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1346713 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/_jsii/cdk8s-plus-29@2.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.615425 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)  3031236 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:04:24.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:04:34.615425 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 06:04:34.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 06:04:34.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:04:34.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 06:04:34.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 06:04:34.000000 cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.334792 cdk8s-plus-29-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 06:35:33.334792 cdk8s-plus-29-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:35:33.334792 cdk8s-plus-29-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.326792 cdk8s-plus-29-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.330792 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/
+-rw-r--r--   0 runner    (1001) docker     (127)  1167638 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.330792 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1345198 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/_jsii/cdk8s-plus-29@2.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.330792 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)  3031236 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:35:23.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:35:33.330792 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 06:35:33.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 06:35:33.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:35:33.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 06:35:33.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 06:35:33.000000 cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-29-2.0.0/LICENSE` & `cdk8s-plus-29-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-29-2.0.0/PKG-INFO` & `cdk8s-plus-29-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-29
-Version: 2.0.0
+Version: 2.0.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-29 synthesizes Kubernetes manifests for Kubernetes 1.29.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-29-2.0.0/README.md` & `cdk8s-plus-29-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-29-2.0.0/setup.py` & `cdk8s-plus-29-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-29",
-    "version": "2.0.0",
+    "version": "2.0.1",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-29 synthesizes Kubernetes manifests for Kubernetes 1.29.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_29",
         "cdk8s_plus_29._jsii",
         "cdk8s_plus_29.k8s"
     ],
     "package_data": {
         "cdk8s_plus_29._jsii": [
-            "cdk8s-plus-29@2.0.0.jsii.tgz"
+            "cdk8s-plus-29@2.0.1.jsii.tgz"
         ],
         "cdk8s_plus_29": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/__init__.py` & `cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-29-2.0.0/src/cdk8s_plus_29/k8s/__init__.py` & `cdk8s-plus-29-2.0.1/src/cdk8s_plus_29/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-29-2.0.0/src/cdk8s_plus_29.egg-info/PKG-INFO` & `cdk8s-plus-29-2.0.1/src/cdk8s_plus_29.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-29
-Version: 2.0.0
+Version: 2.0.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-29 synthesizes Kubernetes manifests for Kubernetes 1.29.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

