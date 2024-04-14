# Comparing `tmp/genflowly_lambda_utils-0.0.6.tar.gz` & `tmp/genflowly_lambda_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly_lambda_utils-0.0.6.tar", last modified: Sun Apr 14 21:38:25 2024, max compression
+gzip compressed data, was "genflowly_lambda_utils-0.0.7.tar", last modified: Sun Apr 14 21:54:58 2024, max compression
```

## Comparing `genflowly_lambda_utils-0.0.6.tar` & `genflowly_lambda_utils-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/hashing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:54:58.297491 genflowly_lambda_utils-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:54:58.297491 genflowly_lambda_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:54:58.297491 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:54:58.000000 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 21:54:58.000000 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:54:58.000000 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 21:54:58.000000 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:54:58.000000 genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:54:58.297491 genflowly_lambda_utils-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:54:58.297491 genflowly_lambda_utils-0.0.7/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/hashing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 21:54:32.000000 genflowly_lambda_utils-0.0.7/utils/jwt_utils.py
```

### Comparing `genflowly_lambda_utils-0.0.6/PKG-INFO` & `genflowly_lambda_utils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.6/README.md` & `genflowly_lambda_utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly_lambda_utils-0.0.7/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.6/setup.py` & `genflowly_lambda_utils-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly_lambda_utils-0.0.6/utils/aws_dynamodb_utils.py` & `genflowly_lambda_utils-0.0.7/utils/aws_dynamodb_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import boto3
 import logging
 
+from botocore.client import BaseClient
+
 from utils.contants import AWS_DEFAULT_REGION
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 def save_to_dynamodb(table_name: str, data: dict, aws_region: str = AWS_DEFAULT_REGION) -> dict:
@@ -33,7 +35,26 @@
             return {"status": 200, "response": item}
         else:
             logger.error("No item found with key: %s", key)
             return {"status": 404, "response": "No item found"}
     except Exception as e:
         logger.error("Read from DynamoDB failed: %s", e)
         return {"status": 500, "response": e}
+
+
+def update_to_dynamodb(table_name: str, key: dict, value: dict, update_expression: str,
+                       aws_region: str = AWS_DEFAULT_REGION) -> dict:
+    try:
+        dynamodb: BaseClient = boto3.resource('dynamodb', region_name=aws_region)
+        table = dynamodb.Table(table_name)
+        response = table.update_item(
+            Key=key,
+            UpdateExpression=update_expression,
+            ExpressionAttributeValues=value,
+            ReturnValues='UPDATED_NEW'
+        )
+        return {"status": 200, "response": response}
+    except Exception as e:
+        logging.error(f"Failed to update item in DynamoDB: {e}")
+        return {"status": 500, "response": e}
+
+
```

### Comparing `genflowly_lambda_utils-0.0.6/utils/aws_secrets_utils.py` & `genflowly_lambda_utils-0.0.7/utils/aws_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.6/utils/aws_sns_utils.py` & `genflowly_lambda_utils-0.0.7/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.6/utils/aws_step_functions_utils.py` & `genflowly_lambda_utils-0.0.7/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.6/utils/jwt_utils.py` & `genflowly_lambda_utils-0.0.7/utils/jwt_utils.py`

 * *Files identical despite different names*

