# Comparing `tmp/boto3-helpers-2.1.0.tar.gz` & `tmp/boto3-helpers-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-helpers-2.1.0.tar", last modified: Wed Oct 25 19:20:38 2023, max compression
+gzip compressed data, was "boto3-helpers-2.2.0.tar", last modified: Mon Apr 15 20:51:53 2024, max compression
```

## Comparing `boto3-helpers-2.1.0.tar` & `boto3-helpers-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-10-25 19:20:38.425841 boto3-helpers-2.1.0/
--rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-2.1.0/LICENSE
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2623 2023-10-25 19:20:38.425640 boto3-helpers-2.1.0/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-2.1.0/README.rst
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-10-25 19:20:38.360428 boto3-helpers-2.1.0/boto3_helpers/
--rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-2.1.0/boto3_helpers/__init__.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-2.1.0/boto3_helpers/arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-2.1.0/boto3_helpers/awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-2.1.0/boto3_helpers/cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4713 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-2.1.0/boto3_helpers/events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     5510 2023-10-25 19:17:57.000000 boto3-helpers-2.1.0/boto3_helpers/kinesis.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2574 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/medialive.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2213 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/boto3_helpers/signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-2.1.0/boto3_helpers/sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-2.1.0/boto3_helpers/sts.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-10-25 19:20:38.363183 boto3-helpers-2.1.0/boto3_helpers.egg-info/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2623 2023-10-25 19:20:38.000000 boto3-helpers-2.1.0/boto3_helpers.egg-info/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)      883 2023-10-25 19:20:38.000000 boto3-helpers-2.1.0/boto3_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2023-10-25 19:20:38.000000 boto3-helpers-2.1.0/boto3_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2023-10-25 19:20:38.000000 boto3-helpers-2.1.0/boto3_helpers.egg-info/requires.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2023-10-25 19:20:38.000000 boto3-helpers-2.1.0/boto3_helpers.egg-info/top_level.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-2.1.0/pyproject.toml
--rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2023-10-25 19:20:38.427159 boto3-helpers-2.1.0/setup.cfg
--rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-2.1.0/setup.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-10-25 19:20:38.424808 boto3-helpers-2.1.0/tests/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-2.1.0/tests/test_arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-2.1.0/tests/test_awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-2.1.0/tests/test_cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     5664 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/tests/test_dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-2.1.0/tests/test_events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     9591 2023-10-19 19:24:49.000000 boto3-helpers-2.1.0/tests/test_kinesis.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4261 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/tests/test_medialive.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-2.1.0/tests/test_mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2023-04-28 15:58:17.000000 boto3-helpers-2.1.0/tests/test_pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/tests/test_s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-08-30 21:01:55.000000 boto3-helpers-2.1.0/tests/test_signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-2.1.0/tests/test_sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-2.1.0/tests/test_sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2024-04-15 20:51:53.329558 boto3-helpers-2.2.0/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-2.2.0/LICENSE
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2623 2024-04-15 20:51:53.329171 boto3-helpers-2.2.0/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-2.2.0/README.rst
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2024-04-15 20:51:53.314140 boto3-helpers-2.2.0/boto3_helpers/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-2.2.0/boto3_helpers/__init__.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-2.2.0/boto3_helpers/arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-2.2.0/boto3_helpers/awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-2.2.0/boto3_helpers/cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6676 2024-04-15 20:50:50.000000 boto3-helpers-2.2.0/boto3_helpers/dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-2.2.0/boto3_helpers/events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     5510 2023-10-25 19:17:57.000000 boto3-helpers-2.2.0/boto3_helpers/kinesis.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2574 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/boto3_helpers/medialive.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/boto3_helpers/mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2213 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/boto3_helpers/pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/boto3_helpers/s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/boto3_helpers/signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-2.2.0/boto3_helpers/sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-2.2.0/boto3_helpers/sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2024-04-15 20:51:53.317007 boto3-helpers-2.2.0/boto3_helpers.egg-info/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2623 2024-04-15 20:51:53.000000 boto3-helpers-2.2.0/boto3_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      883 2024-04-15 20:51:53.000000 boto3-helpers-2.2.0/boto3_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2024-04-15 20:51:53.000000 boto3-helpers-2.2.0/boto3_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2024-04-15 20:51:53.000000 boto3-helpers-2.2.0/boto3_helpers.egg-info/requires.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2024-04-15 20:51:53.000000 boto3-helpers-2.2.0/boto3_helpers.egg-info/top_level.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-2.2.0/pyproject.toml
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2024-04-15 20:51:53.330803 boto3-helpers-2.2.0/setup.cfg
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-2.2.0/setup.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2024-04-15 20:51:53.328038 boto3-helpers-2.2.0/tests/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-2.2.0/tests/test_arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-2.2.0/tests/test_awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-2.2.0/tests/test_cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     8722 2024-04-15 20:50:50.000000 boto3-helpers-2.2.0/tests/test_dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-2.2.0/tests/test_events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     9591 2023-10-19 19:24:49.000000 boto3-helpers-2.2.0/tests/test_kinesis.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4261 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/tests/test_medialive.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-2.2.0/tests/test_mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2023-04-28 15:58:17.000000 boto3-helpers-2.2.0/tests/test_pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/tests/test_s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-08-30 21:01:55.000000 boto3-helpers-2.2.0/tests/test_signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-2.2.0/tests/test_sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-2.2.0/tests/test_sts.py
```

### Comparing `boto3-helpers-2.1.0/LICENSE` & `boto3-helpers-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/PKG-INFO` & `boto3-helpers-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 2.1.0
+Version: 2.2.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boto3-helpers-2.1.0/README.rst` & `boto3-helpers-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/arn.py` & `boto3-helpers-2.2.0/boto3_helpers/arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/awslambda.py` & `boto3-helpers-2.2.0/boto3_helpers/awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/cloudwatch.py` & `boto3-helpers-2.2.0/boto3_helpers/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/events.py` & `boto3-helpers-2.2.0/boto3_helpers/events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/kinesis.py` & `boto3-helpers-2.2.0/boto3_helpers/kinesis.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/medialive.py` & `boto3-helpers-2.2.0/boto3_helpers/medialive.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/mediatailor.py` & `boto3-helpers-2.2.0/boto3_helpers/mediatailor.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/pagination.py` & `boto3-helpers-2.2.0/boto3_helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/s3.py` & `boto3-helpers-2.2.0/boto3_helpers/s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/signed_requests.py` & `boto3-helpers-2.2.0/boto3_helpers/signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/sqs.py` & `boto3-helpers-2.2.0/boto3_helpers/sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers/sts.py` & `boto3-helpers-2.2.0/boto3_helpers/sts.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/boto3_helpers.egg-info/PKG-INFO` & `boto3-helpers-2.2.0/boto3_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 2.1.0
+Version: 2.2.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boto3-helpers-2.1.0/boto3_helpers.egg-info/SOURCES.txt` & `boto3-helpers-2.2.0/boto3_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/setup.cfg` & `boto3-helpers-2.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = boto3-helpers
-version = 2.1.0
+version = 2.2.0
 description = Helper utilities for boto3
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Bo Bayles
 author_email = bo.bayles@wurl.com
 license = Apache 2.0
 license_files =
```

### Comparing `boto3-helpers-2.1.0/tests/test_arn.py` & `boto3-helpers-2.2.0/tests/test_arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_awslambda.py` & `boto3-helpers-2.2.0/tests/test_awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_cloudwatch.py` & `boto3-helpers-2.2.0/tests/test_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_dynamodb.py` & `boto3-helpers-2.2.0/tests/test_dynamodb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from decimal import Decimal
 from unittest import TestCase
-from unittest.mock import patch
+from unittest.mock import call as MockCall, patch
 
 from boto3.dynamodb.conditions import Attr as ddb_attr, Key as ddb_key
 from boto3 import resource as boto3_resource
 from botocore.stub import Stubber
 
-from boto3_helpers.dynamodb import query_table, scan_table, update_attributes
+from boto3_helpers.dynamodb import (
+    batch_yield_items,
+    query_table,
+    scan_table,
+    update_attributes,
+)
 
 
 class DynamoDBTests(TestCase):
     def test_query_table(self):
         # Set up the stubber
         ddb_resource = boto3_resource('dynamodb', region_name='not-a-region')
         ddb_table = ddb_resource.Table('test-table')
@@ -149,7 +154,83 @@
                 'username': 'janedoe',
                 'last_name': 'Doe',
                 'age': Decimal(26),
                 'weight_kg': Decimal(70),
             }
         }
         self.assertEqual(actual, expected)
+
+    @patch('boto3_helpers.dynamodb.sleep', autospec=True)
+    @patch('boto3_helpers.dynamodb.boto3_resource', autospec=True)
+    def test_batch_yield_items(self, mock_boto3_resource, mock_sleep):
+        table_name = 'test-table'
+        all_keys = [
+            {'primary_key': '1', 'sort_key': 'a'},
+            {'primary_key': '1', 'sort_key': 'b'},
+            {'primary_key': '2', 'sort_key': 'a'},
+            {'primary_key': '2', 'sort_key': 'b'},
+            {'primary_key': '3', 'sort_key': 'a'},
+            {'primary_key': '3', 'sort_key': 'b'},
+        ]
+
+        mock_boto3_resource.return_value.batch_get_item.side_effect = [
+            {
+                'Responses': {table_name: all_keys[:3]},
+                'UnprocessedKeys': {table_name: all_keys[3:]},
+            },
+            {
+                'Responses': {table_name: all_keys[3:]},
+                'UnprocessedKeys': {},
+            },
+        ]
+        actual = list(batch_yield_items(table_name, all_keys[:], backoff_base=0.1))
+        self.assertEqual(actual, all_keys)
+
+        mock_sleep.assert_called_once_with(0.1)
+        mock_boto3_resource.assert_called_once_with('dynamodb')
+        self.assertEqual(mock_boto3_resource.return_value.batch_get_item.call_count, 2)
+
+    @patch('boto3_helpers.dynamodb.sleep', autospec=True)
+    @patch('boto3_helpers.dynamodb.boto3_resource', autospec=True)
+    def test_batch_yield_items_batch_size(self, mock_boto3_resource, mock_sleep):
+        table_name = 'test-table'
+        all_keys = [
+            {'primary_key': '1', 'sort_key': 'a'},
+            {'primary_key': '1', 'sort_key': 'b'},
+            {'primary_key': '2', 'sort_key': 'a'},
+            {'primary_key': '2', 'sort_key': 'b'},
+            {'primary_key': '3', 'sort_key': 'a'},
+            {'primary_key': '3', 'sort_key': 'b'},
+            {'primary_key': '4', 'sort_key': 'a'},
+            {'primary_key': '4', 'sort_key': 'b'},
+        ]
+
+        mock_boto3_resource.return_value.batch_get_item.side_effect = [
+            {
+                'Responses': {table_name: all_keys[:2]},
+                'UnprocessedKeys': {},
+            },
+            {
+                'Responses': {table_name: all_keys[2:4]},
+                'UnprocessedKeys': {},
+            },
+            {
+                'Responses': {table_name: all_keys[4:6]},
+                'UnprocessedKeys': {},
+            },
+            {
+                'Responses': {table_name: all_keys[6:8]},
+                'UnprocessedKeys': {},
+            },
+        ]
+        actual = list(
+            batch_yield_items(
+                table_name, all_keys[:], batch_size=2, backoff_base=0.1, backoff_max=0.2
+            )
+        )
+        self.assertEqual(actual, all_keys)
+
+        self.assertEqual(
+            mock_sleep.mock_calls, [MockCall(0.1), MockCall(0.2), MockCall(0.2)]
+        )
+        mock_boto3_resource.assert_called_once_with('dynamodb')
+        self.assertEqual(mock_boto3_resource.return_value.batch_get_item.call_count, 4)
```

### Comparing `boto3-helpers-2.1.0/tests/test_events.py` & `boto3-helpers-2.2.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_kinesis.py` & `boto3-helpers-2.2.0/tests/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_medialive.py` & `boto3-helpers-2.2.0/tests/test_medialive.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_mediatailor.py` & `boto3-helpers-2.2.0/tests/test_mediatailor.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_pagination.py` & `boto3-helpers-2.2.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_s3.py` & `boto3-helpers-2.2.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_signed_requests.py` & `boto3-helpers-2.2.0/tests/test_signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_sqs.py` & `boto3-helpers-2.2.0/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-2.1.0/tests/test_sts.py` & `boto3-helpers-2.2.0/tests/test_sts.py`

 * *Files identical despite different names*

