# Comparing `tmp/gammarer.aws-secure-bucket-1.2.1.tar.gz` & `tmp/gammarer.aws-secure-bucket-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-bucket-1.2.1.tar", last modified: Sun Apr  7 17:14:11 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-bucket-1.2.2.tar", last modified: Sun Apr 14 22:48:49 2024, max compression
```

## Comparing `gammarer.aws-secure-bucket-1.2.1.tar` & `gammarer.aws-secure-bucket-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.936133 gammarer.aws-secure-bucket-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.936133 gammarer.aws-secure-bucket-1.2.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:14:01.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:14:11.940133 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-07 17:14:11.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-07 17:14:11.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:14:11.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 17:14:11.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 17:14:11.000000 gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33689 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-bucket-1.2.1/LICENSE` & `gammarer.aws-secure-bucket-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.1/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.2.1
+Version: 1.2.2
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-1.2.1/README.md` & `gammarer.aws-secure-bucket-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.1/setup.py` & `gammarer.aws-secure-bucket-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-bucket",
-    "version": "1.2.1",
+    "version": "1.2.2",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_secure_bucket",
         "gammarer.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@1.2.1.jsii.tgz"
+            "aws-secure-bucket@1.2.2.jsii.tgz"
         ],
         "gammarer.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
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

### Comparing `gammarer.aws-secure-bucket-1.2.1/src/gammarer/aws_secure_bucket/__init__.py` & `gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.2.1
+Version: 1.2.2
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-1.2.1/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_bucket/__init__.py
 src/gammarer/aws_secure_bucket/py.typed
 src/gammarer/aws_secure_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.1.jsii.tgz
+src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.2.jsii.tgz
```

