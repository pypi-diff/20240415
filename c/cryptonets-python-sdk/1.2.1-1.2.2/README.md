# Comparing `tmp/cryptonets_python_sdk-1.2.1.tar.gz` & `tmp/cryptonets_python_sdk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonets_python_sdk-1.2.1.tar", last modified: Fri Apr 12 17:41:41 2024, max compression
+gzip compressed data, was "cryptonets_python_sdk-1.2.2.tar", last modified: Mon Apr 15 21:48:07 2024, max compression
```

## Comparing `cryptonets_python_sdk-1.2.1.tar` & `cryptonets_python_sdk-1.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.1/LICENSE
--rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.1/MANIFEST.in
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/README.md
--rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/setup.cfg
--rw-rw-r--   0 azam      (1000) azam      (1000)     3787 2024-04-12 17:40:59.000000 cryptonets_python_sdk-1.2.1/setup.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.300005 cryptonets_python_sdk-1.2.1/src/
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.300005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.304005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor_modules/
--rw-rw-r--   0 azam      (1000) azam      (1000)    15198 2024-04-09 13:03:31.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor_modules/FaceModule.py
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor_modules/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.304005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.304005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/lib/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/lib/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    44084 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/nativeMethods.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.304005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/decorators.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2964 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/messages.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3670 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/utils.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/cacheType.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    16918 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/configuration.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/loggingLevel.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/supportedPlatforms.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.304005 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-12 17:41:41.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-12 17:41:41.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-12 17:41:41.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       39 2024-04-12 17:41:41.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-12 17:41:41.000000 cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-12 17:41:41.308005 cryptonets_python_sdk-1.2.1/tests/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19915 2024-04-10 12:45:30.000000 cryptonets_python_sdk-1.2.1/tests/test.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.1/tests/test_suite.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.2/LICENSE
+-rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.2/MANIFEST.in
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/README.md
+-rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/setup.cfg
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/setup.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.439253 cryptonets_python_sdk-1.2.2/src/
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    17344 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/lib/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/lib/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    44098 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/nativeMethods.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/decorators.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2964 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/messages.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4641 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/utils.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/cacheType.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    16918 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/configuration.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/loggingLevel.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/supportedPlatforms.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/requires.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/tests/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/tests/test.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/tests/test_suite.py
```

### Comparing `cryptonets_python_sdk-1.2.1/PKG-INFO` & `cryptonets_python_sdk-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets_python_sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.1/README.md` & `cryptonets_python_sdk-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/setup.py` & `cryptonets_python_sdk-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 @author: Private Identity
 """
 NAME = "cryptonets_python_sdk"
 DESCRIPTION = "Cryptonets SDK Library for Python"
 AUTHOR = "Private Identity"
 AUTHOR_EMAIL = "support@private.id"
 URL = "https://privateid.com/"
-VERSION = "1.2.1"
-REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm"]
+VERSION = "1.2.2"
+REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm","exifread"]
 
 LONG_DESCRIPTION = ""
 if os.path.exists("./README.md"):
     with open("README.md", encoding="utf-8") as fp:
         LONG_DESCRIPTION = fp.read()
 setup(
     name=NAME,
```

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/factor_modules/FaceModule.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import string
 import traceback
 from typing import Union, List
 import numpy as np
-
+import json
 from ..handler.nativeMethods import NativeMethods
 from ..helper.decorators import Singleton
 from ..helper.messages import Message
 from ..helper.result_objects.compareResult import FaceCompareResult
 from ..helper.result_objects.deleteResult import FaceDeleteResult
 from ..helper.result_objects.enrollPredictResult import FaceEnrollPredictResult
 from ..helper.result_objects.faceValidationResult import FaceValidationResult
@@ -54,23 +54,35 @@
                 return FaceEnrollPredictResult(
                     message=self.message.EXCEPTION_ERROR_ENROLL
                 )
             else:
                 # we received a json response and thus call is successful
                 call_status = FaceEnrollPredictResult.CALL_STATUS_SUCCESS
 
-            api_response=json_data.get("enroll_onefa", {}).get("api_response", {});
+            c_response=json_data.get("enroll_onefa", {})
+            api_response=c_response.get("api_response", {})
+            face_validation_data=c_response.get("face_validation_data", {})
+            if face_validation_data.get("face_validation_status",0)!=0:
+                return FaceEnrollPredictResult(
+                status=face_validation_data.get("face_validation_status",0),
+                enroll_level=json_data.get("enroll_level", None),
+                puid=api_response.get("puid", None),
+                guid=api_response.get("guid", None),
+                token=api_response.get("token", None),
+                score=api_response.get("score", None),
+                message=c_response.get("message", "something went wrong"),
+                 )
             return FaceEnrollPredictResult(
                 status=call_status,
                 enroll_level=json_data.get("enroll_level", None),
                 puid=api_response.get("puid", None),
                 guid=api_response.get("guid", None),
                 token=api_response.get("token", None),
                 score=api_response.get("score", None),
-                message=api_response.get("message", ""),
+                message=api_response.get("message", "ok"),
             )
         except Exception as e:
             print(e, traceback.format_exc())
             return FaceEnrollPredictResult(message=self.message.EXCEPTION_ERROR_ENROLL)
 
     def predict(
         self, image_data: np.array, config_object: ConfigObject = None
@@ -84,15 +96,39 @@
                 return FaceEnrollPredictResult(
                     message=self.message.EXCEPTION_ERROR_PREDICT
                 )
             else:
                 # we received a json response and thus call is successful
                 call_status = FaceEnrollPredictResult.CALL_STATUS_SUCCESS
 
-            api_response=json_data.get("predict_onefa", {}).get("api_response", {});
+            c_response=json_data.get("predict_onefa", {})
+            api_response=c_response.get("api_response", {})
+            face_validation_data=c_response.get("face_validation_data", {})
+            if face_validation_data.get("face_validation_status",0)!=0:
+                if config_object and json.loads(config_object.get_config_param()).get("neighbors",0)>0:
+                        return [FaceEnrollPredictResult(
+                        status=face_validation_data.get("face_validation_status",0),
+                        enroll_level=json_data.get("enroll_level", None),
+                        puid=api_response.get("puid", None),
+                        guid=api_response.get("guid", None),
+                        token=api_response.get("token", None),
+                        score=api_response.get("score", None),
+                        message=c_response.get("message", "something went wrong"),
+                        )]
+                else:
+                     return FaceEnrollPredictResult(
+                        status=face_validation_data.get("face_validation_status",0),
+                        enroll_level=json_data.get("enroll_level", None),
+                        puid=api_response.get("puid", None),
+                        guid=api_response.get("guid", None),
+                        token=api_response.get("token", None),
+                        score=api_response.get("score", None),
+                        message=c_response.get("message", "something went wrong"),
+                        )
+
             if not api_response.get("PI_list", []):
                 return FaceEnrollPredictResult(
                     status=call_status,
                     enroll_level=json_data.get("enroll_level", None),
                     puid=api_response.get("puid", None),
                     guid=api_response.get("guid", None),
                     token=api_response.get("token", None),
```

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/handler/nativeMethods.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/nativeMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,27 +668,27 @@
 
             rim_height, rim_width, _ = right_image.shape
             rim_size = (
                 right_image.shape[1] * right_image.shape[0] * right_image.shape[2]
             )
             p_buffer_result = c_char_p()
             p_buffer_result_length = c_int()
-            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.15, "face_thresholds_med": 1.15}
+            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.275, "face_thresholds_med": 1.275,"conf_score_thr_enroll":0.2,"conf_score_thr_enroll":0.2}
 
             if config_object and hasattr(config_object, 'get_config_param') and config_object.get_config_param():
                 config_param_str = config_object.get_config_param()
                 config_from_object = json.loads(config_param_str)
                 for key, value in config_object_default.items():
                     if key not in config_from_object:
                         config_from_object[key] = value
                 config_from_object["face_thresholds_rem_bad_emb_default"]=config_from_object["face_thresholds_med"]
                 config_param_str = json.dumps(config_from_object)
             else:
                 config_param_str = json.dumps(config_object_default)
-            print("config_param_str",config_param_str)
+            
             c_config_param = c_char_p(bytes(config_param_str, "utf-8"))
             c_config_param_len = c_int(len(config_param_str))
 
             success = self._spl_so_face.privid_face_compare_files(
                 self._spl_so_face.handle,
                 c_float(fudge_factor),
                 c_config_param,
@@ -757,15 +757,14 @@
                 # Ensure disable_enroll_mf is always added
                 config_dict["disable_enroll_mf"] = True
                 config_json = json.dumps(config_dict)
             else:
                 # Create a new config dict with disable_enroll_mf set to True
                 config_dict = {"disable_enroll_mf": True}
                 config_json = json.dumps(config_dict)
-
             # Common logic for converting the config dict to the required C types
             c_config_param = c_char_p(bytes(config_json, "utf-8"))
             c_config_param_len = c_int(len(config_json))
 
 
             best_input_out = c_uint8()  # uint8_t** best_input_out
             best_input_length = c_int()  # int *best_input_length
@@ -925,15 +924,14 @@
                 byref(c_cropped_face), byref(c_cropped_face_len),
                 byref(c_result), byref(c_result_len))
 
             if not c_result.value or not c_result_len.value:
                 raise Exception("Something went wrong. Couldn't process the image for Document.")
             output_json = json.loads(c_result.value[:c_result_len.value].decode())
 
-
             if output_json.get("doc_face",{}).get("document_data",{}).get("document_validation_status",-1)==0:
                 doc_info = output_json['doc_face']['document_data']['cropped_document_image']['info']
                 face_info = output_json['doc_face']['cropped_face_image']['info']
         
                 cropped_doc_bytes = c_cropped_doc[:c_cropped_doc_len.value]
                 output_json["doc_face"]["cropped_document"] =np.uint8(np.reshape(cropped_doc_bytes, (
                         doc_info['height'], doc_info['width'], doc_info['channels']
```

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/decorators.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/decorators.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/messages.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/messages.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/compareResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk/settings/configuration.py` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/configuration.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/PKG-INFO` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets-python-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.1/src/cryptonets_python_sdk.egg-info/SOURCES.txt` & `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.1/tests/test.py` & `cryptonets_python_sdk-1.2.2/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=line-too-long
 import pathlib
 import sys
 import os
 from timeit import default_timer
 import os
 from PIL import Image
 from termcolor import colored
@@ -409,17 +410,17 @@
     # (face_factor, img1, img2) = setup_compare_test(
     #     "3_predict_cropped_images_0.png", "8.png"
     # )
     # (face_factor, img1, img2) = setup_compare_test("8.png", "8.png")
 
 
     config_param = {
-        PARAMETERS.COLLECTION_NAME:"collection_d",
-        PARAMETERS.ALLOWED_RESULTS: [FaceValidationCode.GlassesOn.value],
-        PARAMETERS.K:100
+        # PARAMETERS.COLLECTION_NAME:"collection_d",
+        # PARAMETERS.ALLOWED_RESULTS: [FaceValidationCode.GlassesOn.value],
+        # PARAMETERS.K:100
 
 
     }
     config_object = ConfigObject(config_param)
 
 
     print(colored("{}\n{}".format("Compare", "=" * 25), "green"))
@@ -456,16 +457,16 @@
     #         compare_handle.first_validation_result,
     #         compare_handle.second_validation_result,
     #     )
     # )
 
     test_enroll(face_factor, test_im,config=config_object)  # => no billing reservation
     
-    result_handle = test_predict(face_factor, test_im, config=config_object) # => no billing reservation
-    # test_delete(face_factor, result_handle, config=config_object)
+    # result_handle = test_predict(face_factor, test_im, config=config_object) # => no billing reservation
+    # # test_delete(face_factor, result_handle, config=config_object)
     # result_handle = test_predict(face_factor, image_path, config=config_object) #
     # result_handle = test_predict(face_factor, image_path)  # => no billing reservation
 
     # test_delete(face_factor)
     # test_predict_enrol_valid_image_with_no_cache()
     # test_valid_with_cache()
     # test_valid(face_factor, "/home/azam/projects/openinfer/python sdk/cryptonets-python-sdk/docs/source/Usage/images/johny.jpg")
```

### Comparing `cryptonets_python_sdk-1.2.1/tests/test_suite.py` & `cryptonets_python_sdk-1.2.2/tests/test_suite.py`

 * *Files identical despite different names*

