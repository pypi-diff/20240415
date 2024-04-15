# Comparing `tmp/mrgrain.cdk-esbuild-5.0.8.tar.gz` & `tmp/mrgrain.cdk-esbuild-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-5.0.8.tar", last modified: Sun Dec 24 15:29:08 2023, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-5.0.9.tar", last modified: Mon Jan  1 05:06:42 2024, max compression
```

## Comparing `mrgrain.cdk-esbuild-5.0.8.tar` & `mrgrain.cdk-esbuild-5.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19422 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18514 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.720520 mrgrain.cdk-esbuild-5.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.720520 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (127)   354597 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79492 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 15:28:58.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 15:29:08.724520 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19422 2023-12-24 15:29:08.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-24 15:29:08.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 15:29:08.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-24 15:29:08.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-24 15:29:08.000000 mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19422 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (127)   354597 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80145 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19422 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-5.0.8/LICENSE` & `mrgrain.cdk-esbuild-5.0.9/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Moritz Kornher
+Copyright (c) 2024 Moritz Kornher
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mrgrain.cdk-esbuild-5.0.8/PKG-INFO` & `mrgrain.cdk-esbuild-5.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.0.8
+Version: 5.0.9
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `mrgrain.cdk-esbuild-5.0.8/README.md` & `mrgrain.cdk-esbuild-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.0.8/setup.py` & `mrgrain.cdk-esbuild-5.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "5.0.8",
+    "version": "5.0.9",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@5.0.8.jsii.tgz"
+            "cdk-esbuild@5.0.9.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `mrgrain.cdk-esbuild-5.0.8/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.0.8/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.0.8
+Version: 5.0.9
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

