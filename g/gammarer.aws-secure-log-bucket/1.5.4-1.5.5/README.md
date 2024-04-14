# Comparing `tmp/gammarer.aws-secure-log-bucket-1.5.4.tar.gz` & `tmp/gammarer.aws-secure-log-bucket-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-log-bucket-1.5.4.tar", last modified: Sun Apr  7 18:22:24 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-log-bucket-1.5.5.tar", last modified: Sun Apr 14 23:00:18 2024, max compression
```

## Comparing `gammarer.aws-secure-log-bucket-1.5.4.tar` & `gammarer.aws-secure-log-bucket-1.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.088228 gammarer.aws-secure-log-bucket-1.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.088228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24438 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.165587 gammarer.aws-secure-log-bucket-1.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.165587 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24433 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:00:06.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:18.169587 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-14 23:00:18.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-14 23:00:18.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:00:18.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-14 23:00:18.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 23:00:18.000000 gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/LICENSE` & `gammarer.aws-secure-log-bucket-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/PKG-INFO` & `gammarer.aws-secure-log-bucket-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-log-bucket
-Version: 1.5.4
+Version: 1.5.5
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarer/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/README.md` & `gammarer.aws-secure-log-bucket-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/setup.py` & `gammarer.aws-secure-log-bucket-1.5.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-log-bucket",
-    "version": "1.5.4",
+    "version": "1.5.5",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "gammarer.aws_secure_log_bucket",
         "gammarer.aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@1.5.4.jsii.tgz"
+            "aws-secure-log-bucket@1.5.5.jsii.tgz"
         ],
         "gammarer.aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "gammarer.aws-secure-bucket>=1.1.0, <1.2.0",
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

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/__init__.py` & `gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py` & `gammarer.aws-secure-log-bucket-1.5.5/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-log-bucket",
-    "1.5.4",
+    "1.5.5",
     __name__[0:-6],
-    "aws-secure-log-bucket@1.5.4.jsii.tgz",
+    "aws-secure-log-bucket@1.5.5.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-log-bucket
-Version: 1.5.4
+Version: 1.5.5
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarer/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-log-bucket-1.5.5/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_log_bucket/__init__.py
 src/gammarer/aws_secure_log_bucket/py.typed
 src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.4.jsii.tgz
+src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.5.jsii.tgz
```

