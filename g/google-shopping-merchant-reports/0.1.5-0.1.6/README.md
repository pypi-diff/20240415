# Comparing `tmp/google-shopping-merchant-reports-0.1.5.tar.gz` & `tmp/google-shopping-merchant-reports-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-reports-0.1.5.tar", last modified: Tue Mar  5 19:01:52 2024, max compression
+gzip compressed data, was "google-shopping-merchant-reports-0.1.6.tar", last modified: Mon Apr 15 13:59:02 2024, max compression
```

## Comparing `google-shopping-merchant-reports-0.1.5.tar` & `google-shopping-merchant-reports-0.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.205305 google-shopping-merchant-reports-0.1.5/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5310 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3857 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.193304 google-shopping-merchant-reports-0.1.5/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.193304 google-shopping-merchant-reports-0.1.5/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.197304 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/
--rw-rw-r--   0 root         (0)     1003     2062 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.197304 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/
--rw-rw-r--   0 root         (0)     1003     1878 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     1005 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.197304 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.197304 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/
--rw-rw-r--   0 root         (0)     1003      765 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15830 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31828 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/client.py
--rw-rw-r--   0 root         (0)     1003     5666 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.197304 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6086 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11951 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12170 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12038 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    82999 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/types/reports.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/
--rw-r--r--   0 root         (0)     1003     5310 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1822 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      343 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:52.000000 google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:52.205305 google-shopping-merchant-reports-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3265 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:52.201305 google-shopping-merchant-reports-0.1.5/tests/unit/gapic/merchant_reports_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/tests/unit/gapic/merchant_reports_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    94666 2024-03-05 18:46:03.000000 google-shopping-merchant-reports-0.1.5/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5310 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3857 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.424641 google-shopping-merchant-reports-0.1.6/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.424641 google-shopping-merchant-reports-0.1.6/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/
+-rw-rw-r--   0 root         (0)     1003     2062 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1878 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1005 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/
+-rw-rw-r--   0 root         (0)     1003      765 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15830 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31828 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5666 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6086 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11951 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12170 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12038 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    84961 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/reports.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/
+-rw-r--r--   0 root         (0)     1003     5310 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1822 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      343 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3265 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    96721 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py
```

### Comparing `google-shopping-merchant-reports-0.1.5/LICENSE` & `google-shopping-merchant-reports-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.5/MANIFEST.in` & `google-shopping-merchant-reports-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.5/PKG-INFO` & `google-shopping-merchant-reports-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-reports
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Merchant Reports API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reports
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-reports-0.1.5/README.rst` & `google-shopping-merchant-reports-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports/gapic_version.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.5"  # {x-release-please-version}
+__version__ = "0.1.6"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/gapic_metadata.json` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/gapic_version.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.5"  # {x-release-please-version}
+__version__ = "0.1.6"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/client.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/types/__init__.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/google/shopping/merchant_reports_v1beta/types/reports.py` & `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 2320 436f 7079 7269  f-8 -*-.# Copyri
-00000020: 6768 7420 3230 3233 2047 6f6f 676c 6520  ght 2023 Google 
+00000020: 6768 7420 3230 3234 2047 6f6f 676c 6520  ght 2024 Google 
 00000030: 4c4c 430a 230a 2320 4c69 6365 6e73 6564  LLC.#.# Licensed
 00000040: 2075 6e64 6572 2074 6865 2041 7061 6368   under the Apach
 00000050: 6520 4c69 6365 6e73 652c 2056 6572 7369  e License, Versi
 00000060: 6f6e 2032 2e30 2028 7468 6520 224c 6963  on 2.0 (the "Lic
 00000070: 656e 7365 2229 3b0a 2320 796f 7520 6d61  ense");.# you ma
 00000080: 7920 6e6f 7420 7573 6520 7468 6973 2066  y not use this f
 00000090: 696c 6520 6578 6365 7074 2069 6e20 636f  ile except in co
@@ -135,5054 +135,5177 @@
 00000860: 2020 2020 2020 7061 6765 5f73 697a 6520        page_size 
 00000870: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
 00000880: 2020 204f 7074 696f 6e61 6c2e 204e 756d     Optional. Num
 00000890: 6265 7220 6f66 2060 6052 6570 6f72 7452  ber of ``ReportR
 000008a0: 6f77 7360 6020 746f 2072 6574 7269 6576  ows`` to retriev
 000008b0: 6520 696e 2061 2073 696e 676c 650a 2020  e in a single.  
 000008c0: 2020 2020 2020 2020 2020 7061 6765 2e20            page. 
-000008d0: 4465 6661 756c 7473 2074 6f20 7468 6520  Defaults to the 
-000008e0: 6d61 7869 6d75 6d20 6f66 2031 3030 302e  maximum of 1000.
-000008f0: 2056 616c 7565 7320 6162 6f76 6520 3130   Values above 10
-00000900: 3030 2061 7265 0a20 2020 2020 2020 2020  00 are.         
-00000910: 2020 2063 6f65 7263 6564 2074 6f20 3130     coerced to 10
-00000920: 3030 2e0a 2020 2020 2020 2020 7061 6765  00..        page
-00000930: 5f74 6f6b 656e 2028 7374 7229 3a0a 2020  _token (str):.  
-00000940: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
-00000950: 616c 2e20 546f 6b65 6e20 6f66 2074 6865  al. Token of the
-00000960: 2070 6167 6520 746f 2072 6574 7269 6576   page to retriev
-00000970: 652e 2049 6620 6e6f 7420 7370 6563 6966  e. If not specif
-00000980: 6965 642c 0a20 2020 2020 2020 2020 2020  ied,.           
-00000990: 2074 6865 2066 6972 7374 2070 6167 6520   the first page 
-000009a0: 6f66 2072 6573 756c 7473 2069 7320 7265  of results is re
-000009b0: 7475 726e 6564 2e20 496e 206f 7264 6572  turned. In order
-000009c0: 2074 6f20 7265 7175 6573 740a 2020 2020   to request.    
-000009d0: 2020 2020 2020 2020 7468 6520 6e65 7874          the next
-000009e0: 2070 6167 6520 6f66 2072 6573 756c 7473   page of results
-000009f0: 2c20 7468 6520 7661 6c75 6520 6f62 7461  , the value obta
-00000a00: 696e 6564 2066 726f 6d0a 2020 2020 2020  ined from.      
-00000a10: 2020 2020 2020 6060 6e65 7874 5f70 6167        ``next_pag
-00000a20: 655f 746f 6b65 6e60 6020 696e 2074 6865  e_token`` in the
-00000a30: 2070 7265 7669 6f75 7320 7265 7370 6f6e   previous respon
-00000a40: 7365 2073 686f 756c 6420 6265 2075 7365  se should be use
-00000a50: 642e 0a20 2020 2022 2222 0a0a 2020 2020  d..    """..    
-00000a60: 7061 7265 6e74 3a20 7374 7220 3d20 7072  parent: str = pr
-00000a70: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00000a80: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00000a90: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00000aa0: 312c 0a20 2020 2029 0a20 2020 2071 7565  1,.    ).    que
-00000ab0: 7279 3a20 7374 7220 3d20 7072 6f74 6f2e  ry: str = proto.
-00000ac0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00000ad0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00000ae0: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
-00000af0: 2020 2029 0a20 2020 2070 6167 655f 7369     ).    page_si
-00000b00: 7a65 3a20 696e 7420 3d20 7072 6f74 6f2e  ze: int = proto.
-00000b10: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00000b20: 726f 746f 2e49 4e54 3332 2c0a 2020 2020  roto.INT32,.    
-00000b30: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-00000b40: 2020 290a 2020 2020 7061 6765 5f74 6f6b    ).    page_tok
-00000b50: 656e 3a20 7374 7220 3d20 7072 6f74 6f2e  en: str = proto.
-00000b60: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00000b70: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00000b80: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
-00000b90: 2020 2029 0a0a 0a63 6c61 7373 2053 6561     )...class Sea
-00000ba0: 7263 6852 6573 706f 6e73 6528 7072 6f74  rchResponse(prot
-00000bb0: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00000bc0: 7222 2222 5265 7370 6f6e 7365 206d 6573  r"""Response mes
-00000bd0: 7361 6765 2066 6f72 2074 6865 2060 6052  sage for the ``R
-00000be0: 6570 6f72 7453 6572 7669 6365 2e53 6561  eportService.Sea
-00000bf0: 7263 6860 6020 6d65 7468 6f64 2e0a 0a20  rch`` method... 
-00000c00: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-00000c10: 2020 2020 2020 2072 6573 756c 7473 2028         results (
-00000c20: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
-00000c30: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-00000c40: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-00000c50: 5f76 3162 6574 612e 7479 7065 732e 5265  _v1beta.types.Re
-00000c60: 706f 7274 526f 775d 293a 0a20 2020 2020  portRow]):.     
-00000c70: 2020 2020 2020 2052 6f77 7320 7468 6174         Rows that
-00000c80: 206d 6174 6368 6564 2074 6865 2073 6561   matched the sea
-00000c90: 7263 6820 7175 6572 792e 0a20 2020 2020  rch query..     
-00000ca0: 2020 206e 6578 745f 7061 6765 5f74 6f6b     next_page_tok
-00000cb0: 656e 2028 7374 7229 3a0a 2020 2020 2020  en (str):.      
-00000cc0: 2020 2020 2020 546f 6b65 6e20 7768 6963        Token whic
-00000cd0: 6820 6361 6e20 6265 2073 656e 7420 6173  h can be sent as
-00000ce0: 2060 6070 6167 655f 746f 6b65 6e60 6020   ``page_token`` 
-00000cf0: 746f 2072 6574 7269 6576 6520 7468 650a  to retrieve the.
-00000d00: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00000d10: 2070 6167 652e 2049 6620 6f6d 6974 7465   page. If omitte
-00000d20: 642c 2074 6865 7265 2061 7265 206e 6f20  d, there are no 
-00000d30: 7375 6273 6571 7565 6e74 2070 6167 6573  subsequent pages
-00000d40: 2e0a 2020 2020 2222 220a 0a20 2020 2040  ..    """..    @
-00000d50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00000d60: 2072 6177 5f70 6167 6528 7365 6c66 293a   raw_page(self):
-00000d70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000d80: 7365 6c66 0a0a 2020 2020 7265 7375 6c74  self..    result
-00000d90: 733a 204d 7574 6162 6c65 5365 7175 656e  s: MutableSequen
-00000da0: 6365 5b22 5265 706f 7274 526f 7722 5d20  ce["ReportRow"] 
-00000db0: 3d20 7072 6f74 6f2e 5265 7065 6174 6564  = proto.Repeated
-00000dc0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00000dd0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00000de0: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
-00000df0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00000e00: 2252 6570 6f72 7452 6f77 222c 0a20 2020  "ReportRow",.   
-00000e10: 2029 0a20 2020 206e 6578 745f 7061 6765   ).    next_page
-00000e20: 5f74 6f6b 656e 3a20 7374 7220 3d20 7072  _token: str = pr
-00000e30: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00000e40: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00000e50: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00000e60: 322c 0a20 2020 2029 0a0a 0a63 6c61 7373  2,.    )...class
-00000e70: 2052 6570 6f72 7452 6f77 2870 726f 746f   ReportRow(proto
-00000e80: 2e4d 6573 7361 6765 293a 0a20 2020 2072  .Message):.    r
-00000e90: 2222 2252 6573 756c 7420 726f 7720 7265  """Result row re
-00000ea0: 7475 726e 6564 2066 726f 6d20 7468 6520  turned from the 
-00000eb0: 7365 6172 6368 2071 7565 7279 2e0a 0a20  search query... 
-00000ec0: 2020 204f 6e6c 7920 7468 6520 6d65 7373     Only the mess
-00000ed0: 6167 6520 636f 7272 6573 706f 6e64 696e  age correspondin
-00000ee0: 6720 746f 2074 6865 2071 7565 7269 6564  g to the queried
-00000ef0: 2074 6162 6c65 2069 7320 706f 7075 6c61   table is popula
-00000f00: 7465 640a 2020 2020 696e 2074 6865 2072  ted.    in the r
-00000f10: 6573 706f 6e73 652e 2057 6974 6869 6e20  esponse. Within 
-00000f20: 7468 6520 706f 7075 6c61 7465 6420 6d65  the populated me
-00000f30: 7373 6167 652c 206f 6e6c 7920 7468 6520  ssage, only the 
-00000f40: 6669 656c 6473 0a20 2020 2072 6571 7565  fields.    reque
-00000f50: 7374 6564 2065 7870 6c69 6369 746c 7920  sted explicitly 
-00000f60: 696e 2074 6865 2071 7565 7279 2061 7265  in the query are
-00000f70: 2070 6f70 756c 6174 6564 2e0a 0a20 2020   populated...   
-00000f80: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-00000f90: 2020 2020 2070 726f 6475 6374 5f70 6572       product_per
-00000fa0: 666f 726d 616e 6365 5f76 6965 7720 2867  formance_view (g
-00000fb0: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
-00000fc0: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
-00000fd0: 7631 6265 7461 2e74 7970 6573 2e50 726f  v1beta.types.Pro
-00000fe0: 6475 6374 5065 7266 6f72 6d61 6e63 6556  ductPerformanceV
-00000ff0: 6965 7729 3a0a 2020 2020 2020 2020 2020  iew):.          
-00001000: 2020 4669 656c 6473 2061 7661 696c 6162    Fields availab
-00001010: 6c65 2066 6f72 2071 7565 7279 2069 6e20  le for query in 
-00001020: 6060 7072 6f64 7563 745f 7065 7266 6f72  ``product_perfor
-00001030: 6d61 6e63 655f 7669 6577 6060 0a20 2020  mance_view``.   
-00001040: 2020 2020 2020 2020 2074 6162 6c65 2e0a           table..
-00001050: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-00001060: 7669 6577 2028 676f 6f67 6c65 2e73 686f  view (google.sho
-00001070: 7070 696e 672e 6d65 7263 6861 6e74 5f72  pping.merchant_r
-00001080: 6570 6f72 7473 5f76 3162 6574 612e 7479  eports_v1beta.ty
-00001090: 7065 732e 5072 6f64 7563 7456 6965 7729  pes.ProductView)
-000010a0: 3a0a 2020 2020 2020 2020 2020 2020 4669  :.            Fi
-000010b0: 656c 6473 2061 7661 696c 6162 6c65 2066  elds available f
-000010c0: 6f72 2071 7565 7279 2069 6e20 6060 7072  or query in ``pr
-000010d0: 6f64 7563 745f 7669 6577 6060 2074 6162  oduct_view`` tab
-000010e0: 6c65 2e0a 2020 2020 2020 2020 7072 6963  le..        pric
-000010f0: 655f 636f 6d70 6574 6974 6976 656e 6573  e_competitivenes
-00001100: 735f 7072 6f64 7563 745f 7669 6577 2028  s_product_view (
-00001110: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-00001120: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-00001130: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
-00001140: 6963 6543 6f6d 7065 7469 7469 7665 6e65  iceCompetitivene
-00001150: 7373 5072 6f64 7563 7456 6965 7729 3a0a  ssProductView):.
-00001160: 2020 2020 2020 2020 2020 2020 4669 656c              Fiel
-00001170: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
-00001180: 2071 7565 7279 2069 6e0a 2020 2020 2020   query in.      
-00001190: 2020 2020 2020 6060 7072 6963 655f 636f        ``price_co
-000011a0: 6d70 6574 6974 6976 656e 6573 735f 7072  mpetitiveness_pr
-000011b0: 6f64 7563 745f 7669 6577 6060 2074 6162  oduct_view`` tab
-000011c0: 6c65 2e0a 2020 2020 2020 2020 7072 6963  le..        pric
-000011d0: 655f 696e 7369 6768 7473 5f70 726f 6475  e_insights_produ
-000011e0: 6374 5f76 6965 7720 2867 6f6f 676c 652e  ct_view (google.
-000011f0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-00001200: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-00001210: 2e74 7970 6573 2e50 7269 6365 496e 7369  .types.PriceInsi
-00001220: 6768 7473 5072 6f64 7563 7456 6965 7729  ghtsProductView)
-00001230: 3a0a 2020 2020 2020 2020 2020 2020 4669  :.            Fi
-00001240: 656c 6473 2061 7661 696c 6162 6c65 2066  elds available f
-00001250: 6f72 2071 7565 7279 2069 6e0a 2020 2020  or query in.    
-00001260: 2020 2020 2020 2020 6060 7072 6963 655f          ``price_
-00001270: 696e 7369 6768 7473 5f70 726f 6475 6374  insights_product
-00001280: 5f76 6965 7760 6020 7461 626c 652e 0a20  _view`` table.. 
-00001290: 2020 2020 2020 2062 6573 745f 7365 6c6c         best_sell
-000012a0: 6572 735f 7072 6f64 7563 745f 636c 7573  ers_product_clus
-000012b0: 7465 725f 7669 6577 2028 676f 6f67 6c65  ter_view (google
-000012c0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
-000012d0: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
-000012e0: 612e 7479 7065 732e 4265 7374 5365 6c6c  a.types.BestSell
-000012f0: 6572 7350 726f 6475 6374 436c 7573 7465  ersProductCluste
-00001300: 7256 6965 7729 3a0a 2020 2020 2020 2020  rView):.        
-00001310: 2020 2020 4669 656c 6473 2061 7661 696c      Fields avail
-00001320: 6162 6c65 2066 6f72 2071 7565 7279 2069  able for query i
-00001330: 6e0a 2020 2020 2020 2020 2020 2020 6060  n.            ``
-00001340: 6265 7374 5f73 656c 6c65 7273 5f70 726f  best_sellers_pro
-00001350: 6475 6374 5f63 6c75 7374 6572 5f76 6965  duct_cluster_vie
-00001360: 7760 6020 7461 626c 652e 0a20 2020 2020  w`` table..     
-00001370: 2020 2062 6573 745f 7365 6c6c 6572 735f     best_sellers_
-00001380: 6272 616e 645f 7669 6577 2028 676f 6f67  brand_view (goog
-00001390: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
-000013a0: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
-000013b0: 6574 612e 7479 7065 732e 4265 7374 5365  eta.types.BestSe
-000013c0: 6c6c 6572 7342 7261 6e64 5669 6577 293a  llersBrandView):
-000013d0: 0a20 2020 2020 2020 2020 2020 2046 6965  .            Fie
-000013e0: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
-000013f0: 7220 7175 6572 7920 696e 2060 6062 6573  r query in ``bes
-00001400: 745f 7365 6c6c 6572 735f 6272 616e 645f  t_sellers_brand_
-00001410: 7669 6577 6060 0a20 2020 2020 2020 2020  view``.         
-00001420: 2020 2074 6162 6c65 2e0a 2020 2020 2020     table..      
-00001430: 2020 636f 6d70 6574 6974 6976 655f 7669    competitive_vi
-00001440: 7369 6269 6c69 7479 5f63 6f6d 7065 7469  sibility_competi
-00001450: 746f 725f 7669 6577 2028 676f 6f67 6c65  tor_view (google
-00001460: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
-00001470: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
-00001480: 612e 7479 7065 732e 436f 6d70 6574 6974  a.types.Competit
-00001490: 6976 6556 6973 6962 696c 6974 7943 6f6d  iveVisibilityCom
-000014a0: 7065 7469 746f 7256 6965 7729 3a0a 2020  petitorView):.  
-000014b0: 2020 2020 2020 2020 2020 4669 656c 6473            Fields
-000014c0: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
-000014d0: 7565 7279 2069 6e0a 2020 2020 2020 2020  uery in.        
-000014e0: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
-000014f0: 655f 7669 7369 6269 6c69 7479 5f63 6f6d  e_visibility_com
-00001500: 7065 7469 746f 725f 7669 6577 6060 2074  petitor_view`` t
-00001510: 6162 6c65 2e0a 2020 2020 2020 2020 636f  able..        co
-00001520: 6d70 6574 6974 6976 655f 7669 7369 6269  mpetitive_visibi
-00001530: 6c69 7479 5f74 6f70 5f6d 6572 6368 616e  lity_top_merchan
-00001540: 745f 7669 6577 2028 676f 6f67 6c65 2e73  t_view (google.s
-00001550: 686f 7070 696e 672e 6d65 7263 6861 6e74  hopping.merchant
-00001560: 5f72 6570 6f72 7473 5f76 3162 6574 612e  _reports_v1beta.
-00001570: 7479 7065 732e 436f 6d70 6574 6974 6976  types.Competitiv
-00001580: 6556 6973 6962 696c 6974 7954 6f70 4d65  eVisibilityTopMe
-00001590: 7263 6861 6e74 5669 6577 293a 0a20 2020  rchantView):.   
-000015a0: 2020 2020 2020 2020 2046 6965 6c64 7320           Fields 
-000015b0: 6176 6169 6c61 626c 6520 666f 7220 7175  available for qu
-000015c0: 6572 7920 696e 0a20 2020 2020 2020 2020  ery in.         
-000015d0: 2020 2060 6063 6f6d 7065 7469 7469 7665     ``competitive
-000015e0: 5f76 6973 6962 696c 6974 795f 746f 705f  _visibility_top_
-000015f0: 6d65 7263 6861 6e74 5f76 6965 7760 6020  merchant_view`` 
-00001600: 7461 626c 652e 0a20 2020 2020 2020 2063  table..        c
-00001610: 6f6d 7065 7469 7469 7665 5f76 6973 6962  ompetitive_visib
-00001620: 696c 6974 795f 6265 6e63 686d 6172 6b5f  ility_benchmark_
-00001630: 7669 6577 2028 676f 6f67 6c65 2e73 686f  view (google.sho
-00001640: 7070 696e 672e 6d65 7263 6861 6e74 5f72  pping.merchant_r
-00001650: 6570 6f72 7473 5f76 3162 6574 612e 7479  eports_v1beta.ty
-00001660: 7065 732e 436f 6d70 6574 6974 6976 6556  pes.CompetitiveV
-00001670: 6973 6962 696c 6974 7942 656e 6368 6d61  isibilityBenchma
-00001680: 726b 5669 6577 293a 0a20 2020 2020 2020  rkView):.       
-00001690: 2020 2020 2046 6965 6c64 7320 6176 6169       Fields avai
-000016a0: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
-000016b0: 696e 0a20 2020 2020 2020 2020 2020 2060  in.            `
-000016c0: 6063 6f6d 7065 7469 7469 7665 5f76 6973  `competitive_vis
-000016d0: 6962 696c 6974 795f 6265 6e63 686d 6172  ibility_benchmar
-000016e0: 6b5f 7669 6577 6060 2074 6162 6c65 2e0a  k_view`` table..
-000016f0: 2020 2020 2222 220a 0a20 2020 2070 726f      """..    pro
-00001700: 6475 6374 5f70 6572 666f 726d 616e 6365  duct_performance
-00001710: 5f76 6965 773a 2022 5072 6f64 7563 7450  _view: "ProductP
-00001720: 6572 666f 726d 616e 6365 5669 6577 2220  erformanceView" 
-00001730: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00001740: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00001750: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00001760: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
-00001770: 6d65 7373 6167 653d 2250 726f 6475 6374  message="Product
-00001780: 5065 7266 6f72 6d61 6e63 6556 6965 7722  PerformanceView"
-00001790: 2c0a 2020 2020 290a 2020 2020 7072 6f64  ,.    ).    prod
-000017a0: 7563 745f 7669 6577 3a20 2250 726f 6475  uct_view: "Produ
-000017b0: 6374 5669 6577 2220 3d20 7072 6f74 6f2e  ctView" = proto.
-000017c0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-000017d0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-000017e0: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-000017f0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00001800: 2250 726f 6475 6374 5669 6577 222c 0a20  "ProductView",. 
-00001810: 2020 2029 0a20 2020 2070 7269 6365 5f63     ).    price_c
-00001820: 6f6d 7065 7469 7469 7665 6e65 7373 5f70  ompetitiveness_p
-00001830: 726f 6475 6374 5f76 6965 773a 2022 5072  roduct_view: "Pr
-00001840: 6963 6543 6f6d 7065 7469 7469 7665 6e65  iceCompetitivene
-00001850: 7373 5072 6f64 7563 7456 6965 7722 203d  ssProductView" =
-00001860: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00001870: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
-00001880: 4147 452c 0a20 2020 2020 2020 206e 756d  AGE,.        num
-00001890: 6265 723d 332c 0a20 2020 2020 2020 206d  ber=3,.        m
-000018a0: 6573 7361 6765 3d22 5072 6963 6543 6f6d  essage="PriceCom
-000018b0: 7065 7469 7469 7665 6e65 7373 5072 6f64  petitivenessProd
-000018c0: 7563 7456 6965 7722 2c0a 2020 2020 290a  uctView",.    ).
-000018d0: 2020 2020 7072 6963 655f 696e 7369 6768      price_insigh
-000018e0: 7473 5f70 726f 6475 6374 5f76 6965 773a  ts_product_view:
-000018f0: 2022 5072 6963 6549 6e73 6967 6874 7350   "PriceInsightsP
-00001900: 726f 6475 6374 5669 6577 2220 3d20 7072  roductView" = pr
-00001910: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00001920: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
-00001930: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00001940: 3d34 2c0a 2020 2020 2020 2020 6d65 7373  =4,.        mess
-00001950: 6167 653d 2250 7269 6365 496e 7369 6768  age="PriceInsigh
-00001960: 7473 5072 6f64 7563 7456 6965 7722 2c0a  tsProductView",.
-00001970: 2020 2020 290a 2020 2020 6265 7374 5f73      ).    best_s
-00001980: 656c 6c65 7273 5f70 726f 6475 6374 5f63  ellers_product_c
-00001990: 6c75 7374 6572 5f76 6965 773a 2022 4265  luster_view: "Be
-000019a0: 7374 5365 6c6c 6572 7350 726f 6475 6374  stSellersProduct
-000019b0: 436c 7573 7465 7256 6965 7722 203d 2070  ClusterView" = p
-000019c0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000019d0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-000019e0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-000019f0: 723d 352c 0a20 2020 2020 2020 206d 6573  r=5,.        mes
-00001a00: 7361 6765 3d22 4265 7374 5365 6c6c 6572  sage="BestSeller
-00001a10: 7350 726f 6475 6374 436c 7573 7465 7256  sProductClusterV
-00001a20: 6965 7722 2c0a 2020 2020 290a 2020 2020  iew",.    ).    
-00001a30: 6265 7374 5f73 656c 6c65 7273 5f62 7261  best_sellers_bra
-00001a40: 6e64 5f76 6965 773a 2022 4265 7374 5365  nd_view: "BestSe
-00001a50: 6c6c 6572 7342 7261 6e64 5669 6577 2220  llersBrandView" 
-00001a60: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00001a70: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00001a80: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00001a90: 6d62 6572 3d36 2c0a 2020 2020 2020 2020  mber=6,.        
-00001aa0: 6d65 7373 6167 653d 2242 6573 7453 656c  message="BestSel
-00001ab0: 6c65 7273 4272 616e 6456 6965 7722 2c0a  lersBrandView",.
-00001ac0: 2020 2020 290a 2020 2020 636f 6d70 6574      ).    compet
-00001ad0: 6974 6976 655f 7669 7369 6269 6c69 7479  itive_visibility
-00001ae0: 5f63 6f6d 7065 7469 746f 725f 7669 6577  _competitor_view
-00001af0: 3a20 2243 6f6d 7065 7469 7469 7665 5669  : "CompetitiveVi
-00001b00: 7369 6269 6c69 7479 436f 6d70 6574 6974  sibilityCompetit
-00001b10: 6f72 5669 6577 2220 3d20 280a 2020 2020  orView" = (.    
-00001b20: 2020 2020 7072 6f74 6f2e 4669 656c 6428      proto.Field(
-00001b30: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00001b40: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00001b50: 2020 2020 2020 2020 6e75 6d62 6572 3d38          number=8
-00001b60: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-00001b70: 7373 6167 653d 2243 6f6d 7065 7469 7469  ssage="Competiti
-00001b80: 7665 5669 7369 6269 6c69 7479 436f 6d70  veVisibilityComp
-00001b90: 6574 6974 6f72 5669 6577 222c 0a20 2020  etitorView",.   
-00001ba0: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
-00001bb0: 2063 6f6d 7065 7469 7469 7665 5f76 6973   competitive_vis
-00001bc0: 6962 696c 6974 795f 746f 705f 6d65 7263  ibility_top_merc
-00001bd0: 6861 6e74 5f76 6965 773a 2022 436f 6d70  hant_view: "Comp
-00001be0: 6574 6974 6976 6556 6973 6962 696c 6974  etitiveVisibilit
-00001bf0: 7954 6f70 4d65 7263 6861 6e74 5669 6577  yTopMerchantView
-00001c00: 2220 3d20 280a 2020 2020 2020 2020 7072  " = (.        pr
-00001c10: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00001c20: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00001c30: 5341 4745 2c0a 2020 2020 2020 2020 2020  SAGE,.          
-00001c40: 2020 6e75 6d62 6572 3d39 2c0a 2020 2020    number=9,.    
-00001c50: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00001c60: 2243 6f6d 7065 7469 7469 7665 5669 7369  "CompetitiveVisi
-00001c70: 6269 6c69 7479 546f 704d 6572 6368 616e  bilityTopMerchan
-00001c80: 7456 6965 7722 2c0a 2020 2020 2020 2020  tView",.        
-00001c90: 290a 2020 2020 290a 2020 2020 636f 6d70  ).    ).    comp
-00001ca0: 6574 6974 6976 655f 7669 7369 6269 6c69  etitive_visibili
-00001cb0: 7479 5f62 656e 6368 6d61 726b 5f76 6965  ty_benchmark_vie
-00001cc0: 773a 2022 436f 6d70 6574 6974 6976 6556  w: "CompetitiveV
-00001cd0: 6973 6962 696c 6974 7942 656e 6368 6d61  isibilityBenchma
-00001ce0: 726b 5669 6577 2220 3d20 280a 2020 2020  rkView" = (.    
-00001cf0: 2020 2020 7072 6f74 6f2e 4669 656c 6428      proto.Field(
-00001d00: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00001d10: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00001d20: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-00001d30: 302c 0a20 2020 2020 2020 2020 2020 206d  0,.            m
-00001d40: 6573 7361 6765 3d22 436f 6d70 6574 6974  essage="Competit
-00001d50: 6976 6556 6973 6962 696c 6974 7942 656e  iveVisibilityBen
-00001d60: 6368 6d61 726b 5669 6577 222c 0a20 2020  chmarkView",.   
-00001d70: 2020 2020 2029 0a20 2020 2029 0a0a 0a63       ).    )...c
-00001d80: 6c61 7373 2050 726f 6475 6374 5065 7266  lass ProductPerf
-00001d90: 6f72 6d61 6e63 6556 6965 7728 7072 6f74  ormanceView(prot
-00001da0: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00001db0: 7222 2222 4669 656c 6473 2061 7661 696c  r"""Fields avail
-00001dc0: 6162 6c65 2066 6f72 2071 7565 7279 2069  able for query i
-00001dd0: 6e20 6060 7072 6f64 7563 745f 7065 7266  n ``product_perf
-00001de0: 6f72 6d61 6e63 655f 7669 6577 6060 2074  ormance_view`` t
-00001df0: 6162 6c65 2e0a 0a20 2020 2050 726f 6475  able...    Produ
-00001e00: 6374 2070 6572 666f 726d 616e 6365 2064  ct performance d
-00001e10: 6174 6120 666f 7220 796f 7572 2061 6363  ata for your acc
-00001e20: 6f75 6e74 2c20 696e 636c 7564 696e 6720  ount, including 
-00001e30: 7065 7266 6f72 6d61 6e63 650a 2020 2020  performance.    
-00001e40: 6d65 7472 6963 7320 2866 6f72 2065 7861  metrics (for exa
-00001e50: 6d70 6c65 2c20 6060 636c 6963 6b73 6060  mple, ``clicks``
-00001e60: 2920 616e 6420 6469 6d65 6e73 696f 6e73  ) and dimensions
-00001e70: 2061 6363 6f72 6469 6e67 2074 6f20 7768   according to wh
-00001e80: 6963 680a 2020 2020 7065 7266 6f72 6d61  ich.    performa
-00001e90: 6e63 6520 6d65 7472 6963 7320 6172 6520  nce metrics are 
-00001ea0: 7365 676d 656e 7465 6420 2866 6f72 2065  segmented (for e
-00001eb0: 7861 6d70 6c65 2c20 6060 6f66 6665 725f  xample, ``offer_
-00001ec0: 6964 6060 292e 0a20 2020 2056 616c 7565  id``)..    Value
-00001ed0: 7320 6f66 2070 726f 6475 6374 2064 696d  s of product dim
-00001ee0: 656e 7369 6f6e 732c 2073 7563 6820 6173  ensions, such as
-00001ef0: 2060 606f 6666 6572 5f69 6460 602c 2072   ``offer_id``, r
-00001f00: 6566 6c65 6374 2074 6865 0a20 2020 2073  eflect the.    s
-00001f10: 7461 7465 206f 6620 6120 7072 6f64 7563  tate of a produc
-00001f20: 7420 6174 2074 6865 2074 696d 6520 6f66  t at the time of
-00001f30: 2074 6865 2069 6d70 7265 7373 696f 6e2e   the impression.
-00001f40: 0a0a 2020 2020 5365 676d 656e 7420 6669  ..    Segment fi
-00001f50: 656c 6473 2063 616e 6e6f 7420 6265 2073  elds cannot be s
-00001f60: 656c 6563 7465 6420 696e 2071 7565 7269  elected in queri
-00001f70: 6573 2077 6974 686f 7574 2061 6c73 6f20  es without also 
-00001f80: 7365 6c65 6374 696e 670a 2020 2020 6174  selecting.    at
-00001f90: 206c 6561 7374 206f 6e65 206d 6574 7269   least one metri
-00001fa0: 6320 6669 656c 642e 0a0a 2020 2020 5661  c field...    Va
-00001fb0: 6c75 6573 2061 7265 206f 6e6c 7920 7365  lues are only se
-00001fc0: 7420 666f 7220 6669 656c 6473 2072 6571  t for fields req
-00001fd0: 7565 7374 6564 2065 7870 6c69 6369 746c  uested explicitl
-00001fe0: 7920 696e 2074 6865 2072 6571 7565 7374  y in the request
-00001ff0: 2773 0a20 2020 2073 6561 7263 6820 7175  's.    search qu
-00002000: 6572 792e 0a0a 0a20 2020 202e 2e20 5f6f  ery....    .. _o
-00002010: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
-00002020: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
-00002030: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00002040: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
-00002050: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
-00002060: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
-00002070: 6965 6c64 730a 0a20 2020 2041 7474 7269  ields..    Attri
-00002080: 6275 7465 733a 0a20 2020 2020 2020 206d  butes:.        m
-00002090: 6172 6b65 7469 6e67 5f6d 6574 686f 6420  arketing_method 
-000020a0: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
-000020b0: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
-000020c0: 735f 7631 6265 7461 2e74 7970 6573 2e4d  s_v1beta.types.M
-000020d0: 6172 6b65 7469 6e67 4d65 7468 6f64 2e4d  arketingMethod.M
-000020e0: 6172 6b65 7469 6e67 4d65 7468 6f64 456e  arketingMethodEn
-000020f0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-00002100: 204d 6172 6b65 7469 6e67 206d 6574 686f   Marketing metho
-00002110: 6420 746f 2077 6869 6368 206d 6574 7269  d to which metri
-00002120: 6373 2061 7070 6c79 2e0a 2020 2020 2020  cs apply..      
-00002130: 2020 2020 2020 5365 676d 656e 742e 0a0a        Segment...
-00002140: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00002150: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00002160: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00002170: 605f 6d61 726b 6574 696e 675f 6d65 7468  `_marketing_meth
-00002180: 6f64 6060 2e0a 2020 2020 2020 2020 6461  od``..        da
-00002190: 7465 2028 676f 6f67 6c65 2e74 7970 652e  te (google.type.
-000021a0: 6461 7465 5f70 6232 2e44 6174 6529 3a0a  date_pb2.Date):.
-000021b0: 2020 2020 2020 2020 2020 2020 4461 7465              Date
-000021c0: 2069 6e20 7468 6520 6d65 7263 6861 6e74   in the merchant
-000021d0: 2074 696d 657a 6f6e 6520 746f 2077 6869   timezone to whi
-000021e0: 6368 206d 6574 7269 6373 2061 7070 6c79  ch metrics apply
-000021f0: 2e0a 2020 2020 2020 2020 2020 2020 5365  ..            Se
-00002200: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
-00002210: 2020 2020 436f 6e64 6974 696f 6e20 6f6e      Condition on
-00002220: 2060 6064 6174 6560 6020 6973 2072 6571   ``date`` is req
-00002230: 7569 7265 6420 696e 2074 6865 2060 6057  uired in the ``W
-00002240: 4845 5245 6060 2063 6c61 7573 652e 0a20  HERE`` clause.. 
-00002250: 2020 2020 2020 2077 6565 6b20 2867 6f6f         week (goo
-00002260: 676c 652e 7479 7065 2e64 6174 655f 7062  gle.type.date_pb
-00002270: 322e 4461 7465 293a 0a20 2020 2020 2020  2.Date):.       
-00002280: 2020 2020 2046 6972 7374 2064 6179 206f       First day o
-00002290: 6620 7468 6520 7765 656b 2028 4d6f 6e64  f the week (Mond
-000022a0: 6179 2920 6f66 2074 6865 206d 6574 7269  ay) of the metri
-000022b0: 6373 0a20 2020 2020 2020 2020 2020 2064  cs.            d
-000022c0: 6174 6520 696e 2074 6865 206d 6572 6368  ate in the merch
-000022d0: 616e 7420 7469 6d65 7a6f 6e65 2e20 5365  ant timezone. Se
-000022e0: 676d 656e 742e 0a20 2020 2020 2020 2063  gment..        c
-000022f0: 7573 746f 6d65 725f 636f 756e 7472 795f  ustomer_country_
-00002300: 636f 6465 2028 7374 7229 3a0a 2020 2020  code (str):.    
-00002310: 2020 2020 2020 2020 436f 6465 206f 6620          Code of 
-00002320: 7468 6520 636f 756e 7472 7920 7768 6572  the country wher
-00002330: 6520 7468 6520 6375 7374 6f6d 6572 2069  e the customer i
-00002340: 730a 2020 2020 2020 2020 2020 2020 6c6f  s.            lo
-00002350: 6361 7465 6420 6174 2074 6865 2074 696d  cated at the tim
-00002360: 6520 6f66 2074 6865 2065 7665 6e74 2e20  e of the event. 
-00002370: 5265 7072 6573 656e 7465 6420 696e 0a20  Represented in. 
-00002380: 2020 2020 2020 2020 2020 2074 6865 2049             the I
-00002390: 534f 2033 3136 3620 666f 726d 6174 2e20  SO 3166 format. 
-000023a0: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
-000023b0: 2020 2020 2020 4966 2074 6865 2063 7573        If the cus
-000023c0: 746f 6d65 7220 636f 756e 7472 7920 6361  tomer country ca
-000023d0: 6e6e 6f74 2062 6520 6465 7465 726d 696e  nnot be determin
-000023e0: 6564 2c20 610a 2020 2020 2020 2020 2020  ed, a.          
-000023f0: 2020 7370 6563 6961 6c20 275a 5a27 2063    special 'ZZ' c
-00002400: 6f64 6520 6973 2072 6574 7572 6e65 642e  ode is returned.
-00002410: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00002420: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00002430: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00002440: 2060 605f 6375 7374 6f6d 6572 5f63 6f75   ``_customer_cou
-00002450: 6e74 7279 5f63 6f64 6560 602e 0a20 2020  ntry_code``..   
-00002460: 2020 2020 206f 6666 6572 5f69 6420 2873       offer_id (s
-00002470: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00002480: 204d 6572 6368 616e 742d 7072 6f76 6964   Merchant-provid
-00002490: 6564 2069 6420 6f66 2074 6865 2070 726f  ed id of the pro
-000024a0: 6475 6374 2e20 5365 676d 656e 742e 0a0a  duct. Segment...
-000024b0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-000024c0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-000024d0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-000024e0: 605f 6f66 6665 725f 6964 6060 2e0a 2020  `_offer_id``..  
-000024f0: 2020 2020 2020 7469 746c 6520 2873 7472        title (str
-00002500: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-00002510: 6974 6c65 206f 6620 7468 6520 7072 6f64  itle of the prod
-00002520: 7563 742e 2053 6567 6d65 6e74 2e0a 0a20  uct. Segment... 
-00002530: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00002540: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00002550: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00002560: 5f74 6974 6c65 6060 2e0a 2020 2020 2020  _title``..      
-00002570: 2020 6272 616e 6420 2873 7472 293a 0a20    brand (str):. 
-00002580: 2020 2020 2020 2020 2020 2042 7261 6e64             Brand
-00002590: 206f 6620 7468 6520 7072 6f64 7563 742e   of the product.
-000025a0: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
-000025b0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-000025c0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-000025d0: 2060 6f6e 656f 6660 5f20 6060 5f62 7261   `oneof`_ ``_bra
-000025e0: 6e64 6060 2e0a 2020 2020 2020 2020 6361  nd``..        ca
-000025f0: 7465 676f 7279 5f6c 3120 2873 7472 293a  tegory_l1 (str):
-00002600: 0a20 2020 2020 2020 2020 2020 2060 5072  .            `Pr
-00002610: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-00002620: 3173 740a 2020 2020 2020 2020 2020 2020  1st.            
-00002630: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-00002640: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00002650: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-00002660: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-00002670: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-00002680: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-00002690: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-000026a0: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-000026b0: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-000026c0: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-000026d0: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-000026e0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-000026f0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002700: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00002710: 6c31 6060 2e0a 2020 2020 2020 2020 6361  l1``..        ca
-00002720: 7465 676f 7279 5f6c 3220 2873 7472 293a  tegory_l2 (str):
-00002730: 0a20 2020 2020 2020 2020 2020 2060 5072  .            `Pr
-00002740: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-00002750: 326e 640a 2020 2020 2020 2020 2020 2020  2nd.            
-00002760: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-00002770: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00002780: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-00002790: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-000027a0: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-000027b0: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-000027c0: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-000027d0: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-000027e0: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-000027f0: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-00002800: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00002810: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00002820: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002830: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00002840: 6c32 6060 2e0a 2020 2020 2020 2020 6361  l2``..        ca
-00002850: 7465 676f 7279 5f6c 3320 2873 7472 293a  tegory_l3 (str):
-00002860: 0a20 2020 2020 2020 2020 2020 2060 5072  .            `Pr
-00002870: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-00002880: 3372 640a 2020 2020 2020 2020 2020 2020  3rd.            
-00002890: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-000028a0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000028b0: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-000028c0: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-000028d0: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-000028e0: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-000028f0: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-00002900: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00002910: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-00002920: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-00002930: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00002940: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00002950: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002960: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00002970: 6c33 6060 2e0a 2020 2020 2020 2020 6361  l3``..        ca
-00002980: 7465 676f 7279 5f6c 3420 2873 7472 293a  tegory_l4 (str):
-00002990: 0a20 2020 2020 2020 2020 2020 2060 5072  .            `Pr
-000029a0: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-000029b0: 3474 680a 2020 2020 2020 2020 2020 2020  4th.            
-000029c0: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-000029d0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000029e0: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-000029f0: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-00002a00: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-00002a10: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-00002a20: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-00002a30: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00002a40: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-00002a50: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-00002a60: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00002a70: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00002a80: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002a90: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00002aa0: 6c34 6060 2e0a 2020 2020 2020 2020 6361  l4``..        ca
-00002ab0: 7465 676f 7279 5f6c 3520 2873 7472 293a  tegory_l5 (str):
-00002ac0: 0a20 2020 2020 2020 2020 2020 2060 5072  .            `Pr
-00002ad0: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-00002ae0: 3574 680a 2020 2020 2020 2020 2020 2020  5th.            
-00002af0: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-00002b00: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00002b10: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-00002b20: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-00002b30: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-00002b40: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-00002b50: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-00002b60: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00002b70: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-00002b80: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-00002b90: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00002ba0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00002bb0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002bc0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00002bd0: 6c35 6060 2e0a 2020 2020 2020 2020 7072  l5``..        pr
-00002be0: 6f64 7563 745f 7479 7065 5f6c 3120 2873  oduct_type_l1 (s
-00002bf0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00002c00: 2060 5072 6f64 7563 7420 7479 7065 2028   `Product type (
-00002c10: 3173 740a 2020 2020 2020 2020 2020 2020  1st.            
-00002c20: 6c65 7665 6c29 203c 6874 7470 733a 2f2f  level) <https://
-00002c30: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00002c40: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
-00002c50: 6f6e 7465 6e74 2f67 7569 6465 732f 7265  ontent/guides/re
-00002c60: 706f 7274 732f 7365 676d 656e 7461 7469  ports/segmentati
-00002c70: 6f6e 2363 6174 6567 6f72 795f 616e 645f  on#category_and_
-00002c80: 7072 6f64 7563 745f 7479 7065 3e60 5f5f  product_type>`__
-00002c90: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00002ca0: 6d65 7263 6861 6e74 2773 206f 776e 2070  merchant's own p
-00002cb0: 726f 6475 6374 2074 6178 6f6e 6f6d 792e  roduct taxonomy.
-00002cc0: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
-00002cd0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00002ce0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00002cf0: 2060 6f6e 656f 6660 5f20 6060 5f70 726f   `oneof`_ ``_pro
-00002d00: 6475 6374 5f74 7970 655f 6c31 6060 2e0a  duct_type_l1``..
-00002d10: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-00002d20: 7479 7065 5f6c 3220 2873 7472 293a 0a20  type_l2 (str):. 
-00002d30: 2020 2020 2020 2020 2020 2060 5072 6f64             `Prod
-00002d40: 7563 7420 7479 7065 2028 326e 640a 2020  uct type (2nd.  
-00002d50: 2020 2020 2020 2020 2020 6c65 7665 6c29            level)
-00002d60: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-00002d70: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-00002d80: 7368 6f70 7069 6e67 2d63 6f6e 7465 6e74  shopping-content
-00002d90: 2f67 7569 6465 732f 7265 706f 7274 732f  /guides/reports/
-00002da0: 7365 676d 656e 7461 7469 6f6e 2363 6174  segmentation#cat
-00002db0: 6567 6f72 795f 616e 645f 7072 6f64 7563  egory_and_produc
-00002dc0: 745f 7479 7065 3e60 5f5f 0a20 2020 2020  t_type>`__.     
-00002dd0: 2020 2020 2020 2069 6e20 6d65 7263 6861         in mercha
-00002de0: 6e74 2773 206f 776e 2070 726f 6475 6374  nt's own product
-00002df0: 2074 6178 6f6e 6f6d 792e 2053 6567 6d65   taxonomy. Segme
-00002e00: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00002e10: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00002e20: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00002e30: 6660 5f20 6060 5f70 726f 6475 6374 5f74  f`_ ``_product_t
-00002e40: 7970 655f 6c32 6060 2e0a 2020 2020 2020  ype_l2``..      
-00002e50: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-00002e60: 3320 2873 7472 293a 0a20 2020 2020 2020  3 (str):.       
-00002e70: 2020 2020 2060 5072 6f64 7563 7420 7479       `Product ty
-00002e80: 7065 2028 3372 640a 2020 2020 2020 2020  pe (3rd.        
-00002e90: 2020 2020 6c65 7665 6c29 203c 6874 7470      level) <http
-00002ea0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-00002eb0: 6f6f 676c 652e 636f 6d2f 7368 6f70 7069  oogle.com/shoppi
-00002ec0: 6e67 2d63 6f6e 7465 6e74 2f67 7569 6465  ng-content/guide
-00002ed0: 732f 7265 706f 7274 732f 7365 676d 656e  s/reports/segmen
-00002ee0: 7461 7469 6f6e 2363 6174 6567 6f72 795f  tation#category_
-00002ef0: 616e 645f 7072 6f64 7563 745f 7479 7065  and_product_type
-00002f00: 3e60 5f5f 0a20 2020 2020 2020 2020 2020  >`__.           
-00002f10: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
-00002f20: 776e 2070 726f 6475 6374 2074 6178 6f6e  wn product taxon
-00002f30: 6f6d 792e 2053 6567 6d65 6e74 2e0a 0a20  omy. Segment... 
-00002f40: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00002f50: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00002f60: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00002f70: 5f70 726f 6475 6374 5f74 7970 655f 6c33  _product_type_l3
-00002f80: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-00002f90: 7563 745f 7479 7065 5f6c 3420 2873 7472  uct_type_l4 (str
-00002fa0: 293a 0a20 2020 2020 2020 2020 2020 2060  ):.            `
-00002fb0: 5072 6f64 7563 7420 7479 7065 2028 3474  Product type (4t
-00002fc0: 680a 2020 2020 2020 2020 2020 2020 6c65  h.            le
-00002fd0: 7665 6c29 203c 6874 7470 733a 2f2f 6465  vel) <https://de
-00002fe0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00002ff0: 636f 6d2f 7368 6f70 7069 6e67 2d63 6f6e  com/shopping-con
-00003000: 7465 6e74 2f67 7569 6465 732f 7265 706f  tent/guides/repo
-00003010: 7274 732f 7365 676d 656e 7461 7469 6f6e  rts/segmentation
-00003020: 2363 6174 6567 6f72 795f 616e 645f 7072  #category_and_pr
-00003030: 6f64 7563 745f 7479 7065 3e60 5f5f 0a20  oduct_type>`__. 
-00003040: 2020 2020 2020 2020 2020 2069 6e20 6d65             in me
-00003050: 7263 6861 6e74 2773 206f 776e 2070 726f  rchant's own pro
-00003060: 6475 6374 2074 6178 6f6e 6f6d 792e 2053  duct taxonomy. S
-00003070: 6567 6d65 6e74 2e0a 0a20 2020 2020 2020  egment...       
-00003080: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00003090: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-000030a0: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
-000030b0: 6374 5f74 7970 655f 6c34 6060 2e0a 2020  ct_type_l4``..  
-000030c0: 2020 2020 2020 7072 6f64 7563 745f 7479        product_ty
-000030d0: 7065 5f6c 3520 2873 7472 293a 0a20 2020  pe_l5 (str):.   
-000030e0: 2020 2020 2020 2020 2060 5072 6f64 7563           `Produc
-000030f0: 7420 7479 7065 2028 3574 680a 2020 2020  t type (5th.    
-00003100: 2020 2020 2020 2020 6c65 7665 6c29 203c          level) <
-00003110: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00003120: 7273 2e67 6f6f 676c 652e 636f 6d2f 7368  rs.google.com/sh
-00003130: 6f70 7069 6e67 2d63 6f6e 7465 6e74 2f67  opping-content/g
-00003140: 7569 6465 732f 7265 706f 7274 732f 7365  uides/reports/se
-00003150: 676d 656e 7461 7469 6f6e 2363 6174 6567  gmentation#categ
-00003160: 6f72 795f 616e 645f 7072 6f64 7563 745f  ory_and_product_
-00003170: 7479 7065 3e60 5f5f 0a20 2020 2020 2020  type>`__.       
-00003180: 2020 2020 2069 6e20 6d65 7263 6861 6e74       in merchant
-00003190: 2773 206f 776e 2070 726f 6475 6374 2074  's own product t
-000031a0: 6178 6f6e 6f6d 792e 2053 6567 6d65 6e74  axonomy. Segment
-000031b0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-000031c0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000031d0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-000031e0: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-000031f0: 655f 6c35 6060 2e0a 2020 2020 2020 2020  e_l5``..        
-00003200: 6375 7374 6f6d 5f6c 6162 656c 3020 2873  custom_label0 (s
-00003210: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00003220: 2043 7573 746f 6d20 6c61 6265 6c20 3020   Custom label 0 
-00003230: 666f 7220 6375 7374 6f6d 2067 726f 7570  for custom group
-00003240: 696e 6720 6f66 0a20 2020 2020 2020 2020  ing of.         
-00003250: 2020 2070 726f 6475 6374 732e 2053 6567     products. Seg
-00003260: 6d65 6e74 2e0a 0a20 2020 2020 2020 2020  ment...         
-00003270: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00003280: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00003290: 656f 6660 5f20 6060 5f63 7573 746f 6d5f  eof`_ ``_custom_
-000032a0: 6c61 6265 6c30 6060 2e0a 2020 2020 2020  label0``..      
-000032b0: 2020 6375 7374 6f6d 5f6c 6162 656c 3120    custom_label1 
-000032c0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-000032d0: 2020 2043 7573 746f 6d20 6c61 6265 6c20     Custom label 
-000032e0: 3120 666f 7220 6375 7374 6f6d 2067 726f  1 for custom gro
-000032f0: 7570 696e 6720 6f66 0a20 2020 2020 2020  uping of.       
-00003300: 2020 2020 2070 726f 6475 6374 732e 2053       products. S
-00003310: 6567 6d65 6e74 2e0a 0a20 2020 2020 2020  egment...       
-00003320: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00003330: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00003340: 6f6e 656f 6660 5f20 6060 5f63 7573 746f  oneof`_ ``_custo
-00003350: 6d5f 6c61 6265 6c31 6060 2e0a 2020 2020  m_label1``..    
-00003360: 2020 2020 6375 7374 6f6d 5f6c 6162 656c      custom_label
-00003370: 3220 2873 7472 293a 0a20 2020 2020 2020  2 (str):.       
-00003380: 2020 2020 2043 7573 746f 6d20 6c61 6265       Custom labe
-00003390: 6c20 3220 666f 7220 6375 7374 6f6d 2067  l 2 for custom g
-000033a0: 726f 7570 696e 6720 6f66 0a20 2020 2020  rouping of.     
-000033b0: 2020 2020 2020 2070 726f 6475 6374 732e         products.
-000033c0: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
-000033d0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-000033e0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-000033f0: 2060 6f6e 656f 6660 5f20 6060 5f63 7573   `oneof`_ ``_cus
-00003400: 746f 6d5f 6c61 6265 6c32 6060 2e0a 2020  tom_label2``..  
-00003410: 2020 2020 2020 6375 7374 6f6d 5f6c 6162        custom_lab
-00003420: 656c 3320 2873 7472 293a 0a20 2020 2020  el3 (str):.     
-00003430: 2020 2020 2020 2043 7573 746f 6d20 6c61         Custom la
-00003440: 6265 6c20 3320 666f 7220 6375 7374 6f6d  bel 3 for custom
-00003450: 2067 726f 7570 696e 6720 6f66 0a20 2020   grouping of.   
-00003460: 2020 2020 2020 2020 2070 726f 6475 6374           product
-00003470: 732e 2053 6567 6d65 6e74 2e0a 0a20 2020  s. Segment...   
-00003480: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00003490: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-000034a0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f63  of `oneof`_ ``_c
-000034b0: 7573 746f 6d5f 6c61 6265 6c33 6060 2e0a  ustom_label3``..
-000034c0: 2020 2020 2020 2020 6375 7374 6f6d 5f6c          custom_l
-000034d0: 6162 656c 3420 2873 7472 293a 0a20 2020  abel4 (str):.   
-000034e0: 2020 2020 2020 2020 2043 7573 746f 6d20           Custom 
-000034f0: 6c61 6265 6c20 3420 666f 7220 6375 7374  label 4 for cust
-00003500: 6f6d 2067 726f 7570 696e 6720 6f66 0a20  om grouping of. 
-00003510: 2020 2020 2020 2020 2020 2070 726f 6475             produ
-00003520: 6374 732e 2053 6567 6d65 6e74 2e0a 0a20  cts. Segment... 
-00003530: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00003540: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00003550: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00003560: 5f63 7573 746f 6d5f 6c61 6265 6c34 6060  _custom_label4``
-00003570: 2e0a 2020 2020 2020 2020 636c 6963 6b73  ..        clicks
-00003580: 2028 696e 7429 3a0a 2020 2020 2020 2020   (int):.        
-00003590: 2020 2020 4e75 6d62 6572 206f 6620 636c      Number of cl
-000035a0: 6963 6b73 2e20 4d65 7472 6963 2e0a 0a20  icks. Metric... 
-000035b0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-000035c0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-000035d0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-000035e0: 5f63 6c69 636b 7360 602e 0a20 2020 2020  _clicks``..     
-000035f0: 2020 2069 6d70 7265 7373 696f 6e73 2028     impressions (
-00003600: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00003610: 2020 4e75 6d62 6572 206f 6620 7469 6d65    Number of time
-00003620: 7320 6d65 7263 6861 6e74 2773 2070 726f  s merchant's pro
-00003630: 6475 6374 7320 6172 650a 2020 2020 2020  ducts are.      
-00003640: 2020 2020 2020 7368 6f77 6e2e 204d 6574        shown. Met
-00003650: 7269 632e 0a0a 2020 2020 2020 2020 2020  ric...          
-00003660: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00003670: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00003680: 6f66 605f 2060 605f 696d 7072 6573 7369  of`_ ``_impressi
-00003690: 6f6e 7360 602e 0a20 2020 2020 2020 2063  ons``..        c
-000036a0: 6c69 636b 5f74 6872 6f75 6768 5f72 6174  lick_through_rat
-000036b0: 6520 2866 6c6f 6174 293a 0a20 2020 2020  e (float):.     
-000036c0: 2020 2020 2020 2043 6c69 636b 2d74 6872         Click-thr
-000036d0: 6f75 6768 2072 6174 6520 2d20 7468 6520  ough rate - the 
-000036e0: 6e75 6d62 6572 206f 6620 636c 6963 6b73  number of clicks
-000036f0: 0a20 2020 2020 2020 2020 2020 206d 6572  .            mer
-00003700: 6368 616e 7427 7320 7072 6f64 7563 7473  chant's products
-00003710: 2072 6563 6569 7665 2028 636c 6963 6b73   receive (clicks
-00003720: 2920 6469 7669 6465 6420 6279 0a20 2020  ) divided by.   
-00003730: 2020 2020 2020 2020 2074 6865 206e 756d           the num
-00003740: 6265 7220 6f66 2074 696d 6573 2074 6865  ber of times the
-00003750: 2070 726f 6475 6374 7320 6172 6520 7368   products are sh
-00003760: 6f77 6e0a 2020 2020 2020 2020 2020 2020  own.            
-00003770: 2869 6d70 7265 7373 696f 6e73 292e 204d  (impressions). M
-00003780: 6574 7269 632e 0a0a 2020 2020 2020 2020  etric...        
-00003790: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-000037a0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000037b0: 6e65 6f66 605f 2060 605f 636c 6963 6b5f  neof`_ ``_click_
-000037c0: 7468 726f 7567 685f 7261 7465 6060 2e0a  through_rate``..
-000037d0: 2020 2020 2020 2020 636f 6e76 6572 7369          conversi
-000037e0: 6f6e 7320 2866 6c6f 6174 293a 0a20 2020  ons (float):.   
-000037f0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00003800: 6f66 2063 6f6e 7665 7273 696f 6e73 2061  of conversions a
-00003810: 7474 7269 6275 7465 6420 746f 2074 6865  ttributed to the
-00003820: 2070 726f 6475 6374 2c20 7265 706f 7274   product, report
-00003830: 6564 206f 6e0a 2020 2020 2020 2020 2020  ed on.          
-00003840: 2020 7468 6520 636f 6e76 6572 7369 6f6e    the conversion
-00003850: 2064 6174 652e 2044 6570 656e 6469 6e67   date. Depending
-00003860: 206f 6e20 7468 6520 6174 7472 6962 7574   on the attribut
-00003870: 696f 6e20 6d6f 6465 6c2c 2061 0a20 2020  ion model, a.   
-00003880: 2020 2020 2020 2020 2063 6f6e 7665 7273           convers
-00003890: 696f 6e20 6d69 6768 7420 6265 2064 6973  ion might be dis
-000038a0: 7472 6962 7574 6564 2061 6372 6f73 7320  tributed across 
-000038b0: 6d75 6c74 6970 6c65 2063 6c69 636b 732c  multiple clicks,
-000038c0: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
-000038d0: 7265 2065 6163 6820 636c 6963 6b20 6765  re each click ge
-000038e0: 7473 2069 7473 206f 776e 2063 7265 6469  ts its own credi
-000038f0: 7420 6173 7369 676e 6564 2e20 5468 6973  t assigned. This
-00003900: 206d 6574 7269 630a 2020 2020 2020 2020   metric.        
-00003910: 2020 2020 6973 2061 2073 756d 206f 6620      is a sum of 
-00003920: 616c 6c20 7375 6368 2063 7265 6469 7473  all such credits
-00003930: 2e20 4d65 7472 6963 2e0a 0a20 2020 2020  . Metric...     
-00003940: 2020 2020 2020 2041 7661 696c 6162 6c65         Available
-00003950: 206f 6e6c 7920 666f 7220 7468 6520 6060   only for the ``
-00003960: 4652 4545 6060 2074 7261 6666 6963 2073  FREE`` traffic s
-00003970: 6f75 7263 652e 0a0a 2020 2020 2020 2020  ource...        
-00003980: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00003990: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000039a0: 6e65 6f66 605f 2060 605f 636f 6e76 6572  neof`_ ``_conver
-000039b0: 7369 6f6e 7360 602e 0a20 2020 2020 2020  sions``..       
-000039c0: 2063 6f6e 7665 7273 696f 6e5f 7661 6c75   conversion_valu
-000039d0: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
-000039e0: 6e67 2e74 7970 652e 7479 7065 732e 5072  ng.type.types.Pr
-000039f0: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
-00003a00: 2020 5661 6c75 6520 6f66 2063 6f6e 7665    Value of conve
-00003a10: 7273 696f 6e73 2061 7474 7269 6275 7465  rsions attribute
-00003a20: 6420 746f 2074 6865 2070 726f 6475 6374  d to the product
-00003a30: 2c20 7265 706f 7274 6564 206f 6e0a 2020  , reported on.  
-00003a40: 2020 2020 2020 2020 2020 7468 6520 636f            the co
-00003a50: 6e76 6572 7369 6f6e 2064 6174 652e 204d  nversion date. M
-00003a60: 6574 7269 632e 0a0a 2020 2020 2020 2020  etric...        
-00003a70: 2020 2020 4176 6169 6c61 626c 6520 6f6e      Available on
-00003a80: 6c79 2066 6f72 2074 6865 2060 6046 5245  ly for the ``FRE
-00003a90: 4560 6020 7472 6166 6669 6320 736f 7572  E`` traffic sour
-00003aa0: 6365 2e0a 2020 2020 2020 2020 636f 6e76  ce..        conv
-00003ab0: 6572 7369 6f6e 5f72 6174 6520 2866 6c6f  ersion_rate (flo
-00003ac0: 6174 293a 0a20 2020 2020 2020 2020 2020  at):.           
-00003ad0: 204e 756d 6265 7220 6f66 2063 6f6e 7665   Number of conve
-00003ae0: 7273 696f 6e73 2064 6976 6964 6564 2062  rsions divided b
-00003af0: 7920 7468 6520 6e75 6d62 6572 206f 6620  y the number of 
-00003b00: 636c 6963 6b73 2c0a 2020 2020 2020 2020  clicks,.        
-00003b10: 2020 2020 7265 706f 7274 6564 206f 6e20      reported on 
-00003b20: 7468 6520 696d 7072 6573 7369 6f6e 2064  the impression d
-00003b30: 6174 652e 204d 6574 7269 632e 0a0a 2020  ate. Metric...  
-00003b40: 2020 2020 2020 2020 2020 4176 6169 6c61            Availa
-00003b50: 626c 6520 6f6e 6c79 2066 6f72 2074 6865  ble only for the
-00003b60: 2060 6046 5245 4560 6020 7472 6166 6669   ``FREE`` traffi
-00003b70: 6320 736f 7572 6365 2e0a 0a20 2020 2020  c source...     
-00003b80: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00003b90: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00003ba0: 2060 6f6e 656f 6660 5f20 6060 5f63 6f6e   `oneof`_ ``_con
-00003bb0: 7665 7273 696f 6e5f 7261 7465 6060 2e0a  version_rate``..
-00003bc0: 2020 2020 2222 220a 0a20 2020 206d 6172      """..    mar
-00003bd0: 6b65 7469 6e67 5f6d 6574 686f 643a 2022  keting_method: "
-00003be0: 4d61 726b 6574 696e 674d 6574 686f 642e  MarketingMethod.
-00003bf0: 4d61 726b 6574 696e 674d 6574 686f 6445  MarketingMethodE
-00003c00: 6e75 6d22 203d 2070 726f 746f 2e46 6965  num" = proto.Fie
-00003c10: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00003c20: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
-00003c30: 6e75 6d62 6572 3d31 2c0a 2020 2020 2020  number=1,.      
-00003c40: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00003c50: 0a20 2020 2020 2020 2065 6e75 6d3d 224d  .        enum="M
-00003c60: 6172 6b65 7469 6e67 4d65 7468 6f64 2e4d  arketingMethod.M
-00003c70: 6172 6b65 7469 6e67 4d65 7468 6f64 456e  arketingMethodEn
-00003c80: 756d 222c 0a20 2020 2029 0a20 2020 2064  um",.    ).    d
-00003c90: 6174 653a 2064 6174 655f 7062 322e 4461  ate: date_pb2.Da
-00003ca0: 7465 203d 2070 726f 746f 2e46 6965 6c64  te = proto.Field
-00003cb0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00003cc0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-00003cd0: 206e 756d 6265 723d 322c 0a20 2020 2020   number=2,.     
-00003ce0: 2020 206d 6573 7361 6765 3d64 6174 655f     message=date_
-00003cf0: 7062 322e 4461 7465 2c0a 2020 2020 290a  pb2.Date,.    ).
-00003d00: 2020 2020 7765 656b 3a20 6461 7465 5f70      week: date_p
-00003d10: 6232 2e44 6174 6520 3d20 7072 6f74 6f2e  b2.Date = proto.
-00003d20: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00003d30: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00003d40: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
-00003d50: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00003d60: 6461 7465 5f70 6232 2e44 6174 652c 0a20  date_pb2.Date,. 
-00003d70: 2020 2029 0a20 2020 2063 7573 746f 6d65     ).    custome
-00003d80: 725f 636f 756e 7472 795f 636f 6465 3a20  r_country_code: 
-00003d90: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-00003da0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00003db0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-00003dc0: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
-00003dd0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00003de0: 2c0a 2020 2020 290a 2020 2020 6f66 6665  ,.    ).    offe
-00003df0: 725f 6964 3a20 7374 7220 3d20 7072 6f74  r_id: str = prot
-00003e00: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00003e10: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00003e20: 2020 2020 2020 206e 756d 6265 723d 352c         number=5,
-00003e30: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00003e40: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00003e50: 2020 7469 746c 653a 2073 7472 203d 2070    title: str = p
-00003e60: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00003e70: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00003e80: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00003e90: 3d36 2c0a 2020 2020 2020 2020 6f70 7469  =6,.        opti
-00003ea0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-00003eb0: 0a20 2020 2062 7261 6e64 3a20 7374 7220  .    brand: str 
-00003ec0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00003ed0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00003ee0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00003ef0: 6265 723d 372c 0a20 2020 2020 2020 206f  ber=7,.        o
-00003f00: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00003f10: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-00003f20: 5f6c 313a 2073 7472 203d 2070 726f 746f  _l1: str = proto
-00003f30: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00003f40: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00003f50: 2020 2020 2020 6e75 6d62 6572 3d38 2c0a        number=8,.
-00003f60: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00003f70: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-00003f80: 2063 6174 6567 6f72 795f 6c32 3a20 7374   category_l2: st
-00003f90: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-00003fa0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-00003fb0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00003fc0: 756d 6265 723d 392c 0a20 2020 2020 2020  umber=9,.       
-00003fd0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00003fe0: 2020 2020 290a 2020 2020 6361 7465 676f      ).    catego
-00003ff0: 7279 5f6c 333a 2073 7472 203d 2070 726f  ry_l3: str = pro
-00004000: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00004010: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-00004020: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-00004030: 302c 0a20 2020 2020 2020 206f 7074 696f  0,.        optio
-00004040: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-00004050: 2020 2020 6361 7465 676f 7279 5f6c 343a      category_l4:
-00004060: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00004070: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00004080: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00004090: 2020 6e75 6d62 6572 3d31 312c 0a20 2020    number=11,.   
-000040a0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-000040b0: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
-000040c0: 7465 676f 7279 5f6c 353a 2073 7472 203d  tegory_l5: str =
-000040d0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-000040e0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-000040f0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00004100: 6572 3d31 322c 0a20 2020 2020 2020 206f  er=12,.        o
-00004110: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00004120: 2020 290a 2020 2020 7072 6f64 7563 745f    ).    product_
-00004130: 7479 7065 5f6c 313a 2073 7472 203d 2070  type_l1: str = p
-00004140: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00004150: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00004160: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00004170: 3d31 332c 0a20 2020 2020 2020 206f 7074  =13,.        opt
-00004180: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00004190: 290a 2020 2020 7072 6f64 7563 745f 7479  ).    product_ty
-000041a0: 7065 5f6c 323a 2073 7472 203d 2070 726f  pe_l2: str = pro
-000041b0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-000041c0: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-000041d0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-000041e0: 342c 0a20 2020 2020 2020 206f 7074 696f  4,.        optio
-000041f0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-00004200: 2020 2020 7072 6f64 7563 745f 7479 7065      product_type
-00004210: 5f6c 333a 2073 7472 203d 2070 726f 746f  _l3: str = proto
-00004220: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00004230: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00004240: 2020 2020 2020 6e75 6d62 6572 3d31 352c        number=15,
-00004250: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00004260: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00004270: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-00004280: 343a 2073 7472 203d 2070 726f 746f 2e46  4: str = proto.F
-00004290: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-000042a0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-000042b0: 2020 2020 6e75 6d62 6572 3d31 362c 0a20      number=16,. 
-000042c0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-000042d0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-000042e0: 7072 6f64 7563 745f 7479 7065 5f6c 353a  product_type_l5:
-000042f0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00004300: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00004310: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00004320: 2020 6e75 6d62 6572 3d31 372c 0a20 2020    number=17,.   
-00004330: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00004340: 7565 2c0a 2020 2020 290a 2020 2020 6375  ue,.    ).    cu
-00004350: 7374 6f6d 5f6c 6162 656c 303a 2073 7472  stom_label0: str
-00004360: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00004370: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-00004380: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-00004390: 6d62 6572 3d31 382c 0a20 2020 2020 2020  mber=18,.       
-000043a0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-000043b0: 2020 2020 290a 2020 2020 6375 7374 6f6d      ).    custom
-000043c0: 5f6c 6162 656c 313a 2073 7472 203d 2070  _label1: str = p
-000043d0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000043e0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-000043f0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00004400: 3d31 392c 0a20 2020 2020 2020 206f 7074  =19,.        opt
-00004410: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00004420: 290a 2020 2020 6375 7374 6f6d 5f6c 6162  ).    custom_lab
-00004430: 656c 323a 2073 7472 203d 2070 726f 746f  el2: str = proto
-00004440: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00004450: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00004460: 2020 2020 2020 6e75 6d62 6572 3d32 302c        number=20,
-00004470: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00004480: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00004490: 2020 6375 7374 6f6d 5f6c 6162 656c 333a    custom_label3:
-000044a0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-000044b0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-000044c0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-000044d0: 2020 6e75 6d62 6572 3d32 312c 0a20 2020    number=21,.   
-000044e0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-000044f0: 7565 2c0a 2020 2020 290a 2020 2020 6375  ue,.    ).    cu
-00004500: 7374 6f6d 5f6c 6162 656c 343a 2073 7472  stom_label4: str
-00004510: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00004520: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-00004530: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-00004540: 6d62 6572 3d32 322c 0a20 2020 2020 2020  mber=22,.       
-00004550: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00004560: 2020 2020 290a 2020 2020 636c 6963 6b73      ).    clicks
-00004570: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
-00004580: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00004590: 746f 2e49 4e54 3634 2c0a 2020 2020 2020  to.INT64,.      
-000045a0: 2020 6e75 6d62 6572 3d32 332c 0a20 2020    number=23,.   
-000045b0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-000045c0: 7565 2c0a 2020 2020 290a 2020 2020 696d  ue,.    ).    im
-000045d0: 7072 6573 7369 6f6e 733a 2069 6e74 203d  pressions: int =
-000045e0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-000045f0: 2020 2020 2020 7072 6f74 6f2e 494e 5436        proto.INT6
-00004600: 342c 0a20 2020 2020 2020 206e 756d 6265  4,.        numbe
-00004610: 723d 3234 2c0a 2020 2020 2020 2020 6f70  r=24,.        op
-00004620: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00004630: 2029 0a20 2020 2063 6c69 636b 5f74 6872   ).    click_thr
-00004640: 6f75 6768 5f72 6174 653a 2066 6c6f 6174  ough_rate: float
-00004650: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00004660: 2020 2020 2020 2020 7072 6f74 6f2e 444f          proto.DO
-00004670: 5542 4c45 2c0a 2020 2020 2020 2020 6e75  UBLE,.        nu
-00004680: 6d62 6572 3d32 352c 0a20 2020 2020 2020  mber=25,.       
-00004690: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-000046a0: 2020 2020 290a 2020 2020 636f 6e76 6572      ).    conver
-000046b0: 7369 6f6e 733a 2066 6c6f 6174 203d 2070  sions: float = p
-000046c0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000046d0: 2020 2020 7072 6f74 6f2e 444f 5542 4c45      proto.DOUBLE
-000046e0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-000046f0: 3d32 362c 0a20 2020 2020 2020 206f 7074  =26,.        opt
-00004700: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00004710: 290a 2020 2020 636f 6e76 6572 7369 6f6e  ).    conversion
-00004720: 5f76 616c 7565 3a20 7479 7065 732e 5072  _value: types.Pr
-00004730: 6963 6520 3d20 7072 6f74 6f2e 4669 656c  ice = proto.Fiel
-00004740: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00004750: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-00004760: 2020 6e75 6d62 6572 3d32 372c 0a20 2020    number=27,.   
-00004770: 2020 2020 206d 6573 7361 6765 3d74 7970       message=typ
-00004780: 6573 2e50 7269 6365 2c0a 2020 2020 290a  es.Price,.    ).
-00004790: 2020 2020 636f 6e76 6572 7369 6f6e 5f72      conversion_r
-000047a0: 6174 653a 2066 6c6f 6174 203d 2070 726f  ate: float = pro
-000047b0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-000047c0: 2020 7072 6f74 6f2e 444f 5542 4c45 2c0a    proto.DOUBLE,.
-000047d0: 2020 2020 2020 2020 6e75 6d62 6572 3d32          number=2
-000047e0: 382c 0a20 2020 2020 2020 206f 7074 696f  8,.        optio
-000047f0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-00004800: 0a0a 636c 6173 7320 5072 6f64 7563 7456  ..class ProductV
-00004810: 6965 7728 7072 6f74 6f2e 4d65 7373 6167  iew(proto.Messag
-00004820: 6529 3a0a 2020 2020 7222 2222 4669 656c  e):.    r"""Fiel
-00004830: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
-00004840: 2071 7565 7279 2069 6e20 6060 7072 6f64   query in ``prod
-00004850: 7563 745f 7669 6577 6060 2074 6162 6c65  uct_view`` table
-00004860: 2e0a 0a20 2020 2050 726f 6475 6374 7320  ...    Products 
-00004870: 696e 2074 6865 2063 7572 7265 6e74 2069  in the current i
-00004880: 6e76 656e 746f 7279 2e20 5072 6f64 7563  nventory. Produc
-00004890: 7473 2069 6e20 7468 6973 2074 6162 6c65  ts in this table
-000048a0: 2061 7265 2074 6865 0a20 2020 2073 616d   are the.    sam
-000048b0: 6520 6173 2069 6e20 5072 6f64 7563 7473  e as in Products
-000048c0: 2073 7562 2d41 5049 2062 7574 206e 6f74   sub-API but not
-000048d0: 2061 6c6c 2070 726f 6475 6374 2061 7474   all product att
-000048e0: 7269 6275 7465 7320 6672 6f6d 0a20 2020  ributes from.   
-000048f0: 2050 726f 6475 6374 7320 7375 622d 4150   Products sub-AP
-00004900: 4920 6172 6520 6176 6169 6c61 626c 6520  I are available 
-00004910: 666f 7220 7175 6572 7920 696e 2074 6869  for query in thi
-00004920: 7320 7461 626c 652e 2049 6e20 636f 6e74  s table. In cont
-00004930: 7261 7374 0a20 2020 2074 6f20 5072 6f64  rast.    to Prod
-00004940: 7563 7473 2073 7562 2d41 5049 2c20 7468  ucts sub-API, th
-00004950: 6973 2074 6162 6c65 2061 6c6c 6f77 7320  is table allows 
-00004960: 746f 2066 696c 7465 7220 7468 6520 7265  to filter the re
-00004970: 7475 726e 6564 206c 6973 740a 2020 2020  turned list.    
-00004980: 6f66 2070 726f 6475 6374 7320 6279 2070  of products by p
-00004990: 726f 6475 6374 2061 7474 7269 6275 7465  roduct attribute
-000049a0: 732e 2054 6f20 7265 7472 6965 7665 2061  s. To retrieve a
-000049b0: 2073 696e 676c 6520 7072 6f64 7563 7420   single product 
-000049c0: 6279 0a20 2020 2060 6069 6460 6020 6f72  by.    ``id`` or
-000049d0: 206c 6973 7420 616c 6c20 7072 6f64 7563   list all produc
-000049e0: 7473 2c20 5072 6f64 7563 7473 2073 7562  ts, Products sub
-000049f0: 2d41 5049 2073 686f 756c 6420 6265 2075  -API should be u
-00004a00: 7365 642e 0a0a 2020 2020 5661 6c75 6573  sed...    Values
-00004a10: 2061 7265 206f 6e6c 7920 7365 7420 666f   are only set fo
-00004a20: 7220 6669 656c 6473 2072 6571 7565 7374  r fields request
-00004a30: 6564 2065 7870 6c69 6369 746c 7920 696e  ed explicitly in
-00004a40: 2074 6865 2072 6571 7565 7374 2773 0a20   the request's. 
-00004a50: 2020 2073 6561 7263 6820 7175 6572 792e     search query.
-00004a60: 0a0a 0a20 2020 202e 2e20 5f6f 6e65 6f66  ...    .. _oneof
-00004a70: 3a20 6874 7470 733a 2f2f 7072 6f74 6f2d  : https://proto-
-00004a80: 706c 7573 2d70 7974 686f 6e2e 7265 6164  plus-python.read
-00004a90: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00004aa0: 6162 6c65 2f66 6965 6c64 732e 6874 6d6c  able/fields.html
-00004ab0: 236f 6e65 6f66 732d 6d75 7475 616c 6c79  #oneofs-mutually
-00004ac0: 2d65 7863 6c75 7369 7665 2d66 6965 6c64  -exclusive-field
-00004ad0: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
-00004ae0: 733a 0a20 2020 2020 2020 2069 6420 2873  s:.        id (s
-00004af0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00004b00: 2052 4553 5420 4944 206f 6620 7468 6520   REST ID of the 
-00004b10: 7072 6f64 7563 742c 2069 6e20 7468 6520  product, in the 
-00004b20: 666f 726d 206f 660a 2020 2020 2020 2020  form of.        
-00004b30: 2020 2020 6060 6368 616e 6e65 6c7e 6c61      ``channel~la
-00004b40: 6e67 7561 6765 436f 6465 7e66 6565 644c  nguageCode~feedL
-00004b50: 6162 656c 7e6f 6666 6572 4964 6060 2e20  abel~offerId``. 
-00004b60: 4d65 7263 6861 6e74 2041 5049 0a20 2020  Merchant API.   
-00004b70: 2020 2020 2020 2020 206d 6574 686f 6473           methods
-00004b80: 2074 6861 7420 6f70 6572 6174 6520 6f6e   that operate on
-00004b90: 2070 726f 6475 6374 7320 7461 6b65 2074   products take t
-00004ba0: 6869 7320 6173 2074 6865 6972 2060 606e  his as their ``n
-00004bb0: 616d 6560 600a 2020 2020 2020 2020 2020  ame``.          
-00004bc0: 2020 7061 7261 6d65 7465 722e 0a0a 2020    parameter...  
-00004bd0: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-00004be0: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
-00004bf0: 4354 6060 2063 6c61 7573 652e 0a0a 2020  CT`` clause...  
-00004c00: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00004c10: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00004c20: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00004c30: 6964 6060 2e0a 2020 2020 2020 2020 6368  id``..        ch
-00004c40: 616e 6e65 6c20 2867 6f6f 676c 652e 7368  annel (google.sh
-00004c50: 6f70 7069 6e67 2e74 7970 652e 7479 7065  opping.type.type
-00004c60: 732e 4368 616e 6e65 6c2e 4368 616e 6e65  s.Channel.Channe
-00004c70: 6c45 6e75 6d29 3a0a 2020 2020 2020 2020  lEnum):.        
-00004c80: 2020 2020 4368 616e 6e65 6c20 6f66 2074      Channel of t
-00004c90: 6865 2070 726f 6475 6374 2e20 4361 6e20  he product. Can 
-00004ca0: 6265 2060 604f 4e4c 494e 4560 6020 6f72  be ``ONLINE`` or
-00004cb0: 2060 604c 4f43 414c 6060 2e0a 0a20 2020   ``LOCAL``...   
-00004cc0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00004cd0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00004ce0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f63  of `oneof`_ ``_c
-00004cf0: 6861 6e6e 656c 6060 2e0a 2020 2020 2020  hannel``..      
-00004d00: 2020 6c61 6e67 7561 6765 5f63 6f64 6520    language_code 
-00004d10: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00004d20: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
-00004d30: 206f 6620 7468 6520 7072 6f64 7563 7420   of the product 
-00004d40: 696e 2042 4350 2034 370a 2020 2020 2020  in BCP 47.      
-00004d50: 2020 2020 2020 666f 726d 6174 2e0a 0a20        format... 
-00004d60: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00004d70: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00004d80: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00004d90: 5f6c 616e 6775 6167 655f 636f 6465 6060  _language_code``
-00004da0: 2e0a 2020 2020 2020 2020 6665 6564 5f6c  ..        feed_l
-00004db0: 6162 656c 2028 7374 7229 3a0a 2020 2020  abel (str):.    
-00004dc0: 2020 2020 2020 2020 4665 6564 206c 6162          Feed lab
-00004dd0: 656c 206f 6620 7468 6520 7072 6f64 7563  el of the produc
-00004de0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00004df0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00004e00: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00004e10: 605f 2060 605f 6665 6564 5f6c 6162 656c  `_ ``_feed_label
-00004e20: 6060 2e0a 2020 2020 2020 2020 6f66 6665  ``..        offe
-00004e30: 725f 6964 2028 7374 7229 3a0a 2020 2020  r_id (str):.    
-00004e40: 2020 2020 2020 2020 4d65 7263 6861 6e74          Merchant
-00004e50: 2d70 726f 7669 6465 6420 6964 206f 6620  -provided id of 
-00004e60: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
-00004e70: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00004e80: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00004e90: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00004ea0: 6f66 6665 725f 6964 6060 2e0a 2020 2020  offer_id``..    
-00004eb0: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
-00004ec0: 0a20 2020 2020 2020 2020 2020 2054 6974  .            Tit
-00004ed0: 6c65 206f 6620 7468 6520 7072 6f64 7563  le of the produc
-00004ee0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00004ef0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00004f00: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00004f10: 605f 2060 605f 7469 746c 6560 602e 0a20  `_ ``_title``.. 
-00004f20: 2020 2020 2020 2062 7261 6e64 2028 7374         brand (st
-00004f30: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00004f40: 4272 616e 6420 6f66 2074 6865 2070 726f  Brand of the pro
-00004f50: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
-00004f60: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00004f70: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00004f80: 656f 6660 5f20 6060 5f62 7261 6e64 6060  eof`_ ``_brand``
-00004f90: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-00004fa0: 7279 5f6c 3120 2873 7472 293a 0a20 2020  ry_l1 (str):.   
-00004fb0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-00004fc0: 2063 6174 6567 6f72 7920 2831 7374 206c   category (1st l
-00004fd0: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
-00004fe0: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-00004ff0: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00005000: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00005010: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00005020: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-00005030: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-00005040: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00005050: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00005060: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-00005070: 6567 6f72 795f 6c31 6060 2e0a 2020 2020  egory_l1``..    
-00005080: 2020 2020 6361 7465 676f 7279 5f6c 3220      category_l2 
-00005090: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-000050a0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-000050b0: 6f72 7920 2832 6e64 206c 6576 656c 2920  ory (2nd level) 
-000050c0: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-000050d0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-000050e0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-000050f0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00005100: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00005110: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-00005120: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-00005130: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00005140: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00005150: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00005160: 6c32 6060 2e0a 2020 2020 2020 2020 6361  l2``..        ca
-00005170: 7465 676f 7279 5f6c 3320 2873 7472 293a  tegory_l3 (str):
-00005180: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-00005190: 6475 6374 2063 6174 6567 6f72 7920 2833  duct category (3
-000051a0: 7264 206c 6576 656c 2920 696e 2060 476f  rd level) in `Go
-000051b0: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-000051c0: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-000051d0: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-000051e0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-000051f0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-00005200: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-00005210: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00005220: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00005230: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00005240: 5f63 6174 6567 6f72 795f 6c33 6060 2e0a  _category_l3``..
-00005250: 2020 2020 2020 2020 6361 7465 676f 7279          category
-00005260: 5f6c 3420 2873 7472 293a 0a20 2020 2020  _l4 (str):.     
-00005270: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-00005280: 6174 6567 6f72 7920 2834 7468 206c 6576  ategory (4th lev
-00005290: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
-000052a0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-000052b0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-000052c0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-000052d0: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-000052e0: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-000052f0: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-00005300: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00005310: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00005320: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-00005330: 6f72 795f 6c34 6060 2e0a 2020 2020 2020  ory_l4``..      
-00005340: 2020 6361 7465 676f 7279 5f6c 3520 2873    category_l5 (s
-00005350: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00005360: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
-00005370: 7920 2835 7468 206c 6576 656c 2920 696e  y (5th level) in
-00005380: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
-00005390: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-000053a0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-000053b0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-000053c0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-000053d0: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
-000053e0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-000053f0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00005400: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00005410: 5f20 6060 5f63 6174 6567 6f72 795f 6c35  _ ``_category_l5
-00005420: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-00005430: 7563 745f 7479 7065 5f6c 3120 2873 7472  uct_type_l1 (str
-00005440: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-00005450: 726f 6475 6374 2074 7970 6520 2831 7374  roduct type (1st
-00005460: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
-00005470: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
-00005480: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-00005490: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-000054a0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-000054b0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-000054c0: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
-000054d0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-000054e0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000054f0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00005500: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-00005510: 655f 6c31 6060 2e0a 2020 2020 2020 2020  e_l1``..        
-00005520: 7072 6f64 7563 745f 7479 7065 5f6c 3220  product_type_l2 
-00005530: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00005540: 2020 2050 726f 6475 6374 2074 7970 6520     Product type 
-00005550: 2832 6e64 206c 6576 656c 2920 696e 206d  (2nd level) in m
-00005560: 6572 6368 616e 7427 7320 6f77 6e20 6070  erchant's own `p
-00005570: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
-00005580: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
-00005590: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-000055a0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-000055b0: 732f 616e 7377 6572 2f36 3332 3434 3036  s/answer/6324406
-000055c0: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
-000055d0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-000055e0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-000055f0: 656f 6660 5f20 6060 5f70 726f 6475 6374  eof`_ ``_product
-00005600: 5f74 7970 655f 6c32 6060 2e0a 2020 2020  _type_l2``..    
-00005610: 2020 2020 7072 6f64 7563 745f 7479 7065      product_type
-00005620: 5f6c 3320 2873 7472 293a 0a20 2020 2020  _l3 (str):.     
-00005630: 2020 2020 2020 2050 726f 6475 6374 2074         Product t
-00005640: 7970 6520 2833 7264 206c 6576 656c 2920  ype (3rd level) 
-00005650: 696e 206d 6572 6368 616e 7427 7320 6f77  in merchant's ow
-00005660: 6e20 6070 726f 6475 6374 0a20 2020 2020  n `product.     
-00005670: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00005680: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00005690: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-000056a0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-000056b0: 3434 3036 3e60 5f5f 2e0a 0a20 2020 2020  4406>`__...     
-000056c0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-000056d0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-000056e0: 2060 6f6e 656f 6660 5f20 6060 5f70 726f   `oneof`_ ``_pro
-000056f0: 6475 6374 5f74 7970 655f 6c33 6060 2e0a  duct_type_l3``..
-00005700: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-00005710: 7479 7065 5f6c 3420 2873 7472 293a 0a20  type_l4 (str):. 
-00005720: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-00005730: 6374 2074 7970 6520 2834 7468 206c 6576  ct type (4th lev
-00005740: 656c 2920 696e 206d 6572 6368 616e 7427  el) in merchant'
-00005750: 7320 6f77 6e20 6070 726f 6475 6374 0a20  s own `product. 
-00005760: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-00005770: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-00005780: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-00005790: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-000057a0: 2f36 3332 3434 3036 3e60 5f5f 2e0a 0a20  /6324406>`__... 
-000057b0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-000057c0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-000057d0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-000057e0: 5f70 726f 6475 6374 5f74 7970 655f 6c34  _product_type_l4
-000057f0: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-00005800: 7563 745f 7479 7065 5f6c 3520 2873 7472  uct_type_l5 (str
-00005810: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-00005820: 726f 6475 6374 2074 7970 6520 2835 7468  roduct type (5th
-00005830: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
-00005840: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
-00005850: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-00005860: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-00005870: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-00005880: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-00005890: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
-000058a0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-000058b0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000058c0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-000058d0: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-000058e0: 655f 6c35 6060 2e0a 2020 2020 2020 2020  e_l5``..        
-000058f0: 7072 6963 6520 2867 6f6f 676c 652e 7368  price (google.sh
-00005900: 6f70 7069 6e67 2e74 7970 652e 7479 7065  opping.type.type
-00005910: 732e 5072 6963 6529 3a0a 2020 2020 2020  s.Price):.      
-00005920: 2020 2020 2020 5072 6f64 7563 7420 7072        Product pr
-00005930: 6963 652e 2041 6273 656e 7420 6966 2074  ice. Absent if t
-00005940: 6865 2069 6e66 6f72 6d61 7469 6f6e 0a20  he information. 
-00005950: 2020 2020 2020 2020 2020 2061 626f 7574             about
-00005960: 2074 6865 2070 7269 6365 206f 6620 7468   the price of th
-00005970: 6520 7072 6f64 7563 7420 6973 206e 6f74  e product is not
-00005980: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
-00005990: 2020 2020 636f 6e64 6974 696f 6e20 2873      condition (s
-000059a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000059b0: 2060 436f 6e64 6974 696f 6e20 3c68 7474   `Condition <htt
-000059c0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-000059d0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-000059e0: 732f 616e 7377 6572 2f36 3332 3434 3639  s/answer/6324469
-000059f0: 3e60 5f5f 0a20 2020 2020 2020 2020 2020  >`__.           
-00005a00: 206f 6620 7468 6520 7072 6f64 7563 742e   of the product.
-00005a10: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00005a20: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00005a30: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00005a40: 2060 605f 636f 6e64 6974 696f 6e60 602e   ``_condition``.
-00005a50: 0a20 2020 2020 2020 2061 7661 696c 6162  .        availab
-00005a60: 696c 6974 7920 2873 7472 293a 0a20 2020  ility (str):.   
-00005a70: 2020 2020 2020 2020 2060 4176 6169 6c61           `Availa
-00005a80: 6269 6c69 7479 203c 6874 7470 733a 2f2f  bility <https://
-00005a90: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
-00005aa0: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
-00005ab0: 7765 722f 3633 3234 3434 383e 605f 5f0a  wer/6324448>`__.
-00005ac0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-00005ad0: 6865 2070 726f 6475 6374 2e0a 0a20 2020  he product...   
-00005ae0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00005af0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00005b00: 6f66 2060 6f6e 656f 6660 5f20 6060 5f61  of `oneof`_ ``_a
-00005b10: 7661 696c 6162 696c 6974 7960 602e 0a20  vailability``.. 
-00005b20: 2020 2020 2020 2073 6869 7070 696e 675f         shipping_
-00005b30: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
-00005b40: 2020 2020 2020 2020 204e 6f72 6d61 6c69           Normali
-00005b50: 7a65 6420 6073 6869 7070 696e 670a 2020  zed `shipping.  
-00005b60: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-00005b70: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00005b80: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00005b90: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-00005ba0: 3435 3034 3e60 5f5f 0a20 2020 2020 2020  4504>`__.       
-00005bb0: 2020 2020 2073 7065 6369 6669 6564 2069       specified i
-00005bc0: 6e20 7468 6520 6665 6564 2e0a 0a20 2020  n the feed...   
-00005bd0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00005be0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00005bf0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f73  of `oneof`_ ``_s
-00005c00: 6869 7070 696e 675f 6c61 6265 6c60 602e  hipping_label``.
-00005c10: 0a20 2020 2020 2020 2067 7469 6e20 284d  .        gtin (M
-00005c20: 7574 6162 6c65 5365 7175 656e 6365 5b73  utableSequence[s
-00005c30: 7472 5d29 3a0a 2020 2020 2020 2020 2020  tr]):.          
-00005c40: 2020 4c69 7374 206f 6620 476c 6f62 616c    List of Global
-00005c50: 2054 7261 6465 2049 7465 6d20 4e75 6d62   Trade Item Numb
-00005c60: 6572 7320 2847 5449 4e73 2920 6f66 0a20  ers (GTINs) of. 
-00005c70: 2020 2020 2020 2020 2020 2074 6865 2070             the p
-00005c80: 726f 6475 6374 2e0a 2020 2020 2020 2020  roduct..        
-00005c90: 6974 656d 5f67 726f 7570 5f69 6420 2873  item_group_id (s
-00005ca0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00005cb0: 2049 7465 6d20 6772 6f75 7020 6964 2070   Item group id p
-00005cc0: 726f 7669 6465 6420 6279 2074 6865 206d  rovided by the m
-00005cd0: 6572 6368 616e 7420 666f 720a 2020 2020  erchant for.    
-00005ce0: 2020 2020 2020 2020 6772 6f75 7069 6e67          grouping
-00005cf0: 2076 6172 6961 6e74 7320 746f 6765 7468   variants togeth
-00005d00: 6572 2e0a 0a20 2020 2020 2020 2020 2020  er...           
-00005d10: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00005d20: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00005d30: 6660 5f20 6060 5f69 7465 6d5f 6772 6f75  f`_ ``_item_grou
-00005d40: 705f 6964 6060 2e0a 2020 2020 2020 2020  p_id``..        
-00005d50: 7468 756d 626e 6169 6c5f 6c69 6e6b 2028  thumbnail_link (
-00005d60: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00005d70: 2020 4c69 6e6b 2074 6f20 7468 6520 7072    Link to the pr
-00005d80: 6f63 6573 7365 6420 696d 6167 6520 6f66  ocessed image of
-00005d90: 2074 6865 2070 726f 6475 6374 2c0a 2020   the product,.  
-00005da0: 2020 2020 2020 2020 2020 686f 7374 6564            hosted
-00005db0: 206f 6e20 7468 6520 476f 6f67 6c65 2069   on the Google i
-00005dc0: 6e66 7261 7374 7275 6374 7572 652e 0a0a  nfrastructure...
-00005dd0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00005de0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00005df0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00005e00: 605f 7468 756d 626e 6169 6c5f 6c69 6e6b  `_thumbnail_link
-00005e10: 6060 2e0a 2020 2020 2020 2020 6372 6561  ``..        crea
-00005e20: 7469 6f6e 5f74 696d 6520 2867 6f6f 676c  tion_time (googl
-00005e30: 652e 7072 6f74 6f62 7566 2e74 696d 6573  e.protobuf.times
-00005e40: 7461 6d70 5f70 6232 2e54 696d 6573 7461  tamp_pb2.Timesta
-00005e50: 6d70 293a 0a20 2020 2020 2020 2020 2020  mp):.           
-00005e60: 2054 6865 2074 696d 6520 7468 6520 6d65   The time the me
-00005e70: 7263 6861 6e74 2063 7265 6174 6564 2074  rchant created t
-00005e80: 6865 2070 726f 6475 6374 2069 6e0a 2020  he product in.  
-00005e90: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
-00005ea0: 616d 7020 7365 636f 6e64 732e 0a20 2020  amp seconds..   
-00005eb0: 2020 2020 2065 7870 6972 6174 696f 6e5f       expiration_
-00005ec0: 6461 7465 2028 676f 6f67 6c65 2e74 7970  date (google.typ
-00005ed0: 652e 6461 7465 5f70 6232 2e44 6174 6529  e.date_pb2.Date)
-00005ee0: 3a0a 2020 2020 2020 2020 2020 2020 4578  :.            Ex
-00005ef0: 7069 7261 7469 6f6e 2064 6174 6520 666f  piration date fo
-00005f00: 7220 7468 6520 7072 6f64 7563 742c 2073  r the product, s
-00005f10: 7065 6369 6669 6564 206f 6e0a 2020 2020  pecified on.    
-00005f20: 2020 2020 2020 2020 696e 7365 7274 696f          insertio
-00005f30: 6e2e 0a20 2020 2020 2020 2061 6767 7265  n..        aggre
-00005f40: 6761 7465 645f 7265 706f 7274 696e 675f  gated_reporting_
-00005f50: 636f 6e74 6578 745f 7374 6174 7573 2028  context_status (
-00005f60: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-00005f70: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-00005f80: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
-00005f90: 6f64 7563 7456 6965 772e 4167 6772 6567  oductView.Aggreg
-00005fa0: 6174 6564 5265 706f 7274 696e 6743 6f6e  atedReportingCon
-00005fb0: 7465 7874 5374 6174 7573 293a 0a20 2020  textStatus):.   
-00005fc0: 2020 2020 2020 2020 2041 6767 7265 6761           Aggrega
-00005fd0: 7465 6420 7374 6174 7573 2e0a 0a20 2020  ted status...   
-00005fe0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00005ff0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00006000: 6f66 2060 6f6e 656f 6660 5f20 6060 5f61  of `oneof`_ ``_a
-00006010: 6767 7265 6761 7465 645f 7265 706f 7274  ggregated_report
-00006020: 696e 675f 636f 6e74 6578 745f 7374 6174  ing_context_stat
-00006030: 7573 6060 2e0a 2020 2020 2020 2020 6974  us``..        it
-00006040: 656d 5f69 7373 7565 7320 284d 7574 6162  em_issues (Mutab
-00006050: 6c65 5365 7175 656e 6365 5b67 6f6f 676c  leSequence[googl
-00006060: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
-00006070: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
-00006080: 7461 2e74 7970 6573 2e50 726f 6475 6374  ta.types.Product
-00006090: 5669 6577 2e49 7465 6d49 7373 7565 5d29  View.ItemIssue])
-000060a0: 3a0a 2020 2020 2020 2020 2020 2020 4c69  :.            Li
-000060b0: 7374 206f 6620 6974 656d 2069 7373 7565  st of item issue
-000060c0: 7320 666f 7220 7468 6520 7072 6f64 7563  s for the produc
-000060d0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-000060e0: 2a2a 5468 6973 2066 6965 6c64 2063 616e  **This field can
-000060f0: 6e6f 7420 6265 2075 7365 6420 666f 7220  not be used for 
-00006100: 736f 7274 696e 6720 7468 6520 7265 7375  sorting the resu
-00006110: 6c74 732e 2a2a 0a0a 2020 2020 2020 2020  lts.**..        
-00006120: 2020 2020 2a2a 4f6e 6c79 2073 656c 6563      **Only selec
-00006130: 7465 6420 6174 7472 6962 7574 6573 206f  ted attributes o
-00006140: 6620 7468 6973 2066 6965 6c64 2028 666f  f this field (fo
-00006150: 7220 6578 616d 706c 652c 0a20 2020 2020  r example,.     
-00006160: 2020 2020 2020 2060 6069 7465 6d5f 6973         ``item_is
-00006170: 7375 6573 2e73 6576 6572 6974 792e 6167  sues.severity.ag
-00006180: 6772 6567 6174 6564 5f73 6576 6572 6974  gregated_severit
-00006190: 7960 6029 2063 616e 2062 6520 7573 6564  y``) can be used
-000061a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000061b0: 2066 696c 7465 7269 6e67 2074 6865 2072   filtering the r
-000061c0: 6573 756c 7473 2e2a 2a0a 2020 2020 2222  esults.**.    ""
-000061d0: 220a 0a20 2020 2063 6c61 7373 2041 6767  "..    class Agg
-000061e0: 7265 6761 7465 6452 6570 6f72 7469 6e67  regatedReporting
-000061f0: 436f 6e74 6578 7453 7461 7475 7328 7072  ContextStatus(pr
-00006200: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
-00006210: 2020 2072 2222 2253 7461 7475 7320 6f66     r"""Status of
-00006220: 2074 6865 2070 726f 6475 6374 2061 6767   the product agg
-00006230: 7265 6761 7465 6420 666f 7220 616c 6c20  regated for all 
-00006240: 7265 706f 7274 696e 6720 636f 6e74 6578  reporting contex
-00006250: 7473 2e0a 0a20 2020 2020 2020 2048 6572  ts...        Her
-00006260: 6527 7320 616e 2065 7861 6d70 6c65 206f  e's an example o
-00006270: 6620 686f 7720 7468 6520 6167 6772 6567  f how the aggreg
-00006280: 6174 6564 2073 7461 7475 7320 6973 2063  ated status is c
-00006290: 6f6d 7075 7465 643a 0a0a 2020 2020 2020  omputed:..      
-000062a0: 2020 6060 600a 2020 2020 2020 2020 4672    ```.        Fr
-000062b0: 6565 206c 6973 7469 6e67 7320 5c7c 2053  ee listings \| S
-000062c0: 686f 7070 696e 6720 4164 7320 5c7c 2053  hopping Ads \| S
-000062d0: 7461 7475 730a 2020 2020 2020 2020 2d2d  tatus.        --
-000062e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
-000062f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00006300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006310: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00006320: 2020 2041 7070 726f 7665 6420 5c7c 2041     Approved \| A
-00006330: 7070 726f 7665 6420 5c7c 2045 4c49 4749  pproved \| ELIGI
-00006340: 424c 4520 4170 7072 6f76 6564 205c 7c20  BLE Approved \| 
-00006350: 5065 6e64 696e 6720 5c7c 2045 4c49 4749  Pending \| ELIGI
-00006360: 424c 450a 2020 2020 2020 2020 4170 7072  BLE.        Appr
-00006370: 6f76 6564 205c 7c20 4469 7361 7070 726f  oved \| Disappro
-00006380: 7665 6420 5c7c 2045 4c49 4749 424c 455f  ved \| ELIGIBLE_
-00006390: 4c49 4d49 5445 4420 5065 6e64 696e 6720  LIMITED Pending 
-000063a0: 5c7c 2050 656e 6469 6e67 205c 7c0a 2020  \| Pending \|.  
-000063b0: 2020 2020 2020 5045 4e44 494e 4720 4469        PENDING Di
-000063c0: 7361 7070 726f 7665 6420 5c7c 2044 6973  sapproved \| Dis
-000063d0: 6170 7072 6f76 6564 205c 7c20 4e4f 545f  approved \| NOT_
-000063e0: 454c 4947 4942 4c45 5f4f 525f 4449 5341  ELIGIBLE_OR_DISA
-000063f0: 5050 524f 5645 440a 2020 2020 2020 2020  PPROVED.        
-00006400: 6060 600a 0a20 2020 2020 2020 2056 616c  ```..        Val
-00006410: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
-00006420: 2041 4747 5245 4741 5445 445f 5245 504f   AGGREGATED_REPO
-00006430: 5254 494e 475f 434f 4e54 4558 545f 5354  RTING_CONTEXT_ST
-00006440: 4154 5553 5f55 4e53 5045 4349 4649 4544  ATUS_UNSPECIFIED
-00006450: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
-00006460: 2020 2020 2020 4e6f 7420 7370 6563 6966        Not specif
-00006470: 6965 642e 0a20 2020 2020 2020 2020 2020  ied..           
-00006480: 204e 4f54 5f45 4c49 4749 424c 455f 4f52   NOT_ELIGIBLE_OR
-00006490: 5f44 4953 4150 5052 4f56 4544 2028 3129  _DISAPPROVED (1)
-000064a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000064b0: 2020 5072 6f64 7563 7420 6973 206e 6f74    Product is not
-000064c0: 2065 6c69 6769 626c 6520 6f72 2069 7320   eligible or is 
-000064d0: 6469 7361 7070 726f 7665 6420 666f 720a  disapproved for.
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 616c 6c20 7265 706f 7274 696e 6720 636f  all reporting co
-00006500: 6e74 6578 7473 2e0a 2020 2020 2020 2020  ntexts..        
-00006510: 2020 2020 5045 4e44 494e 4720 2832 293a      PENDING (2):
-00006520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006530: 2050 726f 6475 6374 2773 2073 7461 7475   Product's statu
-00006540: 7320 6973 2070 656e 6469 6e67 2069 6e20  s is pending in 
-00006550: 616c 6c20 7265 706f 7274 696e 670a 2020  all reporting.  
-00006560: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006570: 6e74 6578 7473 2e0a 2020 2020 2020 2020  ntexts..        
-00006580: 2020 2020 454c 4947 4942 4c45 5f4c 494d      ELIGIBLE_LIM
-00006590: 4954 4544 2028 3329 3a0a 2020 2020 2020  ITED (3):.      
-000065a0: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
-000065b0: 7420 6973 2065 6c69 6769 626c 6520 666f  t is eligible fo
-000065c0: 7220 736f 6d65 2028 6275 7420 6e6f 7420  r some (but not 
-000065d0: 616c 6c29 0a20 2020 2020 2020 2020 2020  all).           
-000065e0: 2020 2020 2072 6570 6f72 7469 6e67 2063       reporting c
-000065f0: 6f6e 7465 7874 732e 0a20 2020 2020 2020  ontexts..       
-00006600: 2020 2020 2045 4c49 4749 424c 4520 2834       ELIGIBLE (4
-00006610: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006620: 2020 2050 726f 6475 6374 2069 7320 656c     Product is el
-00006630: 6967 6962 6c65 2066 6f72 2061 6c6c 2072  igible for all r
-00006640: 6570 6f72 7469 6e67 0a20 2020 2020 2020  eporting.       
-00006650: 2020 2020 2020 2020 2063 6f6e 7465 7874           context
-00006660: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00006670: 2020 2020 2020 2041 4747 5245 4741 5445         AGGREGATE
-00006680: 445f 5245 504f 5254 494e 475f 434f 4e54  D_REPORTING_CONT
-00006690: 4558 545f 5354 4154 5553 5f55 4e53 5045  EXT_STATUS_UNSPE
-000066a0: 4349 4649 4544 203d 2030 0a20 2020 2020  CIFIED = 0.     
-000066b0: 2020 204e 4f54 5f45 4c49 4749 424c 455f     NOT_ELIGIBLE_
-000066c0: 4f52 5f44 4953 4150 5052 4f56 4544 203d  OR_DISAPPROVED =
-000066d0: 2031 0a20 2020 2020 2020 2050 454e 4449   1.        PENDI
-000066e0: 4e47 203d 2032 0a20 2020 2020 2020 2045  NG = 2.        E
-000066f0: 4c49 4749 424c 455f 4c49 4d49 5445 4420  LIGIBLE_LIMITED 
-00006700: 3d20 330a 2020 2020 2020 2020 454c 4947  = 3.        ELIG
-00006710: 4942 4c45 203d 2034 0a0a 2020 2020 636c  IBLE = 4..    cl
-00006720: 6173 7320 4974 656d 4973 7375 6528 7072  ass ItemIssue(pr
-00006730: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-00006740: 2020 2020 2020 7222 2222 4974 656d 2069        r"""Item i
-00006750: 7373 7565 2061 7373 6f63 6961 7465 6420  ssue associated 
-00006760: 7769 7468 2074 6865 2070 726f 6475 6374  with the product
-00006770: 2e0a 0a20 2020 2020 2020 202e 2e20 5f6f  ...        .. _o
-00006780: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
-00006790: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
-000067a0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000067b0: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
-000067c0: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
-000067d0: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
-000067e0: 6965 6c64 730a 0a20 2020 2020 2020 2041  ields..        A
-000067f0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-00006800: 2020 2020 2020 2074 7970 655f 2028 676f         type_ (go
-00006810: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
-00006820: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
-00006830: 3162 6574 612e 7479 7065 732e 5072 6f64  1beta.types.Prod
-00006840: 7563 7456 6965 772e 4974 656d 4973 7375  uctView.ItemIssu
-00006850: 652e 4974 656d 4973 7375 6554 7970 6529  e.ItemIssueType)
-00006860: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006870: 2020 4974 656d 2069 7373 7565 2074 7970    Item issue typ
-00006880: 652e 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00006890: 6576 6572 6974 7920 2867 6f6f 676c 652e  everity (google.
-000068a0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-000068b0: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-000068c0: 2e74 7970 6573 2e50 726f 6475 6374 5669  .types.ProductVi
-000068d0: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-000068e0: 6d49 7373 7565 5365 7665 7269 7479 293a  mIssueSeverity):
-000068f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006900: 2049 7465 6d20 6973 7375 6520 7365 7665   Item issue seve
-00006910: 7269 7479 2e0a 2020 2020 2020 2020 2020  rity..          
-00006920: 2020 7265 736f 6c75 7469 6f6e 2028 676f    resolution (go
-00006930: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
-00006940: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
-00006950: 3162 6574 612e 7479 7065 732e 5072 6f64  1beta.types.Prod
-00006960: 7563 7456 6965 772e 4974 656d 4973 7375  uctView.ItemIssu
-00006970: 652e 4974 656d 4973 7375 6552 6573 6f6c  e.ItemIssueResol
-00006980: 7574 696f 6e29 3a0a 2020 2020 2020 2020  ution):.        
-00006990: 2020 2020 2020 2020 4974 656d 2069 7373          Item iss
-000069a0: 7565 2072 6573 6f6c 7574 696f 6e2e 0a0a  ue resolution...
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000069d0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-000069e0: 605f 2060 605f 7265 736f 6c75 7469 6f6e  `_ ``_resolution
-000069f0: 6060 2e0a 2020 2020 2020 2020 2222 220a  ``..        """.
-00006a00: 0a20 2020 2020 2020 2063 6c61 7373 2049  .        class I
-00006a10: 7465 6d49 7373 7565 5265 736f 6c75 7469  temIssueResoluti
-00006a20: 6f6e 2870 726f 746f 2e45 6e75 6d29 3a0a  on(proto.Enum):.
-00006a30: 2020 2020 2020 2020 2020 2020 7222 2222              r"""
-00006a40: 486f 7720 746f 2072 6573 6f6c 7665 2074  How to resolve t
-00006a50: 6865 2069 7373 7565 2e0a 0a20 2020 2020  he issue...     
-00006a60: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00006a80: 5445 4d5f 4953 5355 455f 5245 534f 4c55  TEM_ISSUE_RESOLU
-00006a90: 5449 4f4e 5f55 4e53 5045 4349 4649 4544  TION_UNSPECIFIED
-00006aa0: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
-00006ab0: 2020 2020 2020 2020 2020 4e6f 7420 7370            Not sp
-00006ac0: 6563 6966 6965 642e 0a20 2020 2020 2020  ecified..       
-00006ad0: 2020 2020 2020 2020 204d 4552 4348 414e           MERCHAN
-00006ae0: 545f 4143 5449 4f4e 2028 3129 3a0a 2020  T_ACTION (1):.  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 5468 6520 6d65 7263 6861 6e74 2068    The merchant h
-00006b10: 6173 2074 6f20 6669 7820 7468 6520 6973  as to fix the is
-00006b20: 7375 652e 0a20 2020 2020 2020 2020 2020  sue..           
-00006b30: 2020 2020 2050 454e 4449 4e47 5f50 524f       PENDING_PRO
-00006b40: 4345 5353 494e 4720 2832 293a 0a20 2020  CESSING (2):.   
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2054 6865 2069 7373 7565 2077 696c 6c20   The issue will 
-00006b70: 6265 2072 6573 6f6c 7665 6420 6175 746f  be resolved auto
-00006b80: 6d61 7469 6361 6c6c 7920 2866 6f72 0a20  matically (for. 
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2065 7861 6d70 6c65 2c20 696d 6167     example, imag
-00006bb0: 6520 6372 6177 6c29 206f 7220 7468 726f  e crawl) or thro
-00006bc0: 7567 6820 6120 476f 6f67 6c65 0a20 2020  ugh a Google.   
-00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006be0: 2072 6576 6965 772e 204e 6f20 6d65 7263   review. No merc
-00006bf0: 6861 6e74 2061 6374 696f 6e20 6973 2072  hant action is r
-00006c00: 6571 7569 7265 6420 6e6f 772e 0a20 2020  equired now..   
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2052 6573 6f6c 7574 696f 6e20 6d69 6768   Resolution migh
-00006c30: 7420 6c65 6164 2074 6f20 616e 6f74 6865  t lead to anothe
-00006c40: 7220 6973 7375 6520 2866 6f72 0a20 2020  r issue (for.   
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2065 7861 6d70 6c65 2c20 6966 2063 7261   example, if cra
-00006c70: 776c 2066 6169 6c73 292e 0a20 2020 2020  wl fails)..     
-00006c80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006c90: 2020 2020 2020 2049 5445 4d5f 4953 5355         ITEM_ISSU
-00006ca0: 455f 5245 534f 4c55 5449 4f4e 5f55 4e53  E_RESOLUTION_UNS
-00006cb0: 5045 4349 4649 4544 203d 2030 0a20 2020  PECIFIED = 0.   
-00006cc0: 2020 2020 2020 2020 204d 4552 4348 414e           MERCHAN
-00006cd0: 545f 4143 5449 4f4e 203d 2031 0a20 2020  T_ACTION = 1.   
-00006ce0: 2020 2020 2020 2020 2050 454e 4449 4e47           PENDING
-00006cf0: 5f50 524f 4345 5353 494e 4720 3d20 320a  _PROCESSING = 2.
-00006d00: 0a20 2020 2020 2020 2063 6c61 7373 2049  .        class I
-00006d10: 7465 6d49 7373 7565 5479 7065 2870 726f  temIssueType(pro
-00006d20: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-00006d30: 2020 2020 2020 2020 2072 2222 2249 7373           r"""Iss
-00006d40: 7565 2074 7970 652e 0a0a 2020 2020 2020  ue type...      
-00006d50: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
-00006d60: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
-00006d70: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
-00006d80: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00006d90: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
-00006da0: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
-00006db0: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
-00006dc0: 0a0a 2020 2020 2020 2020 2020 2020 4174  ..            At
-00006dd0: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00006de0: 2020 2020 2020 2020 2020 636f 6465 2028            code (
-00006df0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00006e00: 2020 2020 2020 2020 2020 4572 726f 7220            Error 
-00006e10: 636f 6465 206f 6620 7468 6520 6973 7375  code of the issu
-00006e20: 652c 2065 7175 6976 616c 656e 7420 746f  e, equivalent to
-00006e30: 2074 6865 2060 6063 6f64 6560 6020 6f66   the ``code`` of
-00006e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e50: 2020 2020 2060 5072 6f64 7563 740a 2020       `Product.  
-00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e70: 2020 6973 7375 6573 203c 6874 7470 733a    issues <https:
-00006e80: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00006e90: 676c 652e 636f 6d2f 7368 6f70 7069 6e67  gle.com/shopping
-00006ea0: 2d63 6f6e 7465 6e74 2f67 7569 6465 732f  -content/guides/
-00006eb0: 7072 6f64 7563 742d 6973 7375 6573 3e60  product-issues>`
-00006ec0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-00006ed0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00006ee0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00006ef0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f63  of `oneof`_ ``_c
-00006f00: 6f64 6560 602e 0a20 2020 2020 2020 2020  ode``..         
-00006f10: 2020 2020 2020 2063 616e 6f6e 6963 616c         canonical
-00006f20: 5f61 7474 7269 6275 7465 2028 7374 7229  _attribute (str)
-00006f30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006f40: 2020 2020 2020 4361 6e6f 6e69 6361 6c20        Canonical 
-00006f50: 6174 7472 6962 7574 6520 6e61 6d65 2066  attribute name f
-00006f60: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00006f70: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
-00006f80: 2d73 7065 6369 6669 6320 6973 7375 6573  -specific issues
-00006f90: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00006fa0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00006fb0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00006fc0: 2060 6f6e 656f 6660 5f20 6060 5f63 616e   `oneof`_ ``_can
-00006fd0: 6f6e 6963 616c 5f61 7474 7269 6275 7465  onical_attribute
-00006fe0: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
-00006ff0: 2222 220a 0a20 2020 2020 2020 2020 2020  """..           
-00007000: 2063 6f64 653a 2073 7472 203d 2070 726f   code: str = pro
-00007010: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00007020: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-00007030: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00007040: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-00007050: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007060: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00007070: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00007080: 2020 2020 2020 2020 2020 2063 616e 6f6e             canon
-00007090: 6963 616c 5f61 7474 7269 6275 7465 3a20  ical_attribute: 
-000070a0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-000070b0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-000070c0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-000070d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070e0: 206e 756d 6265 723d 322c 0a20 2020 2020   number=2,.     
-000070f0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00007100: 6e61 6c3d 5472 7565 2c0a 2020 2020 2020  nal=True,.      
-00007110: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00007120: 2063 6c61 7373 2049 7465 6d49 7373 7565   class ItemIssue
-00007130: 5365 7665 7269 7479 2870 726f 746f 2e4d  Severity(proto.M
-00007140: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-00007150: 2020 2020 2072 2222 2248 6f77 2074 6865       r"""How the
-00007160: 2069 7373 7565 2061 6666 6563 7473 2074   issue affects t
-00007170: 6865 2073 6572 7669 6e67 206f 6620 7468  he serving of th
-00007180: 6520 7072 6f64 7563 742e 0a0a 2020 2020  e product...    
-00007190: 2020 2020 2020 2020 2e2e 205f 6f6e 656f          .. _oneo
-000071a0: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
-000071b0: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
-000071c0: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-000071d0: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
-000071e0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
-000071f0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
-00007200: 6473 0a0a 2020 2020 2020 2020 2020 2020  ds..            
-00007210: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00007220: 2020 2020 2020 2020 2020 2020 7365 7665              seve
-00007230: 7269 7479 5f70 6572 5f72 6570 6f72 7469  rity_per_reporti
-00007240: 6e67 5f63 6f6e 7465 7874 2028 4d75 7461  ng_context (Muta
-00007250: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
-00007260: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
-00007270: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
-00007280: 6574 612e 7479 7065 732e 5072 6f64 7563  eta.types.Produc
-00007290: 7456 6965 772e 4974 656d 4973 7375 652e  tView.ItemIssue.
-000072a0: 4974 656d 4973 7375 6553 6576 6572 6974  ItemIssueSeverit
-000072b0: 792e 4973 7375 6553 6576 6572 6974 7950  y.IssueSeverityP
-000072c0: 6572 5265 706f 7274 696e 6743 6f6e 7465  erReportingConte
-000072d0: 7874 5d29 3a0a 2020 2020 2020 2020 2020  xt]):.          
-000072e0: 2020 2020 2020 2020 2020 4973 7375 6520            Issue 
-000072f0: 7365 7665 7269 7479 2070 6572 2072 6570  severity per rep
-00007300: 6f72 7469 6e67 2063 6f6e 7465 7874 2e0a  orting context..
-00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007320: 6167 6772 6567 6174 6564 5f73 6576 6572  aggregated_sever
-00007330: 6974 7920 2867 6f6f 676c 652e 7368 6f70  ity (google.shop
-00007340: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
-00007350: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
-00007360: 6573 2e50 726f 6475 6374 5669 6577 2e49  es.ProductView.I
-00007370: 7465 6d49 7373 7565 2e49 7465 6d49 7373  temIssue.ItemIss
-00007380: 7565 5365 7665 7269 7479 2e41 6767 7265  ueSeverity.Aggre
-00007390: 6761 7465 6449 7373 7565 5365 7665 7269  gatedIssueSeveri
-000073a0: 7479 293a 0a20 2020 2020 2020 2020 2020  ty):.           
-000073b0: 2020 2020 2020 2020 2041 6767 7265 6761           Aggrega
-000073c0: 7465 6420 7365 7665 7269 7479 206f 6620  ted severity of 
-000073d0: 7468 6520 6973 7375 6520 666f 7220 616c  the issue for al
-000073e0: 6c20 7265 706f 7274 696e 6720 636f 6e74  l reporting cont
-000073f0: 6578 7473 0a20 2020 2020 2020 2020 2020  exts.           
-00007400: 2020 2020 2020 2020 2069 7420 6166 6665           it affe
-00007410: 6374 732e 0a0a 2020 2020 2020 2020 2020  cts...          
-00007420: 2020 2020 2020 2020 2020 2a2a 5468 6973            **This
-00007430: 2066 6965 6c64 2063 616e 2062 6520 7573   field can be us
-00007440: 6564 2066 6f72 2066 696c 7465 7269 6e67  ed for filtering
-00007450: 2074 6865 2072 6573 756c 7473 2e2a 2a0a   the results.**.
-00007460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007470: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00007480: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00007490: 6f6e 656f 6660 5f20 6060 5f61 6767 7265  oneof`_ ``_aggre
-000074a0: 6761 7465 645f 7365 7665 7269 7479 6060  gated_severity``
-000074b0: 2e0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
-000074c0: 220a 0a20 2020 2020 2020 2020 2020 2063  "..            c
-000074d0: 6c61 7373 2041 6767 7265 6761 7465 6449  lass AggregatedI
-000074e0: 7373 7565 5365 7665 7269 7479 2870 726f  ssueSeverity(pro
-000074f0: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
-00007500: 2020 2020 2020 2020 2020 7222 2222 4973            r"""Is
-00007510: 7375 6520 7365 7665 7269 7479 2061 6767  sue severity agg
-00007520: 7265 6761 7465 6420 666f 7220 616c 6c20  regated for all 
-00007530: 7265 706f 7274 696e 6720 636f 6e74 6578  reporting contex
-00007540: 7473 2e0a 0a20 2020 2020 2020 2020 2020  ts...           
-00007550: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
-00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2041 4747 5245 4741 5445 445f 4953 5355   AGGREGATED_ISSU
-00007580: 455f 5345 5645 5249 5459 5f55 4e53 5045  E_SEVERITY_UNSPE
-00007590: 4349 4649 4544 2028 3029 3a0a 2020 2020  CIFIED (0):.    
-000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075b0: 2020 2020 4e6f 7420 7370 6563 6966 6965      Not specifie
-000075c0: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-000075d0: 2020 2020 2020 2044 4953 4150 5052 4f56         DISAPPROV
-000075e0: 4544 2028 3129 3a0a 2020 2020 2020 2020  ED (1):.        
+000008d0: 4465 6661 756c 7473 2074 6f20 3130 3030  Defaults to 1000
+000008e0: 2e20 5661 6c75 6573 2061 626f 7665 2035  . Values above 5
+000008f0: 3030 3020 6172 6520 636f 6572 6365 6420  000 are coerced 
+00000900: 746f 0a20 2020 2020 2020 2020 2020 2035  to.            5
+00000910: 3030 302e 0a20 2020 2020 2020 2070 6167  000..        pag
+00000920: 655f 746f 6b65 6e20 2873 7472 293a 0a20  e_token (str):. 
+00000930: 2020 2020 2020 2020 2020 204f 7074 696f             Optio
+00000940: 6e61 6c2e 2054 6f6b 656e 206f 6620 7468  nal. Token of th
+00000950: 6520 7061 6765 2074 6f20 7265 7472 6965  e page to retrie
+00000960: 7665 2e20 4966 206e 6f74 2073 7065 6369  ve. If not speci
+00000970: 6669 6564 2c0a 2020 2020 2020 2020 2020  fied,.          
+00000980: 2020 7468 6520 6669 7273 7420 7061 6765    the first page
+00000990: 206f 6620 7265 7375 6c74 7320 6973 2072   of results is r
+000009a0: 6574 7572 6e65 642e 2049 6e20 6f72 6465  eturned. In orde
+000009b0: 7220 746f 2072 6571 7565 7374 0a20 2020  r to request.   
+000009c0: 2020 2020 2020 2020 2074 6865 206e 6578           the nex
+000009d0: 7420 7061 6765 206f 6620 7265 7375 6c74  t page of result
+000009e0: 732c 2074 6865 2076 616c 7565 206f 6274  s, the value obt
+000009f0: 6169 6e65 6420 6672 6f6d 0a20 2020 2020  ained from.     
+00000a00: 2020 2020 2020 2060 606e 6578 745f 7061         ``next_pa
+00000a10: 6765 5f74 6f6b 656e 6060 2069 6e20 7468  ge_token`` in th
+00000a20: 6520 7072 6576 696f 7573 2072 6573 706f  e previous respo
+00000a30: 6e73 6520 7368 6f75 6c64 2062 6520 7573  nse should be us
+00000a40: 6564 2e0a 2020 2020 2222 220a 0a20 2020  ed..    """..   
+00000a50: 2070 6172 656e 743a 2073 7472 203d 2070   parent: str = p
+00000a60: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00000a70: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00000a80: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00000a90: 3d31 2c0a 2020 2020 290a 2020 2020 7175  =1,.    ).    qu
+00000aa0: 6572 793a 2073 7472 203d 2070 726f 746f  ery: str = proto
+00000ab0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00000ac0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+00000ad0: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
+00000ae0: 2020 2020 290a 2020 2020 7061 6765 5f73      ).    page_s
+00000af0: 697a 653a 2069 6e74 203d 2070 726f 746f  ize: int = proto
+00000b00: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00000b10: 7072 6f74 6f2e 494e 5433 322c 0a20 2020  proto.INT32,.   
+00000b20: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
+00000b30: 2020 2029 0a20 2020 2070 6167 655f 746f     ).    page_to
+00000b40: 6b65 6e3a 2073 7472 203d 2070 726f 746f  ken: str = proto
+00000b50: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00000b60: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+00000b70: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
+00000b80: 2020 2020 290a 0a0a 636c 6173 7320 5365      )...class Se
+00000b90: 6172 6368 5265 7370 6f6e 7365 2870 726f  archResponse(pro
+00000ba0: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
+00000bb0: 2072 2222 2252 6573 706f 6e73 6520 6d65   r"""Response me
+00000bc0: 7373 6167 6520 666f 7220 7468 6520 6060  ssage for the ``
+00000bd0: 5265 706f 7274 5365 7276 6963 652e 5365  ReportService.Se
+00000be0: 6172 6368 6060 206d 6574 686f 642e 0a0a  arch`` method...
+00000bf0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+00000c00: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
+00000c10: 284d 7574 6162 6c65 5365 7175 656e 6365  (MutableSequence
+00000c20: 5b67 6f6f 676c 652e 7368 6f70 7069 6e67  [google.shopping
+00000c30: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
+00000c40: 735f 7631 6265 7461 2e74 7970 6573 2e52  s_v1beta.types.R
+00000c50: 6570 6f72 7452 6f77 5d29 3a0a 2020 2020  eportRow]):.    
+00000c60: 2020 2020 2020 2020 526f 7773 2074 6861          Rows tha
+00000c70: 7420 6d61 7463 6865 6420 7468 6520 7365  t matched the se
+00000c80: 6172 6368 2071 7565 7279 2e0a 2020 2020  arch query..    
+00000c90: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
+00000ca0: 6b65 6e20 2873 7472 293a 0a20 2020 2020  ken (str):.     
+00000cb0: 2020 2020 2020 2054 6f6b 656e 2077 6869         Token whi
+00000cc0: 6368 2063 616e 2062 6520 7365 6e74 2061  ch can be sent a
+00000cd0: 7320 6060 7061 6765 5f74 6f6b 656e 6060  s ``page_token``
+00000ce0: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
+00000cf0: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
+00000d00: 7420 7061 6765 2e20 4966 206f 6d69 7474  t page. If omitt
+00000d10: 6564 2c20 7468 6572 6520 6172 6520 6e6f  ed, there are no
+00000d20: 2073 7562 7365 7175 656e 7420 7061 6765   subsequent page
+00000d30: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
+00000d40: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00000d50: 6620 7261 775f 7061 6765 2873 656c 6629  f raw_page(self)
+00000d60: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00000d70: 2073 656c 660a 0a20 2020 2072 6573 756c   self..    resul
+00000d80: 7473 3a20 4d75 7461 626c 6553 6571 7565  ts: MutableSeque
+00000d90: 6e63 655b 2252 6570 6f72 7452 6f77 225d  nce["ReportRow"]
+00000da0: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+00000db0: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+00000dc0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00000dd0: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
+00000de0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00000df0: 3d22 5265 706f 7274 526f 7722 2c0a 2020  ="ReportRow",.  
+00000e00: 2020 290a 2020 2020 6e65 7874 5f70 6167    ).    next_pag
+00000e10: 655f 746f 6b65 6e3a 2073 7472 203d 2070  e_token: str = p
+00000e20: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00000e30: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00000e40: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00000e50: 3d32 2c0a 2020 2020 290a 0a0a 636c 6173  =2,.    )...clas
+00000e60: 7320 5265 706f 7274 526f 7728 7072 6f74  s ReportRow(prot
+00000e70: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
+00000e80: 7222 2222 5265 7375 6c74 2072 6f77 2072  r"""Result row r
+00000e90: 6574 7572 6e65 6420 6672 6f6d 2074 6865  eturned from the
+00000ea0: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
+00000eb0: 2020 2020 4f6e 6c79 2074 6865 206d 6573      Only the mes
+00000ec0: 7361 6765 2063 6f72 7265 7370 6f6e 6469  sage correspondi
+00000ed0: 6e67 2074 6f20 7468 6520 7175 6572 6965  ng to the querie
+00000ee0: 6420 7461 626c 6520 6973 2070 6f70 756c  d table is popul
+00000ef0: 6174 6564 0a20 2020 2069 6e20 7468 6520  ated.    in the 
+00000f00: 7265 7370 6f6e 7365 2e20 5769 7468 696e  response. Within
+00000f10: 2074 6865 2070 6f70 756c 6174 6564 206d   the populated m
+00000f20: 6573 7361 6765 2c20 6f6e 6c79 2074 6865  essage, only the
+00000f30: 2066 6965 6c64 730a 2020 2020 7265 7175   fields.    requ
+00000f40: 6573 7465 6420 6578 706c 6963 6974 6c79  ested explicitly
+00000f50: 2069 6e20 7468 6520 7175 6572 7920 6172   in the query ar
+00000f60: 6520 706f 7075 6c61 7465 642e 0a0a 2020  e populated...  
+00000f70: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
+00000f80: 2020 2020 2020 7072 6f64 7563 745f 7065        product_pe
+00000f90: 7266 6f72 6d61 6e63 655f 7669 6577 2028  rformance_view (
+00000fa0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+00000fb0: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
+00000fc0: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
+00000fd0: 6f64 7563 7450 6572 666f 726d 616e 6365  oductPerformance
+00000fe0: 5669 6577 293a 0a20 2020 2020 2020 2020  View):.         
+00000ff0: 2020 2046 6965 6c64 7320 6176 6169 6c61     Fields availa
+00001000: 626c 6520 666f 7220 7175 6572 7920 696e  ble for query in
+00001010: 2060 6070 726f 6475 6374 5f70 6572 666f   ``product_perfo
+00001020: 726d 616e 6365 5f76 6965 7760 600a 2020  rmance_view``.  
+00001030: 2020 2020 2020 2020 2020 7461 626c 652e            table.
+00001040: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+00001050: 5f76 6965 7720 2867 6f6f 676c 652e 7368  _view (google.sh
+00001060: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+00001070: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+00001080: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
+00001090: 293a 0a20 2020 2020 2020 2020 2020 2046  ):.            F
+000010a0: 6965 6c64 7320 6176 6169 6c61 626c 6520  ields available 
+000010b0: 666f 7220 7175 6572 7920 696e 2060 6070  for query in ``p
+000010c0: 726f 6475 6374 5f76 6965 7760 6020 7461  roduct_view`` ta
+000010d0: 626c 652e 0a20 2020 2020 2020 2070 7269  ble..        pri
+000010e0: 6365 5f63 6f6d 7065 7469 7469 7665 6e65  ce_competitivene
+000010f0: 7373 5f70 726f 6475 6374 5f76 6965 7720  ss_product_view 
+00001100: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
+00001110: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
+00001120: 735f 7631 6265 7461 2e74 7970 6573 2e50  s_v1beta.types.P
+00001130: 7269 6365 436f 6d70 6574 6974 6976 656e  riceCompetitiven
+00001140: 6573 7350 726f 6475 6374 5669 6577 293a  essProductView):
+00001150: 0a20 2020 2020 2020 2020 2020 2046 6965  .            Fie
+00001160: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
+00001170: 7220 7175 6572 7920 696e 0a20 2020 2020  r query in.     
+00001180: 2020 2020 2020 2060 6070 7269 6365 5f63         ``price_c
+00001190: 6f6d 7065 7469 7469 7665 6e65 7373 5f70  ompetitiveness_p
+000011a0: 726f 6475 6374 5f76 6965 7760 6020 7461  roduct_view`` ta
+000011b0: 626c 652e 0a20 2020 2020 2020 2070 7269  ble..        pri
+000011c0: 6365 5f69 6e73 6967 6874 735f 7072 6f64  ce_insights_prod
+000011d0: 7563 745f 7669 6577 2028 676f 6f67 6c65  uct_view (google
+000011e0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
+000011f0: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
+00001200: 612e 7479 7065 732e 5072 6963 6549 6e73  a.types.PriceIns
+00001210: 6967 6874 7350 726f 6475 6374 5669 6577  ightsProductView
+00001220: 293a 0a20 2020 2020 2020 2020 2020 2046  ):.            F
+00001230: 6965 6c64 7320 6176 6169 6c61 626c 6520  ields available 
+00001240: 666f 7220 7175 6572 7920 696e 0a20 2020  for query in.   
+00001250: 2020 2020 2020 2020 2060 6070 7269 6365           ``price
+00001260: 5f69 6e73 6967 6874 735f 7072 6f64 7563  _insights_produc
+00001270: 745f 7669 6577 6060 2074 6162 6c65 2e0a  t_view`` table..
+00001280: 2020 2020 2020 2020 6265 7374 5f73 656c          best_sel
+00001290: 6c65 7273 5f70 726f 6475 6374 5f63 6c75  lers_product_clu
+000012a0: 7374 6572 5f76 6965 7720 2867 6f6f 676c  ster_view (googl
+000012b0: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
+000012c0: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
+000012d0: 7461 2e74 7970 6573 2e42 6573 7453 656c  ta.types.BestSel
+000012e0: 6c65 7273 5072 6f64 7563 7443 6c75 7374  lersProductClust
+000012f0: 6572 5669 6577 293a 0a20 2020 2020 2020  erView):.       
+00001300: 2020 2020 2046 6965 6c64 7320 6176 6169       Fields avai
+00001310: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
+00001320: 696e 0a20 2020 2020 2020 2020 2020 2060  in.            `
+00001330: 6062 6573 745f 7365 6c6c 6572 735f 7072  `best_sellers_pr
+00001340: 6f64 7563 745f 636c 7573 7465 725f 7669  oduct_cluster_vi
+00001350: 6577 6060 2074 6162 6c65 2e0a 2020 2020  ew`` table..    
+00001360: 2020 2020 6265 7374 5f73 656c 6c65 7273      best_sellers
+00001370: 5f62 7261 6e64 5f76 6965 7720 2867 6f6f  _brand_view (goo
+00001380: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
+00001390: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
+000013a0: 6265 7461 2e74 7970 6573 2e42 6573 7453  beta.types.BestS
+000013b0: 656c 6c65 7273 4272 616e 6456 6965 7729  ellersBrandView)
+000013c0: 3a0a 2020 2020 2020 2020 2020 2020 4669  :.            Fi
+000013d0: 656c 6473 2061 7661 696c 6162 6c65 2066  elds available f
+000013e0: 6f72 2071 7565 7279 2069 6e20 6060 6265  or query in ``be
+000013f0: 7374 5f73 656c 6c65 7273 5f62 7261 6e64  st_sellers_brand
+00001400: 5f76 6965 7760 600a 2020 2020 2020 2020  _view``.        
+00001410: 2020 2020 7461 626c 652e 0a20 2020 2020      table..     
+00001420: 2020 2063 6f6d 7065 7469 7469 7665 5f76     competitive_v
+00001430: 6973 6962 696c 6974 795f 636f 6d70 6574  isibility_compet
+00001440: 6974 6f72 5f76 6965 7720 2867 6f6f 676c  itor_view (googl
+00001450: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
+00001460: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
+00001470: 7461 2e74 7970 6573 2e43 6f6d 7065 7469  ta.types.Competi
+00001480: 7469 7665 5669 7369 6269 6c69 7479 436f  tiveVisibilityCo
+00001490: 6d70 6574 6974 6f72 5669 6577 293a 0a20  mpetitorView):. 
+000014a0: 2020 2020 2020 2020 2020 2046 6965 6c64             Field
+000014b0: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
+000014c0: 7175 6572 7920 696e 0a20 2020 2020 2020  query in.       
+000014d0: 2020 2020 2060 6063 6f6d 7065 7469 7469       ``competiti
+000014e0: 7665 5f76 6973 6962 696c 6974 795f 636f  ve_visibility_co
+000014f0: 6d70 6574 6974 6f72 5f76 6965 7760 6020  mpetitor_view`` 
+00001500: 7461 626c 652e 0a20 2020 2020 2020 2063  table..        c
+00001510: 6f6d 7065 7469 7469 7665 5f76 6973 6962  ompetitive_visib
+00001520: 696c 6974 795f 746f 705f 6d65 7263 6861  ility_top_mercha
+00001530: 6e74 5f76 6965 7720 2867 6f6f 676c 652e  nt_view (google.
+00001540: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
+00001550: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
+00001560: 2e74 7970 6573 2e43 6f6d 7065 7469 7469  .types.Competiti
+00001570: 7665 5669 7369 6269 6c69 7479 546f 704d  veVisibilityTopM
+00001580: 6572 6368 616e 7456 6965 7729 3a0a 2020  erchantView):.  
+00001590: 2020 2020 2020 2020 2020 4669 656c 6473            Fields
+000015a0: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
+000015b0: 7565 7279 2069 6e0a 2020 2020 2020 2020  uery in.        
+000015c0: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
+000015d0: 655f 7669 7369 6269 6c69 7479 5f74 6f70  e_visibility_top
+000015e0: 5f6d 6572 6368 616e 745f 7669 6577 6060  _merchant_view``
+000015f0: 2074 6162 6c65 2e0a 2020 2020 2020 2020   table..        
+00001600: 636f 6d70 6574 6974 6976 655f 7669 7369  competitive_visi
+00001610: 6269 6c69 7479 5f62 656e 6368 6d61 726b  bility_benchmark
+00001620: 5f76 6965 7720 2867 6f6f 676c 652e 7368  _view (google.sh
+00001630: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+00001640: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+00001650: 7970 6573 2e43 6f6d 7065 7469 7469 7665  ypes.Competitive
+00001660: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
+00001670: 6172 6b56 6965 7729 3a0a 2020 2020 2020  arkView):.      
+00001680: 2020 2020 2020 4669 656c 6473 2061 7661        Fields ava
+00001690: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
+000016a0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+000016b0: 6060 636f 6d70 6574 6974 6976 655f 7669  ``competitive_vi
+000016c0: 7369 6269 6c69 7479 5f62 656e 6368 6d61  sibility_benchma
+000016d0: 726b 5f76 6965 7760 6020 7461 626c 652e  rk_view`` table.
+000016e0: 0a20 2020 2022 2222 0a0a 2020 2020 7072  .    """..    pr
+000016f0: 6f64 7563 745f 7065 7266 6f72 6d61 6e63  oduct_performanc
+00001700: 655f 7669 6577 3a20 2250 726f 6475 6374  e_view: "Product
+00001710: 5065 7266 6f72 6d61 6e63 6556 6965 7722  PerformanceView"
+00001720: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00001730: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00001740: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00001750: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
+00001760: 206d 6573 7361 6765 3d22 5072 6f64 7563   message="Produc
+00001770: 7450 6572 666f 726d 616e 6365 5669 6577  tPerformanceView
+00001780: 222c 0a20 2020 2029 0a20 2020 2070 726f  ",.    ).    pro
+00001790: 6475 6374 5f76 6965 773a 2022 5072 6f64  duct_view: "Prod
+000017a0: 7563 7456 6965 7722 203d 2070 726f 746f  uctView" = proto
+000017b0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+000017c0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+000017d0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+000017e0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+000017f0: 3d22 5072 6f64 7563 7456 6965 7722 2c0a  ="ProductView",.
+00001800: 2020 2020 290a 2020 2020 7072 6963 655f      ).    price_
+00001810: 636f 6d70 6574 6974 6976 656e 6573 735f  competitiveness_
+00001820: 7072 6f64 7563 745f 7669 6577 3a20 2250  product_view: "P
+00001830: 7269 6365 436f 6d70 6574 6974 6976 656e  riceCompetitiven
+00001840: 6573 7350 726f 6475 6374 5669 6577 2220  essProductView" 
+00001850: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00001860: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00001870: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00001880: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+00001890: 6d65 7373 6167 653d 2250 7269 6365 436f  message="PriceCo
+000018a0: 6d70 6574 6974 6976 656e 6573 7350 726f  mpetitivenessPro
+000018b0: 6475 6374 5669 6577 222c 0a20 2020 2029  ductView",.    )
+000018c0: 0a20 2020 2070 7269 6365 5f69 6e73 6967  .    price_insig
+000018d0: 6874 735f 7072 6f64 7563 745f 7669 6577  hts_product_view
+000018e0: 3a20 2250 7269 6365 496e 7369 6768 7473  : "PriceInsights
+000018f0: 5072 6f64 7563 7456 6965 7722 203d 2070  ProductView" = p
+00001900: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00001910: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+00001920: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+00001930: 723d 342c 0a20 2020 2020 2020 206d 6573  r=4,.        mes
+00001940: 7361 6765 3d22 5072 6963 6549 6e73 6967  sage="PriceInsig
+00001950: 6874 7350 726f 6475 6374 5669 6577 222c  htsProductView",
+00001960: 0a20 2020 2029 0a20 2020 2062 6573 745f  .    ).    best_
+00001970: 7365 6c6c 6572 735f 7072 6f64 7563 745f  sellers_product_
+00001980: 636c 7573 7465 725f 7669 6577 3a20 2242  cluster_view: "B
+00001990: 6573 7453 656c 6c65 7273 5072 6f64 7563  estSellersProduc
+000019a0: 7443 6c75 7374 6572 5669 6577 2220 3d20  tClusterView" = 
+000019b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000019c0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+000019d0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+000019e0: 6572 3d35 2c0a 2020 2020 2020 2020 6d65  er=5,.        me
+000019f0: 7373 6167 653d 2242 6573 7453 656c 6c65  ssage="BestSelle
+00001a00: 7273 5072 6f64 7563 7443 6c75 7374 6572  rsProductCluster
+00001a10: 5669 6577 222c 0a20 2020 2029 0a20 2020  View",.    ).   
+00001a20: 2062 6573 745f 7365 6c6c 6572 735f 6272   best_sellers_br
+00001a30: 616e 645f 7669 6577 3a20 2242 6573 7453  and_view: "BestS
+00001a40: 656c 6c65 7273 4272 616e 6456 6965 7722  ellersBrandView"
+00001a50: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00001a60: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00001a70: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00001a80: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
+00001a90: 206d 6573 7361 6765 3d22 4265 7374 5365   message="BestSe
+00001aa0: 6c6c 6572 7342 7261 6e64 5669 6577 222c  llersBrandView",
+00001ab0: 0a20 2020 2029 0a20 2020 2063 6f6d 7065  .    ).    compe
+00001ac0: 7469 7469 7665 5f76 6973 6962 696c 6974  titive_visibilit
+00001ad0: 795f 636f 6d70 6574 6974 6f72 5f76 6965  y_competitor_vie
+00001ae0: 773a 2022 436f 6d70 6574 6974 6976 6556  w: "CompetitiveV
+00001af0: 6973 6962 696c 6974 7943 6f6d 7065 7469  isibilityCompeti
+00001b00: 746f 7256 6965 7722 203d 2028 0a20 2020  torView" = (.   
+00001b10: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
+00001b20: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00001b30: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+00001b40: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00001b50: 382c 0a20 2020 2020 2020 2020 2020 206d  8,.            m
+00001b60: 6573 7361 6765 3d22 436f 6d70 6574 6974  essage="Competit
+00001b70: 6976 6556 6973 6962 696c 6974 7943 6f6d  iveVisibilityCom
+00001b80: 7065 7469 746f 7256 6965 7722 2c0a 2020  petitorView",.  
+00001b90: 2020 2020 2020 290a 2020 2020 290a 2020        ).    ).  
+00001ba0: 2020 636f 6d70 6574 6974 6976 655f 7669    competitive_vi
+00001bb0: 7369 6269 6c69 7479 5f74 6f70 5f6d 6572  sibility_top_mer
+00001bc0: 6368 616e 745f 7669 6577 3a20 2243 6f6d  chant_view: "Com
+00001bd0: 7065 7469 7469 7665 5669 7369 6269 6c69  petitiveVisibili
+00001be0: 7479 546f 704d 6572 6368 616e 7456 6965  tyTopMerchantVie
+00001bf0: 7722 203d 2028 0a20 2020 2020 2020 2070  w" = (.        p
+00001c00: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00001c10: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00001c20: 5353 4147 452c 0a20 2020 2020 2020 2020  SSAGE,.         
+00001c30: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
+00001c40: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00001c50: 3d22 436f 6d70 6574 6974 6976 6556 6973  ="CompetitiveVis
+00001c60: 6962 696c 6974 7954 6f70 4d65 7263 6861  ibilityTopMercha
+00001c70: 6e74 5669 6577 222c 0a20 2020 2020 2020  ntView",.       
+00001c80: 2029 0a20 2020 2029 0a20 2020 2063 6f6d   ).    ).    com
+00001c90: 7065 7469 7469 7665 5f76 6973 6962 696c  petitive_visibil
+00001ca0: 6974 795f 6265 6e63 686d 6172 6b5f 7669  ity_benchmark_vi
+00001cb0: 6577 3a20 2243 6f6d 7065 7469 7469 7665  ew: "Competitive
+00001cc0: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
+00001cd0: 6172 6b56 6965 7722 203d 2028 0a20 2020  arkView" = (.   
+00001ce0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
+00001cf0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00001d00: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+00001d10: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00001d20: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
+00001d30: 6d65 7373 6167 653d 2243 6f6d 7065 7469  message="Competi
+00001d40: 7469 7665 5669 7369 6269 6c69 7479 4265  tiveVisibilityBe
+00001d50: 6e63 686d 6172 6b56 6965 7722 2c0a 2020  nchmarkView",.  
+00001d60: 2020 2020 2020 290a 2020 2020 290a 0a0a        ).    )...
+00001d70: 636c 6173 7320 5072 6f64 7563 7450 6572  class ProductPer
+00001d80: 666f 726d 616e 6365 5669 6577 2870 726f  formanceView(pro
+00001d90: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
+00001da0: 2072 2222 2246 6965 6c64 7320 6176 6169   r"""Fields avai
+00001db0: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
+00001dc0: 696e 2060 6070 726f 6475 6374 5f70 6572  in ``product_per
+00001dd0: 666f 726d 616e 6365 5f76 6965 7760 6020  formance_view`` 
+00001de0: 7461 626c 652e 0a0a 2020 2020 5072 6f64  table...    Prod
+00001df0: 7563 7420 7065 7266 6f72 6d61 6e63 6520  uct performance 
+00001e00: 6461 7461 2066 6f72 2079 6f75 7220 6163  data for your ac
+00001e10: 636f 756e 742c 2069 6e63 6c75 6469 6e67  count, including
+00001e20: 2070 6572 666f 726d 616e 6365 0a20 2020   performance.   
+00001e30: 206d 6574 7269 6373 2028 666f 7220 6578   metrics (for ex
+00001e40: 616d 706c 652c 2060 6063 6c69 636b 7360  ample, ``clicks`
+00001e50: 6029 2061 6e64 2064 696d 656e 7369 6f6e  `) and dimension
+00001e60: 7320 6163 636f 7264 696e 6720 746f 2077  s according to w
+00001e70: 6869 6368 0a20 2020 2070 6572 666f 726d  hich.    perform
+00001e80: 616e 6365 206d 6574 7269 6373 2061 7265  ance metrics are
+00001e90: 2073 6567 6d65 6e74 6564 2028 666f 7220   segmented (for 
+00001ea0: 6578 616d 706c 652c 2060 606f 6666 6572  example, ``offer
+00001eb0: 5f69 6460 6029 2e0a 2020 2020 5661 6c75  _id``)..    Valu
+00001ec0: 6573 206f 6620 7072 6f64 7563 7420 6469  es of product di
+00001ed0: 6d65 6e73 696f 6e73 2c20 7375 6368 2061  mensions, such a
+00001ee0: 7320 6060 6f66 6665 725f 6964 6060 2c20  s ``offer_id``, 
+00001ef0: 7265 666c 6563 7420 7468 650a 2020 2020  reflect the.    
+00001f00: 7374 6174 6520 6f66 2061 2070 726f 6475  state of a produ
+00001f10: 6374 2061 7420 7468 6520 7469 6d65 206f  ct at the time o
+00001f20: 6620 7468 6520 696d 7072 6573 7369 6f6e  f the impression
+00001f30: 2e0a 0a20 2020 2053 6567 6d65 6e74 2066  ...    Segment f
+00001f40: 6965 6c64 7320 6361 6e6e 6f74 2062 6520  ields cannot be 
+00001f50: 7365 6c65 6374 6564 2069 6e20 7175 6572  selected in quer
+00001f60: 6965 7320 7769 7468 6f75 7420 616c 736f  ies without also
+00001f70: 2073 656c 6563 7469 6e67 0a20 2020 2061   selecting.    a
+00001f80: 7420 6c65 6173 7420 6f6e 6520 6d65 7472  t least one metr
+00001f90: 6963 2066 6965 6c64 2e0a 0a20 2020 2056  ic field...    V
+00001fa0: 616c 7565 7320 6172 6520 6f6e 6c79 2073  alues are only s
+00001fb0: 6574 2066 6f72 2066 6965 6c64 7320 7265  et for fields re
+00001fc0: 7175 6573 7465 6420 6578 706c 6963 6974  quested explicit
+00001fd0: 6c79 2069 6e20 7468 6520 7265 7175 6573  ly in the reques
+00001fe0: 7427 730a 2020 2020 7365 6172 6368 2071  t's.    search q
+00001ff0: 7565 7279 2e0a 0a0a 2020 2020 2e2e 205f  uery....    .. _
+00002000: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
+00002010: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
+00002020: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002030: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
+00002040: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
+00002050: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
+00002060: 6669 656c 6473 0a0a 2020 2020 4174 7472  fields..    Attr
+00002070: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+00002080: 6d61 726b 6574 696e 675f 6d65 7468 6f64  marketing_method
+00002090: 2028 676f 6f67 6c65 2e73 686f 7070 696e   (google.shoppin
+000020a0: 672e 6d65 7263 6861 6e74 5f72 6570 6f72  g.merchant_repor
+000020b0: 7473 5f76 3162 6574 612e 7479 7065 732e  ts_v1beta.types.
+000020c0: 4d61 726b 6574 696e 674d 6574 686f 642e  MarketingMethod.
+000020d0: 4d61 726b 6574 696e 674d 6574 686f 6445  MarketingMethodE
+000020e0: 6e75 6d29 3a0a 2020 2020 2020 2020 2020  num):.          
+000020f0: 2020 4d61 726b 6574 696e 6720 6d65 7468    Marketing meth
+00002100: 6f64 2074 6f20 7768 6963 6820 6d65 7472  od to which metr
+00002110: 6963 7320 6170 706c 792e 0a20 2020 2020  ics apply..     
+00002120: 2020 2020 2020 2053 6567 6d65 6e74 2e0a         Segment..
+00002130: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00002140: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00002150: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00002160: 6060 5f6d 6172 6b65 7469 6e67 5f6d 6574  ``_marketing_met
+00002170: 686f 6460 602e 0a20 2020 2020 2020 2064  hod``..        d
+00002180: 6174 6520 2867 6f6f 676c 652e 7479 7065  ate (google.type
+00002190: 2e64 6174 655f 7062 322e 4461 7465 293a  .date_pb2.Date):
+000021a0: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
+000021b0: 6520 696e 2074 6865 206d 6572 6368 616e  e in the merchan
+000021c0: 7420 7469 6d65 7a6f 6e65 2074 6f20 7768  t timezone to wh
+000021d0: 6963 6820 6d65 7472 6963 7320 6170 706c  ich metrics appl
+000021e0: 792e 0a20 2020 2020 2020 2020 2020 2053  y..            S
+000021f0: 6567 6d65 6e74 2e0a 0a20 2020 2020 2020  egment...       
+00002200: 2020 2020 2043 6f6e 6469 7469 6f6e 206f       Condition o
+00002210: 6e20 6060 6461 7465 6060 2069 7320 7265  n ``date`` is re
+00002220: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+00002230: 5748 4552 4560 6020 636c 6175 7365 2e0a  WHERE`` clause..
+00002240: 2020 2020 2020 2020 7765 656b 2028 676f          week (go
+00002250: 6f67 6c65 2e74 7970 652e 6461 7465 5f70  ogle.type.date_p
+00002260: 6232 2e44 6174 6529 3a0a 2020 2020 2020  b2.Date):.      
+00002270: 2020 2020 2020 4669 7273 7420 6461 7920        First day 
+00002280: 6f66 2074 6865 2077 6565 6b20 284d 6f6e  of the week (Mon
+00002290: 6461 7929 206f 6620 7468 6520 6d65 7472  day) of the metr
+000022a0: 6963 730a 2020 2020 2020 2020 2020 2020  ics.            
+000022b0: 6461 7465 2069 6e20 7468 6520 6d65 7263  date in the merc
+000022c0: 6861 6e74 2074 696d 657a 6f6e 652e 2053  hant timezone. S
+000022d0: 6567 6d65 6e74 2e0a 2020 2020 2020 2020  egment..        
+000022e0: 6375 7374 6f6d 6572 5f63 6f75 6e74 7279  customer_country
+000022f0: 5f63 6f64 6520 2873 7472 293a 0a20 2020  _code (str):.   
+00002300: 2020 2020 2020 2020 2043 6f64 6520 6f66           Code of
+00002310: 2074 6865 2063 6f75 6e74 7279 2077 6865   the country whe
+00002320: 7265 2074 6865 2063 7573 746f 6d65 7220  re the customer 
+00002330: 6973 0a20 2020 2020 2020 2020 2020 206c  is.            l
+00002340: 6f63 6174 6564 2061 7420 7468 6520 7469  ocated at the ti
+00002350: 6d65 206f 6620 7468 6520 6576 656e 742e  me of the event.
+00002360: 2052 6570 7265 7365 6e74 6564 2069 6e0a   Represented in.
+00002370: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00002380: 4953 4f20 3331 3636 2066 6f72 6d61 742e  ISO 3166 format.
+00002390: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
+000023a0: 2020 2020 2020 2049 6620 7468 6520 6375         If the cu
+000023b0: 7374 6f6d 6572 2063 6f75 6e74 7279 2063  stomer country c
+000023c0: 616e 6e6f 7420 6265 2064 6574 6572 6d69  annot be determi
+000023d0: 6e65 642c 2061 0a20 2020 2020 2020 2020  ned, a.         
+000023e0: 2020 2073 7065 6369 616c 2027 5a5a 2720     special 'ZZ' 
+000023f0: 636f 6465 2069 7320 7265 7475 726e 6564  code is returned
+00002400: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+00002410: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+00002420: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+00002430: 5f20 6060 5f63 7573 746f 6d65 725f 636f  _ ``_customer_co
+00002440: 756e 7472 795f 636f 6465 6060 2e0a 2020  untry_code``..  
+00002450: 2020 2020 2020 6f66 6665 725f 6964 2028        offer_id (
+00002460: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00002470: 2020 4d65 7263 6861 6e74 2d70 726f 7669    Merchant-provi
+00002480: 6465 6420 6964 206f 6620 7468 6520 7072  ded id of the pr
+00002490: 6f64 7563 742e 2053 6567 6d65 6e74 2e0a  oduct. Segment..
+000024a0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+000024b0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+000024c0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000024d0: 6060 5f6f 6666 6572 5f69 6460 602e 0a20  ``_offer_id``.. 
+000024e0: 2020 2020 2020 2074 6974 6c65 2028 7374         title (st
+000024f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00002500: 5469 746c 6520 6f66 2074 6865 2070 726f  Title of the pro
+00002510: 6475 6374 2e20 5365 676d 656e 742e 0a0a  duct. Segment...
+00002520: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00002530: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00002540: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00002550: 605f 7469 746c 6560 602e 0a20 2020 2020  `_title``..     
+00002560: 2020 2062 7261 6e64 2028 7374 7229 3a0a     brand (str):.
+00002570: 2020 2020 2020 2020 2020 2020 4272 616e              Bran
+00002580: 6420 6f66 2074 6865 2070 726f 6475 6374  d of the product
+00002590: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+000025a0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000025b0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000025c0: 6620 606f 6e65 6f66 605f 2060 605f 6272  f `oneof`_ ``_br
+000025d0: 616e 6460 602e 0a20 2020 2020 2020 2063  and``..        c
+000025e0: 6174 6567 6f72 795f 6c31 2028 7374 7229  ategory_l1 (str)
+000025f0: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002600: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00002610: 2831 7374 0a20 2020 2020 2020 2020 2020  (1st.           
+00002620: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00002630: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00002640: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+00002650: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+00002660: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+00002670: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+00002680: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+00002690: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+000026a0: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
+000026b0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+000026c0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+000026d0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000026e0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000026f0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00002700: 5f6c 3160 602e 0a20 2020 2020 2020 2063  _l1``..        c
+00002710: 6174 6567 6f72 795f 6c32 2028 7374 7229  ategory_l2 (str)
+00002720: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002730: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00002740: 2832 6e64 0a20 2020 2020 2020 2020 2020  (2nd.           
+00002750: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00002760: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00002770: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+00002780: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+00002790: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+000027a0: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+000027b0: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+000027c0: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+000027d0: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
+000027e0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+000027f0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00002800: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00002810: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00002820: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00002830: 5f6c 3260 602e 0a20 2020 2020 2020 2063  _l2``..        c
+00002840: 6174 6567 6f72 795f 6c33 2028 7374 7229  ategory_l3 (str)
+00002850: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002860: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00002870: 2833 7264 0a20 2020 2020 2020 2020 2020  (3rd.           
+00002880: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00002890: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+000028a0: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+000028b0: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+000028c0: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+000028d0: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+000028e0: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+000028f0: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+00002900: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
+00002910: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+00002920: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00002930: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00002940: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00002950: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00002960: 5f6c 3360 602e 0a20 2020 2020 2020 2063  _l3``..        c
+00002970: 6174 6567 6f72 795f 6c34 2028 7374 7229  ategory_l4 (str)
+00002980: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002990: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+000029a0: 2834 7468 0a20 2020 2020 2020 2020 2020  (4th.           
+000029b0: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+000029c0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+000029d0: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+000029e0: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+000029f0: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+00002a00: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+00002a10: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+00002a20: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+00002a30: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
+00002a40: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+00002a50: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00002a60: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00002a70: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00002a80: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00002a90: 5f6c 3460 602e 0a20 2020 2020 2020 2063  _l4``..        c
+00002aa0: 6174 6567 6f72 795f 6c35 2028 7374 7229  ategory_l5 (str)
+00002ab0: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002ac0: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00002ad0: 2835 7468 0a20 2020 2020 2020 2020 2020  (5th.           
+00002ae0: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00002af0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00002b00: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+00002b10: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+00002b20: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+00002b30: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+00002b40: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+00002b50: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+00002b60: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
+00002b70: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+00002b80: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00002b90: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00002ba0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00002bb0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00002bc0: 5f6c 3560 602e 0a20 2020 2020 2020 2070  _l5``..        p
+00002bd0: 726f 6475 6374 5f74 7970 655f 6c31 2028  roduct_type_l1 (
+00002be0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00002bf0: 2020 6050 726f 6475 6374 2074 7970 6520    `Product type 
+00002c00: 2831 7374 0a20 2020 2020 2020 2020 2020  (1st.           
+00002c10: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00002c20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00002c30: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+00002c40: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+00002c50: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+00002c60: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+00002c70: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+00002c80: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+00002c90: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
+00002ca0: 7072 6f64 7563 7420 7461 786f 6e6f 6d79  product taxonomy
+00002cb0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+00002cc0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00002cd0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00002ce0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+00002cf0: 6f64 7563 745f 7479 7065 5f6c 3160 602e  oduct_type_l1``.
+00002d00: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+00002d10: 5f74 7970 655f 6c32 2028 7374 7229 3a0a  _type_l2 (str):.
+00002d20: 2020 2020 2020 2020 2020 2020 6050 726f              `Pro
+00002d30: 6475 6374 2074 7970 6520 2832 6e64 0a20  duct type (2nd. 
+00002d40: 2020 2020 2020 2020 2020 206c 6576 656c             level
+00002d50: 2920 3c68 7474 7073 3a2f 2f64 6576 656c  ) <https://devel
+00002d60: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00002d70: 2f73 686f 7070 696e 672d 636f 6e74 656e  /shopping-conten
+00002d80: 742f 6775 6964 6573 2f72 6570 6f72 7473  t/guides/reports
+00002d90: 2f73 6567 6d65 6e74 6174 696f 6e23 6361  /segmentation#ca
+00002da0: 7465 676f 7279 5f61 6e64 5f70 726f 6475  tegory_and_produ
+00002db0: 6374 5f74 7970 653e 605f 5f0a 2020 2020  ct_type>`__.    
+00002dc0: 2020 2020 2020 2020 696e 206d 6572 6368          in merch
+00002dd0: 616e 7427 7320 6f77 6e20 7072 6f64 7563  ant's own produc
+00002de0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+00002df0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00002e00: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00002e10: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00002e20: 6f66 605f 2060 605f 7072 6f64 7563 745f  of`_ ``_product_
+00002e30: 7479 7065 5f6c 3260 602e 0a20 2020 2020  type_l2``..     
+00002e40: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+00002e50: 6c33 2028 7374 7229 3a0a 2020 2020 2020  l3 (str):.      
+00002e60: 2020 2020 2020 6050 726f 6475 6374 2074        `Product t
+00002e70: 7970 6520 2833 7264 0a20 2020 2020 2020  ype (3rd.       
+00002e80: 2020 2020 206c 6576 656c 2920 3c68 7474       level) <htt
+00002e90: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00002ea0: 676f 6f67 6c65 2e63 6f6d 2f73 686f 7070  google.com/shopp
+00002eb0: 696e 672d 636f 6e74 656e 742f 6775 6964  ing-content/guid
+00002ec0: 6573 2f72 6570 6f72 7473 2f73 6567 6d65  es/reports/segme
+00002ed0: 6e74 6174 696f 6e23 6361 7465 676f 7279  ntation#category
+00002ee0: 5f61 6e64 5f70 726f 6475 6374 5f74 7970  _and_product_typ
+00002ef0: 653e 605f 5f0a 2020 2020 2020 2020 2020  e>`__.          
+00002f00: 2020 696e 206d 6572 6368 616e 7427 7320    in merchant's 
+00002f10: 6f77 6e20 7072 6f64 7563 7420 7461 786f  own product taxo
+00002f20: 6e6f 6d79 2e20 5365 676d 656e 742e 0a0a  nomy. Segment...
+00002f30: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00002f40: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00002f50: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00002f60: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+00002f70: 3360 602e 0a20 2020 2020 2020 2070 726f  3``..        pro
+00002f80: 6475 6374 5f74 7970 655f 6c34 2028 7374  duct_type_l4 (st
+00002f90: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00002fa0: 6050 726f 6475 6374 2074 7970 6520 2834  `Product type (4
+00002fb0: 7468 0a20 2020 2020 2020 2020 2020 206c  th.            l
+00002fc0: 6576 656c 2920 3c68 7474 7073 3a2f 2f64  evel) <https://d
+00002fd0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00002fe0: 2e63 6f6d 2f73 686f 7070 696e 672d 636f  .com/shopping-co
+00002ff0: 6e74 656e 742f 6775 6964 6573 2f72 6570  ntent/guides/rep
+00003000: 6f72 7473 2f73 6567 6d65 6e74 6174 696f  orts/segmentatio
+00003010: 6e23 6361 7465 676f 7279 5f61 6e64 5f70  n#category_and_p
+00003020: 726f 6475 6374 5f74 7970 653e 605f 5f0a  roduct_type>`__.
+00003030: 2020 2020 2020 2020 2020 2020 696e 206d              in m
+00003040: 6572 6368 616e 7427 7320 6f77 6e20 7072  erchant's own pr
+00003050: 6f64 7563 7420 7461 786f 6e6f 6d79 2e20  oduct taxonomy. 
+00003060: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
+00003070: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00003080: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00003090: 606f 6e65 6f66 605f 2060 605f 7072 6f64  `oneof`_ ``_prod
+000030a0: 7563 745f 7479 7065 5f6c 3460 602e 0a20  uct_type_l4``.. 
+000030b0: 2020 2020 2020 2070 726f 6475 6374 5f74         product_t
+000030c0: 7970 655f 6c35 2028 7374 7229 3a0a 2020  ype_l5 (str):.  
+000030d0: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+000030e0: 6374 2074 7970 6520 2835 7468 0a20 2020  ct type (5th.   
+000030f0: 2020 2020 2020 2020 206c 6576 656c 2920           level) 
+00003100: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+00003110: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f73  ers.google.com/s
+00003120: 686f 7070 696e 672d 636f 6e74 656e 742f  hopping-content/
+00003130: 6775 6964 6573 2f72 6570 6f72 7473 2f73  guides/reports/s
+00003140: 6567 6d65 6e74 6174 696f 6e23 6361 7465  egmentation#cate
+00003150: 676f 7279 5f61 6e64 5f70 726f 6475 6374  gory_and_product
+00003160: 5f74 7970 653e 605f 5f0a 2020 2020 2020  _type>`__.      
+00003170: 2020 2020 2020 696e 206d 6572 6368 616e        in merchan
+00003180: 7427 7320 6f77 6e20 7072 6f64 7563 7420  t's own product 
+00003190: 7461 786f 6e6f 6d79 2e20 5365 676d 656e  taxonomy. Segmen
+000031a0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+000031b0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+000031c0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+000031d0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
+000031e0: 7065 5f6c 3560 602e 0a20 2020 2020 2020  pe_l5``..       
+000031f0: 2063 7573 746f 6d5f 6c61 6265 6c30 2028   custom_label0 (
+00003200: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00003210: 2020 4375 7374 6f6d 206c 6162 656c 2030    Custom label 0
+00003220: 2066 6f72 2063 7573 746f 6d20 6772 6f75   for custom grou
+00003230: 7069 6e67 206f 660a 2020 2020 2020 2020  ping of.        
+00003240: 2020 2020 7072 6f64 7563 7473 2e20 5365      products. Se
+00003250: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
+00003260: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00003270: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00003280: 6e65 6f66 605f 2060 605f 6375 7374 6f6d  neof`_ ``_custom
+00003290: 5f6c 6162 656c 3060 602e 0a20 2020 2020  _label0``..     
+000032a0: 2020 2063 7573 746f 6d5f 6c61 6265 6c31     custom_label1
+000032b0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+000032c0: 2020 2020 4375 7374 6f6d 206c 6162 656c      Custom label
+000032d0: 2031 2066 6f72 2063 7573 746f 6d20 6772   1 for custom gr
+000032e0: 6f75 7069 6e67 206f 660a 2020 2020 2020  ouping of.      
+000032f0: 2020 2020 2020 7072 6f64 7563 7473 2e20        products. 
+00003300: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
+00003310: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00003320: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00003330: 606f 6e65 6f66 605f 2060 605f 6375 7374  `oneof`_ ``_cust
+00003340: 6f6d 5f6c 6162 656c 3160 602e 0a20 2020  om_label1``..   
+00003350: 2020 2020 2063 7573 746f 6d5f 6c61 6265       custom_labe
+00003360: 6c32 2028 7374 7229 3a0a 2020 2020 2020  l2 (str):.      
+00003370: 2020 2020 2020 4375 7374 6f6d 206c 6162        Custom lab
+00003380: 656c 2032 2066 6f72 2063 7573 746f 6d20  el 2 for custom 
+00003390: 6772 6f75 7069 6e67 206f 660a 2020 2020  grouping of.    
+000033a0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
+000033b0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+000033c0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000033d0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000033e0: 6620 606f 6e65 6f66 605f 2060 605f 6375  f `oneof`_ ``_cu
+000033f0: 7374 6f6d 5f6c 6162 656c 3260 602e 0a20  stom_label2``.. 
+00003400: 2020 2020 2020 2063 7573 746f 6d5f 6c61         custom_la
+00003410: 6265 6c33 2028 7374 7229 3a0a 2020 2020  bel3 (str):.    
+00003420: 2020 2020 2020 2020 4375 7374 6f6d 206c          Custom l
+00003430: 6162 656c 2033 2066 6f72 2063 7573 746f  abel 3 for custo
+00003440: 6d20 6772 6f75 7069 6e67 206f 660a 2020  m grouping of.  
+00003450: 2020 2020 2020 2020 2020 7072 6f64 7563            produc
+00003460: 7473 2e20 5365 676d 656e 742e 0a0a 2020  ts. Segment...  
+00003470: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00003480: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00003490: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+000034a0: 6375 7374 6f6d 5f6c 6162 656c 3360 602e  custom_label3``.
+000034b0: 0a20 2020 2020 2020 2063 7573 746f 6d5f  .        custom_
+000034c0: 6c61 6265 6c34 2028 7374 7229 3a0a 2020  label4 (str):.  
+000034d0: 2020 2020 2020 2020 2020 4375 7374 6f6d            Custom
+000034e0: 206c 6162 656c 2034 2066 6f72 2063 7573   label 4 for cus
+000034f0: 746f 6d20 6772 6f75 7069 6e67 206f 660a  tom grouping of.
+00003500: 2020 2020 2020 2020 2020 2020 7072 6f64              prod
+00003510: 7563 7473 2e20 5365 676d 656e 742e 0a0a  ucts. Segment...
+00003520: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00003530: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00003540: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00003550: 605f 6375 7374 6f6d 5f6c 6162 656c 3460  `_custom_label4`
+00003560: 602e 0a20 2020 2020 2020 2063 6c69 636b  `..        click
+00003570: 7320 2869 6e74 293a 0a20 2020 2020 2020  s (int):.       
+00003580: 2020 2020 204e 756d 6265 7220 6f66 2063       Number of c
+00003590: 6c69 636b 732e 204d 6574 7269 632e 0a0a  licks. Metric...
+000035a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000035b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+000035c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+000035d0: 605f 636c 6963 6b73 6060 2e0a 2020 2020  `_clicks``..    
+000035e0: 2020 2020 696d 7072 6573 7369 6f6e 7320      impressions 
+000035f0: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
+00003600: 2020 204e 756d 6265 7220 6f66 2074 696d     Number of tim
+00003610: 6573 206d 6572 6368 616e 7427 7320 7072  es merchant's pr
+00003620: 6f64 7563 7473 2061 7265 0a20 2020 2020  oducts are.     
+00003630: 2020 2020 2020 2073 686f 776e 2e20 4d65         shown. Me
+00003640: 7472 6963 2e0a 0a20 2020 2020 2020 2020  tric...         
+00003650: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00003660: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00003670: 656f 6660 5f20 6060 5f69 6d70 7265 7373  eof`_ ``_impress
+00003680: 696f 6e73 6060 2e0a 2020 2020 2020 2020  ions``..        
+00003690: 636c 6963 6b5f 7468 726f 7567 685f 7261  click_through_ra
+000036a0: 7465 2028 666c 6f61 7429 3a0a 2020 2020  te (float):.    
+000036b0: 2020 2020 2020 2020 436c 6963 6b2d 7468          Click-th
+000036c0: 726f 7567 6820 7261 7465 202d 2074 6865  rough rate - the
+000036d0: 206e 756d 6265 7220 6f66 2063 6c69 636b   number of click
+000036e0: 730a 2020 2020 2020 2020 2020 2020 6d65  s.            me
+000036f0: 7263 6861 6e74 2773 2070 726f 6475 6374  rchant's product
+00003700: 7320 7265 6365 6976 6520 2863 6c69 636b  s receive (click
+00003710: 7329 2064 6976 6964 6564 2062 790a 2020  s) divided by.  
+00003720: 2020 2020 2020 2020 2020 7468 6520 6e75            the nu
+00003730: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
+00003740: 6520 7072 6f64 7563 7473 2061 7265 2073  e products are s
+00003750: 686f 776e 0a20 2020 2020 2020 2020 2020  hown.           
+00003760: 2028 696d 7072 6573 7369 6f6e 7329 2e20   (impressions). 
+00003770: 4d65 7472 6963 2e0a 0a20 2020 2020 2020  Metric...       
+00003780: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00003790: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+000037a0: 6f6e 656f 6660 5f20 6060 5f63 6c69 636b  oneof`_ ``_click
+000037b0: 5f74 6872 6f75 6768 5f72 6174 6560 602e  _through_rate``.
+000037c0: 0a20 2020 2020 2020 2063 6f6e 7665 7273  .        convers
+000037d0: 696f 6e73 2028 666c 6f61 7429 3a0a 2020  ions (float):.  
+000037e0: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
+000037f0: 206f 6620 636f 6e76 6572 7369 6f6e 7320   of conversions 
+00003800: 6174 7472 6962 7574 6564 2074 6f20 7468  attributed to th
+00003810: 6520 7072 6f64 7563 742c 2072 6570 6f72  e product, repor
+00003820: 7465 6420 6f6e 0a20 2020 2020 2020 2020  ted on.         
+00003830: 2020 2074 6865 2063 6f6e 7665 7273 696f     the conversio
+00003840: 6e20 6461 7465 2e20 4465 7065 6e64 696e  n date. Dependin
+00003850: 6720 6f6e 2074 6865 2061 7474 7269 6275  g on the attribu
+00003860: 7469 6f6e 206d 6f64 656c 2c20 610a 2020  tion model, a.  
+00003870: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
+00003880: 7369 6f6e 206d 6967 6874 2062 6520 6469  sion might be di
+00003890: 7374 7269 6275 7465 6420 6163 726f 7373  stributed across
+000038a0: 206d 756c 7469 706c 6520 636c 6963 6b73   multiple clicks
+000038b0: 2c0a 2020 2020 2020 2020 2020 2020 7768  ,.            wh
+000038c0: 6572 6520 6561 6368 2063 6c69 636b 2067  ere each click g
+000038d0: 6574 7320 6974 7320 6f77 6e20 6372 6564  ets its own cred
+000038e0: 6974 2061 7373 6967 6e65 642e 2054 6869  it assigned. Thi
+000038f0: 7320 6d65 7472 6963 0a20 2020 2020 2020  s metric.       
+00003900: 2020 2020 2069 7320 6120 7375 6d20 6f66       is a sum of
+00003910: 2061 6c6c 2073 7563 6820 6372 6564 6974   all such credit
+00003920: 732e 204d 6574 7269 632e 0a0a 2020 2020  s. Metric...    
+00003930: 2020 2020 2020 2020 4176 6169 6c61 626c          Availabl
+00003940: 6520 6f6e 6c79 2066 6f72 2074 6865 2060  e only for the `
+00003950: 6046 5245 4560 6020 7472 6166 6669 6320  `FREE`` traffic 
+00003960: 736f 7572 6365 2e0a 0a20 2020 2020 2020  source...       
+00003970: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00003980: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00003990: 6f6e 656f 6660 5f20 6060 5f63 6f6e 7665  oneof`_ ``_conve
+000039a0: 7273 696f 6e73 6060 2e0a 2020 2020 2020  rsions``..      
+000039b0: 2020 636f 6e76 6572 7369 6f6e 5f76 616c    conversion_val
+000039c0: 7565 2028 676f 6f67 6c65 2e73 686f 7070  ue (google.shopp
+000039d0: 696e 672e 7479 7065 2e74 7970 6573 2e50  ing.type.types.P
+000039e0: 7269 6365 293a 0a20 2020 2020 2020 2020  rice):.         
+000039f0: 2020 2056 616c 7565 206f 6620 636f 6e76     Value of conv
+00003a00: 6572 7369 6f6e 7320 6174 7472 6962 7574  ersions attribut
+00003a10: 6564 2074 6f20 7468 6520 7072 6f64 7563  ed to the produc
+00003a20: 742c 2072 6570 6f72 7465 6420 6f6e 0a20  t, reported on. 
+00003a30: 2020 2020 2020 2020 2020 2074 6865 2063             the c
+00003a40: 6f6e 7665 7273 696f 6e20 6461 7465 2e20  onversion date. 
+00003a50: 4d65 7472 6963 2e0a 0a20 2020 2020 2020  Metric...       
+00003a60: 2020 2020 2041 7661 696c 6162 6c65 206f       Available o
+00003a70: 6e6c 7920 666f 7220 7468 6520 6060 4652  nly for the ``FR
+00003a80: 4545 6060 2074 7261 6666 6963 2073 6f75  EE`` traffic sou
+00003a90: 7263 652e 0a20 2020 2020 2020 2063 6f6e  rce..        con
+00003aa0: 7665 7273 696f 6e5f 7261 7465 2028 666c  version_rate (fl
+00003ab0: 6f61 7429 3a0a 2020 2020 2020 2020 2020  oat):.          
+00003ac0: 2020 4e75 6d62 6572 206f 6620 636f 6e76    Number of conv
+00003ad0: 6572 7369 6f6e 7320 6469 7669 6465 6420  ersions divided 
+00003ae0: 6279 2074 6865 206e 756d 6265 7220 6f66  by the number of
+00003af0: 2063 6c69 636b 732c 0a20 2020 2020 2020   clicks,.       
+00003b00: 2020 2020 2072 6570 6f72 7465 6420 6f6e       reported on
+00003b10: 2074 6865 2069 6d70 7265 7373 696f 6e20   the impression 
+00003b20: 6461 7465 2e20 4d65 7472 6963 2e0a 0a20  date. Metric... 
+00003b30: 2020 2020 2020 2020 2020 2041 7661 696c             Avail
+00003b40: 6162 6c65 206f 6e6c 7920 666f 7220 7468  able only for th
+00003b50: 6520 6060 4652 4545 6060 2074 7261 6666  e ``FREE`` traff
+00003b60: 6963 2073 6f75 7263 652e 0a0a 2020 2020  ic source...    
+00003b70: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00003b80: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00003b90: 6620 606f 6e65 6f66 605f 2060 605f 636f  f `oneof`_ ``_co
+00003ba0: 6e76 6572 7369 6f6e 5f72 6174 6560 602e  nversion_rate``.
+00003bb0: 0a20 2020 2022 2222 0a0a 2020 2020 6d61  .    """..    ma
+00003bc0: 726b 6574 696e 675f 6d65 7468 6f64 3a20  rketing_method: 
+00003bd0: 224d 6172 6b65 7469 6e67 4d65 7468 6f64  "MarketingMethod
+00003be0: 2e4d 6172 6b65 7469 6e67 4d65 7468 6f64  .MarketingMethod
+00003bf0: 456e 756d 2220 3d20 7072 6f74 6f2e 4669  Enum" = proto.Fi
+00003c00: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00003c10: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
+00003c20: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
+00003c30: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00003c40: 2c0a 2020 2020 2020 2020 656e 756d 3d22  ,.        enum="
+00003c50: 4d61 726b 6574 696e 674d 6574 686f 642e  MarketingMethod.
+00003c60: 4d61 726b 6574 696e 674d 6574 686f 6445  MarketingMethodE
+00003c70: 6e75 6d22 2c0a 2020 2020 290a 2020 2020  num",.    ).    
+00003c80: 6461 7465 3a20 6461 7465 5f70 6232 2e44  date: date_pb2.D
+00003c90: 6174 6520 3d20 7072 6f74 6f2e 4669 656c  ate = proto.Fiel
+00003ca0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00003cb0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+00003cc0: 2020 6e75 6d62 6572 3d32 2c0a 2020 2020    number=2,.    
+00003cd0: 2020 2020 6d65 7373 6167 653d 6461 7465      message=date
+00003ce0: 5f70 6232 2e44 6174 652c 0a20 2020 2029  _pb2.Date,.    )
+00003cf0: 0a20 2020 2077 6565 6b3a 2064 6174 655f  .    week: date_
+00003d00: 7062 322e 4461 7465 203d 2070 726f 746f  pb2.Date = proto
+00003d10: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00003d20: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00003d30: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
+00003d40: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00003d50: 3d64 6174 655f 7062 322e 4461 7465 2c0a  =date_pb2.Date,.
+00003d60: 2020 2020 290a 2020 2020 6375 7374 6f6d      ).    custom
+00003d70: 6572 5f63 6f75 6e74 7279 5f63 6f64 653a  er_country_code:
+00003d80: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00003d90: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00003da0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00003db0: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
+00003dc0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00003dd0: 652c 0a20 2020 2029 0a20 2020 206f 6666  e,.    ).    off
+00003de0: 6572 5f69 643a 2073 7472 203d 2070 726f  er_id: str = pro
+00003df0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00003e00: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+00003e10: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
+00003e20: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00003e30: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00003e40: 2020 2074 6974 6c65 3a20 7374 7220 3d20     title: str = 
+00003e50: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00003e60: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00003e70: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00003e80: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
+00003e90: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00003ea0: 290a 2020 2020 6272 616e 643a 2073 7472  ).    brand: str
+00003eb0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00003ec0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+00003ed0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+00003ee0: 6d62 6572 3d37 2c0a 2020 2020 2020 2020  mber=7,.        
+00003ef0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00003f00: 2020 2029 0a20 2020 2063 6174 6567 6f72     ).    categor
+00003f10: 795f 6c31 3a20 7374 7220 3d20 7072 6f74  y_l1: str = prot
+00003f20: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00003f30: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00003f40: 2020 2020 2020 206e 756d 6265 723d 382c         number=8,
+00003f50: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00003f60: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00003f70: 2020 6361 7465 676f 7279 5f6c 323a 2073    category_l2: s
+00003f80: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00003f90: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00003fa0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+00003fb0: 6e75 6d62 6572 3d39 2c0a 2020 2020 2020  number=9,.      
+00003fc0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00003fd0: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
+00003fe0: 6f72 795f 6c33 3a20 7374 7220 3d20 7072  ory_l3: str = pr
+00003ff0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00004000: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+00004010: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00004020: 3130 2c0a 2020 2020 2020 2020 6f70 7469  10,.        opti
+00004030: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00004040: 0a20 2020 2063 6174 6567 6f72 795f 6c34  .    category_l4
+00004050: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+00004060: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00004070: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00004080: 2020 206e 756d 6265 723d 3131 2c0a 2020     number=11,.  
+00004090: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000040a0: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+000040b0: 6174 6567 6f72 795f 6c35 3a20 7374 7220  ategory_l5: str 
+000040c0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+000040d0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+000040e0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+000040f0: 6265 723d 3132 2c0a 2020 2020 2020 2020  ber=12,.        
+00004100: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00004110: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
+00004120: 5f74 7970 655f 6c31 3a20 7374 7220 3d20  _type_l1: str = 
+00004130: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00004140: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00004150: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00004160: 723d 3133 2c0a 2020 2020 2020 2020 6f70  r=13,.        op
+00004170: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004180: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
+00004190: 7970 655f 6c32 3a20 7374 7220 3d20 7072  ype_l2: str = pr
+000041a0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+000041b0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+000041c0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+000041d0: 3134 2c0a 2020 2020 2020 2020 6f70 7469  14,.        opti
+000041e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000041f0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
+00004200: 655f 6c33 3a20 7374 7220 3d20 7072 6f74  e_l3: str = prot
+00004210: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00004220: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00004230: 2020 2020 2020 206e 756d 6265 723d 3135         number=15
+00004240: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00004250: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00004260: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+00004270: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
+00004280: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00004290: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+000042a0: 2020 2020 206e 756d 6265 723d 3136 2c0a       number=16,.
+000042b0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+000042c0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+000042d0: 2070 726f 6475 6374 5f74 7970 655f 6c35   product_type_l5
+000042e0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000042f0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00004300: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00004310: 2020 206e 756d 6265 723d 3137 2c0a 2020     number=17,.  
+00004320: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00004330: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+00004340: 7573 746f 6d5f 6c61 6265 6c30 3a20 7374  ustom_label0: st
+00004350: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00004360: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00004370: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00004380: 756d 6265 723d 3138 2c0a 2020 2020 2020  umber=18,.      
+00004390: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+000043a0: 0a20 2020 2029 0a20 2020 2063 7573 746f  .    ).    custo
+000043b0: 6d5f 6c61 6265 6c31 3a20 7374 7220 3d20  m_label1: str = 
+000043c0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000043d0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+000043e0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+000043f0: 723d 3139 2c0a 2020 2020 2020 2020 6f70  r=19,.        op
+00004400: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004410: 2029 0a20 2020 2063 7573 746f 6d5f 6c61   ).    custom_la
+00004420: 6265 6c32 3a20 7374 7220 3d20 7072 6f74  bel2: str = prot
+00004430: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00004440: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00004450: 2020 2020 2020 206e 756d 6265 723d 3230         number=20
+00004460: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00004470: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00004480: 2020 2063 7573 746f 6d5f 6c61 6265 6c33     custom_label3
+00004490: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000044a0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000044b0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000044c0: 2020 206e 756d 6265 723d 3231 2c0a 2020     number=21,.  
+000044d0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000044e0: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+000044f0: 7573 746f 6d5f 6c61 6265 6c34 3a20 7374  ustom_label4: st
+00004500: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00004510: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00004520: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00004530: 756d 6265 723d 3232 2c0a 2020 2020 2020  umber=22,.      
+00004540: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00004550: 0a20 2020 2029 0a20 2020 2063 6c69 636b  .    ).    click
+00004560: 733a 2069 6e74 203d 2070 726f 746f 2e46  s: int = proto.F
+00004570: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00004580: 6f74 6f2e 494e 5436 342c 0a20 2020 2020  oto.INT64,.     
+00004590: 2020 206e 756d 6265 723d 3233 2c0a 2020     number=23,.  
+000045a0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000045b0: 7275 652c 0a20 2020 2029 0a20 2020 2069  rue,.    ).    i
+000045c0: 6d70 7265 7373 696f 6e73 3a20 696e 7420  mpressions: int 
+000045d0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+000045e0: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
+000045f0: 3634 2c0a 2020 2020 2020 2020 6e75 6d62  64,.        numb
+00004600: 6572 3d32 342c 0a20 2020 2020 2020 206f  er=24,.        o
+00004610: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00004620: 2020 290a 2020 2020 636c 6963 6b5f 7468    ).    click_th
+00004630: 726f 7567 685f 7261 7465 3a20 666c 6f61  rough_rate: floa
+00004640: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+00004650: 0a20 2020 2020 2020 2070 726f 746f 2e44  .        proto.D
+00004660: 4f55 424c 452c 0a20 2020 2020 2020 206e  OUBLE,.        n
+00004670: 756d 6265 723d 3235 2c0a 2020 2020 2020  umber=25,.      
+00004680: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00004690: 0a20 2020 2029 0a20 2020 2063 6f6e 7665  .    ).    conve
+000046a0: 7273 696f 6e73 3a20 666c 6f61 7420 3d20  rsions: float = 
+000046b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000046c0: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
+000046d0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+000046e0: 723d 3236 2c0a 2020 2020 2020 2020 6f70  r=26,.        op
+000046f0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004700: 2029 0a20 2020 2063 6f6e 7665 7273 696f   ).    conversio
+00004710: 6e5f 7661 6c75 653a 2074 7970 6573 2e50  n_value: types.P
+00004720: 7269 6365 203d 2070 726f 746f 2e46 6965  rice = proto.Fie
+00004730: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00004740: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00004750: 2020 206e 756d 6265 723d 3237 2c0a 2020     number=27,.  
+00004760: 2020 2020 2020 6d65 7373 6167 653d 7479        message=ty
+00004770: 7065 732e 5072 6963 652c 0a20 2020 2029  pes.Price,.    )
+00004780: 0a20 2020 2063 6f6e 7665 7273 696f 6e5f  .    conversion_
+00004790: 7261 7465 3a20 666c 6f61 7420 3d20 7072  rate: float = pr
+000047a0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+000047b0: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
+000047c0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+000047d0: 3238 2c0a 2020 2020 2020 2020 6f70 7469  28,.        opti
+000047e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000047f0: 0a0a 0a63 6c61 7373 2050 726f 6475 6374  ...class Product
+00004800: 5669 6577 2870 726f 746f 2e4d 6573 7361  View(proto.Messa
+00004810: 6765 293a 0a20 2020 2072 2222 2246 6965  ge):.    r"""Fie
+00004820: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
+00004830: 7220 7175 6572 7920 696e 2060 6070 726f  r query in ``pro
+00004840: 6475 6374 5f76 6965 7760 6020 7461 626c  duct_view`` tabl
+00004850: 652e 0a0a 2020 2020 5072 6f64 7563 7473  e...    Products
+00004860: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00004870: 696e 7665 6e74 6f72 792e 2050 726f 6475  inventory. Produ
+00004880: 6374 7320 696e 2074 6869 7320 7461 626c  cts in this tabl
+00004890: 6520 6172 6520 7468 650a 2020 2020 7361  e are the.    sa
+000048a0: 6d65 2061 7320 696e 2050 726f 6475 6374  me as in Product
+000048b0: 7320 7375 622d 4150 4920 6275 7420 6e6f  s sub-API but no
+000048c0: 7420 616c 6c20 7072 6f64 7563 7420 6174  t all product at
+000048d0: 7472 6962 7574 6573 2066 726f 6d0a 2020  tributes from.  
+000048e0: 2020 5072 6f64 7563 7473 2073 7562 2d41    Products sub-A
+000048f0: 5049 2061 7265 2061 7661 696c 6162 6c65  PI are available
+00004900: 2066 6f72 2071 7565 7279 2069 6e20 7468   for query in th
+00004910: 6973 2074 6162 6c65 2e20 496e 2063 6f6e  is table. In con
+00004920: 7472 6173 740a 2020 2020 746f 2050 726f  trast.    to Pro
+00004930: 6475 6374 7320 7375 622d 4150 492c 2074  ducts sub-API, t
+00004940: 6869 7320 7461 626c 6520 616c 6c6f 7773  his table allows
+00004950: 2074 6f20 6669 6c74 6572 2074 6865 2072   to filter the r
+00004960: 6574 7572 6e65 6420 6c69 7374 0a20 2020  eturned list.   
+00004970: 206f 6620 7072 6f64 7563 7473 2062 7920   of products by 
+00004980: 7072 6f64 7563 7420 6174 7472 6962 7574  product attribut
+00004990: 6573 2e20 546f 2072 6574 7269 6576 6520  es. To retrieve 
+000049a0: 6120 7369 6e67 6c65 2070 726f 6475 6374  a single product
+000049b0: 2062 790a 2020 2020 6060 6964 6060 206f   by.    ``id`` o
+000049c0: 7220 6c69 7374 2061 6c6c 2070 726f 6475  r list all produ
+000049d0: 6374 732c 2050 726f 6475 6374 7320 7375  cts, Products su
+000049e0: 622d 4150 4920 7368 6f75 6c64 2062 6520  b-API should be 
+000049f0: 7573 6564 2e0a 0a20 2020 2056 616c 7565  used...    Value
+00004a00: 7320 6172 6520 6f6e 6c79 2073 6574 2066  s are only set f
+00004a10: 6f72 2066 6965 6c64 7320 7265 7175 6573  or fields reques
+00004a20: 7465 6420 6578 706c 6963 6974 6c79 2069  ted explicitly i
+00004a30: 6e20 7468 6520 7265 7175 6573 7427 730a  n the request's.
+00004a40: 2020 2020 7365 6172 6368 2071 7565 7279      search query
+00004a50: 2e0a 0a0a 2020 2020 2e2e 205f 6f6e 656f  ....    .. _oneo
+00004a60: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
+00004a70: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
+00004a80: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00004a90: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
+00004aa0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
+00004ab0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
+00004ac0: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
+00004ad0: 6573 3a0a 2020 2020 2020 2020 6964 2028  es:.        id (
+00004ae0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00004af0: 2020 5245 5354 2049 4420 6f66 2074 6865    REST ID of the
+00004b00: 2070 726f 6475 6374 2c20 696e 2074 6865   product, in the
+00004b10: 2066 6f72 6d20 6f66 0a20 2020 2020 2020   form of.       
+00004b20: 2020 2020 2060 6063 6861 6e6e 656c 7e6c       ``channel~l
+00004b30: 616e 6775 6167 6543 6f64 657e 6665 6564  anguageCode~feed
+00004b40: 4c61 6265 6c7e 6f66 6665 7249 6460 602e  Label~offerId``.
+00004b50: 204d 6572 6368 616e 7420 4150 490a 2020   Merchant API.  
+00004b60: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+00004b70: 7320 7468 6174 206f 7065 7261 7465 206f  s that operate o
+00004b80: 6e20 7072 6f64 7563 7473 2074 616b 6520  n products take 
+00004b90: 7468 6973 2061 7320 7468 6569 7220 6060  this as their ``
+00004ba0: 6e61 6d65 6060 0a20 2020 2020 2020 2020  name``.         
+00004bb0: 2020 2070 6172 616d 6574 6572 2e0a 0a20     parameter... 
+00004bc0: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
+00004bd0: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
+00004be0: 4543 5460 6020 636c 6175 7365 2e0a 0a20  ECT`` clause... 
+00004bf0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00004c00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+00004c10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+00004c20: 5f69 6460 602e 0a20 2020 2020 2020 2063  _id``..        c
+00004c30: 6861 6e6e 656c 2028 676f 6f67 6c65 2e73  hannel (google.s
+00004c40: 686f 7070 696e 672e 7479 7065 2e74 7970  hopping.type.typ
+00004c50: 6573 2e43 6861 6e6e 656c 2e43 6861 6e6e  es.Channel.Chann
+00004c60: 656c 456e 756d 293a 0a20 2020 2020 2020  elEnum):.       
+00004c70: 2020 2020 2043 6861 6e6e 656c 206f 6620       Channel of 
+00004c80: 7468 6520 7072 6f64 7563 742e 2043 616e  the product. Can
+00004c90: 2062 6520 6060 4f4e 4c49 4e45 6060 206f   be ``ONLINE`` o
+00004ca0: 7220 6060 4c4f 4341 4c60 602e 0a0a 2020  r ``LOCAL``...  
+00004cb0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00004cc0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00004cd0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00004ce0: 6368 616e 6e65 6c60 602e 0a20 2020 2020  channel``..     
+00004cf0: 2020 206c 616e 6775 6167 655f 636f 6465     language_code
+00004d00: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00004d10: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
+00004d20: 6520 6f66 2074 6865 2070 726f 6475 6374  e of the product
+00004d30: 2069 6e20 4243 5020 3437 0a20 2020 2020   in BCP 47.     
+00004d40: 2020 2020 2020 2066 6f72 6d61 742e 0a0a         format...
+00004d50: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00004d60: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00004d70: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00004d80: 605f 6c61 6e67 7561 6765 5f63 6f64 6560  `_language_code`
+00004d90: 602e 0a20 2020 2020 2020 2066 6565 645f  `..        feed_
+00004da0: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
+00004db0: 2020 2020 2020 2020 2046 6565 6420 6c61           Feed la
+00004dc0: 6265 6c20 6f66 2074 6865 2070 726f 6475  bel of the produ
+00004dd0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
+00004de0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00004df0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00004e00: 6660 5f20 6060 5f66 6565 645f 6c61 6265  f`_ ``_feed_labe
+00004e10: 6c60 602e 0a20 2020 2020 2020 206f 6666  l``..        off
+00004e20: 6572 5f69 6420 2873 7472 293a 0a20 2020  er_id (str):.   
+00004e30: 2020 2020 2020 2020 204d 6572 6368 616e           Merchan
+00004e40: 742d 7072 6f76 6964 6564 2069 6420 6f66  t-provided id of
+00004e50: 2074 6865 2070 726f 6475 6374 2e0a 0a20   the product... 
+00004e60: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00004e70: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+00004e80: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+00004e90: 5f6f 6666 6572 5f69 6460 602e 0a20 2020  _offer_id``..   
+00004ea0: 2020 2020 2074 6974 6c65 2028 7374 7229       title (str)
+00004eb0: 3a0a 2020 2020 2020 2020 2020 2020 5469  :.            Ti
+00004ec0: 746c 6520 6f66 2074 6865 2070 726f 6475  tle of the produ
+00004ed0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
+00004ee0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00004ef0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00004f00: 6660 5f20 6060 5f74 6974 6c65 6060 2e0a  f`_ ``_title``..
+00004f10: 2020 2020 2020 2020 6272 616e 6420 2873          brand (s
+00004f20: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00004f30: 2042 7261 6e64 206f 6620 7468 6520 7072   Brand of the pr
+00004f40: 6f64 7563 742e 0a0a 2020 2020 2020 2020  oduct...        
+00004f50: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00004f60: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00004f70: 6e65 6f66 605f 2060 605f 6272 616e 6460  neof`_ ``_brand`
+00004f80: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+00004f90: 6f72 795f 6c31 2028 7374 7229 3a0a 2020  ory_l1 (str):.  
+00004fa0: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+00004fb0: 7420 6361 7465 676f 7279 2028 3173 7420  t category (1st 
+00004fc0: 6c65 7665 6c29 2069 6e20 6047 6f6f 676c  level) in `Googl
+00004fd0: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
+00004fe0: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+00004ff0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00005000: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00005010: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+00005020: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
+00005030: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00005040: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00005050: 6620 606f 6e65 6f66 605f 2060 605f 6361  f `oneof`_ ``_ca
+00005060: 7465 676f 7279 5f6c 3160 602e 0a20 2020  tegory_l1``..   
+00005070: 2020 2020 2063 6174 6567 6f72 795f 6c32       category_l2
+00005080: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00005090: 2020 2020 5072 6f64 7563 7420 6361 7465      Product cate
+000050a0: 676f 7279 2028 326e 6420 6c65 7665 6c29  gory (2nd level)
+000050b0: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
+000050c0: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+000050d0: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+000050e0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+000050f0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+00005100: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
+00005110: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+00005120: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00005130: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00005140: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+00005150: 5f6c 3260 602e 0a20 2020 2020 2020 2063  _l2``..        c
+00005160: 6174 6567 6f72 795f 6c33 2028 7374 7229  ategory_l3 (str)
+00005170: 3a0a 2020 2020 2020 2020 2020 2020 5072  :.            Pr
+00005180: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
+00005190: 3372 6420 6c65 7665 6c29 2069 6e20 6047  3rd level) in `G
+000051a0: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
+000051b0: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+000051c0: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+000051d0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+000051e0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+000051f0: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
+00005200: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00005210: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00005220: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00005230: 605f 6361 7465 676f 7279 5f6c 3360 602e  `_category_l3``.
+00005240: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
+00005250: 795f 6c34 2028 7374 7229 3a0a 2020 2020  y_l4 (str):.    
+00005260: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
+00005270: 6361 7465 676f 7279 2028 3474 6820 6c65  category (4th le
+00005280: 7665 6c29 2069 6e20 6047 6f6f 676c 6527  vel) in `Google'
+00005290: 7320 7072 6f64 7563 740a 2020 2020 2020  s product.      
+000052a0: 2020 2020 2020 7461 786f 6e6f 6d79 203c        taxonomy <
+000052b0: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
+000052c0: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
+000052d0: 616e 7473 2f61 6e73 7765 722f 3633 3234  ants/answer/6324
+000052e0: 3433 363e 605f 5f2e 0a0a 2020 2020 2020  436>`__...      
+000052f0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00005300: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00005310: 606f 6e65 6f66 605f 2060 605f 6361 7465  `oneof`_ ``_cate
+00005320: 676f 7279 5f6c 3460 602e 0a20 2020 2020  gory_l4``..     
+00005330: 2020 2063 6174 6567 6f72 795f 6c35 2028     category_l5 (
+00005340: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00005350: 2020 5072 6f64 7563 7420 6361 7465 676f    Product catego
+00005360: 7279 2028 3574 6820 6c65 7665 6c29 2069  ry (5th level) i
+00005370: 6e20 6047 6f6f 676c 6527 7320 7072 6f64  n `Google's prod
+00005380: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+00005390: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+000053a0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+000053b0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+000053c0: 6e73 7765 722f 3633 3234 3433 363e 605f  nswer/6324436>`_
+000053d0: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+000053e0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+000053f0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00005400: 605f 2060 605f 6361 7465 676f 7279 5f6c  `_ ``_category_l
+00005410: 3560 602e 0a20 2020 2020 2020 2070 726f  5``..        pro
+00005420: 6475 6374 5f74 7970 655f 6c31 2028 7374  duct_type_l1 (st
+00005430: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005440: 5072 6f64 7563 7420 7479 7065 2028 3173  Product type (1s
+00005450: 7420 6c65 7665 6c29 2069 6e20 6d65 7263  t level) in merc
+00005460: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
+00005470: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+00005480: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+00005490: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+000054a0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+000054b0: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
+000054c0: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+000054d0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+000054e0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+000054f0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
+00005500: 7065 5f6c 3160 602e 0a20 2020 2020 2020  pe_l1``..       
+00005510: 2070 726f 6475 6374 5f74 7970 655f 6c32   product_type_l2
+00005520: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00005530: 2020 2020 5072 6f64 7563 7420 7479 7065      Product type
+00005540: 2028 326e 6420 6c65 7665 6c29 2069 6e20   (2nd level) in 
+00005550: 6d65 7263 6861 6e74 2773 206f 776e 2060  merchant's own `
+00005560: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+00005570: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+00005580: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+00005590: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+000055a0: 7473 2f61 6e73 7765 722f 3633 3234 3430  ts/answer/632440
+000055b0: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+000055c0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+000055d0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+000055e0: 6e65 6f66 605f 2060 605f 7072 6f64 7563  neof`_ ``_produc
+000055f0: 745f 7479 7065 5f6c 3260 602e 0a20 2020  t_type_l2``..   
+00005600: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
+00005610: 655f 6c33 2028 7374 7229 3a0a 2020 2020  e_l3 (str):.    
+00005620: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
+00005630: 7479 7065 2028 3372 6420 6c65 7665 6c29  type (3rd level)
+00005640: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
+00005650: 776e 2060 7072 6f64 7563 740a 2020 2020  wn `product.    
+00005660: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+00005670: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00005680: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00005690: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+000056a0: 3234 3430 363e 605f 5f2e 0a0a 2020 2020  24406>`__...    
+000056b0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000056c0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000056d0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+000056e0: 6f64 7563 745f 7479 7065 5f6c 3360 602e  oduct_type_l3``.
+000056f0: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+00005700: 5f74 7970 655f 6c34 2028 7374 7229 3a0a  _type_l4 (str):.
+00005710: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+00005720: 7563 7420 7479 7065 2028 3474 6820 6c65  uct type (4th le
+00005730: 7665 6c29 2069 6e20 6d65 7263 6861 6e74  vel) in merchant
+00005740: 2773 206f 776e 2060 7072 6f64 7563 740a  's own `product.
+00005750: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+00005760: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+00005770: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00005780: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00005790: 722f 3633 3234 3430 363e 605f 5f2e 0a0a  r/6324406>`__...
+000057a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000057b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+000057c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+000057d0: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+000057e0: 3460 602e 0a20 2020 2020 2020 2070 726f  4``..        pro
+000057f0: 6475 6374 5f74 7970 655f 6c35 2028 7374  duct_type_l5 (st
+00005800: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005810: 5072 6f64 7563 7420 7479 7065 2028 3574  Product type (5t
+00005820: 6820 6c65 7665 6c29 2069 6e20 6d65 7263  h level) in merc
+00005830: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
+00005840: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+00005850: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+00005860: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+00005870: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+00005880: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
+00005890: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+000058a0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+000058b0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+000058c0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
+000058d0: 7065 5f6c 3560 602e 0a20 2020 2020 2020  pe_l5``..       
+000058e0: 2070 7269 6365 2028 676f 6f67 6c65 2e73   price (google.s
+000058f0: 686f 7070 696e 672e 7479 7065 2e74 7970  hopping.type.typ
+00005900: 6573 2e50 7269 6365 293a 0a20 2020 2020  es.Price):.     
+00005910: 2020 2020 2020 2050 726f 6475 6374 2070         Product p
+00005920: 7269 6365 2e20 4162 7365 6e74 2069 6620  rice. Absent if 
+00005930: 7468 6520 696e 666f 726d 6174 696f 6e0a  the information.
+00005940: 2020 2020 2020 2020 2020 2020 6162 6f75              abou
+00005950: 7420 7468 6520 7072 6963 6520 6f66 2074  t the price of t
+00005960: 6865 2070 726f 6475 6374 2069 7320 6e6f  he product is no
+00005970: 7420 6176 6169 6c61 626c 652e 0a20 2020  t available..   
+00005980: 2020 2020 2063 6f6e 6469 7469 6f6e 2028       condition (
+00005990: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+000059a0: 2020 6043 6f6e 6469 7469 6f6e 203c 6874    `Condition <ht
+000059b0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+000059c0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+000059d0: 7473 2f61 6e73 7765 722f 3633 3234 3436  ts/answer/632446
+000059e0: 393e 605f 5f0a 2020 2020 2020 2020 2020  9>`__.          
+000059f0: 2020 6f66 2074 6865 2070 726f 6475 6374    of the product
+00005a00: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+00005a10: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+00005a20: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+00005a30: 5f20 6060 5f63 6f6e 6469 7469 6f6e 6060  _ ``_condition``
+00005a40: 2e0a 2020 2020 2020 2020 6176 6169 6c61  ..        availa
+00005a50: 6269 6c69 7479 2028 7374 7229 3a0a 2020  bility (str):.  
+00005a60: 2020 2020 2020 2020 2020 6041 7661 696c            `Avail
+00005a70: 6162 696c 6974 7920 3c68 7474 7073 3a2f  ability <https:/
+00005a80: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+00005a90: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+00005aa0: 7377 6572 2f36 3332 3434 3438 3e60 5f5f  swer/6324448>`__
+00005ab0: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
+00005ac0: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
+00005ad0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00005ae0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00005af0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00005b00: 6176 6169 6c61 6269 6c69 7479 6060 2e0a  availability``..
+00005b10: 2020 2020 2020 2020 7368 6970 7069 6e67          shipping
+00005b20: 5f6c 6162 656c 2028 7374 7229 3a0a 2020  _label (str):.  
+00005b30: 2020 2020 2020 2020 2020 4e6f 726d 616c            Normal
+00005b40: 697a 6564 2060 7368 6970 7069 6e67 0a20  ized `shipping. 
+00005b50: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00005b60: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00005b70: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00005b80: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+00005b90: 3234 3530 343e 605f 5f0a 2020 2020 2020  24504>`__.      
+00005ba0: 2020 2020 2020 7370 6563 6966 6965 6420        specified 
+00005bb0: 696e 2074 6865 2066 6565 642e 0a0a 2020  in the feed...  
+00005bc0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00005bd0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00005be0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00005bf0: 7368 6970 7069 6e67 5f6c 6162 656c 6060  shipping_label``
+00005c00: 2e0a 2020 2020 2020 2020 6774 696e 2028  ..        gtin (
+00005c10: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
+00005c20: 7374 725d 293a 0a20 2020 2020 2020 2020  str]):.         
+00005c30: 2020 204c 6973 7420 6f66 2047 6c6f 6261     List of Globa
+00005c40: 6c20 5472 6164 6520 4974 656d 204e 756d  l Trade Item Num
+00005c50: 6265 7273 2028 4754 494e 7329 206f 660a  bers (GTINs) of.
+00005c60: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00005c70: 7072 6f64 7563 742e 0a20 2020 2020 2020  product..       
+00005c80: 2069 7465 6d5f 6772 6f75 705f 6964 2028   item_group_id (
+00005c90: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00005ca0: 2020 4974 656d 2067 726f 7570 2069 6420    Item group id 
+00005cb0: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
+00005cc0: 6d65 7263 6861 6e74 2066 6f72 0a20 2020  merchant for.   
+00005cd0: 2020 2020 2020 2020 2067 726f 7570 696e           groupin
+00005ce0: 6720 7661 7269 616e 7473 2074 6f67 6574  g variants toget
+00005cf0: 6865 722e 0a0a 2020 2020 2020 2020 2020  her...          
+00005d00: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00005d10: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00005d20: 6f66 605f 2060 605f 6974 656d 5f67 726f  of`_ ``_item_gro
+00005d30: 7570 5f69 6460 602e 0a20 2020 2020 2020  up_id``..       
+00005d40: 2074 6875 6d62 6e61 696c 5f6c 696e 6b20   thumbnail_link 
+00005d50: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00005d60: 2020 204c 696e 6b20 746f 2074 6865 2070     Link to the p
+00005d70: 726f 6365 7373 6564 2069 6d61 6765 206f  rocessed image o
+00005d80: 6620 7468 6520 7072 6f64 7563 742c 0a20  f the product,. 
+00005d90: 2020 2020 2020 2020 2020 2068 6f73 7465             hoste
+00005da0: 6420 6f6e 2074 6865 2047 6f6f 676c 6520  d on the Google 
+00005db0: 696e 6672 6173 7472 7563 7475 7265 2e0a  infrastructure..
+00005dc0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00005dd0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00005de0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00005df0: 6060 5f74 6875 6d62 6e61 696c 5f6c 696e  ``_thumbnail_lin
+00005e00: 6b60 602e 0a20 2020 2020 2020 2063 7265  k``..        cre
+00005e10: 6174 696f 6e5f 7469 6d65 2028 676f 6f67  ation_time (goog
+00005e20: 6c65 2e70 726f 746f 6275 662e 7469 6d65  le.protobuf.time
+00005e30: 7374 616d 705f 7062 322e 5469 6d65 7374  stamp_pb2.Timest
+00005e40: 616d 7029 3a0a 2020 2020 2020 2020 2020  amp):.          
+00005e50: 2020 5468 6520 7469 6d65 2074 6865 206d    The time the m
+00005e60: 6572 6368 616e 7420 6372 6561 7465 6420  erchant created 
+00005e70: 7468 6520 7072 6f64 7563 7420 696e 0a20  the product in. 
+00005e80: 2020 2020 2020 2020 2020 2074 696d 6573             times
+00005e90: 7461 6d70 2073 6563 6f6e 6473 2e0a 2020  tamp seconds..  
+00005ea0: 2020 2020 2020 6578 7069 7261 7469 6f6e        expiration
+00005eb0: 5f64 6174 6520 2867 6f6f 676c 652e 7479  _date (google.ty
+00005ec0: 7065 2e64 6174 655f 7062 322e 4461 7465  pe.date_pb2.Date
+00005ed0: 293a 0a20 2020 2020 2020 2020 2020 2045  ):.            E
+00005ee0: 7870 6972 6174 696f 6e20 6461 7465 2066  xpiration date f
+00005ef0: 6f72 2074 6865 2070 726f 6475 6374 2c20  or the product, 
+00005f00: 7370 6563 6966 6965 6420 6f6e 0a20 2020  specified on.   
+00005f10: 2020 2020 2020 2020 2069 6e73 6572 7469           inserti
+00005f20: 6f6e 2e0a 2020 2020 2020 2020 6167 6772  on..        aggr
+00005f30: 6567 6174 6564 5f72 6570 6f72 7469 6e67  egated_reporting
+00005f40: 5f63 6f6e 7465 7874 5f73 7461 7475 7320  _context_status 
+00005f50: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
+00005f60: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
+00005f70: 735f 7631 6265 7461 2e74 7970 6573 2e50  s_v1beta.types.P
+00005f80: 726f 6475 6374 5669 6577 2e41 6767 7265  roductView.Aggre
+00005f90: 6761 7465 6452 6570 6f72 7469 6e67 436f  gatedReportingCo
+00005fa0: 6e74 6578 7453 7461 7475 7329 3a0a 2020  ntextStatus):.  
+00005fb0: 2020 2020 2020 2020 2020 4167 6772 6567            Aggreg
+00005fc0: 6174 6564 2073 7461 7475 732e 0a0a 2020  ated status...  
+00005fd0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00005fe0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00005ff0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00006000: 6167 6772 6567 6174 6564 5f72 6570 6f72  aggregated_repor
+00006010: 7469 6e67 5f63 6f6e 7465 7874 5f73 7461  ting_context_sta
+00006020: 7475 7360 602e 0a20 2020 2020 2020 2069  tus``..        i
+00006030: 7465 6d5f 6973 7375 6573 2028 4d75 7461  tem_issues (Muta
+00006040: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
+00006050: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+00006060: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+00006070: 6574 612e 7479 7065 732e 5072 6f64 7563  eta.types.Produc
+00006080: 7456 6965 772e 4974 656d 4973 7375 655d  tView.ItemIssue]
+00006090: 293a 0a20 2020 2020 2020 2020 2020 204c  ):.            L
+000060a0: 6973 7420 6f66 2069 7465 6d20 6973 7375  ist of item issu
+000060b0: 6573 2066 6f72 2074 6865 2070 726f 6475  es for the produ
+000060c0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
+000060d0: 202a 2a54 6869 7320 6669 656c 6420 6361   **This field ca
+000060e0: 6e6e 6f74 2062 6520 7573 6564 2066 6f72  nnot be used for
+000060f0: 2073 6f72 7469 6e67 2074 6865 2072 6573   sorting the res
+00006100: 756c 7473 2e2a 2a0a 0a20 2020 2020 2020  ults.**..       
+00006110: 2020 2020 202a 2a4f 6e6c 7920 7365 6c65       **Only sele
+00006120: 6374 6564 2061 7474 7269 6275 7465 7320  cted attributes 
+00006130: 6f66 2074 6869 7320 6669 656c 6420 2866  of this field (f
+00006140: 6f72 2065 7861 6d70 6c65 2c0a 2020 2020  or example,.    
+00006150: 2020 2020 2020 2020 6060 6974 656d 5f69          ``item_i
+00006160: 7373 7565 732e 7365 7665 7269 7479 2e61  ssues.severity.a
+00006170: 6767 7265 6761 7465 645f 7365 7665 7269  ggregated_severi
+00006180: 7479 6060 2920 6361 6e20 6265 2075 7365  ty``) can be use
+00006190: 640a 2020 2020 2020 2020 2020 2020 666f  d.            fo
+000061a0: 7220 6669 6c74 6572 696e 6720 7468 6520  r filtering the 
+000061b0: 7265 7375 6c74 732e 2a2a 0a20 2020 2020  results.**.     
+000061c0: 2020 2063 6c69 636b 5f70 6f74 656e 7469     click_potenti
+000061d0: 616c 2028 676f 6f67 6c65 2e73 686f 7070  al (google.shopp
+000061e0: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+000061f0: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+00006200: 732e 5072 6f64 7563 7456 6965 772e 436c  s.ProductView.Cl
+00006210: 6963 6b50 6f74 656e 7469 616c 293a 0a20  ickPotential):. 
+00006220: 2020 2020 2020 2020 2020 2045 7374 696d             Estim
+00006230: 6174 6564 2070 6572 666f 726d 616e 6365  ated performance
+00006240: 2070 6f74 656e 7469 616c 2063 6f6d 7061   potential compa
+00006250: 7265 6420 746f 0a20 2020 2020 2020 2020  red to.         
+00006260: 2020 2068 6967 6865 7374 2070 6572 666f     highest perfo
+00006270: 726d 696e 6720 7072 6f64 7563 7473 206f  rming products o
+00006280: 6620 7468 6520 6d65 7263 6861 6e74 2e0a  f the merchant..
+00006290: 2020 2020 2020 2020 636c 6963 6b5f 706f          click_po
+000062a0: 7465 6e74 6961 6c5f 7261 6e6b 2028 696e  tential_rank (in
+000062b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000062c0: 5261 6e6b 206f 6620 7468 6520 7072 6f64  Rank of the prod
+000062d0: 7563 7420 6261 7365 6420 6f6e 2069 7473  uct based on its
+000062e0: 2063 6c69 636b 2070 6f74 656e 7469 616c   click potential
+000062f0: 2e20 4120 7072 6f64 7563 740a 2020 2020  . A product.    
+00006300: 2020 2020 2020 2020 7769 7468 2060 6063          with ``c
+00006310: 6c69 636b 5f70 6f74 656e 7469 616c 5f72  lick_potential_r
+00006320: 616e 6b60 6020 3120 6861 7320 7468 6520  ank`` 1 has the 
+00006330: 6869 6768 6573 7420 636c 6963 6b0a 2020  highest click.  
+00006340: 2020 2020 2020 2020 2020 706f 7465 6e74            potent
+00006350: 6961 6c20 616d 6f6e 6720 7468 6520 6d65  ial among the me
+00006360: 7263 6861 6e74 2773 2070 726f 6475 6374  rchant's product
+00006370: 7320 7468 6174 2066 756c 6669 6c6c 2074  s that fulfill t
+00006380: 6865 0a20 2020 2020 2020 2020 2020 2073  he.            s
+00006390: 6561 7263 6820 7175 6572 7920 636f 6e64  earch query cond
+000063a0: 6974 696f 6e73 2e0a 0a20 2020 2020 2020  itions...       
+000063b0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+000063c0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+000063d0: 6f6e 656f 6660 5f20 6060 5f63 6c69 636b  oneof`_ ``_click
+000063e0: 5f70 6f74 656e 7469 616c 5f72 616e 6b60  _potential_rank`
+000063f0: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
+00006400: 636c 6173 7320 4167 6772 6567 6174 6564  class Aggregated
+00006410: 5265 706f 7274 696e 6743 6f6e 7465 7874  ReportingContext
+00006420: 5374 6174 7573 2870 726f 746f 2e45 6e75  Status(proto.Enu
+00006430: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
+00006440: 5374 6174 7573 206f 6620 7468 6520 7072  Status of the pr
+00006450: 6f64 7563 7420 6167 6772 6567 6174 6564  oduct aggregated
+00006460: 2066 6f72 2061 6c6c 2072 6570 6f72 7469   for all reporti
+00006470: 6e67 2063 6f6e 7465 7874 732e 0a0a 2020  ng contexts...  
+00006480: 2020 2020 2020 4865 7265 2773 2061 6e20        Here's an 
+00006490: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
+000064a0: 6865 2061 6767 7265 6761 7465 6420 7374  he aggregated st
+000064b0: 6174 7573 2069 7320 636f 6d70 7574 6564  atus is computed
+000064c0: 3a0a 0a20 2020 2020 2020 2060 6060 0a20  :..        ```. 
+000064d0: 2020 2020 2020 2046 7265 6520 6c69 7374         Free list
+000064e0: 696e 6773 205c 7c20 5368 6f70 7069 6e67  ings \| Shopping
+000064f0: 2041 6473 205c 7c20 5374 6174 7573 0a20   Ads \| Status. 
+00006500: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00006510: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00006520: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00006530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006540: 2d2d 2d0a 2020 2020 2020 2020 4170 7072  ---.        Appr
+00006550: 6f76 6564 205c 7c20 4170 7072 6f76 6564  oved \| Approved
+00006560: 205c 7c20 454c 4947 4942 4c45 2041 7070   \| ELIGIBLE App
+00006570: 726f 7665 6420 5c7c 2050 656e 6469 6e67  roved \| Pending
+00006580: 205c 7c20 454c 4947 4942 4c45 0a20 2020   \| ELIGIBLE.   
+00006590: 2020 2020 2041 7070 726f 7665 6420 5c7c       Approved \|
+000065a0: 2044 6973 6170 7072 6f76 6564 205c 7c20   Disapproved \| 
+000065b0: 454c 4947 4942 4c45 5f4c 494d 4954 4544  ELIGIBLE_LIMITED
+000065c0: 2050 656e 6469 6e67 205c 7c20 5065 6e64   Pending \| Pend
+000065d0: 696e 6720 5c7c 0a20 2020 2020 2020 2050  ing \|.        P
+000065e0: 454e 4449 4e47 2044 6973 6170 7072 6f76  ENDING Disapprov
+000065f0: 6564 205c 7c20 4469 7361 7070 726f 7665  ed \| Disapprove
+00006600: 6420 5c7c 204e 4f54 5f45 4c49 4749 424c  d \| NOT_ELIGIBL
+00006610: 455f 4f52 5f44 4953 4150 5052 4f56 4544  E_OR_DISAPPROVED
+00006620: 0a20 2020 2020 2020 2060 6060 0a0a 2020  .        ```..  
+00006630: 2020 2020 2020 5661 6c75 6573 3a0a 2020        Values:.  
+00006640: 2020 2020 2020 2020 2020 4147 4752 4547            AGGREG
+00006650: 4154 4544 5f52 4550 4f52 5449 4e47 5f43  ATED_REPORTING_C
+00006660: 4f4e 5445 5854 5f53 5441 5455 535f 554e  ONTEXT_STATUS_UN
+00006670: 5350 4543 4946 4945 4420 2830 293a 0a20  SPECIFIED (0):. 
+00006680: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00006690: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
+000066a0: 2020 2020 2020 2020 2020 4e4f 545f 454c            NOT_EL
+000066b0: 4947 4942 4c45 5f4f 525f 4449 5341 5050  IGIBLE_OR_DISAPP
+000066c0: 524f 5645 4420 2831 293a 0a20 2020 2020  ROVED (1):.     
+000066d0: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
+000066e0: 6374 2069 7320 6e6f 7420 656c 6967 6962  ct is not eligib
+000066f0: 6c65 206f 7220 6973 2064 6973 6170 7072  le or is disappr
+00006700: 6f76 6564 2066 6f72 0a20 2020 2020 2020  oved for.       
+00006710: 2020 2020 2020 2020 2061 6c6c 2072 6570           all rep
+00006720: 6f72 7469 6e67 2063 6f6e 7465 7874 732e  orting contexts.
+00006730: 0a20 2020 2020 2020 2020 2020 2050 454e  .            PEN
+00006740: 4449 4e47 2028 3229 3a0a 2020 2020 2020  DING (2):.      
+00006750: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+00006760: 7427 7320 7374 6174 7573 2069 7320 7065  t's status is pe
+00006770: 6e64 696e 6720 696e 2061 6c6c 2072 6570  nding in all rep
+00006780: 6f72 7469 6e67 0a20 2020 2020 2020 2020  orting.         
+00006790: 2020 2020 2020 2063 6f6e 7465 7874 732e         contexts.
+000067a0: 0a20 2020 2020 2020 2020 2020 2045 4c49  .            ELI
+000067b0: 4749 424c 455f 4c49 4d49 5445 4420 2833  GIBLE_LIMITED (3
+000067c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000067d0: 2020 2050 726f 6475 6374 2069 7320 656c     Product is el
+000067e0: 6967 6962 6c65 2066 6f72 2073 6f6d 6520  igible for some 
+000067f0: 2862 7574 206e 6f74 2061 6c6c 290a 2020  (but not all).  
+00006800: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00006810: 706f 7274 696e 6720 636f 6e74 6578 7473  porting contexts
+00006820: 2e0a 2020 2020 2020 2020 2020 2020 454c  ..            EL
+00006830: 4947 4942 4c45 2028 3429 3a0a 2020 2020  IGIBLE (4):.    
+00006840: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+00006850: 7563 7420 6973 2065 6c69 6769 626c 6520  uct is eligible 
+00006860: 666f 7220 616c 6c20 7265 706f 7274 696e  for all reportin
+00006870: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00006880: 2020 636f 6e74 6578 7473 2e0a 2020 2020    contexts..    
+00006890: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000068a0: 4147 4752 4547 4154 4544 5f52 4550 4f52  AGGREGATED_REPOR
+000068b0: 5449 4e47 5f43 4f4e 5445 5854 5f53 5441  TING_CONTEXT_STA
+000068c0: 5455 535f 554e 5350 4543 4946 4945 4420  TUS_UNSPECIFIED 
+000068d0: 3d20 300a 2020 2020 2020 2020 4e4f 545f  = 0.        NOT_
+000068e0: 454c 4947 4942 4c45 5f4f 525f 4449 5341  ELIGIBLE_OR_DISA
+000068f0: 5050 524f 5645 4420 3d20 310a 2020 2020  PPROVED = 1.    
+00006900: 2020 2020 5045 4e44 494e 4720 3d20 320a      PENDING = 2.
+00006910: 2020 2020 2020 2020 454c 4947 4942 4c45          ELIGIBLE
+00006920: 5f4c 494d 4954 4544 203d 2033 0a20 2020  _LIMITED = 3.   
+00006930: 2020 2020 2045 4c49 4749 424c 4520 3d20       ELIGIBLE = 
+00006940: 340a 0a20 2020 2063 6c61 7373 2043 6c69  4..    class Cli
+00006950: 636b 506f 7465 6e74 6961 6c28 7072 6f74  ckPotential(prot
+00006960: 6f2e 456e 756d 293a 0a20 2020 2020 2020  o.Enum):.       
+00006970: 2072 2222 2241 2070 726f 6475 6374 2773   r"""A product's
+00006980: 2060 636c 6963 6b0a 2020 2020 2020 2020   `click.        
+00006990: 706f 7465 6e74 6961 6c20 3c68 7474 7073  potential <https
+000069a0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+000069b0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+000069c0: 616e 7377 6572 2f31 3838 3438 383e 605f  answer/188488>`_
+000069d0: 5f0a 2020 2020 2020 2020 6573 7469 6d61  _.        estima
+000069e0: 7465 7320 6974 7320 7065 7266 6f72 6d61  tes its performa
+000069f0: 6e63 6520 706f 7465 6e74 6961 6c20 636f  nce potential co
+00006a00: 6d70 6172 6564 2074 6f20 6869 6768 6573  mpared to highes
+00006a10: 7420 7065 7266 6f72 6d69 6e67 0a20 2020  t performing.   
+00006a20: 2020 2020 2070 726f 6475 6374 7320 6f66       products of
+00006a30: 2074 6865 206d 6572 6368 616e 742e 2043   the merchant. C
+00006a40: 6c69 636b 2070 6f74 656e 7469 616c 206f  lick potential o
+00006a50: 6620 6120 7072 6f64 7563 7420 6865 6c70  f a product help
+00006a60: 730a 2020 2020 2020 2020 6d65 7263 6861  s.        mercha
+00006a70: 6e74 7320 746f 2070 7269 6f72 6974 697a  nts to prioritiz
+00006a80: 6520 7768 6963 6820 7072 6f64 7563 7473  e which products
+00006a90: 2074 6f20 6669 7820 616e 6420 6865 6c70   to fix and help
+00006aa0: 7320 7468 656d 0a20 2020 2020 2020 2075  s them.        u
+00006ab0: 6e64 6572 7374 616e 6420 686f 7720 7072  nderstand how pr
+00006ac0: 6f64 7563 7473 2061 7265 2070 6572 666f  oducts are perfo
+00006ad0: 726d 696e 6720 6167 6169 6e73 7420 7468  rming against th
+00006ae0: 6569 7220 706f 7465 6e74 6961 6c2e 0a0a  eir potential...
+00006af0: 2020 2020 2020 2020 5661 6c75 6573 3a0a          Values:.
+00006b00: 2020 2020 2020 2020 2020 2020 434c 4943              CLIC
+00006b10: 4b5f 504f 5445 4e54 4941 4c5f 554e 5350  K_POTENTIAL_UNSP
+00006b20: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
+00006b30: 2020 2020 2020 2020 2020 2020 2055 6e6b               Unk
+00006b40: 6e6f 776e 2070 7265 6469 6374 6564 2063  nown predicted c
+00006b50: 6c69 636b 7320 696d 7061 6374 2e0a 2020  licks impact..  
+00006b60: 2020 2020 2020 2020 2020 4c4f 5720 2831            LOW (1
+00006b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006b80: 2020 2050 6f74 656e 7469 616c 2074 6f20     Potential to 
+00006b90: 7265 6365 6976 6520 6120 6c6f 7720 6e75  receive a low nu
+00006ba0: 6d62 6572 206f 6620 636c 6963 6b73 0a20  mber of clicks. 
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00006bc0: 6f6d 7061 7265 6420 746f 2074 6865 2068  ompared to the h
+00006bd0: 6967 6865 7374 2070 6572 666f 726d 696e  ighest performin
+00006be0: 6720 7072 6f64 7563 7473 206f 660a 2020  g products of.  
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00006c00: 6520 6d65 7263 6861 6e74 2e0a 2020 2020  e merchant..    
+00006c10: 2020 2020 2020 2020 4d45 4449 554d 2028          MEDIUM (
+00006c20: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
+00006c30: 2020 2020 506f 7465 6e74 6961 6c20 746f      Potential to
+00006c40: 2072 6563 6569 7665 2061 206d 6f64 6572   receive a moder
+00006c50: 6174 6520 6e75 6d62 6572 206f 660a 2020  ate number of.  
+00006c60: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00006c70: 6963 6b73 2063 6f6d 7061 7265 6420 746f  icks compared to
+00006c80: 2074 6865 2068 6967 6865 7374 2070 6572   the highest per
+00006c90: 666f 726d 696e 670a 2020 2020 2020 2020  forming.        
+00006ca0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
+00006cb0: 206f 6620 7468 6520 6d65 7263 6861 6e74   of the merchant
+00006cc0: 2e0a 2020 2020 2020 2020 2020 2020 4849  ..            HI
+00006cd0: 4748 2028 3329 3a0a 2020 2020 2020 2020  GH (3):.        
+00006ce0: 2020 2020 2020 2020 506f 7465 6e74 6961          Potentia
+00006cf0: 6c20 746f 2072 6563 6569 7665 2061 2073  l to receive a s
+00006d00: 696d 696c 6172 206e 756d 6265 7220 6f66  imilar number of
+00006d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d20: 2063 6c69 636b 7320 6173 2074 6865 2068   clicks as the h
+00006d30: 6967 6865 7374 2070 6572 666f 726d 696e  ighest performin
+00006d40: 6720 7072 6f64 7563 7473 206f 6620 7468  g products of th
+00006d50: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00006d60: 2020 6d65 7263 6861 6e74 2e0a 2020 2020    merchant..    
+00006d70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006d80: 434c 4943 4b5f 504f 5445 4e54 4941 4c5f  CLICK_POTENTIAL_
+00006d90: 554e 5350 4543 4946 4945 4420 3d20 300a  UNSPECIFIED = 0.
+00006da0: 2020 2020 2020 2020 4c4f 5720 3d20 310a          LOW = 1.
+00006db0: 2020 2020 2020 2020 4d45 4449 554d 203d          MEDIUM =
+00006dc0: 2032 0a20 2020 2020 2020 2048 4947 4820   2.        HIGH 
+00006dd0: 3d20 330a 0a20 2020 2063 6c61 7373 2049  = 3..    class I
+00006de0: 7465 6d49 7373 7565 2870 726f 746f 2e4d  temIssue(proto.M
+00006df0: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
+00006e00: 2072 2222 2249 7465 6d20 6973 7375 6520   r"""Item issue 
+00006e10: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00006e20: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
+00006e30: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
+00006e40: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
+00006e50: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
+00006e60: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+00006e70: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
+00006e80: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
+00006e90: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
+00006ea0: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+00006eb0: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
+00006ec0: 2020 7479 7065 5f20 2867 6f6f 676c 652e    type_ (google.
+00006ed0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
+00006ee0: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
+00006ef0: 2e74 7970 6573 2e50 726f 6475 6374 5669  .types.ProductVi
+00006f00: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
+00006f10: 6d49 7373 7565 5479 7065 293a 0a20 2020  mIssueType):.   
+00006f20: 2020 2020 2020 2020 2020 2020 2049 7465               Ite
+00006f30: 6d20 6973 7375 6520 7479 7065 2e0a 2020  m issue type..  
+00006f40: 2020 2020 2020 2020 2020 7365 7665 7269            severi
+00006f50: 7479 2028 676f 6f67 6c65 2e73 686f 7070  ty (google.shopp
+00006f60: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+00006f70: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+00006f80: 732e 5072 6f64 7563 7456 6965 772e 4974  s.ProductView.It
+00006f90: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
+00006fa0: 6553 6576 6572 6974 7929 3a0a 2020 2020  eSeverity):.    
+00006fb0: 2020 2020 2020 2020 2020 2020 4974 656d              Item
+00006fc0: 2069 7373 7565 2073 6576 6572 6974 792e   issue severity.
+00006fd0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00006fe0: 6f6c 7574 696f 6e20 2867 6f6f 676c 652e  olution (google.
+00006ff0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
+00007000: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
+00007010: 2e74 7970 6573 2e50 726f 6475 6374 5669  .types.ProductVi
+00007020: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
+00007030: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
+00007040: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007050: 2020 2049 7465 6d20 6973 7375 6520 7265     Item issue re
+00007060: 736f 6c75 7469 6f6e 2e0a 0a20 2020 2020  solution...     
+00007070: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00007080: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+00007090: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+000070a0: 5f72 6573 6f6c 7574 696f 6e60 602e 0a20  _resolution``.. 
+000070b0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000070c0: 2020 2020 636c 6173 7320 4974 656d 4973      class ItemIs
+000070d0: 7375 6552 6573 6f6c 7574 696f 6e28 7072  sueResolution(pr
+000070e0: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
+000070f0: 2020 2020 2020 2072 2222 2248 6f77 2074         r"""How t
+00007100: 6f20 7265 736f 6c76 6520 7468 6520 6973  o resolve the is
+00007110: 7375 652e 0a0a 2020 2020 2020 2020 2020  sue...          
+00007120: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
+00007130: 2020 2020 2020 2020 2020 4954 454d 5f49            ITEM_I
+00007140: 5353 5545 5f52 4553 4f4c 5554 494f 4e5f  SSUE_RESOLUTION_
+00007150: 554e 5350 4543 4946 4945 4420 2830 293a  UNSPECIFIED (0):
+00007160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007170: 2020 2020 204e 6f74 2073 7065 6369 6669       Not specifi
+00007180: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00007190: 2020 2020 4d45 5243 4841 4e54 5f41 4354      MERCHANT_ACT
+000071a0: 494f 4e20 2831 293a 0a20 2020 2020 2020  ION (1):.       
+000071b0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+000071c0: 206d 6572 6368 616e 7420 6861 7320 746f   merchant has to
+000071d0: 2066 6978 2074 6865 2069 7373 7565 2e0a   fix the issue..
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 5045 4e44 494e 475f 5052 4f43 4553 5349  PENDING_PROCESSI
+00007200: 4e47 2028 3229 3a0a 2020 2020 2020 2020  NG (2):.        
+00007210: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00007220: 6973 7375 6520 7769 6c6c 2062 6520 7265  issue will be re
+00007230: 736f 6c76 6564 2061 7574 6f6d 6174 6963  solved automatic
+00007240: 616c 6c79 2028 666f 720a 2020 2020 2020  ally (for.      
+00007250: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00007260: 616d 706c 652c 2069 6d61 6765 2063 7261  ample, image cra
+00007270: 776c 2920 6f72 2074 6872 6f75 6768 2061  wl) or through a
+00007280: 2047 6f6f 676c 650a 2020 2020 2020 2020   Google.        
+00007290: 2020 2020 2020 2020 2020 2020 7265 7669              revi
+000072a0: 6577 2e20 4e6f 206d 6572 6368 616e 7420  ew. No merchant 
+000072b0: 6163 7469 6f6e 2069 7320 7265 7175 6972  action is requir
+000072c0: 6564 206e 6f77 2e0a 2020 2020 2020 2020  ed now..        
+000072d0: 2020 2020 2020 2020 2020 2020 5265 736f              Reso
+000072e0: 6c75 7469 6f6e 206d 6967 6874 206c 6561  lution might lea
+000072f0: 6420 746f 2061 6e6f 7468 6572 2069 7373  d to another iss
+00007300: 7565 2028 666f 720a 2020 2020 2020 2020  ue (for.        
+00007310: 2020 2020 2020 2020 2020 2020 6578 616d              exam
+00007320: 706c 652c 2069 6620 6372 6177 6c20 6661  ple, if crawl fa
+00007330: 696c 7329 2e0a 2020 2020 2020 2020 2020  ils)..          
+00007340: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
+00007350: 2020 4954 454d 5f49 5353 5545 5f52 4553    ITEM_ISSUE_RES
+00007360: 4f4c 5554 494f 4e5f 554e 5350 4543 4946  OLUTION_UNSPECIF
+00007370: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
+00007380: 2020 2020 4d45 5243 4841 4e54 5f41 4354      MERCHANT_ACT
+00007390: 494f 4e20 3d20 310a 2020 2020 2020 2020  ION = 1.        
+000073a0: 2020 2020 5045 4e44 494e 475f 5052 4f43      PENDING_PROC
+000073b0: 4553 5349 4e47 203d 2032 0a0a 2020 2020  ESSING = 2..    
+000073c0: 2020 2020 636c 6173 7320 4974 656d 4973      class ItemIs
+000073d0: 7375 6554 7970 6528 7072 6f74 6f2e 4d65  sueType(proto.Me
+000073e0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
+000073f0: 2020 2020 7222 2222 4973 7375 6520 7479      r"""Issue ty
+00007400: 7065 2e0a 0a20 2020 2020 2020 2020 2020  pe...           
+00007410: 202e 2e20 5f6f 6e65 6f66 3a20 6874 7470   .. _oneof: http
+00007420: 733a 2f2f 7072 6f74 6f2d 706c 7573 2d70  s://proto-plus-p
+00007430: 7974 686f 6e2e 7265 6164 7468 6564 6f63  ython.readthedoc
+00007440: 732e 696f 2f65 6e2f 7374 6162 6c65 2f66  s.io/en/stable/f
+00007450: 6965 6c64 732e 6874 6d6c 236f 6e65 6f66  ields.html#oneof
+00007460: 732d 6d75 7475 616c 6c79 2d65 7863 6c75  s-mutually-exclu
+00007470: 7369 7665 2d66 6965 6c64 730a 0a20 2020  sive-fields..   
+00007480: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
+00007490: 7465 733a 0a20 2020 2020 2020 2020 2020  tes:.           
+000074a0: 2020 2020 2063 6f64 6520 2873 7472 293a       code (str):
+000074b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000074c0: 2020 2020 2045 7272 6f72 2063 6f64 6520       Error code 
+000074d0: 6f66 2074 6865 2069 7373 7565 2c20 6571  of the issue, eq
+000074e0: 7569 7661 6c65 6e74 2074 6f20 7468 6520  uivalent to the 
+000074f0: 6060 636f 6465 6060 206f 660a 2020 2020  ``code`` of.    
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 6050 726f 6475 6374 0a20 2020 2020 2020  `Product.       
+00007520: 2020 2020 2020 2020 2020 2020 2069 7373               iss
+00007530: 7565 7320 3c68 7474 7073 3a2f 2f64 6576  ues <https://dev
+00007540: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00007550: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00007560: 656e 742f 6775 6964 6573 2f70 726f 6475  ent/guides/produ
+00007570: 6374 2d69 7373 7565 733e 605f 5f2e 0a0a  ct-issues>`__...
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+000075a0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+000075b0: 6e65 6f66 605f 2060 605f 636f 6465 6060  neof`_ ``_code``
+000075c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000075d0: 2020 6361 6e6f 6e69 6361 6c5f 6174 7472    canonical_attr
+000075e0: 6962 7574 6520 2873 7472 293a 0a20 2020  ibute (str):.   
 000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 4973 7375 6520 6469 7361 7070 726f 7665  Issue disapprove
-00007610: 7320 7468 6520 7072 6f64 7563 7420 696e  s the product in
-00007620: 2061 7420 6c65 6173 7420 6f6e 650a 2020   at least one.  
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 2020 7265 706f 7274 696e 6720        reporting 
-00007650: 636f 6e74 6578 742e 0a20 2020 2020 2020  context..       
-00007660: 2020 2020 2020 2020 2020 2020 2044 454d               DEM
-00007670: 4f54 4544 2028 3229 3a0a 2020 2020 2020  OTED (2):.      
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 4973 7375 6520 6465 6d6f 7465 7320    Issue demotes 
-000076a0: 7468 6520 7072 6f64 7563 7420 696e 2061  the product in a
-000076b0: 6c6c 2072 6570 6f72 7469 6e67 0a20 2020  ll reporting.   
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2063 6f6e 7465 7874 7320 6974       contexts it
-000076e0: 2061 6666 6563 7473 2e0a 2020 2020 2020   affects..      
-000076f0: 2020 2020 2020 2020 2020 2020 2020 5045                PE
-00007700: 4e44 494e 4720 2833 293a 0a20 2020 2020  NDING (3):.     
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 2020 2049 7373 7565 2072 6573 6f6c 7574     Issue resolut
-00007730: 696f 6e20 6973 2060 6050 454e 4449 4e47  ion is ``PENDING
-00007740: 5f50 524f 4345 5353 494e 4760 602e 0a20  _PROCESSING``.. 
-00007750: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007760: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-00007770: 2020 2041 4747 5245 4741 5445 445f 4953     AGGREGATED_IS
-00007780: 5355 455f 5345 5645 5249 5459 5f55 4e53  SUE_SEVERITY_UNS
-00007790: 5045 4349 4649 4544 203d 2030 0a20 2020  PECIFIED = 0.   
-000077a0: 2020 2020 2020 2020 2020 2020 2044 4953               DIS
-000077b0: 4150 5052 4f56 4544 203d 2031 0a20 2020  APPROVED = 1.   
-000077c0: 2020 2020 2020 2020 2020 2020 2044 454d               DEM
-000077d0: 4f54 4544 203d 2032 0a20 2020 2020 2020  OTED = 2.       
-000077e0: 2020 2020 2020 2020 2050 454e 4449 4e47           PENDING
-000077f0: 203d 2033 0a0a 2020 2020 2020 2020 2020   = 3..          
-00007800: 2020 636c 6173 7320 4973 7375 6553 6576    class IssueSev
-00007810: 6572 6974 7950 6572 5265 706f 7274 696e  erityPerReportin
-00007820: 6743 6f6e 7465 7874 2870 726f 746f 2e4d  gContext(proto.M
-00007830: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-00007840: 2020 2020 2020 2020 2072 2222 2249 7373           r"""Iss
-00007850: 7565 2073 6576 6572 6974 7920 7065 7220  ue severity per 
-00007860: 7265 706f 7274 696e 6720 636f 6e74 6578  reporting contex
-00007870: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00007880: 2020 2020 2e2e 205f 6f6e 656f 663a 2068      .. _oneof: h
-00007890: 7474 7073 3a2f 2f70 726f 746f 2d70 6c75  ttps://proto-plu
-000078a0: 732d 7079 7468 6f6e 2e72 6561 6474 6865  s-python.readthe
-000078b0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-000078c0: 652f 6669 656c 6473 2e68 746d 6c23 6f6e  e/fields.html#on
-000078d0: 656f 6673 2d6d 7574 7561 6c6c 792d 6578  eofs-mutually-ex
-000078e0: 636c 7573 6976 652d 6669 656c 6473 0a0a  clusive-fields..
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007900: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 7265 706f 7274 696e 675f 636f 6e74 6578  reporting_contex
-00007930: 7420 2867 6f6f 676c 652e 7368 6f70 7069  t (google.shoppi
-00007940: 6e67 2e74 7970 652e 7479 7065 732e 5265  ng.type.types.Re
-00007950: 706f 7274 696e 6743 6f6e 7465 7874 2e52  portingContext.R
-00007960: 6570 6f72 7469 6e67 436f 6e74 6578 7445  eportingContextE
-00007970: 6e75 6d29 3a0a 2020 2020 2020 2020 2020  num):.          
-00007980: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-00007990: 706f 7274 696e 6720 636f 6e74 6578 7420  porting context 
-000079a0: 7468 6520 6973 7375 6520 6170 706c 6965  the issue applie
-000079b0: 7320 746f 2e0a 0a20 2020 2020 2020 2020  s to...         
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000079d0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000079e0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-000079f0: 5f20 6060 5f72 6570 6f72 7469 6e67 5f63  _ ``_reporting_c
-00007a00: 6f6e 7465 7874 6060 2e0a 2020 2020 2020  ontext``..      
-00007a10: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00007a20: 7361 7070 726f 7665 645f 636f 756e 7472  sapproved_countr
-00007a30: 6965 7320 284d 7574 6162 6c65 5365 7175  ies (MutableSequ
-00007a40: 656e 6365 5b73 7472 5d29 3a0a 2020 2020  ence[str]):.    
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 4c69 7374 206f 6620 6469 7361      List of disa
-00007a70: 7070 726f 7665 6420 636f 756e 7472 6965  pproved countrie
-00007a80: 7320 696e 2074 6865 0a20 2020 2020 2020  s in the.       
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007aa0: 2072 6570 6f72 7469 6e67 2063 6f6e 7465   reporting conte
-00007ab0: 7874 2c20 7265 7072 6573 656e 7465 6420  xt, represented 
-00007ac0: 696e 2049 534f 2033 3136 360a 2020 2020  in ISO 3166.    
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 666f 726d 6174 2e0a 2020 2020      format..    
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 6465 6d6f 7465 645f 636f 756e 7472 6965  demoted_countrie
-00007b10: 7320 284d 7574 6162 6c65 5365 7175 656e  s (MutableSequen
-00007b20: 6365 5b73 7472 5d29 3a0a 2020 2020 2020  ce[str]):.      
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 2020 4c69 7374 206f 6620 6465 6d6f 7465    List of demote
-00007b50: 6420 636f 756e 7472 6965 7320 696e 2074  d countries in t
-00007b60: 6865 2072 6570 6f72 7469 6e67 0a20 2020  he reporting.   
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 2020 2063 6f6e 7465 7874 2c20 7265       context, re
-00007b90: 7072 6573 656e 7465 6420 696e 2049 534f  presented in ISO
-00007ba0: 2033 3136 3620 666f 726d 6174 2e0a 2020   3166 format..  
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
-00007bc0: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
-00007bd0: 2020 2072 6570 6f72 7469 6e67 5f63 6f6e     reporting_con
-00007be0: 7465 7874 3a20 7479 7065 732e 5265 706f  text: types.Repo
-00007bf0: 7274 696e 6743 6f6e 7465 7874 2e52 6570  rtingContext.Rep
-00007c00: 6f72 7469 6e67 436f 6e74 6578 7445 6e75  ortingContextEnu
-00007c10: 6d20 3d20 280a 2020 2020 2020 2020 2020  m = (.          
-00007c20: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-00007c30: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007c50: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
+00007600: 2043 616e 6f6e 6963 616c 2061 7474 7269   Canonical attri
+00007610: 6275 7465 206e 616d 6520 666f 720a 2020  bute name for.  
+00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007630: 2020 6174 7472 6962 7574 652d 7370 6563    attribute-spec
+00007640: 6966 6963 2069 7373 7565 732e 0a0a 2020  ific issues...  
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00007670: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00007680: 6f66 605f 2060 605f 6361 6e6f 6e69 6361  of`_ ``_canonica
+00007690: 6c5f 6174 7472 6962 7574 6560 602e 0a20  l_attribute``.. 
+000076a0: 2020 2020 2020 2020 2020 2022 2222 0a0a             """..
+000076b0: 2020 2020 2020 2020 2020 2020 636f 6465              code
+000076c0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000076d0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000076e0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+000076f0: 472c 0a20 2020 2020 2020 2020 2020 2020  G,.             
+00007700: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
+00007710: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00007720: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00007730: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00007740: 2020 2020 2020 6361 6e6f 6e69 6361 6c5f        canonical_
+00007750: 6174 7472 6962 7574 653a 2073 7472 203d  attribute: str =
+00007760: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00007770: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00007780: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00007790: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+000077a0: 6572 3d32 2c0a 2020 2020 2020 2020 2020  er=2,.          
+000077b0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000077c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000077d0: 2029 0a0a 2020 2020 2020 2020 636c 6173   )..        clas
+000077e0: 7320 4974 656d 4973 7375 6553 6576 6572  s ItemIssueSever
+000077f0: 6974 7928 7072 6f74 6f2e 4d65 7373 6167  ity(proto.Messag
+00007800: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00007810: 7222 2222 486f 7720 7468 6520 6973 7375  r"""How the issu
+00007820: 6520 6166 6665 6374 7320 7468 6520 7365  e affects the se
+00007830: 7276 696e 6720 6f66 2074 6865 2070 726f  rving of the pro
+00007840: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
+00007850: 2020 202e 2e20 5f6f 6e65 6f66 3a20 6874     .. _oneof: ht
+00007860: 7470 733a 2f2f 7072 6f74 6f2d 706c 7573  tps://proto-plus
+00007870: 2d70 7974 686f 6e2e 7265 6164 7468 6564  -python.readthed
+00007880: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
+00007890: 2f66 6965 6c64 732e 6874 6d6c 236f 6e65  /fields.html#one
+000078a0: 6f66 732d 6d75 7475 616c 6c79 2d65 7863  ofs-mutually-exc
+000078b0: 6c75 7369 7665 2d66 6965 6c64 730a 0a20  lusive-fields.. 
+000078c0: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
+000078d0: 6275 7465 733a 0a20 2020 2020 2020 2020  butes:.         
+000078e0: 2020 2020 2020 2073 6576 6572 6974 795f         severity_
+000078f0: 7065 725f 7265 706f 7274 696e 675f 636f  per_reporting_co
+00007900: 6e74 6578 7420 284d 7574 6162 6c65 5365  ntext (MutableSe
+00007910: 7175 656e 6365 5b67 6f6f 676c 652e 7368  quence[google.sh
+00007920: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+00007930: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+00007940: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
+00007950: 2e49 7465 6d49 7373 7565 2e49 7465 6d49  .ItemIssue.ItemI
+00007960: 7373 7565 5365 7665 7269 7479 2e49 7373  ssueSeverity.Iss
+00007970: 7565 5365 7665 7269 7479 5065 7252 6570  ueSeverityPerRep
+00007980: 6f72 7469 6e67 436f 6e74 6578 745d 293a  ortingContext]):
+00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000079a0: 2020 2020 2049 7373 7565 2073 6576 6572       Issue sever
+000079b0: 6974 7920 7065 7220 7265 706f 7274 696e  ity per reportin
+000079c0: 6720 636f 6e74 6578 742e 0a20 2020 2020  g context..     
+000079d0: 2020 2020 2020 2020 2020 2061 6767 7265             aggre
+000079e0: 6761 7465 645f 7365 7665 7269 7479 2028  gated_severity (
+000079f0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+00007a00: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
+00007a10: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
+00007a20: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
+00007a30: 7375 652e 4974 656d 4973 7375 6553 6576  sue.ItemIssueSev
+00007a40: 6572 6974 792e 4167 6772 6567 6174 6564  erity.Aggregated
+00007a50: 4973 7375 6553 6576 6572 6974 7929 3a0a  IssueSeverity):.
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 2020 4167 6772 6567 6174 6564 2073      Aggregated s
+00007a80: 6576 6572 6974 7920 6f66 2074 6865 2069  everity of the i
+00007a90: 7373 7565 2066 6f72 2061 6c6c 2072 6570  ssue for all rep
+00007aa0: 6f72 7469 6e67 2063 6f6e 7465 7874 730a  orting contexts.
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2020 2020 6974 2061 6666 6563 7473 2e0a      it affects..
+00007ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ae0: 2020 2020 202a 2a54 6869 7320 6669 656c       **This fiel
+00007af0: 6420 6361 6e20 6265 2075 7365 6420 666f  d can be used fo
+00007b00: 7220 6669 6c74 6572 696e 6720 7468 6520  r filtering the 
+00007b10: 7265 7375 6c74 732e 2a2a 0a0a 2020 2020  results.**..    
+00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b30: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00007b40: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00007b50: 605f 2060 605f 6167 6772 6567 6174 6564  `_ ``_aggregated
+00007b60: 5f73 6576 6572 6974 7960 602e 0a20 2020  _severity``..   
+00007b70: 2020 2020 2020 2020 2022 2222 0a0a 2020           """..  
+00007b80: 2020 2020 2020 2020 2020 636c 6173 7320            class 
+00007b90: 4167 6772 6567 6174 6564 4973 7375 6553  AggregatedIssueS
+00007ba0: 6576 6572 6974 7928 7072 6f74 6f2e 456e  everity(proto.En
+00007bb0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+00007bc0: 2020 2020 2072 2222 2249 7373 7565 2073       r"""Issue s
+00007bd0: 6576 6572 6974 7920 6167 6772 6567 6174  everity aggregat
+00007be0: 6564 2066 6f72 2061 6c6c 2072 6570 6f72  ed for all repor
+00007bf0: 7469 6e67 2063 6f6e 7465 7874 732e 0a0a  ting contexts...
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
+00007c20: 2020 2020 2020 2020 2020 2020 4147 4752              AGGR
+00007c30: 4547 4154 4544 5f49 5353 5545 5f53 4556  EGATED_ISSUE_SEV
+00007c40: 4552 4954 595f 554e 5350 4543 4946 4945  ERITY_UNSPECIFIE
+00007c50: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
+00007c60: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00007c70: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
 00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00007ca0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00007cb0: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-00007cc0: 3d74 7970 6573 2e52 6570 6f72 7469 6e67  =types.Reporting
-00007cd0: 436f 6e74 6578 742e 5265 706f 7274 696e  Context.Reportin
-00007ce0: 6743 6f6e 7465 7874 456e 756d 2c0a 2020  gContextEnum,.  
+00007c90: 2020 4449 5341 5050 524f 5645 4420 2831    DISAPPROVED (1
+00007ca0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007cb0: 2020 2020 2020 2020 2020 2049 7373 7565             Issue
+00007cc0: 2064 6973 6170 7072 6f76 6573 2074 6865   disapproves the
+00007cd0: 2070 726f 6475 6374 2069 6e20 6174 206c   product in at l
+00007ce0: 6561 7374 206f 6e65 0a20 2020 2020 2020  east one.       
 00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00007d10: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00007d20: 2020 2020 2020 6469 7361 7070 726f 7665        disapprove
-00007d30: 645f 636f 756e 7472 6965 733a 204d 7574  d_countries: Mut
-00007d40: 6162 6c65 5365 7175 656e 6365 5b73 7472  ableSequence[str
-00007d50: 5d20 3d20 7072 6f74 6f2e 5265 7065 6174  ] = proto.Repeat
-00007d60: 6564 4669 656c 6428 0a20 2020 2020 2020  edField(.       
-00007d70: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-00007d80: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-00007d90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00007da0: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-00007db0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00007dc0: 2020 2020 2020 2020 2020 2064 656d 6f74             demot
-00007dd0: 6564 5f63 6f75 6e74 7269 6573 3a20 4d75  ed_countries: Mu
-00007de0: 7461 626c 6553 6571 7565 6e63 655b 7374  tableSequence[st
-00007df0: 725d 203d 2070 726f 746f 2e52 6570 6561  r] = proto.Repea
-00007e00: 7465 6446 6965 6c64 280a 2020 2020 2020  tedField(.      
-00007e10: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00007e20: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 6e75 6d62 6572 3d33 2c0a 2020 2020 2020  number=3,.      
-00007e50: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00007e60: 2020 2020 2020 2020 2073 6576 6572 6974           severit
-00007e70: 795f 7065 725f 7265 706f 7274 696e 675f  y_per_reporting_
-00007e80: 636f 6e74 6578 743a 204d 7574 6162 6c65  context: Mutable
-00007e90: 5365 7175 656e 6365 5b0a 2020 2020 2020  Sequence[.      
-00007ea0: 2020 2020 2020 2020 2020 2250 726f 6475            "Produ
-00007eb0: 6374 5669 6577 2e49 7465 6d49 7373 7565  ctView.ItemIssue
-00007ec0: 2e49 7465 6d49 7373 7565 5365 7665 7269  .ItemIssueSeveri
-00007ed0: 7479 2e49 7373 7565 5365 7665 7269 7479  ty.IssueSeverity
-00007ee0: 5065 7252 6570 6f72 7469 6e67 436f 6e74  PerReportingCont
-00007ef0: 6578 7422 0a20 2020 2020 2020 2020 2020  ext".           
-00007f00: 205d 203d 2070 726f 746f 2e52 6570 6561   ] = proto.Repea
-00007f10: 7465 6446 6965 6c64 280a 2020 2020 2020  tedField(.      
-00007f20: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-00007f30: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-00007f40: 2020 2020 2020 2020 206e 756d 6265 723d           number=
-00007f50: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00007f60: 2020 206d 6573 7361 6765 3d22 5072 6f64     message="Prod
-00007f70: 7563 7456 6965 772e 4974 656d 4973 7375  uctView.ItemIssu
-00007f80: 652e 4974 656d 4973 7375 6553 6576 6572  e.ItemIssueSever
-00007f90: 6974 792e 4973 7375 6553 6576 6572 6974  ity.IssueSeverit
-00007fa0: 7950 6572 5265 706f 7274 696e 6743 6f6e  yPerReportingCon
-00007fb0: 7465 7874 222c 0a20 2020 2020 2020 2020  text",.         
-00007fc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00007fd0: 2061 6767 7265 6761 7465 645f 7365 7665   aggregated_seve
-00007fe0: 7269 7479 3a20 2250 726f 6475 6374 5669  rity: "ProductVi
-00007ff0: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-00008000: 6d49 7373 7565 5365 7665 7269 7479 2e41  mIssueSeverity.A
-00008010: 6767 7265 6761 7465 6449 7373 7565 5365  ggregatedIssueSe
-00008020: 7665 7269 7479 2220 3d20 7072 6f74 6f2e  verity" = proto.
-00008030: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
-00008040: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-00008050: 4d2c 0a20 2020 2020 2020 2020 2020 2020  M,.             
-00008060: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
-00008070: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-00008080: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00008090: 2020 2020 2020 2020 2020 2020 656e 756d              enum
-000080a0: 3d22 5072 6f64 7563 7456 6965 772e 4974  ="ProductView.It
-000080b0: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
-000080c0: 6553 6576 6572 6974 792e 4167 6772 6567  eSeverity.Aggreg
-000080d0: 6174 6564 4973 7375 6553 6576 6572 6974  atedIssueSeverit
-000080e0: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
-000080f0: 290a 0a20 2020 2020 2020 2074 7970 655f  )..        type_
-00008100: 3a20 2250 726f 6475 6374 5669 6577 2e49  : "ProductView.I
-00008110: 7465 6d49 7373 7565 2e49 7465 6d49 7373  temIssue.ItemIss
-00008120: 7565 5479 7065 2220 3d20 7072 6f74 6f2e  ueType" = proto.
-00008130: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
-00008140: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
-00008150: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-00008160: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
-00008170: 2020 2020 6d65 7373 6167 653d 2250 726f      message="Pro
-00008180: 6475 6374 5669 6577 2e49 7465 6d49 7373  ductView.ItemIss
-00008190: 7565 2e49 7465 6d49 7373 7565 5479 7065  ue.ItemIssueType
-000081a0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-000081b0: 2020 2020 2073 6576 6572 6974 793a 2022       severity: "
-000081c0: 5072 6f64 7563 7456 6965 772e 4974 656d  ProductView.Item
-000081d0: 4973 7375 652e 4974 656d 4973 7375 6553  Issue.ItemIssueS
-000081e0: 6576 6572 6974 7922 203d 2070 726f 746f  everity" = proto
-000081f0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00008200: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00008210: 452c 0a20 2020 2020 2020 2020 2020 206e  E,.            n
-00008220: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-00008230: 2020 2020 206d 6573 7361 6765 3d22 5072       message="Pr
-00008240: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
-00008250: 7375 652e 4974 656d 4973 7375 6553 6576  sue.ItemIssueSev
-00008260: 6572 6974 7922 2c0a 2020 2020 2020 2020  erity",.        
-00008270: 290a 2020 2020 2020 2020 7265 736f 6c75  ).        resolu
-00008280: 7469 6f6e 3a20 2250 726f 6475 6374 5669  tion: "ProductVi
-00008290: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-000082a0: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
-000082b0: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
-000082c0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-000082d0: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
-000082e0: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
-000082f0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00008300: 6e61 6c3d 5472 7565 2c0a 2020 2020 2020  nal=True,.      
-00008310: 2020 2020 2020 656e 756d 3d22 5072 6f64        enum="Prod
-00008320: 7563 7456 6965 772e 4974 656d 4973 7375  uctView.ItemIssu
-00008330: 652e 4974 656d 4973 7375 6552 6573 6f6c  e.ItemIssueResol
-00008340: 7574 696f 6e22 2c0a 2020 2020 2020 2020  ution",.        
-00008350: 290a 0a20 2020 2069 643a 2073 7472 203d  )..    id: str =
-00008360: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00008370: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00008380: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00008390: 6572 3d31 2c0a 2020 2020 2020 2020 6f70  er=1,.        op
-000083a0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-000083b0: 2029 0a20 2020 2063 6861 6e6e 656c 3a20   ).    channel: 
-000083c0: 7479 7065 732e 4368 616e 6e65 6c2e 4368  types.Channel.Ch
-000083d0: 616e 6e65 6c45 6e75 6d20 3d20 7072 6f74  annelEnum = prot
-000083e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000083f0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00008400: 2020 2020 206e 756d 6265 723d 3238 2c0a       number=28,.
-00008410: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00008420: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
-00008430: 6e75 6d3d 7479 7065 732e 4368 616e 6e65  num=types.Channe
-00008440: 6c2e 4368 616e 6e65 6c45 6e75 6d2c 0a20  l.ChannelEnum,. 
-00008450: 2020 2029 0a20 2020 206c 616e 6775 6167     ).    languag
-00008460: 655f 636f 6465 3a20 7374 7220 3d20 7072  e_code: str = pr
-00008470: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00008480: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00008490: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-000084a0: 322c 0a20 2020 2020 2020 206f 7074 696f  2,.        optio
-000084b0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-000084c0: 2020 2020 6665 6564 5f6c 6162 656c 3a20      feed_label: 
-000084d0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-000084e0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-000084f0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-00008500: 206e 756d 6265 723d 332c 0a20 2020 2020   number=3,.     
-00008510: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00008520: 2c0a 2020 2020 290a 2020 2020 6f66 6665  ,.    ).    offe
-00008530: 725f 6964 3a20 7374 7220 3d20 7072 6f74  r_id: str = prot
-00008540: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00008550: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00008560: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
-00008570: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00008580: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00008590: 2020 7469 746c 653a 2073 7472 203d 2070    title: str = p
-000085a0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000085b0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-000085c0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-000085d0: 3d35 2c0a 2020 2020 2020 2020 6f70 7469  =5,.        opti
-000085e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-000085f0: 0a20 2020 2062 7261 6e64 3a20 7374 7220  .    brand: str 
-00008600: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00008610: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00008620: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00008630: 6265 723d 362c 0a20 2020 2020 2020 206f  ber=6,.        o
-00008640: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00008650: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-00008660: 5f6c 313a 2073 7472 203d 2070 726f 746f  _l1: str = proto
-00008670: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00008680: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00008690: 2020 2020 2020 6e75 6d62 6572 3d37 2c0a        number=7,.
-000086a0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-000086b0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-000086c0: 2063 6174 6567 6f72 795f 6c32 3a20 7374   category_l2: st
-000086d0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-000086e0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-000086f0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00008700: 756d 6265 723d 382c 0a20 2020 2020 2020  umber=8,.       
-00008710: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00008720: 2020 2020 290a 2020 2020 6361 7465 676f      ).    catego
-00008730: 7279 5f6c 333a 2073 7472 203d 2070 726f  ry_l3: str = pro
-00008740: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00008750: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-00008760: 2020 2020 2020 2020 6e75 6d62 6572 3d39          number=9
-00008770: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00008780: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00008790: 2020 2063 6174 6567 6f72 795f 6c34 3a20     category_l4: 
-000087a0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-000087b0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-000087c0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-000087d0: 206e 756d 6265 723d 3130 2c0a 2020 2020   number=10,.    
-000087e0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-000087f0: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
-00008800: 6567 6f72 795f 6c35 3a20 7374 7220 3d20  egory_l5: str = 
-00008810: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00008820: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00008830: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00008840: 723d 3131 2c0a 2020 2020 2020 2020 6f70  r=11,.        op
-00008850: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00008860: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
-00008870: 7970 655f 6c31 3a20 7374 7220 3d20 7072  ype_l1: str = pr
-00008880: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00008890: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-000088a0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-000088b0: 3132 2c0a 2020 2020 2020 2020 6f70 7469  12,.        opti
-000088c0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-000088d0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
-000088e0: 655f 6c32 3a20 7374 7220 3d20 7072 6f74  e_l2: str = prot
-000088f0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00008900: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00008910: 2020 2020 2020 206e 756d 6265 723d 3133         number=13
-00008920: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00008930: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00008940: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
-00008950: 6c33 3a20 7374 7220 3d20 7072 6f74 6f2e  l3: str = proto.
-00008960: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00008970: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00008980: 2020 2020 206e 756d 6265 723d 3134 2c0a       number=14,.
-00008990: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-000089a0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-000089b0: 2070 726f 6475 6374 5f74 7970 655f 6c34   product_type_l4
-000089c0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-000089d0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-000089e0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-000089f0: 2020 206e 756d 6265 723d 3135 2c0a 2020     number=15,.  
-00008a00: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-00008a10: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
-00008a20: 726f 6475 6374 5f74 7970 655f 6c35 3a20  roduct_type_l5: 
-00008a30: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-00008a40: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00008a50: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-00008a60: 206e 756d 6265 723d 3136 2c0a 2020 2020   number=16,.    
-00008a70: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00008a80: 652c 0a20 2020 2029 0a20 2020 2070 7269  e,.    ).    pri
-00008a90: 6365 3a20 7479 7065 732e 5072 6963 6520  ce: types.Price 
-00008aa0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00008ab0: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00008ac0: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00008ad0: 6d62 6572 3d31 372c 0a20 2020 2020 2020  mber=17,.       
-00008ae0: 206d 6573 7361 6765 3d74 7970 6573 2e50   message=types.P
-00008af0: 7269 6365 2c0a 2020 2020 290a 2020 2020  rice,.    ).    
-00008b00: 636f 6e64 6974 696f 6e3a 2073 7472 203d  condition: str =
-00008b10: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00008b20: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00008b30: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00008b40: 6572 3d31 382c 0a20 2020 2020 2020 206f  er=18,.        o
-00008b50: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00008b60: 2020 290a 2020 2020 6176 6169 6c61 6269    ).    availabi
-00008b70: 6c69 7479 3a20 7374 7220 3d20 7072 6f74  lity: str = prot
-00008b80: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00008b90: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00008ba0: 2020 2020 2020 206e 756d 6265 723d 3139         number=19
-00008bb0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00008bc0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00008bd0: 2020 2073 6869 7070 696e 675f 6c61 6265     shipping_labe
-00008be0: 6c3a 2073 7472 203d 2070 726f 746f 2e46  l: str = proto.F
-00008bf0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00008c00: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-00008c10: 2020 2020 6e75 6d62 6572 3d32 302c 0a20      number=20,. 
-00008c20: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00008c30: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-00008c40: 6774 696e 3a20 4d75 7461 626c 6553 6571  gtin: MutableSeq
-00008c50: 7565 6e63 655b 7374 725d 203d 2070 726f  uence[str] = pro
-00008c60: 746f 2e52 6570 6561 7465 6446 6965 6c64  to.RepeatedField
-00008c70: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00008c80: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00008c90: 6e75 6d62 6572 3d32 312c 0a20 2020 2029  number=21,.    )
-00008ca0: 0a20 2020 2069 7465 6d5f 6772 6f75 705f  .    item_group_
-00008cb0: 6964 3a20 7374 7220 3d20 7072 6f74 6f2e  id: str = proto.
-00008cc0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00008cd0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00008ce0: 2020 2020 206e 756d 6265 723d 3232 2c0a       number=22,.
-00008cf0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00008d00: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-00008d10: 2074 6875 6d62 6e61 696c 5f6c 696e 6b3a   thumbnail_link:
-00008d20: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00008d30: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008d40: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00008d50: 2020 6e75 6d62 6572 3d32 332c 0a20 2020    number=23,.   
-00008d60: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00008d70: 7565 2c0a 2020 2020 290a 2020 2020 6372  ue,.    ).    cr
-00008d80: 6561 7469 6f6e 5f74 696d 653a 2074 696d  eation_time: tim
-00008d90: 6573 7461 6d70 5f70 6232 2e54 696d 6573  estamp_pb2.Times
-00008da0: 7461 6d70 203d 2070 726f 746f 2e46 6965  tamp = proto.Fie
-00008db0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008dc0: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00008dd0: 2020 206e 756d 6265 723d 3234 2c0a 2020     number=24,.  
-00008de0: 2020 2020 2020 6d65 7373 6167 653d 7469        message=ti
-00008df0: 6d65 7374 616d 705f 7062 322e 5469 6d65  mestamp_pb2.Time
-00008e00: 7374 616d 702c 0a20 2020 2029 0a20 2020  stamp,.    ).   
-00008e10: 2065 7870 6972 6174 696f 6e5f 6461 7465   expiration_date
-00008e20: 3a20 6461 7465 5f70 6232 2e44 6174 6520  : date_pb2.Date 
-00008e30: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00008e40: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00008e50: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00008e60: 6d62 6572 3d32 352c 0a20 2020 2020 2020  mber=25,.       
-00008e70: 206d 6573 7361 6765 3d64 6174 655f 7062   message=date_pb
-00008e80: 322e 4461 7465 2c0a 2020 2020 290a 2020  2.Date,.    ).  
-00008e90: 2020 6167 6772 6567 6174 6564 5f72 6570    aggregated_rep
-00008ea0: 6f72 7469 6e67 5f63 6f6e 7465 7874 5f73  orting_context_s
-00008eb0: 7461 7475 733a 2041 6767 7265 6761 7465  tatus: Aggregate
-00008ec0: 6452 6570 6f72 7469 6e67 436f 6e74 6578  dReportingContex
-00008ed0: 7453 7461 7475 7320 3d20 7072 6f74 6f2e  tStatus = proto.
-00008ee0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00008ef0: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
-00008f00: 2020 206e 756d 6265 723d 3236 2c0a 2020     number=26,.  
-00008f10: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-00008f20: 7275 652c 0a20 2020 2020 2020 2065 6e75  rue,.        enu
-00008f30: 6d3d 4167 6772 6567 6174 6564 5265 706f  m=AggregatedRepo
-00008f40: 7274 696e 6743 6f6e 7465 7874 5374 6174  rtingContextStat
-00008f50: 7573 2c0a 2020 2020 290a 2020 2020 6974  us,.    ).    it
-00008f60: 656d 5f69 7373 7565 733a 204d 7574 6162  em_issues: Mutab
-00008f70: 6c65 5365 7175 656e 6365 5b49 7465 6d49  leSequence[ItemI
-00008f80: 7373 7565 5d20 3d20 7072 6f74 6f2e 5265  ssue] = proto.Re
-00008f90: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
-00008fa0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-00008fb0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-00008fc0: 6572 3d32 372c 0a20 2020 2020 2020 206d  er=27,.        m
-00008fd0: 6573 7361 6765 3d49 7465 6d49 7373 7565  essage=ItemIssue
-00008fe0: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
-00008ff0: 5072 6963 6543 6f6d 7065 7469 7469 7665  PriceCompetitive
-00009000: 6e65 7373 5072 6f64 7563 7456 6965 7728  nessProductView(
-00009010: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
-00009020: 2020 2020 7222 2222 4669 656c 6473 2061      r"""Fields a
-00009030: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
-00009040: 7279 2069 6e20 6060 7072 6963 655f 636f  ry in ``price_co
-00009050: 6d70 6574 6974 6976 656e 6573 735f 7072  mpetitiveness_pr
-00009060: 6f64 7563 745f 7669 6577 6060 0a20 2020  oduct_view``.   
-00009070: 2074 6162 6c65 2e0a 0a20 2020 2060 5072   table...    `Pr
-00009080: 6963 650a 2020 2020 636f 6d70 6574 6974  ice.    competit
-00009090: 6976 656e 6573 7320 3c68 7474 7073 3a2f  iveness <https:/
-000090a0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-000090b0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-000090c0: 7377 6572 2f39 3632 3639 3033 3e60 5f5f  swer/9626903>`__
-000090d0: 0a20 2020 2072 6570 6f72 742e 0a0a 2020  .    report...  
-000090e0: 2020 5661 6c75 6573 2061 7265 206f 6e6c    Values are onl
-000090f0: 7920 7365 7420 666f 7220 6669 656c 6473  y set for fields
-00009100: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
-00009110: 6369 746c 7920 696e 2074 6865 2072 6571  citly in the req
-00009120: 7565 7374 2773 0a20 2020 2073 6561 7263  uest's.    searc
-00009130: 6820 7175 6572 792e 0a0a 0a20 2020 202e  h query....    .
-00009140: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
-00009150: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
-00009160: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
-00009170: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
-00009180: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
-00009190: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
-000091a0: 7665 2d66 6965 6c64 730a 0a20 2020 2041  ve-fields..    A
-000091b0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-000091c0: 2020 2072 6570 6f72 745f 636f 756e 7472     report_countr
-000091d0: 795f 636f 6465 2028 7374 7229 3a0a 2020  y_code (str):.  
-000091e0: 2020 2020 2020 2020 2020 436f 756e 7472            Countr
-000091f0: 7920 6f66 2074 6865 2070 7269 6365 2062  y of the price b
-00009200: 656e 6368 6d61 726b 2e20 5265 7072 6573  enchmark. Repres
-00009210: 656e 7465 6420 696e 2074 6865 2049 534f  ented in the ISO
-00009220: 2033 3136 360a 2020 2020 2020 2020 2020   3166.          
-00009230: 2020 666f 726d 6174 2e0a 0a20 2020 2020    format...     
-00009240: 2020 2020 2020 2052 6571 7569 7265 6420         Required 
-00009250: 696e 2074 6865 2060 6053 454c 4543 5460  in the ``SELECT`
-00009260: 6020 636c 6175 7365 2e0a 0a20 2020 2020  ` clause...     
-00009270: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00009280: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00009290: 2060 6f6e 656f 6660 5f20 6060 5f72 6570   `oneof`_ ``_rep
-000092a0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-000092b0: 6060 2e0a 2020 2020 2020 2020 6964 2028  ``..        id (
-000092c0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000092d0: 2020 5245 5354 2049 4420 6f66 2074 6865    REST ID of the
-000092e0: 2070 726f 6475 6374 2c20 696e 2074 6865   product, in the
-000092f0: 2066 6f72 6d20 6f66 0a20 2020 2020 2020   form of.       
-00009300: 2020 2020 2060 6063 6861 6e6e 656c 7e6c       ``channel~l
-00009310: 616e 6775 6167 6543 6f64 657e 6665 6564  anguageCode~feed
-00009320: 4c61 6265 6c7e 6f66 6665 7249 6460 602e  Label~offerId``.
-00009330: 2043 616e 2062 6520 7573 6564 2074 6f0a   Can be used to.
-00009340: 2020 2020 2020 2020 2020 2020 6a6f 696e              join
-00009350: 2064 6174 6120 7769 7468 2074 6865 2060   data with the `
-00009360: 6070 726f 6475 6374 5f76 6965 7760 6020  `product_view`` 
-00009370: 7461 626c 652e 0a0a 2020 2020 2020 2020  table...        
-00009380: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
-00009390: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
-000093a0: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
-000093b0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-000093c0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000093d0: 6e65 6f66 605f 2060 605f 6964 6060 2e0a  neof`_ ``_id``..
-000093e0: 2020 2020 2020 2020 6f66 6665 725f 6964          offer_id
-000093f0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00009400: 2020 2020 4d65 7263 6861 6e74 2d70 726f      Merchant-pro
-00009410: 7669 6465 6420 6964 206f 6620 7468 6520  vided id of the 
-00009420: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
-00009430: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00009440: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00009450: 606f 6e65 6f66 605f 2060 605f 6f66 6665  `oneof`_ ``_offe
-00009460: 725f 6964 6060 2e0a 2020 2020 2020 2020  r_id``..        
-00009470: 7469 746c 6520 2873 7472 293a 0a20 2020  title (str):.   
-00009480: 2020 2020 2020 2020 2054 6974 6c65 206f           Title o
-00009490: 6620 7468 6520 7072 6f64 7563 742e 0a0a  f the product...
-000094a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-000094b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-000094c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-000094d0: 605f 7469 746c 6560 602e 0a20 2020 2020  `_title``..     
-000094e0: 2020 2062 7261 6e64 2028 7374 7229 3a0a     brand (str):.
-000094f0: 2020 2020 2020 2020 2020 2020 4272 616e              Bran
-00009500: 6420 6f66 2074 6865 2070 726f 6475 6374  d of the product
-00009510: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00009520: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00009530: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00009540: 5f20 6060 5f62 7261 6e64 6060 2e0a 2020  _ ``_brand``..  
-00009550: 2020 2020 2020 6361 7465 676f 7279 5f6c        category_l
-00009560: 3120 2873 7472 293a 0a20 2020 2020 2020  1 (str):.       
-00009570: 2020 2020 2050 726f 6475 6374 2063 6174       Product cat
-00009580: 6567 6f72 7920 2831 7374 206c 6576 656c  egory (1st level
-00009590: 2920 696e 2060 476f 6f67 6c65 2773 2070  ) in `Google's p
-000095a0: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
-000095b0: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
-000095c0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-000095d0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-000095e0: 732f 616e 7377 6572 2f36 3332 3434 3336  s/answer/6324436
-000095f0: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
-00009600: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00009610: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00009620: 656f 6660 5f20 6060 5f63 6174 6567 6f72  eof`_ ``_categor
-00009630: 795f 6c31 6060 2e0a 2020 2020 2020 2020  y_l1``..        
-00009640: 6361 7465 676f 7279 5f6c 3220 2873 7472  category_l2 (str
-00009650: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-00009660: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00009670: 2832 6e64 206c 6576 656c 2920 696e 2060  (2nd level) in `
-00009680: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-00009690: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
-000096a0: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
-000096b0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-000096c0: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-000096d0: 6572 2f36 3332 3434 3336 3e60 5f5f 2e0a  er/6324436>`__..
-000096e0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-000096f0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-00009700: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-00009710: 6060 5f63 6174 6567 6f72 795f 6c32 6060  ``_category_l2``
-00009720: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-00009730: 7279 5f6c 3320 2873 7472 293a 0a20 2020  ry_l3 (str):.   
-00009740: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-00009750: 2063 6174 6567 6f72 7920 2833 7264 206c   category (3rd l
-00009760: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
-00009770: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-00009780: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00009790: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-000097a0: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-000097b0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-000097c0: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-000097d0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-000097e0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-000097f0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-00009800: 6567 6f72 795f 6c33 6060 2e0a 2020 2020  egory_l3``..    
-00009810: 2020 2020 6361 7465 676f 7279 5f6c 3420      category_l4 
-00009820: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00009830: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-00009840: 6f72 7920 2834 7468 206c 6576 656c 2920  ory (4th level) 
-00009850: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-00009860: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-00009870: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-00009880: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00009890: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-000098a0: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-000098b0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-000098c0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-000098d0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-000098e0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-000098f0: 6c34 6060 2e0a 2020 2020 2020 2020 6361  l4``..        ca
-00009900: 7465 676f 7279 5f6c 3520 2873 7472 293a  tegory_l5 (str):
-00009910: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-00009920: 6475 6374 2063 6174 6567 6f72 7920 2835  duct category (5
-00009930: 7468 206c 6576 656c 2920 696e 2060 476f  th level) in `Go
-00009940: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-00009950: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-00009960: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-00009970: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-00009980: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-00009990: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-000099a0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-000099b0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-000099c0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-000099d0: 5f63 6174 6567 6f72 795f 6c35 6060 2e0a  _category_l5``..
-000099e0: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-000099f0: 7479 7065 5f6c 3120 2873 7472 293a 0a20  type_l1 (str):. 
-00009a00: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-00009a10: 6374 2074 7970 6520 2831 7374 206c 6576  ct type (1st lev
-00009a20: 656c 2920 696e 206d 6572 6368 616e 7427  el) in merchant'
-00009a30: 7320 6f77 6e20 6070 726f 6475 6374 0a20  s own `product. 
-00009a40: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-00009a50: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-00009a60: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-00009a70: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-00009a80: 2f36 3332 3434 3036 3e60 5f5f 2e0a 0a20  /6324406>`__... 
-00009a90: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00009aa0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00009ab0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00009ac0: 5f70 726f 6475 6374 5f74 7970 655f 6c31  _product_type_l1
-00009ad0: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-00009ae0: 7563 745f 7479 7065 5f6c 3220 2873 7472  uct_type_l2 (str
-00009af0: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-00009b00: 726f 6475 6374 2074 7970 6520 2832 6e64  roduct type (2nd
-00009b10: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
-00009b20: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
-00009b30: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-00009b40: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-00009b50: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-00009b60: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-00009b70: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
-00009b80: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00009b90: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00009ba0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00009bb0: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-00009bc0: 655f 6c32 6060 2e0a 2020 2020 2020 2020  e_l2``..        
-00009bd0: 7072 6f64 7563 745f 7479 7065 5f6c 3320  product_type_l3 
-00009be0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00009bf0: 2020 2050 726f 6475 6374 2074 7970 6520     Product type 
-00009c00: 2833 7264 206c 6576 656c 2920 696e 206d  (3rd level) in m
-00009c10: 6572 6368 616e 7427 7320 6f77 6e20 6070  erchant's own `p
-00009c20: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
-00009c30: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
-00009c40: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-00009c50: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-00009c60: 732f 616e 7377 6572 2f36 3332 3434 3036  s/answer/6324406
-00009c70: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
-00009c80: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00009c90: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00009ca0: 656f 6660 5f20 6060 5f70 726f 6475 6374  eof`_ ``_product
-00009cb0: 5f74 7970 655f 6c33 6060 2e0a 2020 2020  _type_l3``..    
-00009cc0: 2020 2020 7072 6f64 7563 745f 7479 7065      product_type
-00009cd0: 5f6c 3420 2873 7472 293a 0a20 2020 2020  _l4 (str):.     
-00009ce0: 2020 2020 2020 2050 726f 6475 6374 2074         Product t
-00009cf0: 7970 6520 2834 7468 206c 6576 656c 2920  ype (4th level) 
-00009d00: 696e 206d 6572 6368 616e 7427 7320 6f77  in merchant's ow
-00009d10: 6e20 6070 726f 6475 6374 0a20 2020 2020  n `product.     
-00009d20: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00009d30: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00009d40: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00009d50: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-00009d60: 3434 3036 3e60 5f5f 2e0a 0a20 2020 2020  4406>`__...     
-00009d70: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00009d80: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00009d90: 2060 6f6e 656f 6660 5f20 6060 5f70 726f   `oneof`_ ``_pro
-00009da0: 6475 6374 5f74 7970 655f 6c34 6060 2e0a  duct_type_l4``..
-00009db0: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-00009dc0: 7479 7065 5f6c 3520 2873 7472 293a 0a20  type_l5 (str):. 
-00009dd0: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-00009de0: 6374 2074 7970 6520 2835 7468 206c 6576  ct type (5th lev
-00009df0: 656c 2920 696e 206d 6572 6368 616e 7427  el) in merchant'
-00009e00: 7320 6f77 6e20 6070 726f 6475 6374 0a20  s own `product. 
-00009e10: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-00009e20: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-00009e30: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-00009e40: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-00009e50: 2f36 3332 3434 3036 3e60 5f5f 2e0a 0a20  /6324406>`__... 
-00009e60: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00009e70: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00009e80: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00009e90: 5f70 726f 6475 6374 5f74 7970 655f 6c35  _product_type_l5
-00009ea0: 6060 2e0a 2020 2020 2020 2020 7072 6963  ``..        pric
-00009eb0: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
-00009ec0: 6e67 2e74 7970 652e 7479 7065 732e 5072  ng.type.types.Pr
-00009ed0: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
-00009ee0: 2020 4375 7272 656e 7420 7072 6963 6520    Current price 
-00009ef0: 6f66 2074 6865 2070 726f 6475 6374 2e0a  of the product..
-00009f00: 2020 2020 2020 2020 6265 6e63 686d 6172          benchmar
-00009f10: 6b5f 7072 6963 6520 2867 6f6f 676c 652e  k_price (google.
-00009f20: 7368 6f70 7069 6e67 2e74 7970 652e 7479  shopping.type.ty
-00009f30: 7065 732e 5072 6963 6529 3a0a 2020 2020  pes.Price):.    
-00009f40: 2020 2020 2020 2020 4c61 7465 7374 2061          Latest a
-00009f50: 7661 696c 6162 6c65 2070 7269 6365 2062  vailable price b
-00009f60: 656e 6368 6d61 726b 2066 6f72 2074 6865  enchmark for the
-00009f70: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00009f80: 6475 6374 2773 2063 6174 616c 6f67 2069  duct's catalog i
-00009f90: 6e20 7468 6520 6265 6e63 686d 6172 6b20  n the benchmark 
-00009fa0: 636f 756e 7472 792e 0a20 2020 2022 2222  country..    """
-00009fb0: 0a0a 2020 2020 7265 706f 7274 5f63 6f75  ..    report_cou
-00009fc0: 6e74 7279 5f63 6f64 653a 2073 7472 203d  ntry_code: str =
-00009fd0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00009fe0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00009ff0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000a000: 6572 3d31 2c0a 2020 2020 2020 2020 6f70  er=1,.        op
-0000a010: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000a020: 2029 0a20 2020 2069 643a 2073 7472 203d   ).    id: str =
-0000a030: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000a040: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000a050: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000a060: 6572 3d32 2c0a 2020 2020 2020 2020 6f70  er=2,.        op
-0000a070: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000a080: 2029 0a20 2020 206f 6666 6572 5f69 643a   ).    offer_id:
-0000a090: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000a0a0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000a0b0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000a0c0: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-0000a0d0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000a0e0: 652c 0a20 2020 2029 0a20 2020 2074 6974  e,.    ).    tit
-0000a0f0: 6c65 3a20 7374 7220 3d20 7072 6f74 6f2e  le: str = proto.
-0000a100: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000a110: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000a120: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
-0000a130: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000a140: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000a150: 6272 616e 643a 2073 7472 203d 2070 726f  brand: str = pro
-0000a160: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-0000a170: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-0000a180: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
-0000a190: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0000a1a0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-0000a1b0: 2020 2063 6174 6567 6f72 795f 6c31 3a20     category_l1: 
-0000a1c0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000a1d0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000a1e0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000a1f0: 206e 756d 6265 723d 362c 0a20 2020 2020   number=6,.     
-0000a200: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000a210: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
-0000a220: 676f 7279 5f6c 323a 2073 7472 203d 2070  gory_l2: str = p
-0000a230: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000a240: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-0000a250: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000a260: 3d37 2c0a 2020 2020 2020 2020 6f70 7469  =7,.        opti
-0000a270: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000a280: 0a20 2020 2063 6174 6567 6f72 795f 6c33  .    category_l3
-0000a290: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000a2a0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000a2b0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000a2c0: 2020 206e 756d 6265 723d 382c 0a20 2020     number=8,.   
-0000a2d0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000a2e0: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
-0000a2f0: 7465 676f 7279 5f6c 343a 2073 7472 203d  tegory_l4: str =
-0000a300: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000a310: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000a320: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000a330: 6572 3d39 2c0a 2020 2020 2020 2020 6f70  er=9,.        op
-0000a340: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000a350: 2029 0a20 2020 2063 6174 6567 6f72 795f   ).    category_
-0000a360: 6c35 3a20 7374 7220 3d20 7072 6f74 6f2e  l5: str = proto.
-0000a370: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000a380: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000a390: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
-0000a3a0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000a3b0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000a3c0: 2070 726f 6475 6374 5f74 7970 655f 6c31   product_type_l1
-0000a3d0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000a3e0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000a3f0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000a400: 2020 206e 756d 6265 723d 3131 2c0a 2020     number=11,.  
-0000a410: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000a420: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
-0000a430: 726f 6475 6374 5f74 7970 655f 6c32 3a20  roduct_type_l2: 
-0000a440: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000a450: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000a460: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000a470: 206e 756d 6265 723d 3132 2c0a 2020 2020   number=12,.    
-0000a480: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000a490: 652c 0a20 2020 2029 0a20 2020 2070 726f  e,.    ).    pro
-0000a4a0: 6475 6374 5f74 7970 655f 6c33 3a20 7374  duct_type_l3: st
-0000a4b0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000a4c0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000a4d0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000a4e0: 756d 6265 723d 3133 2c0a 2020 2020 2020  umber=13,.      
-0000a4f0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000a500: 0a20 2020 2029 0a20 2020 2070 726f 6475  .    ).    produ
-0000a510: 6374 5f74 7970 655f 6c34 3a20 7374 7220  ct_type_l4: str 
-0000a520: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000a530: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-0000a540: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-0000a550: 6265 723d 3134 2c0a 2020 2020 2020 2020  ber=14,.        
-0000a560: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000a570: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
-0000a580: 5f74 7970 655f 6c35 3a20 7374 7220 3d20  _type_l5: str = 
-0000a590: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000a5a0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000a5b0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000a5c0: 723d 3135 2c0a 2020 2020 2020 2020 6f70  r=15,.        op
-0000a5d0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000a5e0: 2029 0a20 2020 2070 7269 6365 3a20 7479   ).    price: ty
-0000a5f0: 7065 732e 5072 6963 6520 3d20 7072 6f74  pes.Price = prot
-0000a600: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000a610: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
-0000a620: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-0000a630: 362c 0a20 2020 2020 2020 206d 6573 7361  6,.        messa
-0000a640: 6765 3d74 7970 6573 2e50 7269 6365 2c0a  ge=types.Price,.
-0000a650: 2020 2020 290a 2020 2020 6265 6e63 686d      ).    benchm
-0000a660: 6172 6b5f 7072 6963 653a 2074 7970 6573  ark_price: types
-0000a670: 2e50 7269 6365 203d 2070 726f 746f 2e46  .Price = proto.F
-0000a680: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000a690: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-0000a6a0: 2020 2020 206e 756d 6265 723d 3137 2c0a       number=17,.
-0000a6b0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-0000a6c0: 7479 7065 732e 5072 6963 652c 0a20 2020  types.Price,.   
-0000a6d0: 2029 0a0a 0a63 6c61 7373 2050 7269 6365   )...class Price
-0000a6e0: 496e 7369 6768 7473 5072 6f64 7563 7456  InsightsProductV
-0000a6f0: 6965 7728 7072 6f74 6f2e 4d65 7373 6167  iew(proto.Messag
-0000a700: 6529 3a0a 2020 2020 7222 2222 4669 656c  e):.    r"""Fiel
-0000a710: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
-0000a720: 2071 7565 7279 2069 6e20 6060 7072 6963   query in ``pric
-0000a730: 655f 696e 7369 6768 7473 5f70 726f 6475  e_insights_produ
-0000a740: 6374 5f76 6965 7760 6020 7461 626c 652e  ct_view`` table.
-0000a750: 0a0a 2020 2020 6050 7269 6365 0a20 2020  ..    `Price.   
-0000a760: 2069 6e73 6967 6874 7320 3c68 7474 7073   insights <https
-0000a770: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000a780: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000a790: 616e 7377 6572 2f31 3139 3136 3932 363e  answer/11916926>
-0000a7a0: 605f 5f0a 2020 2020 7265 706f 7274 2e0a  `__.    report..
-0000a7b0: 0a20 2020 2056 616c 7565 7320 6172 6520  .    Values are 
-0000a7c0: 6f6e 6c79 2073 6574 2066 6f72 2066 6965  only set for fie
-0000a7d0: 6c64 7320 7265 7175 6573 7465 6420 6578  lds requested ex
-0000a7e0: 706c 6963 6974 6c79 2069 6e20 7468 6520  plicitly in the 
-0000a7f0: 7265 7175 6573 7427 730a 2020 2020 7365  request's.    se
-0000a800: 6172 6368 2071 7565 7279 2e0a 0a0a 2020  arch query....  
-0000a810: 2020 2e2e 205f 6f6e 656f 663a 2068 7474    .. _oneof: htt
-0000a820: 7073 3a2f 2f70 726f 746f 2d70 6c75 732d  ps://proto-plus-
-0000a830: 7079 7468 6f6e 2e72 6561 6474 6865 646f  python.readthedo
-0000a840: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
-0000a850: 6669 656c 6473 2e68 746d 6c23 6f6e 656f  fields.html#oneo
-0000a860: 6673 2d6d 7574 7561 6c6c 792d 6578 636c  fs-mutually-excl
-0000a870: 7573 6976 652d 6669 656c 6473 0a0a 2020  usive-fields..  
-0000a880: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-0000a890: 2020 2020 2020 6964 2028 7374 7229 3a0a        id (str):.
-0000a8a0: 2020 2020 2020 2020 2020 2020 5245 5354              REST
-0000a8b0: 2049 4420 6f66 2074 6865 2070 726f 6475   ID of the produ
-0000a8c0: 6374 2c20 696e 2074 6865 2066 6f72 6d20  ct, in the form 
-0000a8d0: 6f66 0a20 2020 2020 2020 2020 2020 2060  of.            `
-0000a8e0: 6063 6861 6e6e 656c 7e6c 616e 6775 6167  `channel~languag
-0000a8f0: 6543 6f64 657e 6665 6564 4c61 6265 6c7e  eCode~feedLabel~
-0000a900: 6f66 6665 7249 6460 602e 2043 616e 2062  offerId``. Can b
-0000a910: 6520 7573 6564 2074 6f0a 2020 2020 2020  e used to.      
-0000a920: 2020 2020 2020 6a6f 696e 2064 6174 6120        join data 
-0000a930: 7769 7468 2074 6865 2060 6070 726f 6475  with the ``produ
-0000a940: 6374 5f76 6965 7760 6020 7461 626c 652e  ct_view`` table.
-0000a950: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-0000a960: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
-0000a970: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
-0000a980: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000a990: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000a9a0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000a9b0: 2060 605f 6964 6060 2e0a 2020 2020 2020   ``_id``..      
-0000a9c0: 2020 6f66 6665 725f 6964 2028 7374 7229    offer_id (str)
-0000a9d0: 3a0a 2020 2020 2020 2020 2020 2020 4d65  :.            Me
-0000a9e0: 7263 6861 6e74 2d70 726f 7669 6465 6420  rchant-provided 
-0000a9f0: 6964 206f 6620 7468 6520 7072 6f64 7563  id of the produc
-0000aa00: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-0000aa10: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-0000aa20: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-0000aa30: 605f 2060 605f 6f66 6665 725f 6964 6060  `_ ``_offer_id``
-0000aa40: 2e0a 2020 2020 2020 2020 7469 746c 6520  ..        title 
-0000aa50: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000aa60: 2020 2054 6974 6c65 206f 6620 7468 6520     Title of the 
-0000aa70: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
-0000aa80: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-0000aa90: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-0000aaa0: 606f 6e65 6f66 605f 2060 605f 7469 746c  `oneof`_ ``_titl
-0000aab0: 6560 602e 0a20 2020 2020 2020 2062 7261  e``..        bra
-0000aac0: 6e64 2028 7374 7229 3a0a 2020 2020 2020  nd (str):.      
-0000aad0: 2020 2020 2020 4272 616e 6420 6f66 2074        Brand of t
-0000aae0: 6865 2070 726f 6475 6374 2e0a 0a20 2020  he product...   
-0000aaf0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000ab00: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000ab10: 6f66 2060 6f6e 656f 6660 5f20 6060 5f62  of `oneof`_ ``_b
-0000ab20: 7261 6e64 6060 2e0a 2020 2020 2020 2020  rand``..        
-0000ab30: 6361 7465 676f 7279 5f6c 3120 2873 7472  category_l1 (str
-0000ab40: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-0000ab50: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-0000ab60: 2831 7374 206c 6576 656c 2920 696e 2060  (1st level) in `
-0000ab70: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-0000ab80: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
-0000ab90: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
-0000aba0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-0000abb0: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-0000abc0: 6572 2f36 3332 3434 3336 3e60 5f5f 2e0a  er/6324436>`__..
-0000abd0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000abe0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000abf0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000ac00: 6060 5f63 6174 6567 6f72 795f 6c31 6060  ``_category_l1``
-0000ac10: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-0000ac20: 7279 5f6c 3220 2873 7472 293a 0a20 2020  ry_l2 (str):.   
-0000ac30: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-0000ac40: 2063 6174 6567 6f72 7920 2832 6e64 206c   category (2nd l
-0000ac50: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
-0000ac60: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-0000ac70: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-0000ac80: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-0000ac90: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-0000aca0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-0000acb0: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-0000acc0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-0000acd0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-0000ace0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-0000acf0: 6567 6f72 795f 6c32 6060 2e0a 2020 2020  egory_l2``..    
-0000ad00: 2020 2020 6361 7465 676f 7279 5f6c 3320      category_l3 
-0000ad10: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000ad20: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-0000ad30: 6f72 7920 2833 7264 206c 6576 656c 2920  ory (3rd level) 
-0000ad40: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-0000ad50: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000ad60: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000ad70: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000ad80: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000ad90: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-0000ada0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000adb0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000adc0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000add0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-0000ade0: 6c33 6060 2e0a 2020 2020 2020 2020 6361  l3``..        ca
-0000adf0: 7465 676f 7279 5f6c 3420 2873 7472 293a  tegory_l4 (str):
-0000ae00: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000ae10: 6475 6374 2063 6174 6567 6f72 7920 2834  duct category (4
-0000ae20: 7468 206c 6576 656c 2920 696e 2060 476f  th level) in `Go
-0000ae30: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-0000ae40: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000ae50: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000ae60: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000ae70: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000ae80: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-0000ae90: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000aea0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000aeb0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000aec0: 5f63 6174 6567 6f72 795f 6c34 6060 2e0a  _category_l4``..
-0000aed0: 2020 2020 2020 2020 6361 7465 676f 7279          category
-0000aee0: 5f6c 3520 2873 7472 293a 0a20 2020 2020  _l5 (str):.     
-0000aef0: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-0000af00: 6174 6567 6f72 7920 2835 7468 206c 6576  ategory (5th lev
-0000af10: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
-0000af20: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000af30: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000af40: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000af50: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000af60: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000af70: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-0000af80: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000af90: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000afa0: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-0000afb0: 6f72 795f 6c35 6060 2e0a 2020 2020 2020  ory_l5``..      
-0000afc0: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-0000afd0: 3120 2873 7472 293a 0a20 2020 2020 2020  1 (str):.       
-0000afe0: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
-0000aff0: 6520 2831 7374 206c 6576 656c 2920 696e  e (1st level) in
-0000b000: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
-0000b010: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
-0000b020: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000b030: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000b040: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000b050: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000b060: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
-0000b070: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000b080: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000b090: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
-0000b0a0: 6374 5f74 7970 655f 6c31 6060 2e0a 2020  ct_type_l1``..  
-0000b0b0: 2020 2020 2020 7072 6f64 7563 745f 7479        product_ty
-0000b0c0: 7065 5f6c 3220 2873 7472 293a 0a20 2020  pe_l2 (str):.   
-0000b0d0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-0000b0e0: 2074 7970 6520 2832 6e64 206c 6576 656c   type (2nd level
-0000b0f0: 2920 696e 206d 6572 6368 616e 7427 7320  ) in merchant's 
-0000b100: 6f77 6e20 6070 726f 6475 6374 0a20 2020  own `product.   
-0000b110: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
-0000b120: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
-0000b130: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-0000b140: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
-0000b150: 3332 3434 3036 3e60 5f5f 2e0a 0a20 2020  324406>`__...   
-0000b160: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000b170: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000b180: 6f66 2060 6f6e 656f 6660 5f20 6060 5f70  of `oneof`_ ``_p
-0000b190: 726f 6475 6374 5f74 7970 655f 6c32 6060  roduct_type_l2``
-0000b1a0: 2e0a 2020 2020 2020 2020 7072 6f64 7563  ..        produc
-0000b1b0: 745f 7479 7065 5f6c 3320 2873 7472 293a  t_type_l3 (str):
-0000b1c0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000b1d0: 6475 6374 2074 7970 6520 2833 7264 206c  duct type (3rd l
-0000b1e0: 6576 656c 2920 696e 206d 6572 6368 616e  evel) in merchan
-0000b1f0: 7427 7320 6f77 6e20 6070 726f 6475 6374  t's own `product
-0000b200: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
-0000b210: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
-0000b220: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-0000b230: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-0000b240: 6572 2f36 3332 3434 3036 3e60 5f5f 2e0a  er/6324406>`__..
-0000b250: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000b260: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000b270: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000b280: 6060 5f70 726f 6475 6374 5f74 7970 655f  ``_product_type_
-0000b290: 6c33 6060 2e0a 2020 2020 2020 2020 7072  l3``..        pr
-0000b2a0: 6f64 7563 745f 7479 7065 5f6c 3420 2873  oduct_type_l4 (s
-0000b2b0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0000b2c0: 2050 726f 6475 6374 2074 7970 6520 2834   Product type (4
-0000b2d0: 7468 206c 6576 656c 2920 696e 206d 6572  th level) in mer
-0000b2e0: 6368 616e 7427 7320 6f77 6e20 6070 726f  chant's own `pro
-0000b2f0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000b300: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000b310: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000b320: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000b330: 616e 7377 6572 2f36 3332 3434 3036 3e60  answer/6324406>`
-0000b340: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000b350: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000b360: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000b370: 6660 5f20 6060 5f70 726f 6475 6374 5f74  f`_ ``_product_t
-0000b380: 7970 655f 6c34 6060 2e0a 2020 2020 2020  ype_l4``..      
-0000b390: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-0000b3a0: 3520 2873 7472 293a 0a20 2020 2020 2020  5 (str):.       
-0000b3b0: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
-0000b3c0: 6520 2835 7468 206c 6576 656c 2920 696e  e (5th level) in
-0000b3d0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
-0000b3e0: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
-0000b3f0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000b400: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000b410: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000b420: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000b430: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
-0000b440: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000b450: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000b460: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
-0000b470: 6374 5f74 7970 655f 6c35 6060 2e0a 2020  ct_type_l5``..  
-0000b480: 2020 2020 2020 7072 6963 6520 2867 6f6f        price (goo
-0000b490: 676c 652e 7368 6f70 7069 6e67 2e74 7970  gle.shopping.typ
-0000b4a0: 652e 7479 7065 732e 5072 6963 6529 3a0a  e.types.Price):.
-0000b4b0: 2020 2020 2020 2020 2020 2020 4375 7272              Curr
-0000b4c0: 656e 7420 7072 6963 6520 6f66 2074 6865  ent price of the
-0000b4d0: 2070 726f 6475 6374 2e0a 2020 2020 2020   product..      
-0000b4e0: 2020 7375 6767 6573 7465 645f 7072 6963    suggested_pric
-0000b4f0: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
-0000b500: 6e67 2e74 7970 652e 7479 7065 732e 5072  ng.type.types.Pr
-0000b510: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
-0000b520: 2020 4c61 7465 7374 2073 7567 6765 7374    Latest suggest
-0000b530: 6564 2070 7269 6365 2066 6f72 2074 6865  ed price for the
-0000b540: 2070 726f 6475 6374 2e0a 2020 2020 2020   product..      
-0000b550: 2020 7072 6564 6963 7465 645f 696d 7072    predicted_impr
-0000b560: 6573 7369 6f6e 735f 6368 616e 6765 5f66  essions_change_f
-0000b570: 7261 6374 696f 6e20 2866 6c6f 6174 293a  raction (float):
-0000b580: 0a20 2020 2020 2020 2020 2020 2050 7265  .            Pre
-0000b590: 6469 6374 6564 2063 6861 6e67 6520 696e  dicted change in
-0000b5a0: 2069 6d70 7265 7373 696f 6e73 2061 7320   impressions as 
-0000b5b0: 6120 6672 6163 7469 6f6e 0a20 2020 2020  a fraction.     
-0000b5c0: 2020 2020 2020 2061 6674 6572 2069 6e74         after int
-0000b5d0: 726f 6475 6369 6e67 2074 6865 2073 7567  roducing the sug
-0000b5e0: 6765 7374 6564 2070 7269 6365 2063 6f6d  gested price com
-0000b5f0: 7061 7265 640a 2020 2020 2020 2020 2020  pared.          
-0000b600: 2020 746f 2063 7572 7265 6e74 2061 6374    to current act
-0000b610: 6976 6520 7072 6963 652e 2046 6f72 2065  ive price. For e
-0000b620: 7861 6d70 6c65 2c20 302e 3035 2069 7320  xample, 0.05 is 
-0000b630: 610a 2020 2020 2020 2020 2020 2020 3525  a.            5%
-0000b640: 2070 7265 6469 6374 6564 2069 6e63 7265   predicted incre
-0000b650: 6173 6520 696e 2069 6d70 7265 7373 696f  ase in impressio
-0000b660: 6e73 2e0a 0a20 2020 2020 2020 2020 2020  ns...           
-0000b670: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000b680: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000b690: 6660 5f20 6060 5f70 7265 6469 6374 6564  f`_ ``_predicted
-0000b6a0: 5f69 6d70 7265 7373 696f 6e73 5f63 6861  _impressions_cha
-0000b6b0: 6e67 655f 6672 6163 7469 6f6e 6060 2e0a  nge_fraction``..
-0000b6c0: 2020 2020 2020 2020 7072 6564 6963 7465          predicte
-0000b6d0: 645f 636c 6963 6b73 5f63 6861 6e67 655f  d_clicks_change_
-0000b6e0: 6672 6163 7469 6f6e 2028 666c 6f61 7429  fraction (float)
-0000b6f0: 3a0a 2020 2020 2020 2020 2020 2020 5072  :.            Pr
-0000b700: 6564 6963 7465 6420 6368 616e 6765 2069  edicted change i
-0000b710: 6e20 636c 6963 6b73 2061 7320 6120 6672  n clicks as a fr
-0000b720: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-0000b730: 2020 2061 6674 6572 2069 6e74 726f 6475     after introdu
-0000b740: 6369 6e67 2074 6865 2073 7567 6765 7374  cing the suggest
-0000b750: 6564 2070 7269 6365 2063 6f6d 7061 7265  ed price compare
-0000b760: 640a 2020 2020 2020 2020 2020 2020 746f  d.            to
-0000b770: 2063 7572 7265 6e74 2061 6374 6976 6520   current active 
-0000b780: 7072 6963 652e 2046 6f72 2065 7861 6d70  price. For examp
-0000b790: 6c65 2c20 302e 3035 2069 7320 610a 2020  le, 0.05 is a.  
-0000b7a0: 2020 2020 2020 2020 2020 3525 2070 7265            5% pre
-0000b7b0: 6469 6374 6564 2069 6e63 7265 6173 6520  dicted increase 
-0000b7c0: 696e 2063 6c69 636b 732e 0a0a 2020 2020  in clicks...    
-0000b7d0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000b7e0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000b7f0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
-0000b800: 6564 6963 7465 645f 636c 6963 6b73 5f63  edicted_clicks_c
-0000b810: 6861 6e67 655f 6672 6163 7469 6f6e 6060  hange_fraction``
-0000b820: 2e0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
-0000b830: 7465 645f 636f 6e76 6572 7369 6f6e 735f  ted_conversions_
-0000b840: 6368 616e 6765 5f66 7261 6374 696f 6e20  change_fraction 
-0000b850: 2866 6c6f 6174 293a 0a20 2020 2020 2020  (float):.       
-0000b860: 2020 2020 2050 7265 6469 6374 6564 2063       Predicted c
-0000b870: 6861 6e67 6520 696e 2063 6f6e 7665 7273  hange in convers
-0000b880: 696f 6e73 2061 7320 6120 6672 6163 7469  ions as a fracti
-0000b890: 6f6e 0a20 2020 2020 2020 2020 2020 2061  on.            a
-0000b8a0: 6674 6572 2069 6e74 726f 6475 6369 6e67  fter introducing
-0000b8b0: 2074 6865 2073 7567 6765 7374 6564 2070   the suggested p
-0000b8c0: 7269 6365 2063 6f6d 7061 7265 640a 2020  rice compared.  
-0000b8d0: 2020 2020 2020 2020 2020 746f 2063 7572            to cur
-0000b8e0: 7265 6e74 2061 6374 6976 6520 7072 6963  rent active pric
-0000b8f0: 652e 2046 6f72 2065 7861 6d70 6c65 2c20  e. For example, 
-0000b900: 302e 3035 2069 7320 610a 2020 2020 2020  0.05 is a.      
-0000b910: 2020 2020 2020 3525 2070 7265 6469 6374        5% predict
-0000b920: 6564 2069 6e63 7265 6173 6520 696e 2063  ed increase in c
-0000b930: 6f6e 7665 7273 696f 6e73 292e 0a0a 2020  onversions)...  
-0000b940: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000b950: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000b960: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-0000b970: 7072 6564 6963 7465 645f 636f 6e76 6572  predicted_conver
-0000b980: 7369 6f6e 735f 6368 616e 6765 5f66 7261  sions_change_fra
-0000b990: 6374 696f 6e60 602e 0a20 2020 2022 2222  ction``..    """
-0000b9a0: 0a0a 2020 2020 6964 3a20 7374 7220 3d20  ..    id: str = 
-0000b9b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000b9c0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000b9d0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000b9e0: 723d 312c 0a20 2020 2020 2020 206f 7074  r=1,.        opt
-0000b9f0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000ba00: 290a 2020 2020 6f66 6665 725f 6964 3a20  ).    offer_id: 
-0000ba10: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000ba20: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000ba30: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000ba40: 206e 756d 6265 723d 322c 0a20 2020 2020   number=2,.     
-0000ba50: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000ba60: 2c0a 2020 2020 290a 2020 2020 7469 746c  ,.    ).    titl
-0000ba70: 653a 2073 7472 203d 2070 726f 746f 2e46  e: str = proto.F
-0000ba80: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000ba90: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-0000baa0: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-0000bab0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000bac0: 7275 652c 0a20 2020 2029 0a20 2020 2062  rue,.    ).    b
-0000bad0: 7261 6e64 3a20 7374 7220 3d20 7072 6f74  rand: str = prot
-0000bae0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000baf0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-0000bb00: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
-0000bb10: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-0000bb20: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-0000bb30: 2020 6361 7465 676f 7279 5f6c 313a 2073    category_l1: s
-0000bb40: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-0000bb50: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000bb60: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-0000bb70: 6e75 6d62 6572 3d35 2c0a 2020 2020 2020  number=5,.      
-0000bb80: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000bb90: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
-0000bba0: 6f72 795f 6c32 3a20 7374 7220 3d20 7072  ory_l2: str = pr
-0000bbb0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000bbc0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-0000bbd0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000bbe0: 362c 0a20 2020 2020 2020 206f 7074 696f  6,.        optio
-0000bbf0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-0000bc00: 2020 2020 6361 7465 676f 7279 5f6c 333a      category_l3:
-0000bc10: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000bc20: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000bc30: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000bc40: 2020 6e75 6d62 6572 3d37 2c0a 2020 2020    number=7,.    
-0000bc50: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000bc60: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
-0000bc70: 6567 6f72 795f 6c34 3a20 7374 7220 3d20  egory_l4: str = 
-0000bc80: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000bc90: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000bca0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000bcb0: 723d 382c 0a20 2020 2020 2020 206f 7074  r=8,.        opt
-0000bcc0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000bcd0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
-0000bce0: 353a 2073 7472 203d 2070 726f 746f 2e46  5: str = proto.F
-0000bcf0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000bd00: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-0000bd10: 2020 2020 6e75 6d62 6572 3d39 2c0a 2020      number=9,.  
-0000bd20: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000bd30: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
-0000bd40: 726f 6475 6374 5f74 7970 655f 6c31 3a20  roduct_type_l1: 
-0000bd50: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000bd60: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000bd70: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000bd80: 206e 756d 6265 723d 3130 2c0a 2020 2020   number=10,.    
-0000bd90: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000bda0: 652c 0a20 2020 2029 0a20 2020 2070 726f  e,.    ).    pro
-0000bdb0: 6475 6374 5f74 7970 655f 6c32 3a20 7374  duct_type_l2: st
-0000bdc0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000bdd0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000bde0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000bdf0: 756d 6265 723d 3131 2c0a 2020 2020 2020  umber=11,.      
-0000be00: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000be10: 0a20 2020 2029 0a20 2020 2070 726f 6475  .    ).    produ
-0000be20: 6374 5f74 7970 655f 6c33 3a20 7374 7220  ct_type_l3: str 
-0000be30: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000be40: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-0000be50: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-0000be60: 6265 723d 3132 2c0a 2020 2020 2020 2020  ber=12,.        
-0000be70: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000be80: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
-0000be90: 5f74 7970 655f 6c34 3a20 7374 7220 3d20  _type_l4: str = 
-0000bea0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000beb0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000bec0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000bed0: 723d 3133 2c0a 2020 2020 2020 2020 6f70  r=13,.        op
-0000bee0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000bef0: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
-0000bf00: 7970 655f 6c35 3a20 7374 7220 3d20 7072  ype_l5: str = pr
-0000bf10: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000bf20: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-0000bf30: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000bf40: 3134 2c0a 2020 2020 2020 2020 6f70 7469  14,.        opti
-0000bf50: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000bf60: 0a20 2020 2070 7269 6365 3a20 7479 7065  .    price: type
-0000bf70: 732e 5072 6963 6520 3d20 7072 6f74 6f2e  s.Price = proto.
-0000bf80: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000bf90: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-0000bfa0: 2020 2020 2020 6e75 6d62 6572 3d31 352c        number=15,
-0000bfb0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-0000bfc0: 3d74 7970 6573 2e50 7269 6365 2c0a 2020  =types.Price,.  
-0000bfd0: 2020 290a 2020 2020 7375 6767 6573 7465    ).    suggeste
-0000bfe0: 645f 7072 6963 653a 2074 7970 6573 2e50  d_price: types.P
-0000bff0: 7269 6365 203d 2070 726f 746f 2e46 6965  rice = proto.Fie
-0000c000: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000c010: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-0000c020: 2020 206e 756d 6265 723d 3136 2c0a 2020     number=16,.  
-0000c030: 2020 2020 2020 6d65 7373 6167 653d 7479        message=ty
-0000c040: 7065 732e 5072 6963 652c 0a20 2020 2029  pes.Price,.    )
-0000c050: 0a20 2020 2070 7265 6469 6374 6564 5f69  .    predicted_i
-0000c060: 6d70 7265 7373 696f 6e73 5f63 6861 6e67  mpressions_chang
-0000c070: 655f 6672 6163 7469 6f6e 3a20 666c 6f61  e_fraction: floa
-0000c080: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
-0000c090: 0a20 2020 2020 2020 2070 726f 746f 2e44  .        proto.D
-0000c0a0: 4f55 424c 452c 0a20 2020 2020 2020 206e  OUBLE,.        n
-0000c0b0: 756d 6265 723d 3137 2c0a 2020 2020 2020  umber=17,.      
-0000c0c0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000c0d0: 0a20 2020 2029 0a20 2020 2070 7265 6469  .    ).    predi
-0000c0e0: 6374 6564 5f63 6c69 636b 735f 6368 616e  cted_clicks_chan
-0000c0f0: 6765 5f66 7261 6374 696f 6e3a 2066 6c6f  ge_fraction: flo
-0000c100: 6174 203d 2070 726f 746f 2e46 6965 6c64  at = proto.Field
-0000c110: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000c120: 444f 5542 4c45 2c0a 2020 2020 2020 2020  DOUBLE,.        
-0000c130: 6e75 6d62 6572 3d31 382c 0a20 2020 2020  number=18,.     
-0000c140: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000c150: 2c0a 2020 2020 290a 2020 2020 7072 6564  ,.    ).    pred
-0000c160: 6963 7465 645f 636f 6e76 6572 7369 6f6e  icted_conversion
-0000c170: 735f 6368 616e 6765 5f66 7261 6374 696f  s_change_fractio
-0000c180: 6e3a 2066 6c6f 6174 203d 2070 726f 746f  n: float = proto
-0000c190: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000c1a0: 7072 6f74 6f2e 444f 5542 4c45 2c0a 2020  proto.DOUBLE,.  
-0000c1b0: 2020 2020 2020 6e75 6d62 6572 3d31 392c        number=19,
-0000c1c0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-0000c1d0: 6c3d 5472 7565 2c0a 2020 2020 290a 0a0a  l=True,.    )...
-0000c1e0: 636c 6173 7320 4265 7374 5365 6c6c 6572  class BestSeller
-0000c1f0: 7350 726f 6475 6374 436c 7573 7465 7256  sProductClusterV
-0000c200: 6965 7728 7072 6f74 6f2e 4d65 7373 6167  iew(proto.Messag
-0000c210: 6529 3a0a 2020 2020 7222 2222 4669 656c  e):.    r"""Fiel
-0000c220: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
-0000c230: 2071 7565 7279 2069 6e20 6060 6265 7374   query in ``best
-0000c240: 5f73 656c 6c65 7273 5f70 726f 6475 6374  _sellers_product
-0000c250: 5f63 6c75 7374 6572 5f76 6965 7760 600a  _cluster_view``.
-0000c260: 2020 2020 7461 626c 652e 0a0a 2020 2020      table...    
-0000c270: 6042 6573 740a 2020 2020 7365 6c6c 6572  `Best.    seller
-0000c280: 7320 3c68 7474 7073 3a2f 2f73 7570 706f  s <https://suppo
-0000c290: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-0000c2a0: 7263 6861 6e74 732f 616e 7377 6572 2f39  rchants/answer/9
-0000c2b0: 3438 3836 3739 3e60 5f5f 0a20 2020 2072  488679>`__.    r
-0000c2c0: 6570 6f72 7420 7769 7468 2074 6f70 2070  eport with top p
-0000c2d0: 726f 6475 6374 2063 6c75 7374 6572 732e  roduct clusters.
-0000c2e0: 2041 2070 726f 6475 6374 2063 6c75 7374   A product clust
-0000c2f0: 6572 2069 7320 6120 6772 6f75 7069 6e67  er is a grouping
-0000c300: 0a20 2020 2066 6f72 2064 6966 6665 7265  .    for differe
-0000c310: 6e74 206f 6666 6572 7320 616e 6420 7661  nt offers and va
-0000c320: 7269 616e 7473 2074 6861 7420 7265 7072  riants that repr
-0000c330: 6573 656e 7420 7468 6520 7361 6d65 2070  esent the same p
-0000c340: 726f 6475 6374 2c0a 2020 2020 666f 7220  roduct,.    for 
-0000c350: 6578 616d 706c 652c 2047 6f6f 676c 6520  example, Google 
-0000c360: 5069 7865 6c20 372e 0a0a 2020 2020 5661  Pixel 7...    Va
-0000c370: 6c75 6573 2061 7265 206f 6e6c 7920 7365  lues are only se
-0000c380: 7420 666f 7220 6669 656c 6473 2072 6571  t for fields req
-0000c390: 7565 7374 6564 2065 7870 6c69 6369 746c  uested explicitl
-0000c3a0: 7920 696e 2074 6865 2072 6571 7565 7374  y in the request
-0000c3b0: 2773 0a20 2020 2073 6561 7263 6820 7175  's.    search qu
-0000c3c0: 6572 792e 0a0a 0a20 2020 202e 2e20 5f6f  ery....    .. _o
-0000c3d0: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
-0000c3e0: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
-0000c3f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-0000c400: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
-0000c410: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
-0000c420: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
-0000c430: 6965 6c64 730a 0a20 2020 2041 7474 7269  ields..    Attri
-0000c440: 6275 7465 733a 0a20 2020 2020 2020 2072  butes:.        r
-0000c450: 6570 6f72 745f 6461 7465 2028 676f 6f67  eport_date (goog
-0000c460: 6c65 2e74 7970 652e 6461 7465 5f70 6232  le.type.date_pb2
-0000c470: 2e44 6174 6529 3a0a 2020 2020 2020 2020  .Date):.        
-0000c480: 2020 2020 5265 706f 7274 2064 6174 652e      Report date.
-0000c490: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
-0000c4a0: 6973 2066 6965 6c64 2063 616e 206f 6e6c  is field can onl
-0000c4b0: 7920 6265 206f 6e65 206f 6620 7468 650a  y be one of the.
-0000c4c0: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
-0000c4d0: 6f77 696e 673a 0a0a 2020 2020 2020 2020  owing:..        
-0000c4e0: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
-0000c4f0: 2064 6179 206f 6620 7468 6520 7765 656b   day of the week
-0000c500: 2028 4d6f 6e64 6179 2920 666f 7220 7765   (Monday) for we
-0000c510: 656b 6c79 2072 6570 6f72 7473 2c0a 2020  ekly reports,.  
-0000c520: 2020 2020 2020 2020 2020 2d20 2054 6865            -  The
-0000c530: 2066 6972 7374 2064 6179 206f 6620 7468   first day of th
-0000c540: 6520 6d6f 6e74 6820 666f 7220 6d6f 6e74  e month for mont
-0000c550: 686c 7920 7265 706f 7274 732e 0a0a 2020  hly reports...  
-0000c560: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-0000c570: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
-0000c580: 4354 6060 2063 6c61 7573 652e 2049 6620  CT`` clause. If 
-0000c590: 6120 6060 5748 4552 4560 6020 636f 6e64  a ``WHERE`` cond
-0000c5a0: 6974 696f 6e0a 2020 2020 2020 2020 2020  ition.          
-0000c5b0: 2020 6f6e 2060 6072 6570 6f72 745f 6461    on ``report_da
-0000c5c0: 7465 6060 2069 7320 6e6f 7420 7370 6563  te`` is not spec
-0000c5d0: 6966 6965 6420 696e 2074 6865 2071 7565  ified in the que
-0000c5e0: 7279 2c20 7468 6520 6c61 7465 7374 0a20  ry, the latest. 
-0000c5f0: 2020 2020 2020 2020 2020 2061 7661 696c             avail
-0000c600: 6162 6c65 2077 6565 6b6c 7920 6f72 206d  able weekly or m
-0000c610: 6f6e 7468 6c79 2072 6570 6f72 7420 6973  onthly report is
-0000c620: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-0000c630: 2020 2072 6570 6f72 745f 6772 616e 756c     report_granul
-0000c640: 6172 6974 7920 2867 6f6f 676c 652e 7368  arity (google.sh
-0000c650: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
-0000c660: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
-0000c670: 7970 6573 2e52 6570 6f72 7447 7261 6e75  ypes.ReportGranu
-0000c680: 6c61 7269 7479 2e52 6570 6f72 7447 7261  larity.ReportGra
-0000c690: 6e75 6c61 7269 7479 456e 756d 293a 0a20  nularityEnum):. 
-0000c6a0: 2020 2020 2020 2020 2020 2047 7261 6e75             Granu
-0000c6b0: 6c61 7269 7479 206f 6620 7468 6520 7265  larity of the re
-0000c6c0: 706f 7274 2e20 5468 6520 7261 6e6b 696e  port. The rankin
-0000c6d0: 6720 6361 6e20 6265 2064 6f6e 6520 6f76  g can be done ov
-0000c6e0: 6572 2061 0a20 2020 2020 2020 2020 2020  er a.           
-0000c6f0: 2077 6565 6b20 6f72 2061 206d 6f6e 7468   week or a month
-0000c700: 2074 696d 6566 7261 6d65 2e0a 0a20 2020   timeframe...   
-0000c710: 2020 2020 2020 2020 2052 6571 7569 7265           Require
-0000c720: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
-0000c730: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
-0000c740: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
-0000c750: 2020 2020 2060 6072 6570 6f72 745f 6772       ``report_gr
-0000c760: 616e 756c 6172 6974 7960 6020 6973 2072  anularity`` is r
-0000c770: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-0000c780: 6057 4845 5245 6060 2063 6c61 7573 652e  `WHERE`` clause.
-0000c790: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000c7a0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000c7b0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000c7c0: 2060 605f 7265 706f 7274 5f67 7261 6e75   ``_report_granu
-0000c7d0: 6c61 7269 7479 6060 2e0a 2020 2020 2020  larity``..      
-0000c7e0: 2020 7265 706f 7274 5f63 6f75 6e74 7279    report_country
-0000c7f0: 5f63 6f64 6520 2873 7472 293a 0a20 2020  _code (str):.   
-0000c800: 2020 2020 2020 2020 2043 6f75 6e74 7279           Country
-0000c810: 2077 6865 7265 2074 6865 2072 616e 6b69   where the ranki
-0000c820: 6e67 2069 7320 6361 6c63 756c 6174 6564  ng is calculated
-0000c830: 2e20 5265 7072 6573 656e 7465 6420 696e  . Represented in
-0000c840: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000c850: 2049 534f 2033 3136 3620 666f 726d 6174   ISO 3166 format
-0000c860: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-0000c870: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-0000c880: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-0000c890: 2e20 436f 6e64 6974 696f 6e20 6f6e 0a20  . Condition on. 
-0000c8a0: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
-0000c8b0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-0000c8c0: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
-0000c8d0: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
-0000c8e0: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-0000c8f0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000c900: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000c910: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
-0000c920: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
-0000c930: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
-0000c940: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
-0000c950: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000c960: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
-0000c970: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
-0000c980: 6c63 756c 6174 6520 7468 6520 7261 6e6b  lculate the rank
-0000c990: 696e 6720 666f 722c 0a20 2020 2020 2020  ing for,.       
-0000c9a0: 2020 2020 2072 6570 7265 7365 6e74 6564       represented
-0000c9b0: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
-0000c9c0: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
-0000c9d0: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
-0000c9e0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
-0000c9f0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
-0000ca00: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
-0000ca10: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
-0000ca20: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
-0000ca30: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
-0000ca40: 7573 652e 2049 6620 6120 6060 5748 4552  use. If a ``WHER
-0000ca50: 4560 6020 636f 6e64 6974 696f 6e0a 2020  E`` condition.  
-0000ca60: 2020 2020 2020 2020 2020 6f6e 2060 6072            on ``r
-0000ca70: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
-0000ca80: 6460 6020 6973 206e 6f74 2073 7065 6369  d`` is not speci
-0000ca90: 6669 6564 2069 6e20 7468 6520 7175 6572  fied in the quer
-0000caa0: 792c 0a20 2020 2020 2020 2020 2020 2072  y,.            r
-0000cab0: 616e 6b69 6e67 7320 666f 7220 616c 6c20  ankings for all 
-0000cac0: 746f 702d 6c65 7665 6c20 6361 7465 676f  top-level catego
-0000cad0: 7269 6573 2061 7265 2072 6574 7572 6e65  ries are returne
-0000cae0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-0000caf0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-0000cb00: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-0000cb10: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
-0000cb20: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
-0000cb30: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
-0000cb40: 0a20 2020 2020 2020 2020 2020 2054 6974  .            Tit
-0000cb50: 6c65 206f 6620 7468 6520 7072 6f64 7563  le of the produc
-0000cb60: 7420 636c 7573 7465 722e 0a0a 2020 2020  t cluster...    
-0000cb70: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000cb80: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000cb90: 6620 606f 6e65 6f66 605f 2060 605f 7469  f `oneof`_ ``_ti
-0000cba0: 746c 6560 602e 0a20 2020 2020 2020 2062  tle``..        b
-0000cbb0: 7261 6e64 2028 7374 7229 3a0a 2020 2020  rand (str):.    
-0000cbc0: 2020 2020 2020 2020 4272 616e 6420 6f66          Brand of
-0000cbd0: 2074 6865 2070 726f 6475 6374 2063 6c75   the product clu
-0000cbe0: 7374 6572 2e0a 0a20 2020 2020 2020 2020  ster...         
-0000cbf0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000cc00: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000cc10: 656f 6660 5f20 6060 5f62 7261 6e64 6060  eof`_ ``_brand``
-0000cc20: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-0000cc30: 7279 5f6c 3120 2873 7472 293a 0a20 2020  ry_l1 (str):.   
-0000cc40: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-0000cc50: 2063 6174 6567 6f72 7920 2831 7374 206c   category (1st l
-0000cc60: 6576 656c 2920 6f66 2074 6865 2070 726f  evel) of the pro
-0000cc70: 6475 6374 2063 6c75 7374 6572 2c0a 2020  duct cluster,.  
-0000cc80: 2020 2020 2020 2020 2020 7265 7072 6573            repres
-0000cc90: 656e 7465 6420 696e 2060 476f 6f67 6c65  ented in `Google
-0000cca0: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-0000ccb0: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-0000ccc0: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-0000ccd0: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-0000cce0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-0000ccf0: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-0000cd00: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-0000cd10: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-0000cd20: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-0000cd30: 6567 6f72 795f 6c31 6060 2e0a 2020 2020  egory_l1``..    
-0000cd40: 2020 2020 6361 7465 676f 7279 5f6c 3220      category_l2 
-0000cd50: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000cd60: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-0000cd70: 6f72 7920 2832 6e64 206c 6576 656c 2920  ory (2nd level) 
-0000cd80: 6f66 2074 6865 2070 726f 6475 6374 2063  of the product c
-0000cd90: 6c75 7374 6572 2c0a 2020 2020 2020 2020  luster,.        
-0000cda0: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
-0000cdb0: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-0000cdc0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000cdd0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000cde0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000cdf0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000ce00: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-0000ce10: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000ce20: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000ce30: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000ce40: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-0000ce50: 6c32 6060 2e0a 2020 2020 2020 2020 6361  l2``..        ca
-0000ce60: 7465 676f 7279 5f6c 3320 2873 7472 293a  tegory_l3 (str):
-0000ce70: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000ce80: 6475 6374 2063 6174 6567 6f72 7920 2833  duct category (3
-0000ce90: 7264 206c 6576 656c 2920 6f66 2074 6865  rd level) of the
-0000cea0: 2070 726f 6475 6374 2063 6c75 7374 6572   product cluster
-0000ceb0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000cec0: 7072 6573 656e 7465 6420 696e 2060 476f  presented in `Go
-0000ced0: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-0000cee0: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000cef0: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000cf00: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000cf10: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000cf20: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-0000cf30: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000cf40: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000cf50: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000cf60: 5f63 6174 6567 6f72 795f 6c33 6060 2e0a  _category_l3``..
-0000cf70: 2020 2020 2020 2020 6361 7465 676f 7279          category
-0000cf80: 5f6c 3420 2873 7472 293a 0a20 2020 2020  _l4 (str):.     
-0000cf90: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-0000cfa0: 6174 6567 6f72 7920 2834 7468 206c 6576  ategory (4th lev
-0000cfb0: 656c 2920 6f66 2074 6865 2070 726f 6475  el) of the produ
-0000cfc0: 6374 2063 6c75 7374 6572 2c0a 2020 2020  ct cluster,.    
-0000cfd0: 2020 2020 2020 2020 7265 7072 6573 656e          represen
-0000cfe0: 7465 6420 696e 2060 476f 6f67 6c65 2773  ted in `Google's
-0000cff0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000d000: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000d010: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000d020: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000d030: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000d040: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-0000d050: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000d060: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000d070: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-0000d080: 6f72 795f 6c34 6060 2e0a 2020 2020 2020  ory_l4``..      
-0000d090: 2020 6361 7465 676f 7279 5f6c 3520 2873    category_l5 (s
-0000d0a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0000d0b0: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
-0000d0c0: 7920 2835 7468 206c 6576 656c 2920 6f66  y (5th level) of
-0000d0d0: 2074 6865 2070 726f 6475 6374 2063 6c75   the product clu
-0000d0e0: 7374 6572 2c0a 2020 2020 2020 2020 2020  ster,.          
-0000d0f0: 2020 7265 7072 6573 656e 7465 6420 696e    represented in
-0000d100: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
-0000d110: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-0000d120: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-0000d130: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-0000d140: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-0000d150: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
-0000d160: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000d170: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000d180: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000d190: 5f20 6060 5f63 6174 6567 6f72 795f 6c35  _ ``_category_l5
-0000d1a0: 6060 2e0a 2020 2020 2020 2020 7661 7269  ``..        vari
-0000d1b0: 616e 745f 6774 696e 7320 284d 7574 6162  ant_gtins (Mutab
-0000d1c0: 6c65 5365 7175 656e 6365 5b73 7472 5d29  leSequence[str])
-0000d1d0: 3a0a 2020 2020 2020 2020 2020 2020 4754  :.            GT
-0000d1e0: 494e 7320 6f66 2065 7861 6d70 6c65 2076  INs of example v
-0000d1f0: 6172 6961 6e74 7320 6f66 2074 6865 2070  ariants of the p
-0000d200: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
-0000d210: 2020 2063 6c75 7374 6572 2e0a 2020 2020     cluster..    
-0000d220: 2020 2020 696e 7665 6e74 6f72 795f 7374      inventory_st
-0000d230: 6174 7573 2028 676f 6f67 6c65 2e73 686f  atus (google.sho
-0000d240: 7070 696e 672e 6d65 7263 6861 6e74 5f72  pping.merchant_r
-0000d250: 6570 6f72 7473 5f76 3162 6574 612e 7479  eports_v1beta.ty
-0000d260: 7065 732e 4265 7374 5365 6c6c 6572 7350  pes.BestSellersP
-0000d270: 726f 6475 6374 436c 7573 7465 7256 6965  roductClusterVie
-0000d280: 772e 496e 7665 6e74 6f72 7953 7461 7475  w.InventoryStatu
-0000d290: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000d2a0: 5768 6574 6865 7220 7468 6520 7072 6f64  Whether the prod
-0000d2b0: 7563 7420 636c 7573 7465 7220 6973 2060  uct cluster is `
-0000d2c0: 6049 4e5f 5354 4f43 4b60 6020 696e 2079  `IN_STOCK`` in y
-0000d2d0: 6f75 7220 7072 6f64 7563 740a 2020 2020  our product.    
-0000d2e0: 2020 2020 2020 2020 6665 6564 2069 6e20          feed in 
-0000d2f0: 6174 206c 6561 7374 206f 6e65 206f 6620  at least one of 
-0000d300: 7468 6520 636f 756e 7472 6965 732c 2060  the countries, `
-0000d310: 604f 5554 5f4f 465f 5354 4f43 4b60 6020  `OUT_OF_STOCK`` 
-0000d320: 696e 0a20 2020 2020 2020 2020 2020 2079  in.            y
-0000d330: 6f75 7220 7072 6f64 7563 7420 6665 6564  our product feed
-0000d340: 2069 6e20 616c 6c20 636f 756e 7472 6965   in all countrie
-0000d350: 732c 206f 7220 6060 4e4f 545f 494e 5f49  s, or ``NOT_IN_I
-0000d360: 4e56 454e 544f 5259 6060 0a20 2020 2020  NVENTORY``.     
-0000d370: 2020 2020 2020 2061 7420 616c 6c2e 0a0a         at all...
-0000d380: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000d390: 6669 656c 6420 646f 6573 6e27 7420 7461  field doesn't ta
-0000d3a0: 6b65 2074 6865 2042 6573 7420 7365 6c6c  ke the Best sell
-0000d3b0: 6572 7320 7265 706f 7274 2063 6f75 6e74  ers report count
-0000d3c0: 7279 0a20 2020 2020 2020 2020 2020 2066  ry.            f
-0000d3d0: 696c 7465 7220 696e 746f 2061 6363 6f75  ilter into accou
-0000d3e0: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-0000d3f0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000d400: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000d410: 6660 5f20 6060 5f69 6e76 656e 746f 7279  f`_ ``_inventory
-0000d420: 5f73 7461 7475 7360 602e 0a20 2020 2020  _status``..     
-0000d430: 2020 2062 7261 6e64 5f69 6e76 656e 746f     brand_invento
-0000d440: 7279 5f73 7461 7475 7320 2867 6f6f 676c  ry_status (googl
-0000d450: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
-0000d460: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
-0000d470: 7461 2e74 7970 6573 2e42 6573 7453 656c  ta.types.BestSel
-0000d480: 6c65 7273 5072 6f64 7563 7443 6c75 7374  lersProductClust
-0000d490: 6572 5669 6577 2e49 6e76 656e 746f 7279  erView.Inventory
-0000d4a0: 5374 6174 7573 293a 0a20 2020 2020 2020  Status):.       
-0000d4b0: 2020 2020 2057 6865 7468 6572 2074 6865       Whether the
-0000d4c0: 7265 2069 7320 6174 206c 6561 7374 206f  re is at least o
-0000d4d0: 6e65 2070 726f 6475 6374 206f 6620 7468  ne product of th
-0000d4e0: 6520 6272 616e 6420 6375 7272 656e 746c  e brand currentl
-0000d4f0: 790a 2020 2020 2020 2020 2020 2020 6060  y.            ``
-0000d500: 494e 5f53 544f 434b 6060 2069 6e20 796f  IN_STOCK`` in yo
-0000d510: 7572 2070 726f 6475 6374 2066 6565 6420  ur product feed 
-0000d520: 696e 2061 7420 6c65 6173 7420 6f6e 6520  in at least one 
-0000d530: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
-0000d540: 2020 2063 6f75 6e74 7269 6573 2c20 616c     countries, al
-0000d550: 6c20 7072 6f64 7563 7473 2061 7265 2060  l products are `
-0000d560: 604f 5554 5f4f 465f 5354 4f43 4b60 6020  `OUT_OF_STOCK`` 
-0000d570: 696e 2079 6f75 7220 7072 6f64 7563 740a  in your product.
-0000d580: 2020 2020 2020 2020 2020 2020 6665 6564              feed
-0000d590: 2069 6e20 616c 6c20 636f 756e 7472 6965   in all countrie
-0000d5a0: 732c 206f 7220 6060 4e4f 545f 494e 5f49  s, or ``NOT_IN_I
-0000d5b0: 4e56 454e 544f 5259 6060 2e0a 0a20 2020  NVENTORY``...   
-0000d5c0: 2020 2020 2020 2020 2054 6865 2066 6965           The fie
-0000d5d0: 6c64 2064 6f65 736e 2774 2074 616b 6520  ld doesn't take 
-0000d5e0: 7468 6520 4265 7374 2073 656c 6c65 7273  the Best sellers
-0000d5f0: 2072 6570 6f72 7420 636f 756e 7472 790a   report country.
-0000d600: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0000d610: 6572 2069 6e74 6f20 6163 636f 756e 742e  er into account.
-0000d620: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000d630: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000d640: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000d650: 2060 605f 6272 616e 645f 696e 7665 6e74   ``_brand_invent
-0000d660: 6f72 795f 7374 6174 7573 6060 2e0a 2020  ory_status``..  
-0000d670: 2020 2020 2020 7261 6e6b 2028 696e 7429        rank (int)
-0000d680: 3a0a 2020 2020 2020 2020 2020 2020 506f  :.            Po
-0000d690: 7075 6c61 7269 7479 206f 6620 7468 6520  pularity of the 
-0000d6a0: 7072 6f64 7563 7420 636c 7573 7465 7220  product cluster 
-0000d6b0: 6f6e 2041 6473 2061 6e64 0a20 2020 2020  on Ads and.     
-0000d6c0: 2020 2020 2020 206f 7267 616e 6963 2073         organic s
-0000d6d0: 7572 6661 6365 732c 2069 6e20 7468 6520  urfaces, in the 
-0000d6e0: 7365 6c65 6374 6564 2063 6174 6567 6f72  selected categor
-0000d6f0: 7920 616e 640a 2020 2020 2020 2020 2020  y and.          
-0000d700: 2020 636f 756e 7472 792c 2062 6173 6564    country, based
-0000d710: 206f 6e20 7468 6520 6573 7469 6d61 7465   on the estimate
-0000d720: 6420 6e75 6d62 6572 206f 6620 756e 6974  d number of unit
-0000d730: 730a 2020 2020 2020 2020 2020 2020 736f  s.            so
-0000d740: 6c64 2e0a 0a20 2020 2020 2020 2020 2020  ld...           
-0000d750: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000d760: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000d770: 6660 5f20 6060 5f72 616e 6b60 602e 0a20  f`_ ``_rank``.. 
-0000d780: 2020 2020 2020 2070 7265 7669 6f75 735f         previous_
-0000d790: 7261 6e6b 2028 696e 7429 3a0a 2020 2020  rank (int):.    
-0000d7a0: 2020 2020 2020 2020 506f 7075 6c61 7269          Populari
-0000d7b0: 7479 2072 616e 6b20 696e 2074 6865 2070  ty rank in the p
-0000d7c0: 7265 7669 6f75 7320 7765 656b 206f 720a  revious week or.
-0000d7d0: 2020 2020 2020 2020 2020 2020 6d6f 6e74              mont
-0000d7e0: 682e 0a0a 2020 2020 2020 2020 2020 2020  h...            
-0000d7f0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-0000d800: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-0000d810: 605f 2060 605f 7072 6576 696f 7573 5f72  `_ ``_previous_r
-0000d820: 616e 6b60 602e 0a20 2020 2020 2020 2072  ank``..        r
-0000d830: 656c 6174 6976 655f 6465 6d61 6e64 2028  elative_demand (
-0000d840: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-0000d850: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-0000d860: 5f76 3162 6574 612e 7479 7065 732e 5265  _v1beta.types.Re
-0000d870: 6c61 7469 7665 4465 6d61 6e64 2e52 656c  lativeDemand.Rel
-0000d880: 6174 6976 6544 656d 616e 6445 6e75 6d29  ativeDemandEnum)
-0000d890: 3a0a 2020 2020 2020 2020 2020 2020 4573  :.            Es
-0000d8a0: 7469 6d61 7465 6420 6465 6d61 6e64 2069  timated demand i
-0000d8b0: 6e20 7265 6c61 7469 6f6e 2074 6f20 7468  n relation to th
-0000d8c0: 6520 7072 6f64 7563 740a 2020 2020 2020  e product.      
-0000d8d0: 2020 2020 2020 636c 7573 7465 7220 7769        cluster wi
-0000d8e0: 7468 2074 6865 2068 6967 6865 7374 2070  th the highest p
-0000d8f0: 6f70 756c 6172 6974 7920 7261 6e6b 2069  opularity rank i
-0000d900: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
-0000d910: 2020 7361 6d65 2063 6174 6567 6f72 7920    same category 
-0000d920: 616e 6420 636f 756e 7472 792e 0a0a 2020  and country...  
-0000d930: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000d940: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000d950: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-0000d960: 7265 6c61 7469 7665 5f64 656d 616e 6460  relative_demand`
-0000d970: 602e 0a20 2020 2020 2020 2070 7265 7669  `..        previ
-0000d980: 6f75 735f 7265 6c61 7469 7665 5f64 656d  ous_relative_dem
-0000d990: 616e 6420 2867 6f6f 676c 652e 7368 6f70  and (google.shop
-0000d9a0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
-0000d9b0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
-0000d9c0: 6573 2e52 656c 6174 6976 6544 656d 616e  es.RelativeDeman
-0000d9d0: 642e 5265 6c61 7469 7665 4465 6d61 6e64  d.RelativeDemand
-0000d9e0: 456e 756d 293a 0a20 2020 2020 2020 2020  Enum):.         
-0000d9f0: 2020 2045 7374 696d 6174 6564 2064 656d     Estimated dem
-0000da00: 616e 6420 696e 2072 656c 6174 696f 6e20  and in relation 
-0000da10: 746f 2074 6865 2070 726f 6475 6374 0a20  to the product. 
-0000da20: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-0000da30: 6572 2077 6974 6820 7468 6520 6869 6768  er with the high
-0000da40: 6573 7420 706f 7075 6c61 7269 7479 2072  est popularity r
-0000da50: 616e 6b20 696e 2074 6865 0a20 2020 2020  ank in the.     
-0000da60: 2020 2020 2020 2073 616d 6520 6361 7465         same cate
-0000da70: 676f 7279 2061 6e64 2063 6f75 6e74 7279  gory and country
-0000da80: 2069 6e20 7468 6520 7072 6576 696f 7573   in the previous
-0000da90: 2077 6565 6b0a 2020 2020 2020 2020 2020   week.          
-0000daa0: 2020 6f72 206d 6f6e 7468 2e0a 0a20 2020    or month...   
-0000dab0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000dac0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000dad0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f70  of `oneof`_ ``_p
-0000dae0: 7265 7669 6f75 735f 7265 6c61 7469 7665  revious_relative
-0000daf0: 5f64 656d 616e 6460 602e 0a20 2020 2020  _demand``..     
-0000db00: 2020 2072 656c 6174 6976 655f 6465 6d61     relative_dema
-0000db10: 6e64 5f63 6861 6e67 6520 2867 6f6f 676c  nd_change (googl
-0000db20: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
-0000db30: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
-0000db40: 7461 2e74 7970 6573 2e52 656c 6174 6976  ta.types.Relativ
-0000db50: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
-0000db60: 652e 5265 6c61 7469 7665 4465 6d61 6e64  e.RelativeDemand
-0000db70: 4368 616e 6765 5479 7065 456e 756d 293a  ChangeTypeEnum):
-0000db80: 0a20 2020 2020 2020 2020 2020 2043 6861  .            Cha
-0000db90: 6e67 6520 696e 2074 6865 2065 7374 696d  nge in the estim
-0000dba0: 6174 6564 2064 656d 616e 642e 2057 6865  ated demand. Whe
-0000dbb0: 7468 6572 2069 740a 2020 2020 2020 2020  ther it.        
-0000dbc0: 2020 2020 726f 7365 2c20 7361 6e6b 206f      rose, sank o
-0000dbd0: 7220 7265 6d61 696e 6564 2066 6c61 742e  r remained flat.
-0000dbe0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000dbf0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000dc00: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000dc10: 2060 605f 7265 6c61 7469 7665 5f64 656d   ``_relative_dem
-0000dc20: 616e 645f 6368 616e 6765 6060 2e0a 2020  and_change``..  
-0000dc30: 2020 2222 220a 0a20 2020 2063 6c61 7373    """..    class
-0000dc40: 2049 6e76 656e 746f 7279 5374 6174 7573   InventoryStatus
-0000dc50: 2870 726f 746f 2e45 6e75 6d29 3a0a 2020  (proto.Enum):.  
-0000dc60: 2020 2020 2020 7222 2222 5374 6174 7573        r"""Status
-0000dc70: 206f 6620 7468 6520 7072 6f64 7563 7420   of the product 
-0000dc80: 636c 7573 7465 7220 6f72 2062 7261 6e64  cluster or brand
-0000dc90: 2069 6e20 796f 7572 2069 6e76 656e 746f   in your invento
-0000dca0: 7279 2e0a 0a20 2020 2020 2020 2056 616c  ry...        Val
-0000dcb0: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
-0000dcc0: 2049 4e56 454e 544f 5259 5f53 5441 5455   INVENTORY_STATU
-0000dcd0: 535f 554e 5350 4543 4946 4945 4420 2830  S_UNSPECIFIED (0
-0000dce0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000dcf0: 2020 204e 6f74 2073 7065 6369 6669 6564     Not specified
-0000dd00: 2e0a 2020 2020 2020 2020 2020 2020 494e  ..            IN
-0000dd10: 5f53 544f 434b 2028 3129 3a0a 2020 2020  _STOCK (1):.    
-0000dd20: 2020 2020 2020 2020 2020 2020 596f 7520              You 
-0000dd30: 6861 7665 2061 2070 726f 6475 6374 2066  have a product f
-0000dd40: 6f72 2074 6869 7320 7072 6f64 7563 7420  or this product 
-0000dd50: 636c 7573 7465 720a 2020 2020 2020 2020  cluster.        
-0000dd60: 2020 2020 2020 2020 6f72 2062 7261 6e64          or brand
-0000dd70: 2069 6e20 7374 6f63 6b2e 0a20 2020 2020   in stock..     
-0000dd80: 2020 2020 2020 204f 5554 5f4f 465f 5354         OUT_OF_ST
-0000dd90: 4f43 4b20 2832 293a 0a20 2020 2020 2020  OCK (2):.       
-0000dda0: 2020 2020 2020 2020 2059 6f75 2068 6176           You hav
-0000ddb0: 6520 6120 7072 6f64 7563 7420 666f 7220  e a product for 
-0000ddc0: 7468 6973 2070 726f 6475 6374 2063 6c75  this product clu
-0000ddd0: 7374 6572 0a20 2020 2020 2020 2020 2020  ster.           
-0000dde0: 2020 2020 206f 7220 6272 616e 6420 696e       or brand in
-0000ddf0: 2069 6e76 656e 746f 7279 2062 7574 2069   inventory but i
-0000de00: 7420 6973 2063 7572 7265 6e74 6c79 206f  t is currently o
-0000de10: 7574 206f 660a 2020 2020 2020 2020 2020  ut of.          
-0000de20: 2020 2020 2020 7374 6f63 6b2e 0a20 2020        stock..   
-0000de30: 2020 2020 2020 2020 204e 4f54 5f49 4e5f           NOT_IN_
-0000de40: 494e 5645 4e54 4f52 5920 2833 293a 0a20  INVENTORY (3):. 
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
-0000de60: 6f75 2064 6f20 6e6f 7420 6861 7665 2061  ou do not have a
-0000de70: 2070 726f 6475 6374 2066 6f72 2074 6869   product for thi
-0000de80: 7320 7072 6f64 7563 740a 2020 2020 2020  s product.      
-0000de90: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0000dea0: 7220 6f72 2062 7261 6e64 2069 6e20 696e  r or brand in in
-0000deb0: 7665 6e74 6f72 792e 0a20 2020 2020 2020  ventory..       
-0000dec0: 2022 2222 0a20 2020 2020 2020 2049 4e56   """.        INV
-0000ded0: 454e 544f 5259 5f53 5441 5455 535f 554e  ENTORY_STATUS_UN
-0000dee0: 5350 4543 4946 4945 4420 3d20 300a 2020  SPECIFIED = 0.  
-0000def0: 2020 2020 2020 494e 5f53 544f 434b 203d        IN_STOCK =
-0000df00: 2031 0a20 2020 2020 2020 204f 5554 5f4f   1.        OUT_O
-0000df10: 465f 5354 4f43 4b20 3d20 320a 2020 2020  F_STOCK = 2.    
-0000df20: 2020 2020 4e4f 545f 494e 5f49 4e56 454e      NOT_IN_INVEN
-0000df30: 544f 5259 203d 2033 0a0a 2020 2020 7265  TORY = 3..    re
-0000df40: 706f 7274 5f64 6174 653a 2064 6174 655f  port_date: date_
-0000df50: 7062 322e 4461 7465 203d 2070 726f 746f  pb2.Date = proto
-0000df60: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000df70: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-0000df80: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
-0000df90: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-0000dfa0: 3d64 6174 655f 7062 322e 4461 7465 2c0a  =date_pb2.Date,.
-0000dfb0: 2020 2020 290a 2020 2020 7265 706f 7274      ).    report
-0000dfc0: 5f67 7261 6e75 6c61 7269 7479 3a20 2252  _granularity: "R
-0000dfd0: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
-0000dfe0: 2e52 6570 6f72 7447 7261 6e75 6c61 7269  .ReportGranulari
-0000dff0: 7479 456e 756d 2220 3d20 7072 6f74 6f2e  tyEnum" = proto.
-0000e000: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000e010: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
-0000e020: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
-0000e030: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000e040: 7565 2c0a 2020 2020 2020 2020 656e 756d  ue,.        enum
-0000e050: 3d22 5265 706f 7274 4772 616e 756c 6172  ="ReportGranular
-0000e060: 6974 792e 5265 706f 7274 4772 616e 756c  ity.ReportGranul
-0000e070: 6172 6974 7945 6e75 6d22 2c0a 2020 2020  arityEnum",.    
-0000e080: 290a 2020 2020 7265 706f 7274 5f63 6f75  ).    report_cou
-0000e090: 6e74 7279 5f63 6f64 653a 2073 7472 203d  ntry_code: str =
-0000e0a0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000e0b0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000e0c0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000e0d0: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
-0000e0e0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000e0f0: 2029 0a20 2020 2072 6570 6f72 745f 6361   ).    report_ca
-0000e100: 7465 676f 7279 5f69 643a 2069 6e74 203d  tegory_id: int =
-0000e110: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000e120: 2020 2020 2020 7072 6f74 6f2e 494e 5436        proto.INT6
-0000e130: 342c 0a20 2020 2020 2020 206e 756d 6265  4,.        numbe
-0000e140: 723d 342c 0a20 2020 2020 2020 206f 7074  r=4,.        opt
-0000e150: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000e160: 290a 2020 2020 7469 746c 653a 2073 7472  ).    title: str
-0000e170: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000e180: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-0000e190: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-0000e1a0: 6d62 6572 3d36 2c0a 2020 2020 2020 2020  mber=6,.        
-0000e1b0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000e1c0: 2020 2029 0a20 2020 2062 7261 6e64 3a20     ).    brand: 
-0000e1d0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000e1e0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000e1f0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000e200: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
-0000e210: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000e220: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
-0000e230: 676f 7279 5f6c 313a 2073 7472 203d 2070  gory_l1: str = p
-0000e240: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000e250: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-0000e260: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000e270: 3d38 2c0a 2020 2020 2020 2020 6f70 7469  =8,.        opti
-0000e280: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000e290: 0a20 2020 2063 6174 6567 6f72 795f 6c32  .    category_l2
-0000e2a0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000e2b0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000e2c0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000e2d0: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
-0000e2e0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000e2f0: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
-0000e300: 7465 676f 7279 5f6c 333a 2073 7472 203d  tegory_l3: str =
-0000e310: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000e320: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000e330: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000e340: 6572 3d31 302c 0a20 2020 2020 2020 206f  er=10,.        o
-0000e350: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-0000e360: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-0000e370: 5f6c 343a 2073 7472 203d 2070 726f 746f  _l4: str = proto
-0000e380: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000e390: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000e3a0: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
-0000e3b0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-0000e3c0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-0000e3d0: 2020 6361 7465 676f 7279 5f6c 353a 2073    category_l5: s
-0000e3e0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-0000e3f0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000e400: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-0000e410: 6e75 6d62 6572 3d31 322c 0a20 2020 2020  number=12,.     
-0000e420: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000e430: 2c0a 2020 2020 290a 2020 2020 7661 7269  ,.    ).    vari
-0000e440: 616e 745f 6774 696e 733a 204d 7574 6162  ant_gtins: Mutab
-0000e450: 6c65 5365 7175 656e 6365 5b73 7472 5d20  leSequence[str] 
-0000e460: 3d20 7072 6f74 6f2e 5265 7065 6174 6564  = proto.Repeated
-0000e470: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000e480: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000e490: 2020 2020 206e 756d 6265 723d 3133 2c0a       number=13,.
-0000e4a0: 2020 2020 290a 2020 2020 696e 7665 6e74      ).    invent
-0000e4b0: 6f72 795f 7374 6174 7573 3a20 496e 7665  ory_status: Inve
-0000e4c0: 6e74 6f72 7953 7461 7475 7320 3d20 7072  ntoryStatus = pr
-0000e4d0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000e4e0: 2020 2070 726f 746f 2e45 4e55 4d2c 0a20     proto.ENUM,. 
-0000e4f0: 2020 2020 2020 206e 756d 6265 723d 3134         number=14
-0000e500: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0000e510: 616c 3d54 7275 652c 0a20 2020 2020 2020  al=True,.       
-0000e520: 2065 6e75 6d3d 496e 7665 6e74 6f72 7953   enum=InventoryS
-0000e530: 7461 7475 732c 0a20 2020 2029 0a20 2020  tatus,.    ).   
-0000e540: 2062 7261 6e64 5f69 6e76 656e 746f 7279   brand_inventory
-0000e550: 5f73 7461 7475 733a 2049 6e76 656e 746f  _status: Invento
-0000e560: 7279 5374 6174 7573 203d 2070 726f 746f  ryStatus = proto
-0000e570: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000e580: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
-0000e590: 2020 2020 6e75 6d62 6572 3d31 352c 0a20      number=15,. 
-0000e5a0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000e5b0: 5472 7565 2c0a 2020 2020 2020 2020 656e  True,.        en
-0000e5c0: 756d 3d49 6e76 656e 746f 7279 5374 6174  um=InventoryStat
-0000e5d0: 7573 2c0a 2020 2020 290a 2020 2020 7261  us,.    ).    ra
-0000e5e0: 6e6b 3a20 696e 7420 3d20 7072 6f74 6f2e  nk: int = proto.
-0000e5f0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000e600: 726f 746f 2e49 4e54 3634 2c0a 2020 2020  roto.INT64,.    
-0000e610: 2020 2020 6e75 6d62 6572 3d31 362c 0a20      number=16,. 
-0000e620: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000e630: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000e640: 7072 6576 696f 7573 5f72 616e 6b3a 2069  previous_rank: i
-0000e650: 6e74 203d 2070 726f 746f 2e46 6965 6c64  nt = proto.Field
-0000e660: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000e670: 494e 5436 342c 0a20 2020 2020 2020 206e  INT64,.        n
-0000e680: 756d 6265 723d 3137 2c0a 2020 2020 2020  umber=17,.      
-0000e690: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000e6a0: 0a20 2020 2029 0a20 2020 2072 656c 6174  .    ).    relat
-0000e6b0: 6976 655f 6465 6d61 6e64 3a20 2252 656c  ive_demand: "Rel
-0000e6c0: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
-0000e6d0: 7469 7665 4465 6d61 6e64 456e 756d 2220  tiveDemandEnum" 
-0000e6e0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000e6f0: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-0000e700: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
-0000e710: 723d 3138 2c0a 2020 2020 2020 2020 6f70  r=18,.        op
-0000e720: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000e730: 2020 2020 2065 6e75 6d3d 2252 656c 6174       enum="Relat
-0000e740: 6976 6544 656d 616e 642e 5265 6c61 7469  iveDemand.Relati
-0000e750: 7665 4465 6d61 6e64 456e 756d 222c 0a20  veDemandEnum",. 
-0000e760: 2020 2029 0a20 2020 2070 7265 7669 6f75     ).    previou
-0000e770: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
-0000e780: 643a 2022 5265 6c61 7469 7665 4465 6d61  d: "RelativeDema
-0000e790: 6e64 2e52 656c 6174 6976 6544 656d 616e  nd.RelativeDeman
-0000e7a0: 6445 6e75 6d22 203d 2070 726f 746f 2e46  dEnum" = proto.F
-0000e7b0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000e7c0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
-0000e7d0: 2020 6e75 6d62 6572 3d31 392c 0a20 2020    number=19,.   
-0000e7e0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000e7f0: 7565 2c0a 2020 2020 2020 2020 656e 756d  ue,.        enum
-0000e800: 3d22 5265 6c61 7469 7665 4465 6d61 6e64  ="RelativeDemand
-0000e810: 2e52 656c 6174 6976 6544 656d 616e 6445  .RelativeDemandE
+00007d00: 2072 6570 6f72 7469 6e67 2063 6f6e 7465   reporting conte
+00007d10: 7874 2e0a 2020 2020 2020 2020 2020 2020  xt..            
+00007d20: 2020 2020 2020 2020 4445 4d4f 5445 4420          DEMOTED 
+00007d30: 2832 293a 0a20 2020 2020 2020 2020 2020  (2):.           
+00007d40: 2020 2020 2020 2020 2020 2020 2049 7373               Iss
+00007d50: 7565 2064 656d 6f74 6573 2074 6865 2070  ue demotes the p
+00007d60: 726f 6475 6374 2069 6e20 616c 6c20 7265  roduct in all re
+00007d70: 706f 7274 696e 670a 2020 2020 2020 2020  porting.        
+00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d90: 636f 6e74 6578 7473 2069 7420 6166 6665  contexts it affe
+00007da0: 6374 732e 0a20 2020 2020 2020 2020 2020  cts..           
+00007db0: 2020 2020 2020 2020 2050 454e 4449 4e47           PENDING
+00007dc0: 2028 3329 3a0a 2020 2020 2020 2020 2020   (3):.          
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 4973                Is
+00007de0: 7375 6520 7265 736f 6c75 7469 6f6e 2069  sue resolution i
+00007df0: 7320 6060 5045 4e44 494e 475f 5052 4f43  s ``PENDING_PROC
+00007e00: 4553 5349 4e47 6060 2e0a 2020 2020 2020  ESSING``..      
+00007e10: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+00007e20: 2020 2020 2020 2020 2020 2020 2020 4147                AG
+00007e30: 4752 4547 4154 4544 5f49 5353 5545 5f53  GREGATED_ISSUE_S
+00007e40: 4556 4552 4954 595f 554e 5350 4543 4946  EVERITY_UNSPECIF
+00007e50: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
+00007e60: 2020 2020 2020 2020 4449 5341 5050 524f          DISAPPRO
+00007e70: 5645 4420 3d20 310a 2020 2020 2020 2020  VED = 1.        
+00007e80: 2020 2020 2020 2020 4445 4d4f 5445 4420          DEMOTED 
+00007e90: 3d20 320a 2020 2020 2020 2020 2020 2020  = 2.            
+00007ea0: 2020 2020 5045 4e44 494e 4720 3d20 330a      PENDING = 3.
+00007eb0: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
+00007ec0: 7373 2049 7373 7565 5365 7665 7269 7479  ss IssueSeverity
+00007ed0: 5065 7252 6570 6f72 7469 6e67 436f 6e74  PerReportingCont
+00007ee0: 6578 7428 7072 6f74 6f2e 4d65 7373 6167  ext(proto.Messag
+00007ef0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00007f00: 2020 2020 7222 2222 4973 7375 6520 7365      r"""Issue se
+00007f10: 7665 7269 7479 2070 6572 2072 6570 6f72  verity per repor
+00007f20: 7469 6e67 2063 6f6e 7465 7874 2e0a 0a20  ting context... 
+00007f30: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00007f40: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
+00007f50: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
+00007f60: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+00007f70: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
+00007f80: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
+00007f90: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
+00007fa0: 7665 2d66 6965 6c64 730a 0a20 2020 2020  ve-fields..     
+00007fb0: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
+00007fc0: 6275 7465 733a 0a20 2020 2020 2020 2020  butes:.         
+00007fd0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+00007fe0: 7469 6e67 5f63 6f6e 7465 7874 2028 676f  ting_context (go
+00007ff0: 6f67 6c65 2e73 686f 7070 696e 672e 7479  ogle.shopping.ty
+00008000: 7065 2e74 7970 6573 2e52 6570 6f72 7469  pe.types.Reporti
+00008010: 6e67 436f 6e74 6578 742e 5265 706f 7274  ngContext.Report
+00008020: 696e 6743 6f6e 7465 7874 456e 756d 293a  ingContextEnum):
+00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008040: 2020 2020 2020 2020 2052 6570 6f72 7469           Reporti
+00008050: 6e67 2063 6f6e 7465 7874 2074 6865 2069  ng context the i
+00008060: 7373 7565 2061 7070 6c69 6573 2074 6f2e  ssue applies to.
+00008070: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008080: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00008090: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000080a0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+000080b0: 7265 706f 7274 696e 675f 636f 6e74 6578  reporting_contex
+000080c0: 7460 602e 0a20 2020 2020 2020 2020 2020  t``..           
+000080d0: 2020 2020 2020 2020 2064 6973 6170 7072           disappr
+000080e0: 6f76 6564 5f63 6f75 6e74 7269 6573 2028  oved_countries (
+000080f0: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
+00008100: 7374 725d 293a 0a20 2020 2020 2020 2020  str]):.         
+00008110: 2020 2020 2020 2020 2020 2020 2020 204c                 L
+00008120: 6973 7420 6f66 2064 6973 6170 7072 6f76  ist of disapprov
+00008130: 6564 2063 6f75 6e74 7269 6573 2069 6e20  ed countries in 
+00008140: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00008150: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00008160: 7274 696e 6720 636f 6e74 6578 742c 2072  rting context, r
+00008170: 6570 7265 7365 6e74 6564 2069 6e20 4953  epresented in IS
+00008180: 4f20 3331 3636 0a20 2020 2020 2020 2020  O 3166.         
+00008190: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000081a0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+000081b0: 2020 2020 2020 2020 2020 2064 656d 6f74             demot
+000081c0: 6564 5f63 6f75 6e74 7269 6573 2028 4d75  ed_countries (Mu
+000081d0: 7461 626c 6553 6571 7565 6e63 655b 7374  tableSequence[st
+000081e0: 725d 293a 0a20 2020 2020 2020 2020 2020  r]):.           
+000081f0: 2020 2020 2020 2020 2020 2020 204c 6973               Lis
+00008200: 7420 6f66 2064 656d 6f74 6564 2063 6f75  t of demoted cou
+00008210: 6e74 7269 6573 2069 6e20 7468 6520 7265  ntries in the re
+00008220: 706f 7274 696e 670a 2020 2020 2020 2020  porting.        
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 636f 6e74 6578 742c 2072 6570 7265 7365  context, represe
+00008250: 6e74 6564 2069 6e20 4953 4f20 3331 3636  nted in ISO 3166
+00008260: 2066 6f72 6d61 742e 0a20 2020 2020 2020   format..       
+00008270: 2020 2020 2020 2020 2022 2222 0a0a 2020           """..  
+00008280: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00008290: 706f 7274 696e 675f 636f 6e74 6578 743a  porting_context:
+000082a0: 2074 7970 6573 2e52 6570 6f72 7469 6e67   types.Reporting
+000082b0: 436f 6e74 6578 742e 5265 706f 7274 696e  Context.Reportin
+000082c0: 6743 6f6e 7465 7874 456e 756d 203d 2028  gContextEnum = (
+000082d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000082e0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
+000082f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008300: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+00008310: 454e 554d 2c0a 2020 2020 2020 2020 2020  ENUM,.          
+00008320: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00008330: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008370: 2020 2020 2020 2065 6e75 6d3d 7479 7065         enum=type
+00008380: 732e 5265 706f 7274 696e 6743 6f6e 7465  s.ReportingConte
+00008390: 7874 2e52 6570 6f72 7469 6e67 436f 6e74  xt.ReportingCont
+000083a0: 6578 7445 6e75 6d2c 0a20 2020 2020 2020  extEnum,.       
+000083b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000083d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083e0: 2064 6973 6170 7072 6f76 6564 5f63 6f75   disapproved_cou
+000083f0: 6e74 7269 6573 3a20 4d75 7461 626c 6553  ntries: MutableS
+00008400: 6571 7565 6e63 655b 7374 725d 203d 2070  equence[str] = p
+00008410: 726f 746f 2e52 6570 6561 7465 6446 6965  roto.RepeatedFie
+00008420: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00008430: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+00008440: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
+00008450: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00008460: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+00008470: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00008480: 2020 2020 2020 6465 6d6f 7465 645f 636f        demoted_co
+00008490: 756e 7472 6965 733a 204d 7574 6162 6c65  untries: Mutable
+000084a0: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
+000084b0: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
+000084c0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000084d0: 2020 2020 2020 2020 2070 726f 746f 2e53           proto.S
+000084e0: 5452 494e 472c 0a20 2020 2020 2020 2020  TRING,.         
+000084f0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00008500: 723d 332c 0a20 2020 2020 2020 2020 2020  r=3,.           
+00008510: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00008520: 2020 2020 7365 7665 7269 7479 5f70 6572      severity_per
+00008530: 5f72 6570 6f72 7469 6e67 5f63 6f6e 7465  _reporting_conte
+00008540: 7874 3a20 4d75 7461 626c 6553 6571 7565  xt: MutableSeque
+00008550: 6e63 655b 0a20 2020 2020 2020 2020 2020  nce[.           
+00008560: 2020 2020 2022 5072 6f64 7563 7456 6965       "ProductVie
+00008570: 772e 4974 656d 4973 7375 652e 4974 656d  w.ItemIssue.Item
+00008580: 4973 7375 6553 6576 6572 6974 792e 4973  IssueSeverity.Is
+00008590: 7375 6553 6576 6572 6974 7950 6572 5265  sueSeverityPerRe
+000085a0: 706f 7274 696e 6743 6f6e 7465 7874 220a  portingContext".
+000085b0: 2020 2020 2020 2020 2020 2020 5d20 3d20              ] = 
+000085c0: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
+000085d0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000085e0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+000085f0: 4745 2c0a 2020 2020 2020 2020 2020 2020  GE,.            
+00008600: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
+00008610: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00008620: 7373 6167 653d 2250 726f 6475 6374 5669  ssage="ProductVi
+00008630: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
+00008640: 6d49 7373 7565 5365 7665 7269 7479 2e49  mIssueSeverity.I
+00008650: 7373 7565 5365 7665 7269 7479 5065 7252  ssueSeverityPerR
+00008660: 6570 6f72 7469 6e67 436f 6e74 6578 7422  eportingContext"
+00008670: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00008680: 2020 2020 2020 2020 2020 2020 6167 6772              aggr
+00008690: 6567 6174 6564 5f73 6576 6572 6974 793a  egated_severity:
+000086a0: 2022 5072 6f64 7563 7456 6965 772e 4974   "ProductView.It
+000086b0: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
+000086c0: 6553 6576 6572 6974 792e 4167 6772 6567  eSeverity.Aggreg
+000086d0: 6174 6564 4973 7375 6553 6576 6572 6974  atedIssueSeverit
+000086e0: 7922 203d 2070 726f 746f 2e46 6965 6c64  y" = proto.Field
+000086f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008700: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+00008710: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00008720: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
+00008730: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00008740: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00008750: 2020 2020 2020 2065 6e75 6d3d 2250 726f         enum="Pro
+00008760: 6475 6374 5669 6577 2e49 7465 6d49 7373  ductView.ItemIss
+00008770: 7565 2e49 7465 6d49 7373 7565 5365 7665  ue.ItemIssueSeve
+00008780: 7269 7479 2e41 6767 7265 6761 7465 6449  rity.AggregatedI
+00008790: 7373 7565 5365 7665 7269 7479 222c 0a20  ssueSeverity",. 
+000087a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000087b0: 2020 2020 2020 7479 7065 5f3a 2022 5072        type_: "Pr
+000087c0: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
+000087d0: 7375 652e 4974 656d 4973 7375 6554 7970  sue.ItemIssueTyp
+000087e0: 6522 203d 2070 726f 746f 2e46 6965 6c64  e" = proto.Field
+000087f0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00008800: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+00008810: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00008820: 312c 0a20 2020 2020 2020 2020 2020 206d  1,.            m
+00008830: 6573 7361 6765 3d22 5072 6f64 7563 7456  essage="ProductV
+00008840: 6965 772e 4974 656d 4973 7375 652e 4974  iew.ItemIssue.It
+00008850: 656d 4973 7375 6554 7970 6522 2c0a 2020  emIssueType",.  
+00008860: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008870: 7365 7665 7269 7479 3a20 2250 726f 6475  severity: "Produ
+00008880: 6374 5669 6577 2e49 7465 6d49 7373 7565  ctView.ItemIssue
+00008890: 2e49 7465 6d49 7373 7565 5365 7665 7269  .ItemIssueSeveri
+000088a0: 7479 2220 3d20 7072 6f74 6f2e 4669 656c  ty" = proto.Fiel
+000088b0: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
+000088c0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+000088d0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+000088e0: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+000088f0: 6d65 7373 6167 653d 2250 726f 6475 6374  message="Product
+00008900: 5669 6577 2e49 7465 6d49 7373 7565 2e49  View.ItemIssue.I
+00008910: 7465 6d49 7373 7565 5365 7665 7269 7479  temIssueSeverity
+00008920: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+00008930: 2020 2020 2072 6573 6f6c 7574 696f 6e3a       resolution:
+00008940: 2022 5072 6f64 7563 7456 6965 772e 4974   "ProductView.It
+00008950: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
+00008960: 6552 6573 6f6c 7574 696f 6e22 203d 2070  eResolution" = p
+00008970: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00008980: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
+00008990: 554d 2c0a 2020 2020 2020 2020 2020 2020  UM,.            
+000089a0: 6e75 6d62 6572 3d33 2c0a 2020 2020 2020  number=3,.      
+000089b0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000089c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000089d0: 2065 6e75 6d3d 2250 726f 6475 6374 5669   enum="ProductVi
+000089e0: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
+000089f0: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
+00008a00: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+00008a10: 2020 6964 3a20 7374 7220 3d20 7072 6f74    id: str = prot
+00008a20: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00008a30: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00008a40: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
+00008a50: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00008a60: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00008a70: 2020 6368 616e 6e65 6c3a 2074 7970 6573    channel: types
+00008a80: 2e43 6861 6e6e 656c 2e43 6861 6e6e 656c  .Channel.Channel
+00008a90: 456e 756d 203d 2070 726f 746f 2e46 6965  Enum = proto.Fie
+00008aa0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00008ab0: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
+00008ac0: 6e75 6d62 6572 3d32 382c 0a20 2020 2020  number=28,.     
+00008ad0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00008ae0: 2c0a 2020 2020 2020 2020 656e 756d 3d74  ,.        enum=t
+00008af0: 7970 6573 2e43 6861 6e6e 656c 2e43 6861  ypes.Channel.Cha
+00008b00: 6e6e 656c 456e 756d 2c0a 2020 2020 290a  nnelEnum,.    ).
+00008b10: 2020 2020 6c61 6e67 7561 6765 5f63 6f64      language_cod
+00008b20: 653a 2073 7472 203d 2070 726f 746f 2e46  e: str = proto.F
+00008b30: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00008b40: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00008b50: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+00008b60: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00008b70: 7275 652c 0a20 2020 2029 0a20 2020 2066  rue,.    ).    f
+00008b80: 6565 645f 6c61 6265 6c3a 2073 7472 203d  eed_label: str =
+00008b90: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00008ba0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00008bb0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00008bc0: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
+00008bd0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00008be0: 2029 0a20 2020 206f 6666 6572 5f69 643a   ).    offer_id:
+00008bf0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00008c00: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00008c10: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00008c20: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
+00008c30: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00008c40: 652c 0a20 2020 2029 0a20 2020 2074 6974  e,.    ).    tit
+00008c50: 6c65 3a20 7374 7220 3d20 7072 6f74 6f2e  le: str = proto.
+00008c60: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00008c70: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00008c80: 2020 2020 206e 756d 6265 723d 352c 0a20       number=5,. 
+00008c90: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00008ca0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00008cb0: 6272 616e 643a 2073 7472 203d 2070 726f  brand: str = pro
+00008cc0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00008cd0: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+00008ce0: 2020 2020 2020 2020 6e75 6d62 6572 3d36          number=6
+00008cf0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00008d00: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00008d10: 2020 2063 6174 6567 6f72 795f 6c31 3a20     category_l1: 
+00008d20: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+00008d30: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00008d40: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+00008d50: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
+00008d60: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00008d70: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
+00008d80: 676f 7279 5f6c 323a 2073 7472 203d 2070  gory_l2: str = p
+00008d90: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00008da0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00008db0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00008dc0: 3d38 2c0a 2020 2020 2020 2020 6f70 7469  =8,.        opti
+00008dd0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00008de0: 0a20 2020 2063 6174 6567 6f72 795f 6c33  .    category_l3
+00008df0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+00008e00: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00008e10: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00008e20: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
+00008e30: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00008e40: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
+00008e50: 7465 676f 7279 5f6c 343a 2073 7472 203d  tegory_l4: str =
+00008e60: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00008e70: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00008e80: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00008e90: 6572 3d31 302c 0a20 2020 2020 2020 206f  er=10,.        o
+00008ea0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00008eb0: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
+00008ec0: 5f6c 353a 2073 7472 203d 2070 726f 746f  _l5: str = proto
+00008ed0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00008ee0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+00008ef0: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
+00008f00: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00008f10: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00008f20: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
+00008f30: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
+00008f40: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00008f50: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00008f60: 2020 2020 6e75 6d62 6572 3d31 322c 0a20      number=12,. 
+00008f70: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00008f80: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00008f90: 7072 6f64 7563 745f 7479 7065 5f6c 323a  product_type_l2:
+00008fa0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00008fb0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00008fc0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00008fd0: 2020 6e75 6d62 6572 3d31 332c 0a20 2020    number=13,.   
+00008fe0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00008ff0: 7565 2c0a 2020 2020 290a 2020 2020 7072  ue,.    ).    pr
+00009000: 6f64 7563 745f 7479 7065 5f6c 333a 2073  oduct_type_l3: s
+00009010: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00009020: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00009030: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+00009040: 6e75 6d62 6572 3d31 342c 0a20 2020 2020  number=14,.     
+00009050: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00009060: 2c0a 2020 2020 290a 2020 2020 7072 6f64  ,.    ).    prod
+00009070: 7563 745f 7479 7065 5f6c 343a 2073 7472  uct_type_l4: str
+00009080: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00009090: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+000090a0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+000090b0: 6d62 6572 3d31 352c 0a20 2020 2020 2020  mber=15,.       
+000090c0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+000090d0: 2020 2020 290a 2020 2020 7072 6f64 7563      ).    produc
+000090e0: 745f 7479 7065 5f6c 353a 2073 7472 203d  t_type_l5: str =
+000090f0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00009100: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00009110: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00009120: 6572 3d31 362c 0a20 2020 2020 2020 206f  er=16,.        o
+00009130: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00009140: 2020 290a 2020 2020 7072 6963 653a 2074    ).    price: t
+00009150: 7970 6573 2e50 7269 6365 203d 2070 726f  ypes.Price = pro
+00009160: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00009170: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+00009180: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00009190: 3137 2c0a 2020 2020 2020 2020 6d65 7373  17,.        mess
+000091a0: 6167 653d 7479 7065 732e 5072 6963 652c  age=types.Price,
+000091b0: 0a20 2020 2029 0a20 2020 2063 6f6e 6469  .    ).    condi
+000091c0: 7469 6f6e 3a20 7374 7220 3d20 7072 6f74  tion: str = prot
+000091d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000091e0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+000091f0: 2020 2020 2020 206e 756d 6265 723d 3138         number=18
+00009200: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00009210: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00009220: 2020 2061 7661 696c 6162 696c 6974 793a     availability:
+00009230: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00009240: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00009250: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00009260: 2020 6e75 6d62 6572 3d31 392c 0a20 2020    number=19,.   
+00009270: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00009280: 7565 2c0a 2020 2020 290a 2020 2020 7368  ue,.    ).    sh
+00009290: 6970 7069 6e67 5f6c 6162 656c 3a20 7374  ipping_label: st
+000092a0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+000092b0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000092c0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+000092d0: 756d 6265 723d 3230 2c0a 2020 2020 2020  umber=20,.      
+000092e0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+000092f0: 0a20 2020 2029 0a20 2020 2067 7469 6e3a  .    ).    gtin:
+00009300: 204d 7574 6162 6c65 5365 7175 656e 6365   MutableSequence
+00009310: 5b73 7472 5d20 3d20 7072 6f74 6f2e 5265  [str] = proto.Re
+00009320: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
+00009330: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00009340: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00009350: 723d 3231 2c0a 2020 2020 290a 2020 2020  r=21,.    ).    
+00009360: 6974 656d 5f67 726f 7570 5f69 643a 2073  item_group_id: s
+00009370: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00009380: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00009390: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+000093a0: 6e75 6d62 6572 3d32 322c 0a20 2020 2020  number=22,.     
+000093b0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+000093c0: 2c0a 2020 2020 290a 2020 2020 7468 756d  ,.    ).    thum
+000093d0: 626e 6169 6c5f 6c69 6e6b 3a20 7374 7220  bnail_link: str 
+000093e0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+000093f0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00009400: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00009410: 6265 723d 3233 2c0a 2020 2020 2020 2020  ber=23,.        
+00009420: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00009430: 2020 2029 0a20 2020 2063 7265 6174 696f     ).    creatio
+00009440: 6e5f 7469 6d65 3a20 7469 6d65 7374 616d  n_time: timestam
+00009450: 705f 7062 322e 5469 6d65 7374 616d 7020  p_pb2.Timestamp 
+00009460: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00009470: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00009480: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00009490: 6d62 6572 3d32 342c 0a20 2020 2020 2020  mber=24,.       
+000094a0: 206d 6573 7361 6765 3d74 696d 6573 7461   message=timesta
+000094b0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
+000094c0: 2c0a 2020 2020 290a 2020 2020 6578 7069  ,.    ).    expi
+000094d0: 7261 7469 6f6e 5f64 6174 653a 2064 6174  ration_date: dat
+000094e0: 655f 7062 322e 4461 7465 203d 2070 726f  e_pb2.Date = pro
+000094f0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00009500: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+00009510: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00009520: 3235 2c0a 2020 2020 2020 2020 6d65 7373  25,.        mess
+00009530: 6167 653d 6461 7465 5f70 6232 2e44 6174  age=date_pb2.Dat
+00009540: 652c 0a20 2020 2029 0a20 2020 2061 6767  e,.    ).    agg
+00009550: 7265 6761 7465 645f 7265 706f 7274 696e  regated_reportin
+00009560: 675f 636f 6e74 6578 745f 7374 6174 7573  g_context_status
+00009570: 3a20 4167 6772 6567 6174 6564 5265 706f  : AggregatedRepo
+00009580: 7274 696e 6743 6f6e 7465 7874 5374 6174  rtingContextStat
+00009590: 7573 203d 2070 726f 746f 2e46 6965 6c64  us = proto.Field
+000095a0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+000095b0: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+000095c0: 6d62 6572 3d32 362c 0a20 2020 2020 2020  mber=26,.       
+000095d0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+000095e0: 2020 2020 2020 2020 656e 756d 3d41 6767          enum=Agg
+000095f0: 7265 6761 7465 6452 6570 6f72 7469 6e67  regatedReporting
+00009600: 436f 6e74 6578 7453 7461 7475 732c 0a20  ContextStatus,. 
+00009610: 2020 2029 0a20 2020 2069 7465 6d5f 6973     ).    item_is
+00009620: 7375 6573 3a20 4d75 7461 626c 6553 6571  sues: MutableSeq
+00009630: 7565 6e63 655b 4974 656d 4973 7375 655d  uence[ItemIssue]
+00009640: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+00009650: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+00009660: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00009670: 2020 2020 2020 206e 756d 6265 723d 3237         number=27
+00009680: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00009690: 653d 4974 656d 4973 7375 652c 0a20 2020  e=ItemIssue,.   
+000096a0: 2029 0a20 2020 2063 6c69 636b 5f70 6f74   ).    click_pot
+000096b0: 656e 7469 616c 3a20 436c 6963 6b50 6f74  ential: ClickPot
+000096c0: 656e 7469 616c 203d 2070 726f 746f 2e46  ential = proto.F
+000096d0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+000096e0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
+000096f0: 2020 6e75 6d62 6572 3d32 392c 0a20 2020    number=29,.   
+00009700: 2020 2020 2065 6e75 6d3d 436c 6963 6b50       enum=ClickP
+00009710: 6f74 656e 7469 616c 2c0a 2020 2020 290a  otential,.    ).
+00009720: 2020 2020 636c 6963 6b5f 706f 7465 6e74      click_potent
+00009730: 6961 6c5f 7261 6e6b 3a20 696e 7420 3d20  ial_rank: int = 
+00009740: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00009750: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
+00009760: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00009770: 3d33 302c 0a20 2020 2020 2020 206f 7074  =30,.        opt
+00009780: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00009790: 290a 0a0a 636c 6173 7320 5072 6963 6543  )...class PriceC
+000097a0: 6f6d 7065 7469 7469 7665 6e65 7373 5072  ompetitivenessPr
+000097b0: 6f64 7563 7456 6965 7728 7072 6f74 6f2e  oductView(proto.
+000097c0: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+000097d0: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
+000097e0: 6c65 2066 6f72 2071 7565 7279 2069 6e20  le for query in 
+000097f0: 6060 7072 6963 655f 636f 6d70 6574 6974  ``price_competit
+00009800: 6976 656e 6573 735f 7072 6f64 7563 745f  iveness_product_
+00009810: 7669 6577 6060 0a20 2020 2074 6162 6c65  view``.    table
+00009820: 2e0a 0a20 2020 2060 5072 6963 650a 2020  ...    `Price.  
+00009830: 2020 636f 6d70 6574 6974 6976 656e 6573    competitivenes
+00009840: 7320 3c68 7474 7073 3a2f 2f73 7570 706f  s <https://suppo
+00009850: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+00009860: 7263 6861 6e74 732f 616e 7377 6572 2f39  rchants/answer/9
+00009870: 3632 3639 3033 3e60 5f5f 0a20 2020 2072  626903>`__.    r
+00009880: 6570 6f72 742e 0a0a 2020 2020 5661 6c75  eport...    Valu
+00009890: 6573 2061 7265 206f 6e6c 7920 7365 7420  es are only set 
+000098a0: 666f 7220 6669 656c 6473 2072 6571 7565  for fields reque
+000098b0: 7374 6564 2065 7870 6c69 6369 746c 7920  sted explicitly 
+000098c0: 696e 2074 6865 2072 6571 7565 7374 2773  in the request's
+000098d0: 0a20 2020 2073 6561 7263 6820 7175 6572  .    search quer
+000098e0: 792e 0a0a 0a20 2020 202e 2e20 5f6f 6e65  y....    .. _one
+000098f0: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
+00009900: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
+00009910: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00009920: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
+00009930: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
+00009940: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
+00009950: 6c64 730a 0a20 2020 2041 7474 7269 6275  lds..    Attribu
+00009960: 7465 733a 0a20 2020 2020 2020 2072 6570  tes:.        rep
+00009970: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+00009980: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00009990: 2020 2020 436f 756e 7472 7920 6f66 2074      Country of t
+000099a0: 6865 2070 7269 6365 2062 656e 6368 6d61  he price benchma
+000099b0: 726b 2e20 5265 7072 6573 656e 7465 6420  rk. Represented 
+000099c0: 696e 2074 6865 2049 534f 2033 3136 360a  in the ISO 3166.
+000099d0: 2020 2020 2020 2020 2020 2020 666f 726d              form
+000099e0: 6174 2e0a 0a20 2020 2020 2020 2020 2020  at...           
+000099f0: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
+00009a00: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
+00009a10: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+00009a20: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00009a30: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00009a40: 6660 5f20 6060 5f72 6570 6f72 745f 636f  f`_ ``_report_co
+00009a50: 756e 7472 795f 636f 6465 6060 2e0a 2020  untry_code``..  
+00009a60: 2020 2020 2020 6964 2028 7374 7229 3a0a        id (str):.
+00009a70: 2020 2020 2020 2020 2020 2020 5245 5354              REST
+00009a80: 2049 4420 6f66 2074 6865 2070 726f 6475   ID of the produ
+00009a90: 6374 2c20 696e 2074 6865 2066 6f72 6d20  ct, in the form 
+00009aa0: 6f66 0a20 2020 2020 2020 2020 2020 2060  of.            `
+00009ab0: 6063 6861 6e6e 656c 7e6c 616e 6775 6167  `channel~languag
+00009ac0: 6543 6f64 657e 6665 6564 4c61 6265 6c7e  eCode~feedLabel~
+00009ad0: 6f66 6665 7249 6460 602e 2043 616e 2062  offerId``. Can b
+00009ae0: 6520 7573 6564 2074 6f0a 2020 2020 2020  e used to.      
+00009af0: 2020 2020 2020 6a6f 696e 2064 6174 6120        join data 
+00009b00: 7769 7468 2074 6865 2060 6070 726f 6475  with the ``produ
+00009b10: 6374 5f76 6965 7760 6020 7461 626c 652e  ct_view`` table.
+00009b20: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00009b30: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+00009b40: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
+00009b50: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00009b60: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00009b70: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00009b80: 2060 605f 6964 6060 2e0a 2020 2020 2020   ``_id``..      
+00009b90: 2020 6f66 6665 725f 6964 2028 7374 7229    offer_id (str)
+00009ba0: 3a0a 2020 2020 2020 2020 2020 2020 4d65  :.            Me
+00009bb0: 7263 6861 6e74 2d70 726f 7669 6465 6420  rchant-provided 
+00009bc0: 6964 206f 6620 7468 6520 7072 6f64 7563  id of the produc
+00009bd0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+00009be0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00009bf0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00009c00: 605f 2060 605f 6f66 6665 725f 6964 6060  `_ ``_offer_id``
+00009c10: 2e0a 2020 2020 2020 2020 7469 746c 6520  ..        title 
+00009c20: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00009c30: 2020 2054 6974 6c65 206f 6620 7468 6520     Title of the 
+00009c40: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
+00009c50: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00009c60: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00009c70: 606f 6e65 6f66 605f 2060 605f 7469 746c  `oneof`_ ``_titl
+00009c80: 6560 602e 0a20 2020 2020 2020 2062 7261  e``..        bra
+00009c90: 6e64 2028 7374 7229 3a0a 2020 2020 2020  nd (str):.      
+00009ca0: 2020 2020 2020 4272 616e 6420 6f66 2074        Brand of t
+00009cb0: 6865 2070 726f 6475 6374 2e0a 0a20 2020  he product...   
+00009cc0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00009cd0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+00009ce0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f62  of `oneof`_ ``_b
+00009cf0: 7261 6e64 6060 2e0a 2020 2020 2020 2020  rand``..        
+00009d00: 6361 7465 676f 7279 5f6c 3120 2873 7472  category_l1 (str
+00009d10: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
+00009d20: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00009d30: 2831 7374 206c 6576 656c 2920 696e 2060  (1st level) in `
+00009d40: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
+00009d50: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
+00009d60: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
+00009d70: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
+00009d80: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
+00009d90: 6572 2f36 3332 3434 3336 3e60 5f5f 2e0a  er/6324436>`__..
+00009da0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00009db0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00009dc0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00009dd0: 6060 5f63 6174 6567 6f72 795f 6c31 6060  ``_category_l1``
+00009de0: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
+00009df0: 7279 5f6c 3220 2873 7472 293a 0a20 2020  ry_l2 (str):.   
+00009e00: 2020 2020 2020 2020 2050 726f 6475 6374           Product
+00009e10: 2063 6174 6567 6f72 7920 2832 6e64 206c   category (2nd l
+00009e20: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
+00009e30: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
+00009e40: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
+00009e50: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
+00009e60: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
+00009e70: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
+00009e80: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
+00009e90: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00009ea0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00009eb0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
+00009ec0: 6567 6f72 795f 6c32 6060 2e0a 2020 2020  egory_l2``..    
+00009ed0: 2020 2020 6361 7465 676f 7279 5f6c 3320      category_l3 
+00009ee0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00009ef0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
+00009f00: 6f72 7920 2833 7264 206c 6576 656c 2920  ory (3rd level) 
+00009f10: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+00009f20: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+00009f30: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+00009f40: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+00009f50: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+00009f60: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+00009f70: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+00009f80: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00009f90: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00009fa0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
+00009fb0: 6c33 6060 2e0a 2020 2020 2020 2020 6361  l3``..        ca
+00009fc0: 7465 676f 7279 5f6c 3420 2873 7472 293a  tegory_l4 (str):
+00009fd0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
+00009fe0: 6475 6374 2063 6174 6567 6f72 7920 2834  duct category (4
+00009ff0: 7468 206c 6576 656c 2920 696e 2060 476f  th level) in `Go
+0000a000: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
+0000a010: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
+0000a020: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
+0000a030: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000a040: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000a050: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
+0000a060: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000a070: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000a080: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000a090: 5f63 6174 6567 6f72 795f 6c34 6060 2e0a  _category_l4``..
+0000a0a0: 2020 2020 2020 2020 6361 7465 676f 7279          category
+0000a0b0: 5f6c 3520 2873 7472 293a 0a20 2020 2020  _l5 (str):.     
+0000a0c0: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
+0000a0d0: 6174 6567 6f72 7920 2835 7468 206c 6576  ategory (5th lev
+0000a0e0: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
+0000a0f0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
+0000a100: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
+0000a110: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000a120: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000a130: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
+0000a140: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
+0000a150: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000a160: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000a170: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
+0000a180: 6f72 795f 6c35 6060 2e0a 2020 2020 2020  ory_l5``..      
+0000a190: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
+0000a1a0: 3120 2873 7472 293a 0a20 2020 2020 2020  1 (str):.       
+0000a1b0: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
+0000a1c0: 6520 2831 7374 206c 6576 656c 2920 696e  e (1st level) in
+0000a1d0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
+0000a1e0: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
+0000a1f0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
+0000a200: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000a210: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000a220: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
+0000a230: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
+0000a240: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000a250: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000a260: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
+0000a270: 6374 5f74 7970 655f 6c31 6060 2e0a 2020  ct_type_l1``..  
+0000a280: 2020 2020 2020 7072 6f64 7563 745f 7479        product_ty
+0000a290: 7065 5f6c 3220 2873 7472 293a 0a20 2020  pe_l2 (str):.   
+0000a2a0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
+0000a2b0: 2074 7970 6520 2832 6e64 206c 6576 656c   type (2nd level
+0000a2c0: 2920 696e 206d 6572 6368 616e 7427 7320  ) in merchant's 
+0000a2d0: 6f77 6e20 6070 726f 6475 6374 0a20 2020  own `product.   
+0000a2e0: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
+0000a2f0: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
+0000a300: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+0000a310: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
+0000a320: 3332 3434 3036 3e60 5f5f 2e0a 0a20 2020  324406>`__...   
+0000a330: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+0000a340: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+0000a350: 6f66 2060 6f6e 656f 6660 5f20 6060 5f70  of `oneof`_ ``_p
+0000a360: 726f 6475 6374 5f74 7970 655f 6c32 6060  roduct_type_l2``
+0000a370: 2e0a 2020 2020 2020 2020 7072 6f64 7563  ..        produc
+0000a380: 745f 7479 7065 5f6c 3320 2873 7472 293a  t_type_l3 (str):
+0000a390: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
+0000a3a0: 6475 6374 2074 7970 6520 2833 7264 206c  duct type (3rd l
+0000a3b0: 6576 656c 2920 696e 206d 6572 6368 616e  evel) in merchan
+0000a3c0: 7427 7320 6f77 6e20 6070 726f 6475 6374  t's own `product
+0000a3d0: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
+0000a3e0: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
+0000a3f0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
+0000a400: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
+0000a410: 6572 2f36 3332 3434 3036 3e60 5f5f 2e0a  er/6324406>`__..
+0000a420: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000a430: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000a440: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000a450: 6060 5f70 726f 6475 6374 5f74 7970 655f  ``_product_type_
+0000a460: 6c33 6060 2e0a 2020 2020 2020 2020 7072  l3``..        pr
+0000a470: 6f64 7563 745f 7479 7065 5f6c 3420 2873  oduct_type_l4 (s
+0000a480: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000a490: 2050 726f 6475 6374 2074 7970 6520 2834   Product type (4
+0000a4a0: 7468 206c 6576 656c 2920 696e 206d 6572  th level) in mer
+0000a4b0: 6368 616e 7427 7320 6f77 6e20 6070 726f  chant's own `pro
+0000a4c0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+0000a4d0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+0000a4e0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+0000a4f0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+0000a500: 616e 7377 6572 2f36 3332 3434 3036 3e60  answer/6324406>`
+0000a510: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+0000a520: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+0000a530: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+0000a540: 6660 5f20 6060 5f70 726f 6475 6374 5f74  f`_ ``_product_t
+0000a550: 7970 655f 6c34 6060 2e0a 2020 2020 2020  ype_l4``..      
+0000a560: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
+0000a570: 3520 2873 7472 293a 0a20 2020 2020 2020  5 (str):.       
+0000a580: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
+0000a590: 6520 2835 7468 206c 6576 656c 2920 696e  e (5th level) in
+0000a5a0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
+0000a5b0: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
+0000a5c0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
+0000a5d0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000a5e0: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000a5f0: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
+0000a600: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
+0000a610: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000a620: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000a630: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
+0000a640: 6374 5f74 7970 655f 6c35 6060 2e0a 2020  ct_type_l5``..  
+0000a650: 2020 2020 2020 7072 6963 6520 2867 6f6f        price (goo
+0000a660: 676c 652e 7368 6f70 7069 6e67 2e74 7970  gle.shopping.typ
+0000a670: 652e 7479 7065 732e 5072 6963 6529 3a0a  e.types.Price):.
+0000a680: 2020 2020 2020 2020 2020 2020 4375 7272              Curr
+0000a690: 656e 7420 7072 6963 6520 6f66 2074 6865  ent price of the
+0000a6a0: 2070 726f 6475 6374 2e0a 2020 2020 2020   product..      
+0000a6b0: 2020 6265 6e63 686d 6172 6b5f 7072 6963    benchmark_pric
+0000a6c0: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
+0000a6d0: 6e67 2e74 7970 652e 7479 7065 732e 5072  ng.type.types.Pr
+0000a6e0: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
+0000a6f0: 2020 4c61 7465 7374 2061 7661 696c 6162    Latest availab
+0000a700: 6c65 2070 7269 6365 2062 656e 6368 6d61  le price benchma
+0000a710: 726b 2066 6f72 2074 6865 0a20 2020 2020  rk for the.     
+0000a720: 2020 2020 2020 2070 726f 6475 6374 2773         product's
+0000a730: 2063 6174 616c 6f67 2069 6e20 7468 6520   catalog in the 
+0000a740: 6265 6e63 686d 6172 6b20 636f 756e 7472  benchmark countr
+0000a750: 792e 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
+0000a760: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
+0000a770: 6f64 653a 2073 7472 203d 2070 726f 746f  ode: str = proto
+0000a780: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000a790: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+0000a7a0: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
+0000a7b0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000a7c0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000a7d0: 2069 643a 2073 7472 203d 2070 726f 746f   id: str = proto
+0000a7e0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000a7f0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+0000a800: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
+0000a810: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000a820: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000a830: 206f 6666 6572 5f69 643a 2073 7472 203d   offer_id: str =
+0000a840: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000a850: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000a860: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000a870: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
+0000a880: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000a890: 2029 0a20 2020 2074 6974 6c65 3a20 7374   ).    title: st
+0000a8a0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+0000a8b0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+0000a8c0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+0000a8d0: 756d 6265 723d 342c 0a20 2020 2020 2020  umber=4,.       
+0000a8e0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000a8f0: 2020 2020 290a 2020 2020 6272 616e 643a      ).    brand:
+0000a900: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+0000a910: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000a920: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+0000a930: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
+0000a940: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+0000a950: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
+0000a960: 6567 6f72 795f 6c31 3a20 7374 7220 3d20  egory_l1: str = 
+0000a970: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000a980: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+0000a990: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+0000a9a0: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
+0000a9b0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000a9c0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
+0000a9d0: 323a 2073 7472 203d 2070 726f 746f 2e46  2: str = proto.F
+0000a9e0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000a9f0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000aa00: 2020 2020 6e75 6d62 6572 3d37 2c0a 2020      number=7,.  
+0000aa10: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000aa20: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+0000aa30: 6174 6567 6f72 795f 6c33 3a20 7374 7220  ategory_l3: str 
+0000aa40: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+0000aa50: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+0000aa60: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+0000aa70: 6265 723d 382c 0a20 2020 2020 2020 206f  ber=8,.        o
+0000aa80: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000aa90: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
+0000aaa0: 5f6c 343a 2073 7472 203d 2070 726f 746f  _l4: str = proto
+0000aab0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000aac0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+0000aad0: 2020 2020 2020 6e75 6d62 6572 3d39 2c0a        number=9,.
+0000aae0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000aaf0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000ab00: 2063 6174 6567 6f72 795f 6c35 3a20 7374   category_l5: st
+0000ab10: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+0000ab20: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+0000ab30: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+0000ab40: 756d 6265 723d 3130 2c0a 2020 2020 2020  umber=10,.      
+0000ab50: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+0000ab60: 0a20 2020 2029 0a20 2020 2070 726f 6475  .    ).    produ
+0000ab70: 6374 5f74 7970 655f 6c31 3a20 7374 7220  ct_type_l1: str 
+0000ab80: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+0000ab90: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+0000aba0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+0000abb0: 6265 723d 3131 2c0a 2020 2020 2020 2020  ber=11,.        
+0000abc0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000abd0: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
+0000abe0: 5f74 7970 655f 6c32 3a20 7374 7220 3d20  _type_l2: str = 
+0000abf0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000ac00: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+0000ac10: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+0000ac20: 723d 3132 2c0a 2020 2020 2020 2020 6f70  r=12,.        op
+0000ac30: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000ac40: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
+0000ac50: 7970 655f 6c33 3a20 7374 7220 3d20 7072  ype_l3: str = pr
+0000ac60: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000ac70: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000ac80: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000ac90: 3133 2c0a 2020 2020 2020 2020 6f70 7469  13,.        opti
+0000aca0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000acb0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
+0000acc0: 655f 6c34 3a20 7374 7220 3d20 7072 6f74  e_l4: str = prot
+0000acd0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000ace0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000acf0: 2020 2020 2020 206e 756d 6265 723d 3134         number=14
+0000ad00: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+0000ad10: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+0000ad20: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+0000ad30: 6c35 3a20 7374 7220 3d20 7072 6f74 6f2e  l5: str = proto.
+0000ad40: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000ad50: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000ad60: 2020 2020 206e 756d 6265 723d 3135 2c0a       number=15,.
+0000ad70: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000ad80: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000ad90: 2070 7269 6365 3a20 7479 7065 732e 5072   price: types.Pr
+0000ada0: 6963 6520 3d20 7072 6f74 6f2e 4669 656c  ice = proto.Fiel
+0000adb0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+0000adc0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+0000add0: 2020 6e75 6d62 6572 3d31 362c 0a20 2020    number=16,.   
+0000ade0: 2020 2020 206d 6573 7361 6765 3d74 7970       message=typ
+0000adf0: 6573 2e50 7269 6365 2c0a 2020 2020 290a  es.Price,.    ).
+0000ae00: 2020 2020 6265 6e63 686d 6172 6b5f 7072      benchmark_pr
+0000ae10: 6963 653a 2074 7970 6573 2e50 7269 6365  ice: types.Price
+0000ae20: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ae30: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+0000ae40: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+0000ae50: 756d 6265 723d 3137 2c0a 2020 2020 2020  umber=17,.      
+0000ae60: 2020 6d65 7373 6167 653d 7479 7065 732e    message=types.
+0000ae70: 5072 6963 652c 0a20 2020 2029 0a0a 0a63  Price,.    )...c
+0000ae80: 6c61 7373 2050 7269 6365 496e 7369 6768  lass PriceInsigh
+0000ae90: 7473 5072 6f64 7563 7456 6965 7728 7072  tsProductView(pr
+0000aea0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+0000aeb0: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
+0000aec0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
+0000aed0: 2069 6e20 6060 7072 6963 655f 696e 7369   in ``price_insi
+0000aee0: 6768 7473 5f70 726f 6475 6374 5f76 6965  ghts_product_vie
+0000aef0: 7760 6020 7461 626c 652e 0a0a 2020 2020  w`` table...    
+0000af00: 6050 7269 6365 0a20 2020 2069 6e73 6967  `Price.    insig
+0000af10: 6874 7320 3c68 7474 7073 3a2f 2f73 7570  hts <https://sup
+0000af20: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000af30: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000af40: 2f31 3139 3136 3932 363e 605f 5f0a 2020  /11916926>`__.  
+0000af50: 2020 7265 706f 7274 2e0a 0a20 2020 2056    report...    V
+0000af60: 616c 7565 7320 6172 6520 6f6e 6c79 2073  alues are only s
+0000af70: 6574 2066 6f72 2066 6965 6c64 7320 7265  et for fields re
+0000af80: 7175 6573 7465 6420 6578 706c 6963 6974  quested explicit
+0000af90: 6c79 2069 6e20 7468 6520 7265 7175 6573  ly in the reques
+0000afa0: 7427 730a 2020 2020 7365 6172 6368 2071  t's.    search q
+0000afb0: 7565 7279 2e0a 0a0a 2020 2020 2e2e 205f  uery....    .. _
+0000afc0: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
+0000afd0: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
+0000afe0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+0000aff0: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
+0000b000: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
+0000b010: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
+0000b020: 6669 656c 6473 0a0a 2020 2020 4174 7472  fields..    Attr
+0000b030: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+0000b040: 6964 2028 7374 7229 3a0a 2020 2020 2020  id (str):.      
+0000b050: 2020 2020 2020 5245 5354 2049 4420 6f66        REST ID of
+0000b060: 2074 6865 2070 726f 6475 6374 2c20 696e   the product, in
+0000b070: 2074 6865 2066 6f72 6d20 6f66 0a20 2020   the form of.   
+0000b080: 2020 2020 2020 2020 2060 6063 6861 6e6e           ``chann
+0000b090: 656c 7e6c 616e 6775 6167 6543 6f64 657e  el~languageCode~
+0000b0a0: 6665 6564 4c61 6265 6c7e 6f66 6665 7249  feedLabel~offerI
+0000b0b0: 6460 602e 2043 616e 2062 6520 7573 6564  d``. Can be used
+0000b0c0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+0000b0d0: 6a6f 696e 2064 6174 6120 7769 7468 2074  join data with t
+0000b0e0: 6865 2060 6070 726f 6475 6374 5f76 6965  he ``product_vie
+0000b0f0: 7760 6020 7461 626c 652e 0a0a 2020 2020  w`` table...    
+0000b100: 2020 2020 2020 2020 5265 7175 6972 6564          Required
+0000b110: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
+0000b120: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
+0000b130: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000b140: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000b150: 6620 606f 6e65 6f66 605f 2060 605f 6964  f `oneof`_ ``_id
+0000b160: 6060 2e0a 2020 2020 2020 2020 6f66 6665  ``..        offe
+0000b170: 725f 6964 2028 7374 7229 3a0a 2020 2020  r_id (str):.    
+0000b180: 2020 2020 2020 2020 4d65 7263 6861 6e74          Merchant
+0000b190: 2d70 726f 7669 6465 6420 6964 206f 6620  -provided id of 
+0000b1a0: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
+0000b1b0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000b1c0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000b1d0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000b1e0: 6f66 6665 725f 6964 6060 2e0a 2020 2020  offer_id``..    
+0000b1f0: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
+0000b200: 0a20 2020 2020 2020 2020 2020 2054 6974  .            Tit
+0000b210: 6c65 206f 6620 7468 6520 7072 6f64 7563  le of the produc
+0000b220: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+0000b230: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+0000b240: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+0000b250: 605f 2060 605f 7469 746c 6560 602e 0a20  `_ ``_title``.. 
+0000b260: 2020 2020 2020 2062 7261 6e64 2028 7374         brand (st
+0000b270: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000b280: 4272 616e 6420 6f66 2074 6865 2070 726f  Brand of the pro
+0000b290: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
+0000b2a0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000b2b0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000b2c0: 656f 6660 5f20 6060 5f62 7261 6e64 6060  eof`_ ``_brand``
+0000b2d0: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
+0000b2e0: 7279 5f6c 3120 2873 7472 293a 0a20 2020  ry_l1 (str):.   
+0000b2f0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
+0000b300: 2063 6174 6567 6f72 7920 2831 7374 206c   category (1st l
+0000b310: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
+0000b320: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
+0000b330: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
+0000b340: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
+0000b350: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
+0000b360: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
+0000b370: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
+0000b380: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+0000b390: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+0000b3a0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
+0000b3b0: 6567 6f72 795f 6c31 6060 2e0a 2020 2020  egory_l1``..    
+0000b3c0: 2020 2020 6361 7465 676f 7279 5f6c 3220      category_l2 
+0000b3d0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000b3e0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
+0000b3f0: 6f72 7920 2832 6e64 206c 6576 656c 2920  ory (2nd level) 
+0000b400: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+0000b410: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+0000b420: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+0000b430: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+0000b440: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+0000b450: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+0000b460: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+0000b470: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+0000b480: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+0000b490: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
+0000b4a0: 6c32 6060 2e0a 2020 2020 2020 2020 6361  l2``..        ca
+0000b4b0: 7465 676f 7279 5f6c 3320 2873 7472 293a  tegory_l3 (str):
+0000b4c0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
+0000b4d0: 6475 6374 2063 6174 6567 6f72 7920 2833  duct category (3
+0000b4e0: 7264 206c 6576 656c 2920 696e 2060 476f  rd level) in `Go
+0000b4f0: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
+0000b500: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
+0000b510: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
+0000b520: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000b530: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000b540: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
+0000b550: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000b560: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000b570: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000b580: 5f63 6174 6567 6f72 795f 6c33 6060 2e0a  _category_l3``..
+0000b590: 2020 2020 2020 2020 6361 7465 676f 7279          category
+0000b5a0: 5f6c 3420 2873 7472 293a 0a20 2020 2020  _l4 (str):.     
+0000b5b0: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
+0000b5c0: 6174 6567 6f72 7920 2834 7468 206c 6576  ategory (4th lev
+0000b5d0: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
+0000b5e0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
+0000b5f0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
+0000b600: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000b610: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000b620: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
+0000b630: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
+0000b640: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000b650: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000b660: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
+0000b670: 6f72 795f 6c34 6060 2e0a 2020 2020 2020  ory_l4``..      
+0000b680: 2020 6361 7465 676f 7279 5f6c 3520 2873    category_l5 (s
+0000b690: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000b6a0: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
+0000b6b0: 7920 2835 7468 206c 6576 656c 2920 696e  y (5th level) in
+0000b6c0: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
+0000b6d0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
+0000b6e0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
+0000b6f0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+0000b700: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+0000b710: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
+0000b720: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000b730: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000b740: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000b750: 5f20 6060 5f63 6174 6567 6f72 795f 6c35  _ ``_category_l5
+0000b760: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
+0000b770: 7563 745f 7479 7065 5f6c 3120 2873 7472  uct_type_l1 (str
+0000b780: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
+0000b790: 726f 6475 6374 2074 7970 6520 2831 7374  roduct type (1st
+0000b7a0: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
+0000b7b0: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
+0000b7c0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
+0000b7d0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
+0000b7e0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+0000b7f0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+0000b800: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
+0000b810: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000b820: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000b830: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000b840: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
+0000b850: 655f 6c31 6060 2e0a 2020 2020 2020 2020  e_l1``..        
+0000b860: 7072 6f64 7563 745f 7479 7065 5f6c 3220  product_type_l2 
+0000b870: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000b880: 2020 2050 726f 6475 6374 2074 7970 6520     Product type 
+0000b890: 2832 6e64 206c 6576 656c 2920 696e 206d  (2nd level) in m
+0000b8a0: 6572 6368 616e 7427 7320 6f77 6e20 6070  erchant's own `p
+0000b8b0: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
+0000b8c0: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
+0000b8d0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
+0000b8e0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
+0000b8f0: 732f 616e 7377 6572 2f36 3332 3434 3036  s/answer/6324406
+0000b900: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
+0000b910: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000b920: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000b930: 656f 6660 5f20 6060 5f70 726f 6475 6374  eof`_ ``_product
+0000b940: 5f74 7970 655f 6c32 6060 2e0a 2020 2020  _type_l2``..    
+0000b950: 2020 2020 7072 6f64 7563 745f 7479 7065      product_type
+0000b960: 5f6c 3320 2873 7472 293a 0a20 2020 2020  _l3 (str):.     
+0000b970: 2020 2020 2020 2050 726f 6475 6374 2074         Product t
+0000b980: 7970 6520 2833 7264 206c 6576 656c 2920  ype (3rd level) 
+0000b990: 696e 206d 6572 6368 616e 7427 7320 6f77  in merchant's ow
+0000b9a0: 6e20 6070 726f 6475 6374 0a20 2020 2020  n `product.     
+0000b9b0: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
+0000b9c0: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
+0000b9d0: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
+0000b9e0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
+0000b9f0: 3434 3036 3e60 5f5f 2e0a 0a20 2020 2020  4406>`__...     
+0000ba00: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+0000ba10: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+0000ba20: 2060 6f6e 656f 6660 5f20 6060 5f70 726f   `oneof`_ ``_pro
+0000ba30: 6475 6374 5f74 7970 655f 6c33 6060 2e0a  duct_type_l3``..
+0000ba40: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
+0000ba50: 7479 7065 5f6c 3420 2873 7472 293a 0a20  type_l4 (str):. 
+0000ba60: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
+0000ba70: 6374 2074 7970 6520 2834 7468 206c 6576  ct type (4th lev
+0000ba80: 656c 2920 696e 206d 6572 6368 616e 7427  el) in merchant'
+0000ba90: 7320 6f77 6e20 6070 726f 6475 6374 0a20  s own `product. 
+0000baa0: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
+0000bab0: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
+0000bac0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000bad0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000bae0: 2f36 3332 3434 3036 3e60 5f5f 2e0a 0a20  /6324406>`__... 
+0000baf0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000bb00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000bb10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000bb20: 5f70 726f 6475 6374 5f74 7970 655f 6c34  _product_type_l4
+0000bb30: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
+0000bb40: 7563 745f 7479 7065 5f6c 3520 2873 7472  uct_type_l5 (str
+0000bb50: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
+0000bb60: 726f 6475 6374 2074 7970 6520 2835 7468  roduct type (5th
+0000bb70: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
+0000bb80: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
+0000bb90: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
+0000bba0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
+0000bbb0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+0000bbc0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+0000bbd0: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
+0000bbe0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000bbf0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000bc00: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000bc10: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
+0000bc20: 655f 6c35 6060 2e0a 2020 2020 2020 2020  e_l5``..        
+0000bc30: 7072 6963 6520 2867 6f6f 676c 652e 7368  price (google.sh
+0000bc40: 6f70 7069 6e67 2e74 7970 652e 7479 7065  opping.type.type
+0000bc50: 732e 5072 6963 6529 3a0a 2020 2020 2020  s.Price):.      
+0000bc60: 2020 2020 2020 4375 7272 656e 7420 7072        Current pr
+0000bc70: 6963 6520 6f66 2074 6865 2070 726f 6475  ice of the produ
+0000bc80: 6374 2e0a 2020 2020 2020 2020 7375 6767  ct..        sugg
+0000bc90: 6573 7465 645f 7072 6963 6520 2867 6f6f  ested_price (goo
+0000bca0: 676c 652e 7368 6f70 7069 6e67 2e74 7970  gle.shopping.typ
+0000bcb0: 652e 7479 7065 732e 5072 6963 6529 3a0a  e.types.Price):.
+0000bcc0: 2020 2020 2020 2020 2020 2020 4c61 7465              Late
+0000bcd0: 7374 2073 7567 6765 7374 6564 2070 7269  st suggested pri
+0000bce0: 6365 2066 6f72 2074 6865 2070 726f 6475  ce for the produ
+0000bcf0: 6374 2e0a 2020 2020 2020 2020 7072 6564  ct..        pred
+0000bd00: 6963 7465 645f 696d 7072 6573 7369 6f6e  icted_impression
+0000bd10: 735f 6368 616e 6765 5f66 7261 6374 696f  s_change_fractio
+0000bd20: 6e20 2866 6c6f 6174 293a 0a20 2020 2020  n (float):.     
+0000bd30: 2020 2020 2020 2050 7265 6469 6374 6564         Predicted
+0000bd40: 2063 6861 6e67 6520 696e 2069 6d70 7265   change in impre
+0000bd50: 7373 696f 6e73 2061 7320 6120 6672 6163  ssions as a frac
+0000bd60: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+0000bd70: 2061 6674 6572 2069 6e74 726f 6475 6369   after introduci
+0000bd80: 6e67 2074 6865 2073 7567 6765 7374 6564  ng the suggested
+0000bd90: 2070 7269 6365 2063 6f6d 7061 7265 640a   price compared.
+0000bda0: 2020 2020 2020 2020 2020 2020 746f 2063              to c
+0000bdb0: 7572 7265 6e74 2061 6374 6976 6520 7072  urrent active pr
+0000bdc0: 6963 652e 2046 6f72 2065 7861 6d70 6c65  ice. For example
+0000bdd0: 2c20 302e 3035 2069 7320 610a 2020 2020  , 0.05 is a.    
+0000bde0: 2020 2020 2020 2020 3525 2070 7265 6469          5% predi
+0000bdf0: 6374 6564 2069 6e63 7265 6173 6520 696e  cted increase in
+0000be00: 2069 6d70 7265 7373 696f 6e73 2e0a 0a20   impressions... 
+0000be10: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000be20: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000be30: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000be40: 5f70 7265 6469 6374 6564 5f69 6d70 7265  _predicted_impre
+0000be50: 7373 696f 6e73 5f63 6861 6e67 655f 6672  ssions_change_fr
+0000be60: 6163 7469 6f6e 6060 2e0a 2020 2020 2020  action``..      
+0000be70: 2020 7072 6564 6963 7465 645f 636c 6963    predicted_clic
+0000be80: 6b73 5f63 6861 6e67 655f 6672 6163 7469  ks_change_fracti
+0000be90: 6f6e 2028 666c 6f61 7429 3a0a 2020 2020  on (float):.    
+0000bea0: 2020 2020 2020 2020 5072 6564 6963 7465          Predicte
+0000beb0: 6420 6368 616e 6765 2069 6e20 636c 6963  d change in clic
+0000bec0: 6b73 2061 7320 6120 6672 6163 7469 6f6e  ks as a fraction
+0000bed0: 0a20 2020 2020 2020 2020 2020 2061 6674  .            aft
+0000bee0: 6572 2069 6e74 726f 6475 6369 6e67 2074  er introducing t
+0000bef0: 6865 2073 7567 6765 7374 6564 2070 7269  he suggested pri
+0000bf00: 6365 2063 6f6d 7061 7265 640a 2020 2020  ce compared.    
+0000bf10: 2020 2020 2020 2020 746f 2063 7572 7265          to curre
+0000bf20: 6e74 2061 6374 6976 6520 7072 6963 652e  nt active price.
+0000bf30: 2046 6f72 2065 7861 6d70 6c65 2c20 302e   For example, 0.
+0000bf40: 3035 2069 7320 610a 2020 2020 2020 2020  05 is a.        
+0000bf50: 2020 2020 3525 2070 7265 6469 6374 6564      5% predicted
+0000bf60: 2069 6e63 7265 6173 6520 696e 2063 6c69   increase in cli
+0000bf70: 636b 732e 0a0a 2020 2020 2020 2020 2020  cks...          
+0000bf80: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000bf90: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000bfa0: 6f66 605f 2060 605f 7072 6564 6963 7465  of`_ ``_predicte
+0000bfb0: 645f 636c 6963 6b73 5f63 6861 6e67 655f  d_clicks_change_
+0000bfc0: 6672 6163 7469 6f6e 6060 2e0a 2020 2020  fraction``..    
+0000bfd0: 2020 2020 7072 6564 6963 7465 645f 636f      predicted_co
+0000bfe0: 6e76 6572 7369 6f6e 735f 6368 616e 6765  nversions_change
+0000bff0: 5f66 7261 6374 696f 6e20 2866 6c6f 6174  _fraction (float
+0000c000: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
+0000c010: 7265 6469 6374 6564 2063 6861 6e67 6520  redicted change 
+0000c020: 696e 2063 6f6e 7665 7273 696f 6e73 2061  in conversions a
+0000c030: 7320 6120 6672 6163 7469 6f6e 0a20 2020  s a fraction.   
+0000c040: 2020 2020 2020 2020 2061 6674 6572 2069           after i
+0000c050: 6e74 726f 6475 6369 6e67 2074 6865 2073  ntroducing the s
+0000c060: 7567 6765 7374 6564 2070 7269 6365 2063  uggested price c
+0000c070: 6f6d 7061 7265 640a 2020 2020 2020 2020  ompared.        
+0000c080: 2020 2020 746f 2063 7572 7265 6e74 2061      to current a
+0000c090: 6374 6976 6520 7072 6963 652e 2046 6f72  ctive price. For
+0000c0a0: 2065 7861 6d70 6c65 2c20 302e 3035 2069   example, 0.05 i
+0000c0b0: 7320 610a 2020 2020 2020 2020 2020 2020  s a.            
+0000c0c0: 3525 2070 7265 6469 6374 6564 2069 6e63  5% predicted inc
+0000c0d0: 7265 6173 6520 696e 2063 6f6e 7665 7273  rease in convers
+0000c0e0: 696f 6e73 292e 0a0a 2020 2020 2020 2020  ions)...        
+0000c0f0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000c100: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000c110: 6e65 6f66 605f 2060 605f 7072 6564 6963  neof`_ ``_predic
+0000c120: 7465 645f 636f 6e76 6572 7369 6f6e 735f  ted_conversions_
+0000c130: 6368 616e 6765 5f66 7261 6374 696f 6e60  change_fraction`
+0000c140: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
+0000c150: 6964 3a20 7374 7220 3d20 7072 6f74 6f2e  id: str = proto.
+0000c160: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000c170: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000c180: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
+0000c190: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000c1a0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000c1b0: 6f66 6665 725f 6964 3a20 7374 7220 3d20  offer_id: str = 
+0000c1c0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000c1d0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+0000c1e0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+0000c1f0: 723d 322c 0a20 2020 2020 2020 206f 7074  r=2,.        opt
+0000c200: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000c210: 290a 2020 2020 7469 746c 653a 2073 7472  ).    title: str
+0000c220: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000c230: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000c240: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000c250: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+0000c260: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000c270: 2020 2029 0a20 2020 2062 7261 6e64 3a20     ).    brand: 
+0000c280: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+0000c290: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+0000c2a0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+0000c2b0: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
+0000c2c0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000c2d0: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
+0000c2e0: 676f 7279 5f6c 313a 2073 7472 203d 2070  gory_l1: str = p
+0000c2f0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000c300: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000c310: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000c320: 3d35 2c0a 2020 2020 2020 2020 6f70 7469  =5,.        opti
+0000c330: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000c340: 0a20 2020 2063 6174 6567 6f72 795f 6c32  .    category_l2
+0000c350: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+0000c360: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000c370: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+0000c380: 2020 206e 756d 6265 723d 362c 0a20 2020     number=6,.   
+0000c390: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+0000c3a0: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
+0000c3b0: 7465 676f 7279 5f6c 333a 2073 7472 203d  tegory_l3: str =
+0000c3c0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000c3d0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000c3e0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000c3f0: 6572 3d37 2c0a 2020 2020 2020 2020 6f70  er=7,.        op
+0000c400: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000c410: 2029 0a20 2020 2063 6174 6567 6f72 795f   ).    category_
+0000c420: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
+0000c430: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000c440: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000c450: 2020 2020 206e 756d 6265 723d 382c 0a20       number=8,. 
+0000c460: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000c470: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000c480: 6361 7465 676f 7279 5f6c 353a 2073 7472  category_l5: str
+0000c490: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000c4a0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000c4b0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000c4c0: 6d62 6572 3d39 2c0a 2020 2020 2020 2020  mber=9,.        
+0000c4d0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000c4e0: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
+0000c4f0: 5f74 7970 655f 6c31 3a20 7374 7220 3d20  _type_l1: str = 
+0000c500: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000c510: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+0000c520: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+0000c530: 723d 3130 2c0a 2020 2020 2020 2020 6f70  r=10,.        op
+0000c540: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000c550: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
+0000c560: 7970 655f 6c32 3a20 7374 7220 3d20 7072  ype_l2: str = pr
+0000c570: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000c580: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000c590: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000c5a0: 3131 2c0a 2020 2020 2020 2020 6f70 7469  11,.        opti
+0000c5b0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000c5c0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
+0000c5d0: 655f 6c33 3a20 7374 7220 3d20 7072 6f74  e_l3: str = prot
+0000c5e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000c5f0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000c600: 2020 2020 2020 206e 756d 6265 723d 3132         number=12
+0000c610: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+0000c620: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+0000c630: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+0000c640: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
+0000c650: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000c660: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000c670: 2020 2020 206e 756d 6265 723d 3133 2c0a       number=13,.
+0000c680: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000c690: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000c6a0: 2070 726f 6475 6374 5f74 7970 655f 6c35   product_type_l5
+0000c6b0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+0000c6c0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000c6d0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+0000c6e0: 2020 206e 756d 6265 723d 3134 2c0a 2020     number=14,.  
+0000c6f0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000c700: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
+0000c710: 7269 6365 3a20 7479 7065 732e 5072 6963  rice: types.Pric
+0000c720: 6520 3d20 7072 6f74 6f2e 4669 656c 6428  e = proto.Field(
+0000c730: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
+0000c740: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
+0000c750: 6e75 6d62 6572 3d31 352c 0a20 2020 2020  number=15,.     
+0000c760: 2020 206d 6573 7361 6765 3d74 7970 6573     message=types
+0000c770: 2e50 7269 6365 2c0a 2020 2020 290a 2020  .Price,.    ).  
+0000c780: 2020 7375 6767 6573 7465 645f 7072 6963    suggested_pric
+0000c790: 653a 2074 7970 6573 2e50 7269 6365 203d  e: types.Price =
+0000c7a0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000c7b0: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
+0000c7c0: 4147 452c 0a20 2020 2020 2020 206e 756d  AGE,.        num
+0000c7d0: 6265 723d 3136 2c0a 2020 2020 2020 2020  ber=16,.        
+0000c7e0: 6d65 7373 6167 653d 7479 7065 732e 5072  message=types.Pr
+0000c7f0: 6963 652c 0a20 2020 2029 0a20 2020 2070  ice,.    ).    p
+0000c800: 7265 6469 6374 6564 5f69 6d70 7265 7373  redicted_impress
+0000c810: 696f 6e73 5f63 6861 6e67 655f 6672 6163  ions_change_frac
+0000c820: 7469 6f6e 3a20 666c 6f61 7420 3d20 7072  tion: float = pr
+0000c830: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000c840: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
+0000c850: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000c860: 3137 2c0a 2020 2020 2020 2020 6f70 7469  17,.        opti
+0000c870: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000c880: 0a20 2020 2070 7265 6469 6374 6564 5f63  .    predicted_c
+0000c890: 6c69 636b 735f 6368 616e 6765 5f66 7261  licks_change_fra
+0000c8a0: 6374 696f 6e3a 2066 6c6f 6174 203d 2070  ction: float = p
+0000c8b0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000c8c0: 2020 2020 7072 6f74 6f2e 444f 5542 4c45      proto.DOUBLE
+0000c8d0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000c8e0: 3d31 382c 0a20 2020 2020 2020 206f 7074  =18,.        opt
+0000c8f0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000c900: 290a 2020 2020 7072 6564 6963 7465 645f  ).    predicted_
+0000c910: 636f 6e76 6572 7369 6f6e 735f 6368 616e  conversions_chan
+0000c920: 6765 5f66 7261 6374 696f 6e3a 2066 6c6f  ge_fraction: flo
+0000c930: 6174 203d 2070 726f 746f 2e46 6965 6c64  at = proto.Field
+0000c940: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000c950: 444f 5542 4c45 2c0a 2020 2020 2020 2020  DOUBLE,.        
+0000c960: 6e75 6d62 6572 3d31 392c 0a20 2020 2020  number=19,.     
+0000c970: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000c980: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
+0000c990: 4265 7374 5365 6c6c 6572 7350 726f 6475  BestSellersProdu
+0000c9a0: 6374 436c 7573 7465 7256 6965 7728 7072  ctClusterView(pr
+0000c9b0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+0000c9c0: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
+0000c9d0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
+0000c9e0: 2069 6e20 6060 6265 7374 5f73 656c 6c65   in ``best_selle
+0000c9f0: 7273 5f70 726f 6475 6374 5f63 6c75 7374  rs_product_clust
+0000ca00: 6572 5f76 6965 7760 600a 2020 2020 7461  er_view``.    ta
+0000ca10: 626c 652e 0a0a 2020 2020 6042 6573 740a  ble...    `Best.
+0000ca20: 2020 2020 7365 6c6c 6572 7320 3c68 7474      sellers <htt
+0000ca30: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
+0000ca40: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
+0000ca50: 732f 616e 7377 6572 2f39 3438 3836 3739  s/answer/9488679
+0000ca60: 3e60 5f5f 0a20 2020 2072 6570 6f72 7420  >`__.    report 
+0000ca70: 7769 7468 2074 6f70 2070 726f 6475 6374  with top product
+0000ca80: 2063 6c75 7374 6572 732e 2041 2070 726f   clusters. A pro
+0000ca90: 6475 6374 2063 6c75 7374 6572 2069 7320  duct cluster is 
+0000caa0: 6120 6772 6f75 7069 6e67 0a20 2020 2066  a grouping.    f
+0000cab0: 6f72 2064 6966 6665 7265 6e74 206f 6666  or different off
+0000cac0: 6572 7320 616e 6420 7661 7269 616e 7473  ers and variants
+0000cad0: 2074 6861 7420 7265 7072 6573 656e 7420   that represent 
+0000cae0: 7468 6520 7361 6d65 2070 726f 6475 6374  the same product
+0000caf0: 2c0a 2020 2020 666f 7220 6578 616d 706c  ,.    for exampl
+0000cb00: 652c 2047 6f6f 676c 6520 5069 7865 6c20  e, Google Pixel 
+0000cb10: 372e 0a0a 2020 2020 5661 6c75 6573 2061  7...    Values a
+0000cb20: 7265 206f 6e6c 7920 7365 7420 666f 7220  re only set for 
+0000cb30: 6669 656c 6473 2072 6571 7565 7374 6564  fields requested
+0000cb40: 2065 7870 6c69 6369 746c 7920 696e 2074   explicitly in t
+0000cb50: 6865 2072 6571 7565 7374 2773 0a20 2020  he request's.   
+0000cb60: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
+0000cb70: 0a20 2020 202e 2e20 5f6f 6e65 6f66 3a20  .    .. _oneof: 
+0000cb80: 6874 7470 733a 2f2f 7072 6f74 6f2d 706c  https://proto-pl
+0000cb90: 7573 2d70 7974 686f 6e2e 7265 6164 7468  us-python.readth
+0000cba0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000cbb0: 6c65 2f66 6965 6c64 732e 6874 6d6c 236f  le/fields.html#o
+0000cbc0: 6e65 6f66 732d 6d75 7475 616c 6c79 2d65  neofs-mutually-e
+0000cbd0: 7863 6c75 7369 7665 2d66 6965 6c64 730a  xclusive-fields.
+0000cbe0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+0000cbf0: 0a20 2020 2020 2020 2072 6570 6f72 745f  .        report_
+0000cc00: 6461 7465 2028 676f 6f67 6c65 2e74 7970  date (google.typ
+0000cc10: 652e 6461 7465 5f70 6232 2e44 6174 6529  e.date_pb2.Date)
+0000cc20: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+0000cc30: 706f 7274 2064 6174 652e 2054 6865 2076  port date. The v
+0000cc40: 616c 7565 206f 6620 7468 6973 2066 6965  alue of this fie
+0000cc50: 6c64 2063 616e 206f 6e6c 7920 6265 206f  ld can only be o
+0000cc60: 6e65 206f 6620 7468 650a 2020 2020 2020  ne of the.      
+0000cc70: 2020 2020 2020 666f 6c6c 6f77 696e 673a        following:
+0000cc80: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+0000cc90: 2054 6865 2066 6972 7374 2064 6179 206f   The first day o
+0000cca0: 6620 7468 6520 7765 656b 2028 4d6f 6e64  f the week (Mond
+0000ccb0: 6179 2920 666f 7220 7765 656b 6c79 2072  ay) for weekly r
+0000ccc0: 6570 6f72 7473 2c0a 2020 2020 2020 2020  eports,.        
+0000ccd0: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
+0000cce0: 2064 6179 206f 6620 7468 6520 6d6f 6e74   day of the mont
+0000ccf0: 6820 666f 7220 6d6f 6e74 686c 7920 7265  h for monthly re
+0000cd00: 706f 7274 732e 0a0a 2020 2020 2020 2020  ports...        
+0000cd10: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
+0000cd20: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
+0000cd30: 6c61 7573 652e 2049 6620 6120 6060 5748  lause. If a ``WH
+0000cd40: 4552 4560 6020 636f 6e64 6974 696f 6e0a  ERE`` condition.
+0000cd50: 2020 2020 2020 2020 2020 2020 6f6e 2060              on `
+0000cd60: 6072 6570 6f72 745f 6461 7465 6060 2069  `report_date`` i
+0000cd70: 7320 6e6f 7420 7370 6563 6966 6965 6420  s not specified 
+0000cd80: 696e 2074 6865 2071 7565 7279 2c20 7468  in the query, th
+0000cd90: 6520 6c61 7465 7374 0a20 2020 2020 2020  e latest.       
+0000cda0: 2020 2020 2061 7661 696c 6162 6c65 2077       available w
+0000cdb0: 6565 6b6c 7920 6f72 206d 6f6e 7468 6c79  eekly or monthly
+0000cdc0: 2072 6570 6f72 7420 6973 2072 6574 7572   report is retur
+0000cdd0: 6e65 642e 0a20 2020 2020 2020 2072 6570  ned..        rep
+0000cde0: 6f72 745f 6772 616e 756c 6172 6974 7920  ort_granularity 
+0000cdf0: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
+0000ce00: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
+0000ce10: 735f 7631 6265 7461 2e74 7970 6573 2e52  s_v1beta.types.R
+0000ce20: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
+0000ce30: 2e52 6570 6f72 7447 7261 6e75 6c61 7269  .ReportGranulari
+0000ce40: 7479 456e 756d 293a 0a20 2020 2020 2020  tyEnum):.       
+0000ce50: 2020 2020 2047 7261 6e75 6c61 7269 7479       Granularity
+0000ce60: 206f 6620 7468 6520 7265 706f 7274 2e20   of the report. 
+0000ce70: 5468 6520 7261 6e6b 696e 6720 6361 6e20  The ranking can 
+0000ce80: 6265 2064 6f6e 6520 6f76 6572 2061 0a20  be done over a. 
+0000ce90: 2020 2020 2020 2020 2020 2077 6565 6b20             week 
+0000cea0: 6f72 2061 206d 6f6e 7468 2074 696d 6566  or a month timef
+0000ceb0: 7261 6d65 2e0a 0a20 2020 2020 2020 2020  rame...         
+0000cec0: 2020 2052 6571 7569 7265 6420 696e 2074     Required in t
+0000ced0: 6865 2060 6053 454c 4543 5460 6020 636c  he ``SELECT`` cl
+0000cee0: 6175 7365 2e20 436f 6e64 6974 696f 6e20  ause. Condition 
+0000cef0: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
+0000cf00: 6072 6570 6f72 745f 6772 616e 756c 6172  `report_granular
+0000cf10: 6974 7960 6020 6973 2072 6571 7569 7265  ity`` is require
+0000cf20: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
+0000cf30: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
+0000cf40: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000cf50: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000cf60: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+0000cf70: 706f 7274 5f67 7261 6e75 6c61 7269 7479  port_granularity
+0000cf80: 6060 2e0a 2020 2020 2020 2020 7265 706f  ``..        repo
+0000cf90: 7274 5f63 6f75 6e74 7279 5f63 6f64 6520  rt_country_code 
+0000cfa0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000cfb0: 2020 2043 6f75 6e74 7279 2077 6865 7265     Country where
+0000cfc0: 2074 6865 2072 616e 6b69 6e67 2069 7320   the ranking is 
+0000cfd0: 6361 6c63 756c 6174 6564 2e20 5265 7072  calculated. Repr
+0000cfe0: 6573 656e 7465 6420 696e 2074 6865 0a20  esented in the. 
+0000cff0: 2020 2020 2020 2020 2020 2049 534f 2033             ISO 3
+0000d000: 3136 3620 666f 726d 6174 2e0a 0a20 2020  166 format...   
+0000d010: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+0000d020: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+0000d030: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
+0000d040: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
+0000d050: 2020 2020 2060 6072 6570 6f72 745f 636f       ``report_co
+0000d060: 756e 7472 795f 636f 6465 6060 2069 7320  untry_code`` is 
+0000d070: 7265 7175 6972 6564 2069 6e20 7468 6520  required in the 
+0000d080: 6060 5748 4552 4560 6020 636c 6175 7365  ``WHERE`` clause
+0000d090: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000d0a0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000d0b0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000d0c0: 5f20 6060 5f72 6570 6f72 745f 636f 756e  _ ``_report_coun
+0000d0d0: 7472 795f 636f 6465 6060 2e0a 2020 2020  try_code``..    
+0000d0e0: 2020 2020 7265 706f 7274 5f63 6174 6567      report_categ
+0000d0f0: 6f72 795f 6964 2028 696e 7429 3a0a 2020  ory_id (int):.  
+0000d100: 2020 2020 2020 2020 2020 476f 6f67 6c65            Google
+0000d110: 2070 726f 6475 6374 2063 6174 6567 6f72   product categor
+0000d120: 7920 4944 2074 6f20 6361 6c63 756c 6174  y ID to calculat
+0000d130: 6520 7468 6520 7261 6e6b 696e 6720 666f  e the ranking fo
+0000d140: 722c 0a20 2020 2020 2020 2020 2020 2072  r,.            r
+0000d150: 6570 7265 7365 6e74 6564 2069 6e20 6047  epresented in `G
+0000d160: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
+0000d170: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+0000d180: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+0000d190: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+0000d1a0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+0000d1b0: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
+0000d1c0: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+0000d1d0: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
+0000d1e0: 4c45 4354 6060 2063 6c61 7573 652e 2049  LECT`` clause. I
+0000d1f0: 6620 6120 6060 5748 4552 4560 6020 636f  f a ``WHERE`` co
+0000d200: 6e64 6974 696f 6e0a 2020 2020 2020 2020  ndition.        
+0000d210: 2020 2020 6f6e 2060 6072 6570 6f72 745f      on ``report_
+0000d220: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
+0000d230: 206e 6f74 2073 7065 6369 6669 6564 2069   not specified i
+0000d240: 6e20 7468 6520 7175 6572 792c 0a20 2020  n the query,.   
+0000d250: 2020 2020 2020 2020 2072 616e 6b69 6e67           ranking
+0000d260: 7320 666f 7220 616c 6c20 746f 702d 6c65  s for all top-le
+0000d270: 7665 6c20 6361 7465 676f 7269 6573 2061  vel categories a
+0000d280: 7265 2072 6574 7572 6e65 642e 0a0a 2020  re returned...  
+0000d290: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000d2a0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000d2b0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000d2c0: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
+0000d2d0: 6964 6060 2e0a 2020 2020 2020 2020 7469  id``..        ti
+0000d2e0: 746c 6520 2873 7472 293a 0a20 2020 2020  tle (str):.     
+0000d2f0: 2020 2020 2020 2054 6974 6c65 206f 6620         Title of 
+0000d300: 7468 6520 7072 6f64 7563 7420 636c 7573  the product clus
+0000d310: 7465 722e 0a0a 2020 2020 2020 2020 2020  ter...          
+0000d320: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000d330: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000d340: 6f66 605f 2060 605f 7469 746c 6560 602e  of`_ ``_title``.
+0000d350: 0a20 2020 2020 2020 2062 7261 6e64 2028  .        brand (
+0000d360: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000d370: 2020 4272 616e 6420 6f66 2074 6865 2070    Brand of the p
+0000d380: 726f 6475 6374 2063 6c75 7374 6572 2e0a  roduct cluster..
+0000d390: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000d3a0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000d3b0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000d3c0: 6060 5f62 7261 6e64 6060 2e0a 2020 2020  ``_brand``..    
+0000d3d0: 2020 2020 6361 7465 676f 7279 5f6c 3120      category_l1 
+0000d3e0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000d3f0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
+0000d400: 6f72 7920 2831 7374 206c 6576 656c 2920  ory (1st level) 
+0000d410: 6f66 2074 6865 2070 726f 6475 6374 2063  of the product c
+0000d420: 6c75 7374 6572 2c0a 2020 2020 2020 2020  luster,.        
+0000d430: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
+0000d440: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+0000d450: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+0000d460: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+0000d470: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+0000d480: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+0000d490: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+0000d4a0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+0000d4b0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+0000d4c0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+0000d4d0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
+0000d4e0: 6c31 6060 2e0a 2020 2020 2020 2020 6361  l1``..        ca
+0000d4f0: 7465 676f 7279 5f6c 3220 2873 7472 293a  tegory_l2 (str):
+0000d500: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
+0000d510: 6475 6374 2063 6174 6567 6f72 7920 2832  duct category (2
+0000d520: 6e64 206c 6576 656c 2920 6f66 2074 6865  nd level) of the
+0000d530: 2070 726f 6475 6374 2063 6c75 7374 6572   product cluster
+0000d540: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+0000d550: 7072 6573 656e 7465 6420 696e 2060 476f  presented in `Go
+0000d560: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
+0000d570: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
+0000d580: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
+0000d590: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000d5a0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000d5b0: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
+0000d5c0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000d5d0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000d5e0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000d5f0: 5f63 6174 6567 6f72 795f 6c32 6060 2e0a  _category_l2``..
+0000d600: 2020 2020 2020 2020 6361 7465 676f 7279          category
+0000d610: 5f6c 3320 2873 7472 293a 0a20 2020 2020  _l3 (str):.     
+0000d620: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
+0000d630: 6174 6567 6f72 7920 2833 7264 206c 6576  ategory (3rd lev
+0000d640: 656c 2920 6f66 2074 6865 2070 726f 6475  el) of the produ
+0000d650: 6374 2063 6c75 7374 6572 2c0a 2020 2020  ct cluster,.    
+0000d660: 2020 2020 2020 2020 7265 7072 6573 656e          represen
+0000d670: 7465 6420 696e 2060 476f 6f67 6c65 2773  ted in `Google's
+0000d680: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
+0000d690: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
+0000d6a0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000d6b0: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000d6c0: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
+0000d6d0: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
+0000d6e0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000d6f0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000d700: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
+0000d710: 6f72 795f 6c33 6060 2e0a 2020 2020 2020  ory_l3``..      
+0000d720: 2020 6361 7465 676f 7279 5f6c 3420 2873    category_l4 (s
+0000d730: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000d740: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
+0000d750: 7920 2834 7468 206c 6576 656c 2920 6f66  y (4th level) of
+0000d760: 2074 6865 2070 726f 6475 6374 2063 6c75   the product clu
+0000d770: 7374 6572 2c0a 2020 2020 2020 2020 2020  ster,.          
+0000d780: 2020 7265 7072 6573 656e 7465 6420 696e    represented in
+0000d790: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
+0000d7a0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
+0000d7b0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
+0000d7c0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+0000d7d0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+0000d7e0: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
+0000d7f0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000d800: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000d810: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000d820: 5f20 6060 5f63 6174 6567 6f72 795f 6c34  _ ``_category_l4
+0000d830: 6060 2e0a 2020 2020 2020 2020 6361 7465  ``..        cate
+0000d840: 676f 7279 5f6c 3520 2873 7472 293a 0a20  gory_l5 (str):. 
+0000d850: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
+0000d860: 6374 2063 6174 6567 6f72 7920 2835 7468  ct category (5th
+0000d870: 206c 6576 656c 2920 6f66 2074 6865 2070   level) of the p
+0000d880: 726f 6475 6374 2063 6c75 7374 6572 2c0a  roduct cluster,.
+0000d890: 2020 2020 2020 2020 2020 2020 7265 7072              repr
+0000d8a0: 6573 656e 7465 6420 696e 2060 476f 6f67  esented in `Goog
+0000d8b0: 6c65 2773 2070 726f 6475 6374 0a20 2020  le's product.   
+0000d8c0: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
+0000d8d0: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
+0000d8e0: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+0000d8f0: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
+0000d900: 3332 3434 3336 3e60 5f5f 2e0a 0a20 2020  324436>`__...   
+0000d910: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+0000d920: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+0000d930: 6f66 2060 6f6e 656f 6660 5f20 6060 5f63  of `oneof`_ ``_c
+0000d940: 6174 6567 6f72 795f 6c35 6060 2e0a 2020  ategory_l5``..  
+0000d950: 2020 2020 2020 7661 7269 616e 745f 6774        variant_gt
+0000d960: 696e 7320 284d 7574 6162 6c65 5365 7175  ins (MutableSequ
+0000d970: 656e 6365 5b73 7472 5d29 3a0a 2020 2020  ence[str]):.    
+0000d980: 2020 2020 2020 2020 4754 494e 7320 6f66          GTINs of
+0000d990: 2065 7861 6d70 6c65 2076 6172 6961 6e74   example variant
+0000d9a0: 7320 6f66 2074 6865 2070 726f 6475 6374  s of the product
+0000d9b0: 0a20 2020 2020 2020 2020 2020 2063 6c75  .            clu
+0000d9c0: 7374 6572 2e0a 2020 2020 2020 2020 696e  ster..        in
+0000d9d0: 7665 6e74 6f72 795f 7374 6174 7573 2028  ventory_status (
+0000d9e0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+0000d9f0: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
+0000da00: 5f76 3162 6574 612e 7479 7065 732e 4265  _v1beta.types.Be
+0000da10: 7374 5365 6c6c 6572 7350 726f 6475 6374  stSellersProduct
+0000da20: 436c 7573 7465 7256 6965 772e 496e 7665  ClusterView.Inve
+0000da30: 6e74 6f72 7953 7461 7475 7329 3a0a 2020  ntoryStatus):.  
+0000da40: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+0000da50: 7220 7468 6520 7072 6f64 7563 7420 636c  r the product cl
+0000da60: 7573 7465 7220 6973 2060 6049 4e5f 5354  uster is ``IN_ST
+0000da70: 4f43 4b60 6020 696e 2079 6f75 7220 7072  OCK`` in your pr
+0000da80: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+0000da90: 2020 6665 6564 2069 6e20 6174 206c 6561    feed in at lea
+0000daa0: 7374 206f 6e65 206f 6620 7468 6520 636f  st one of the co
+0000dab0: 756e 7472 6965 732c 2060 604f 5554 5f4f  untries, ``OUT_O
+0000dac0: 465f 5354 4f43 4b60 6020 696e 0a20 2020  F_STOCK`` in.   
+0000dad0: 2020 2020 2020 2020 2079 6f75 7220 7072           your pr
+0000dae0: 6f64 7563 7420 6665 6564 2069 6e20 616c  oduct feed in al
+0000daf0: 6c20 636f 756e 7472 6965 732c 206f 7220  l countries, or 
+0000db00: 6060 4e4f 545f 494e 5f49 4e56 454e 544f  ``NOT_IN_INVENTO
+0000db10: 5259 6060 0a20 2020 2020 2020 2020 2020  RY``.           
+0000db20: 2061 7420 616c 6c2e 0a0a 2020 2020 2020   at all...      
+0000db30: 2020 2020 2020 5468 6520 6669 656c 6420        The field 
+0000db40: 646f 6573 6e27 7420 7461 6b65 2074 6865  doesn't take the
+0000db50: 2042 6573 7420 7365 6c6c 6572 7320 7265   Best sellers re
+0000db60: 706f 7274 2063 6f75 6e74 7279 0a20 2020  port country.   
+0000db70: 2020 2020 2020 2020 2066 696c 7465 7220           filter 
+0000db80: 696e 746f 2061 6363 6f75 6e74 2e0a 0a20  into account... 
+0000db90: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000dba0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000dbb0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000dbc0: 5f69 6e76 656e 746f 7279 5f73 7461 7475  _inventory_statu
+0000dbd0: 7360 602e 0a20 2020 2020 2020 2062 7261  s``..        bra
+0000dbe0: 6e64 5f69 6e76 656e 746f 7279 5f73 7461  nd_inventory_sta
+0000dbf0: 7475 7320 2867 6f6f 676c 652e 7368 6f70  tus (google.shop
+0000dc00: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
+0000dc10: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
+0000dc20: 6573 2e42 6573 7453 656c 6c65 7273 5072  es.BestSellersPr
+0000dc30: 6f64 7563 7443 6c75 7374 6572 5669 6577  oductClusterView
+0000dc40: 2e49 6e76 656e 746f 7279 5374 6174 7573  .InventoryStatus
+0000dc50: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
+0000dc60: 6865 7468 6572 2074 6865 7265 2069 7320  hether there is 
+0000dc70: 6174 206c 6561 7374 206f 6e65 2070 726f  at least one pro
+0000dc80: 6475 6374 206f 6620 7468 6520 6272 616e  duct of the bran
+0000dc90: 6420 6375 7272 656e 746c 790a 2020 2020  d currently.    
+0000dca0: 2020 2020 2020 2020 6060 494e 5f53 544f          ``IN_STO
+0000dcb0: 434b 6060 2069 6e20 796f 7572 2070 726f  CK`` in your pro
+0000dcc0: 6475 6374 2066 6565 6420 696e 2061 7420  duct feed in at 
+0000dcd0: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
+0000dce0: 0a20 2020 2020 2020 2020 2020 2063 6f75  .            cou
+0000dcf0: 6e74 7269 6573 2c20 616c 6c20 7072 6f64  ntries, all prod
+0000dd00: 7563 7473 2061 7265 2060 604f 5554 5f4f  ucts are ``OUT_O
+0000dd10: 465f 5354 4f43 4b60 6020 696e 2079 6f75  F_STOCK`` in you
+0000dd20: 7220 7072 6f64 7563 740a 2020 2020 2020  r product.      
+0000dd30: 2020 2020 2020 6665 6564 2069 6e20 616c        feed in al
+0000dd40: 6c20 636f 756e 7472 6965 732c 206f 7220  l countries, or 
+0000dd50: 6060 4e4f 545f 494e 5f49 4e56 454e 544f  ``NOT_IN_INVENTO
+0000dd60: 5259 6060 2e0a 0a20 2020 2020 2020 2020  RY``...         
+0000dd70: 2020 2054 6865 2066 6965 6c64 2064 6f65     The field doe
+0000dd80: 736e 2774 2074 616b 6520 7468 6520 4265  sn't take the Be
+0000dd90: 7374 2073 656c 6c65 7273 2072 6570 6f72  st sellers repor
+0000dda0: 7420 636f 756e 7472 790a 2020 2020 2020  t country.      
+0000ddb0: 2020 2020 2020 6669 6c74 6572 2069 6e74        filter int
+0000ddc0: 6f20 6163 636f 756e 742e 0a0a 2020 2020  o account...    
+0000ddd0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000dde0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000ddf0: 6620 606f 6e65 6f66 605f 2060 605f 6272  f `oneof`_ ``_br
+0000de00: 616e 645f 696e 7665 6e74 6f72 795f 7374  and_inventory_st
+0000de10: 6174 7573 6060 2e0a 2020 2020 2020 2020  atus``..        
+0000de20: 7261 6e6b 2028 696e 7429 3a0a 2020 2020  rank (int):.    
+0000de30: 2020 2020 2020 2020 506f 7075 6c61 7269          Populari
+0000de40: 7479 206f 6620 7468 6520 7072 6f64 7563  ty of the produc
+0000de50: 7420 636c 7573 7465 7220 6f6e 2041 6473  t cluster on Ads
+0000de60: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000de70: 206f 7267 616e 6963 2073 7572 6661 6365   organic surface
+0000de80: 732c 2069 6e20 7468 6520 7365 6c65 6374  s, in the select
+0000de90: 6564 2063 6174 6567 6f72 7920 616e 640a  ed category and.
+0000dea0: 2020 2020 2020 2020 2020 2020 636f 756e              coun
+0000deb0: 7472 792c 2062 6173 6564 206f 6e20 7468  try, based on th
+0000dec0: 6520 6573 7469 6d61 7465 6420 6e75 6d62  e estimated numb
+0000ded0: 6572 206f 6620 756e 6974 730a 2020 2020  er of units.    
+0000dee0: 2020 2020 2020 2020 736f 6c64 2e0a 0a20          sold... 
+0000def0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000df00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000df10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000df20: 5f72 616e 6b60 602e 0a20 2020 2020 2020  _rank``..       
+0000df30: 2070 7265 7669 6f75 735f 7261 6e6b 2028   previous_rank (
+0000df40: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+0000df50: 2020 506f 7075 6c61 7269 7479 2072 616e    Popularity ran
+0000df60: 6b20 696e 2074 6865 2070 7265 7669 6f75  k in the previou
+0000df70: 7320 7765 656b 206f 720a 2020 2020 2020  s week or.      
+0000df80: 2020 2020 2020 6d6f 6e74 682e 0a0a 2020        month...  
+0000df90: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000dfa0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000dfb0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000dfc0: 7072 6576 696f 7573 5f72 616e 6b60 602e  previous_rank``.
+0000dfd0: 0a20 2020 2020 2020 2072 656c 6174 6976  .        relativ
+0000dfe0: 655f 6465 6d61 6e64 2028 676f 6f67 6c65  e_demand (google
+0000dff0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
+0000e000: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
+0000e010: 612e 7479 7065 732e 5265 6c61 7469 7665  a.types.Relative
+0000e020: 4465 6d61 6e64 2e52 656c 6174 6976 6544  Demand.RelativeD
+0000e030: 656d 616e 6445 6e75 6d29 3a0a 2020 2020  emandEnum):.    
+0000e040: 2020 2020 2020 2020 4573 7469 6d61 7465          Estimate
+0000e050: 6420 6465 6d61 6e64 2069 6e20 7265 6c61  d demand in rela
+0000e060: 7469 6f6e 2074 6f20 7468 6520 7072 6f64  tion to the prod
+0000e070: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+0000e080: 636c 7573 7465 7220 7769 7468 2074 6865  cluster with the
+0000e090: 2068 6967 6865 7374 2070 6f70 756c 6172   highest popular
+0000e0a0: 6974 7920 7261 6e6b 2069 6e20 7468 650a  ity rank in the.
+0000e0b0: 2020 2020 2020 2020 2020 2020 7361 6d65              same
+0000e0c0: 2063 6174 6567 6f72 7920 616e 6420 636f   category and co
+0000e0d0: 756e 7472 792e 0a0a 2020 2020 2020 2020  untry...        
+0000e0e0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000e0f0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000e100: 6e65 6f66 605f 2060 605f 7265 6c61 7469  neof`_ ``_relati
+0000e110: 7665 5f64 656d 616e 6460 602e 0a20 2020  ve_demand``..   
+0000e120: 2020 2020 2070 7265 7669 6f75 735f 7265       previous_re
+0000e130: 6c61 7469 7665 5f64 656d 616e 6420 2867  lative_demand (g
+0000e140: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
+0000e150: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
+0000e160: 7631 6265 7461 2e74 7970 6573 2e52 656c  v1beta.types.Rel
+0000e170: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
+0000e180: 7469 7665 4465 6d61 6e64 456e 756d 293a  tiveDemandEnum):
+0000e190: 0a20 2020 2020 2020 2020 2020 2045 7374  .            Est
+0000e1a0: 696d 6174 6564 2064 656d 616e 6420 696e  imated demand in
+0000e1b0: 2072 656c 6174 696f 6e20 746f 2074 6865   relation to the
+0000e1c0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
+0000e1d0: 2020 2020 2063 6c75 7374 6572 2077 6974       cluster wit
+0000e1e0: 6820 7468 6520 6869 6768 6573 7420 706f  h the highest po
+0000e1f0: 7075 6c61 7269 7479 2072 616e 6b20 696e  pularity rank in
+0000e200: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+0000e210: 2073 616d 6520 6361 7465 676f 7279 2061   same category a
+0000e220: 6e64 2063 6f75 6e74 7279 2069 6e20 7468  nd country in th
+0000e230: 6520 7072 6576 696f 7573 2077 6565 6b0a  e previous week.
+0000e240: 2020 2020 2020 2020 2020 2020 6f72 206d              or m
+0000e250: 6f6e 7468 2e0a 0a20 2020 2020 2020 2020  onth...         
+0000e260: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000e270: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000e280: 656f 6660 5f20 6060 5f70 7265 7669 6f75  eof`_ ``_previou
+0000e290: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
+0000e2a0: 6460 602e 0a20 2020 2020 2020 2072 656c  d``..        rel
+0000e2b0: 6174 6976 655f 6465 6d61 6e64 5f63 6861  ative_demand_cha
+0000e2c0: 6e67 6520 2867 6f6f 676c 652e 7368 6f70  nge (google.shop
+0000e2d0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
+0000e2e0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
+0000e2f0: 6573 2e52 656c 6174 6976 6544 656d 616e  es.RelativeDeman
+0000e300: 6443 6861 6e67 6554 7970 652e 5265 6c61  dChangeType.Rela
+0000e310: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
+0000e320: 5479 7065 456e 756d 293a 0a20 2020 2020  TypeEnum):.     
+0000e330: 2020 2020 2020 2043 6861 6e67 6520 696e         Change in
+0000e340: 2074 6865 2065 7374 696d 6174 6564 2064   the estimated d
+0000e350: 656d 616e 642e 2057 6865 7468 6572 2069  emand. Whether i
+0000e360: 740a 2020 2020 2020 2020 2020 2020 726f  t.            ro
+0000e370: 7365 2c20 7361 6e6b 206f 7220 7265 6d61  se, sank or rema
+0000e380: 696e 6564 2066 6c61 742e 0a0a 2020 2020  ined flat...    
+0000e390: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000e3a0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000e3b0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+0000e3c0: 6c61 7469 7665 5f64 656d 616e 645f 6368  lative_demand_ch
+0000e3d0: 616e 6765 6060 2e0a 2020 2020 2222 220a  ange``..    """.
+0000e3e0: 0a20 2020 2063 6c61 7373 2049 6e76 656e  .    class Inven
+0000e3f0: 746f 7279 5374 6174 7573 2870 726f 746f  toryStatus(proto
+0000e400: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
+0000e410: 7222 2222 5374 6174 7573 206f 6620 7468  r"""Status of th
+0000e420: 6520 7072 6f64 7563 7420 636c 7573 7465  e product cluste
+0000e430: 7220 6f72 2062 7261 6e64 2069 6e20 796f  r or brand in yo
+0000e440: 7572 2069 6e76 656e 746f 7279 2e0a 0a20  ur inventory... 
+0000e450: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
+0000e460: 2020 2020 2020 2020 2020 2049 4e56 454e             INVEN
+0000e470: 544f 5259 5f53 5441 5455 535f 554e 5350  TORY_STATUS_UNSP
+0000e480: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
+0000e490: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
+0000e4a0: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
+0000e4b0: 2020 2020 2020 2020 494e 5f53 544f 434b          IN_STOCK
+0000e4c0: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+0000e4d0: 2020 2020 2020 596f 7520 6861 7665 2061        You have a
+0000e4e0: 2070 726f 6475 6374 2066 6f72 2074 6869   product for thi
+0000e4f0: 7320 7072 6f64 7563 7420 636c 7573 7465  s product cluste
+0000e500: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000e510: 2020 6f72 2062 7261 6e64 2069 6e20 7374    or brand in st
+0000e520: 6f63 6b2e 0a20 2020 2020 2020 2020 2020  ock..           
+0000e530: 204f 5554 5f4f 465f 5354 4f43 4b20 2832   OUT_OF_STOCK (2
+0000e540: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e550: 2020 2059 6f75 2068 6176 6520 6120 7072     You have a pr
+0000e560: 6f64 7563 7420 666f 7220 7468 6973 2070  oduct for this p
+0000e570: 726f 6475 6374 2063 6c75 7374 6572 0a20  roduct cluster. 
+0000e580: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000e590: 7220 6272 616e 6420 696e 2069 6e76 656e  r brand in inven
+0000e5a0: 746f 7279 2062 7574 2069 7420 6973 2063  tory but it is c
+0000e5b0: 7572 7265 6e74 6c79 206f 7574 206f 660a  urrently out of.
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 7374 6f63 6b2e 0a20 2020 2020 2020 2020  stock..         
+0000e5e0: 2020 204e 4f54 5f49 4e5f 494e 5645 4e54     NOT_IN_INVENT
+0000e5f0: 4f52 5920 2833 293a 0a20 2020 2020 2020  ORY (3):.       
+0000e600: 2020 2020 2020 2020 2059 6f75 2064 6f20           You do 
+0000e610: 6e6f 7420 6861 7665 2061 2070 726f 6475  not have a produ
+0000e620: 6374 2066 6f72 2074 6869 7320 7072 6f64  ct for this prod
+0000e630: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+0000e640: 2020 2020 636c 7573 7465 7220 6f72 2062      cluster or b
+0000e650: 7261 6e64 2069 6e20 696e 7665 6e74 6f72  rand in inventor
+0000e660: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+0000e670: 2020 2020 2020 2049 4e56 454e 544f 5259         INVENTORY
+0000e680: 5f53 5441 5455 535f 554e 5350 4543 4946  _STATUS_UNSPECIF
+0000e690: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
+0000e6a0: 494e 5f53 544f 434b 203d 2031 0a20 2020  IN_STOCK = 1.   
+0000e6b0: 2020 2020 204f 5554 5f4f 465f 5354 4f43       OUT_OF_STOC
+0000e6c0: 4b20 3d20 320a 2020 2020 2020 2020 4e4f  K = 2.        NO
+0000e6d0: 545f 494e 5f49 4e56 454e 544f 5259 203d  T_IN_INVENTORY =
+0000e6e0: 2033 0a0a 2020 2020 7265 706f 7274 5f64   3..    report_d
+0000e6f0: 6174 653a 2064 6174 655f 7062 322e 4461  ate: date_pb2.Da
+0000e700: 7465 203d 2070 726f 746f 2e46 6965 6c64  te = proto.Field
+0000e710: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000e720: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+0000e730: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
+0000e740: 2020 206d 6573 7361 6765 3d64 6174 655f     message=date_
+0000e750: 7062 322e 4461 7465 2c0a 2020 2020 290a  pb2.Date,.    ).
+0000e760: 2020 2020 7265 706f 7274 5f67 7261 6e75      report_granu
+0000e770: 6c61 7269 7479 3a20 2252 6570 6f72 7447  larity: "ReportG
+0000e780: 7261 6e75 6c61 7269 7479 2e52 6570 6f72  ranularity.Repor
+0000e790: 7447 7261 6e75 6c61 7269 7479 456e 756d  tGranularityEnum
+0000e7a0: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
+0000e7b0: 0a20 2020 2020 2020 2070 726f 746f 2e45  .        proto.E
+0000e7c0: 4e55 4d2c 0a20 2020 2020 2020 206e 756d  NUM,.        num
+0000e7d0: 6265 723d 322c 0a20 2020 2020 2020 206f  ber=2,.        o
+0000e7e0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000e7f0: 2020 2020 2020 656e 756d 3d22 5265 706f        enum="Repo
+0000e800: 7274 4772 616e 756c 6172 6974 792e 5265  rtGranularity.Re
+0000e810: 706f 7274 4772 616e 756c 6172 6974 7945  portGranularityE
 0000e820: 6e75 6d22 2c0a 2020 2020 290a 2020 2020  num",.    ).    
-0000e830: 7265 6c61 7469 7665 5f64 656d 616e 645f  relative_demand_
-0000e840: 6368 616e 6765 3a20 2252 656c 6174 6976  change: "Relativ
-0000e850: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
-0000e860: 652e 5265 6c61 7469 7665 4465 6d61 6e64  e.RelativeDemand
-0000e870: 4368 616e 6765 5479 7065 456e 756d 2220  ChangeTypeEnum" 
-0000e880: 3d20 280a 2020 2020 2020 2020 7072 6f74  = (.        prot
-0000e890: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000e8a0: 2020 2020 2070 726f 746f 2e45 4e55 4d2c       proto.ENUM,
-0000e8b0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-0000e8c0: 6265 723d 3230 2c0a 2020 2020 2020 2020  ber=20,.        
-0000e8d0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000e8e0: 652c 0a20 2020 2020 2020 2020 2020 2065  e,.            e
-0000e8f0: 6e75 6d3d 2252 656c 6174 6976 6544 656d  num="RelativeDem
-0000e900: 616e 6443 6861 6e67 6554 7970 652e 5265  andChangeType.Re
-0000e910: 6c61 7469 7665 4465 6d61 6e64 4368 616e  lativeDemandChan
-0000e920: 6765 5479 7065 456e 756d 222c 0a20 2020  geTypeEnum",.   
-0000e930: 2020 2020 2029 0a20 2020 2029 0a0a 0a63       ).    )...c
-0000e940: 6c61 7373 2042 6573 7453 656c 6c65 7273  lass BestSellers
-0000e950: 4272 616e 6456 6965 7728 7072 6f74 6f2e  BrandView(proto.
-0000e960: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-0000e970: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
-0000e980: 6c65 2066 6f72 2071 7565 7279 2069 6e20  le for query in 
-0000e990: 6060 6265 7374 5f73 656c 6c65 7273 5f62  ``best_sellers_b
-0000e9a0: 7261 6e64 5f76 6965 7760 6020 7461 626c  rand_view`` tabl
-0000e9b0: 652e 0a0a 2020 2020 6042 6573 740a 2020  e...    `Best.  
-0000e9c0: 2020 7365 6c6c 6572 7320 3c68 7474 7073    sellers <https
-0000e9d0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000e9e0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000e9f0: 616e 7377 6572 2f39 3438 3836 3739 3e60  answer/9488679>`
-0000ea00: 5f5f 0a20 2020 2072 6570 6f72 7420 7769  __.    report wi
-0000ea10: 7468 2074 6f70 2062 7261 6e64 732e 0a0a  th top brands...
-0000ea20: 2020 2020 5661 6c75 6573 2061 7265 206f      Values are o
-0000ea30: 6e6c 7920 7365 7420 666f 7220 6669 656c  nly set for fiel
-0000ea40: 6473 2072 6571 7565 7374 6564 2065 7870  ds requested exp
-0000ea50: 6c69 6369 746c 7920 696e 2074 6865 2072  licitly in the r
-0000ea60: 6571 7565 7374 2773 0a20 2020 2073 6561  equest's.    sea
-0000ea70: 7263 6820 7175 6572 792e 0a0a 0a20 2020  rch query....   
-0000ea80: 202e 2e20 5f6f 6e65 6f66 3a20 6874 7470   .. _oneof: http
-0000ea90: 733a 2f2f 7072 6f74 6f2d 706c 7573 2d70  s://proto-plus-p
-0000eaa0: 7974 686f 6e2e 7265 6164 7468 6564 6f63  ython.readthedoc
-0000eab0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f66  s.io/en/stable/f
-0000eac0: 6965 6c64 732e 6874 6d6c 236f 6e65 6f66  ields.html#oneof
-0000ead0: 732d 6d75 7475 616c 6c79 2d65 7863 6c75  s-mutually-exclu
-0000eae0: 7369 7665 2d66 6965 6c64 730a 0a20 2020  sive-fields..   
-0000eaf0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-0000eb00: 2020 2020 2072 6570 6f72 745f 6461 7465       report_date
-0000eb10: 2028 676f 6f67 6c65 2e74 7970 652e 6461   (google.type.da
-0000eb20: 7465 5f70 6232 2e44 6174 6529 3a0a 2020  te_pb2.Date):.  
-0000eb30: 2020 2020 2020 2020 2020 5265 706f 7274            Report
-0000eb40: 2064 6174 652e 2054 6865 2076 616c 7565   date. The value
-0000eb50: 206f 6620 7468 6973 2066 6965 6c64 2063   of this field c
-0000eb60: 616e 206f 6e6c 7920 6265 206f 6e65 206f  an only be one o
-0000eb70: 6620 7468 650a 2020 2020 2020 2020 2020  f the.          
-0000eb80: 2020 666f 6c6c 6f77 696e 673a 0a0a 2020    following:..  
-0000eb90: 2020 2020 2020 2020 2020 2d20 2054 6865            -  The
-0000eba0: 2066 6972 7374 2064 6179 206f 6620 7468   first day of th
-0000ebb0: 6520 7765 656b 2028 4d6f 6e64 6179 2920  e week (Monday) 
-0000ebc0: 666f 7220 7765 656b 6c79 2072 6570 6f72  for weekly repor
-0000ebd0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0000ebe0: 2d20 2054 6865 2066 6972 7374 2064 6179  -  The first day
-0000ebf0: 206f 6620 7468 6520 6d6f 6e74 6820 666f   of the month fo
-0000ec00: 7220 6d6f 6e74 686c 7920 7265 706f 7274  r monthly report
-0000ec10: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
-0000ec20: 5265 7175 6972 6564 2069 6e20 7468 6520  Required in the 
-0000ec30: 6060 5345 4c45 4354 6060 2063 6c61 7573  ``SELECT`` claus
-0000ec40: 652e 2049 6620 6120 6060 5748 4552 4560  e. If a ``WHERE`
-0000ec50: 6020 636f 6e64 6974 696f 6e0a 2020 2020  ` condition.    
-0000ec60: 2020 2020 2020 2020 6f6e 2060 6072 6570          on ``rep
-0000ec70: 6f72 745f 6461 7465 6060 2069 7320 6e6f  ort_date`` is no
-0000ec80: 7420 7370 6563 6966 6965 6420 696e 2074  t specified in t
-0000ec90: 6865 2071 7565 7279 2c20 7468 6520 6c61  he query, the la
-0000eca0: 7465 7374 0a20 2020 2020 2020 2020 2020  test.           
-0000ecb0: 2061 7661 696c 6162 6c65 2077 6565 6b6c   available weekl
-0000ecc0: 7920 6f72 206d 6f6e 7468 6c79 2072 6570  y or monthly rep
-0000ecd0: 6f72 7420 6973 2072 6574 7572 6e65 642e  ort is returned.
-0000ece0: 0a20 2020 2020 2020 2072 6570 6f72 745f  .        report_
-0000ecf0: 6772 616e 756c 6172 6974 7920 2867 6f6f  granularity (goo
-0000ed00: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
-0000ed10: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
-0000ed20: 6265 7461 2e74 7970 6573 2e52 6570 6f72  beta.types.Repor
-0000ed30: 7447 7261 6e75 6c61 7269 7479 2e52 6570  tGranularity.Rep
-0000ed40: 6f72 7447 7261 6e75 6c61 7269 7479 456e  ortGranularityEn
-0000ed50: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-0000ed60: 2047 7261 6e75 6c61 7269 7479 206f 6620   Granularity of 
-0000ed70: 7468 6520 7265 706f 7274 2e20 5468 6520  the report. The 
-0000ed80: 7261 6e6b 696e 6720 6361 6e20 6265 2064  ranking can be d
-0000ed90: 6f6e 6520 6f76 6572 2061 0a20 2020 2020  one over a.     
-0000eda0: 2020 2020 2020 2077 6565 6b20 6f72 2061         week or a
-0000edb0: 206d 6f6e 7468 2074 696d 6566 7261 6d65   month timeframe
-0000edc0: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-0000edd0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-0000ede0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-0000edf0: 2e20 436f 6e64 6974 696f 6e20 6f6e 0a20  . Condition on. 
-0000ee00: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
-0000ee10: 6f72 745f 6772 616e 756c 6172 6974 7960  ort_granularity`
-0000ee20: 6020 6973 2072 6571 7569 7265 6420 696e  ` is required in
-0000ee30: 2074 6865 2060 6057 4845 5245 6060 2063   the ``WHERE`` c
-0000ee40: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
-0000ee50: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-0000ee60: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-0000ee70: 6e65 6f66 605f 2060 605f 7265 706f 7274  neof`_ ``_report
-0000ee80: 5f67 7261 6e75 6c61 7269 7479 6060 2e0a  _granularity``..
-0000ee90: 2020 2020 2020 2020 7265 706f 7274 5f63          report_c
-0000eea0: 6f75 6e74 7279 5f63 6f64 6520 2873 7472  ountry_code (str
-0000eeb0: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
-0000eec0: 6f75 6e74 7279 2077 6865 7265 2074 6865  ountry where the
-0000eed0: 2072 616e 6b69 6e67 2069 7320 6361 6c63   ranking is calc
-0000eee0: 756c 6174 6564 2e20 5265 7072 6573 656e  ulated. Represen
-0000eef0: 7465 6420 696e 2074 6865 0a20 2020 2020  ted in the.     
-0000ef00: 2020 2020 2020 2049 534f 2033 3136 3620         ISO 3166 
-0000ef10: 666f 726d 6174 2e0a 0a20 2020 2020 2020  format...       
-0000ef20: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
-0000ef30: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
-0000ef40: 636c 6175 7365 2e20 436f 6e64 6974 696f  clause. Conditio
-0000ef50: 6e20 6f6e 0a20 2020 2020 2020 2020 2020  n on.           
-0000ef60: 2060 6072 6570 6f72 745f 636f 756e 7472   ``report_countr
-0000ef70: 795f 636f 6465 6060 2069 7320 7265 7175  y_code`` is requ
-0000ef80: 6972 6564 2069 6e20 7468 6520 6060 5748  ired in the ``WH
-0000ef90: 4552 4560 6020 636c 6175 7365 2e0a 0a20  ERE`` clause... 
-0000efa0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000efb0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000efc0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000efd0: 5f72 6570 6f72 745f 636f 756e 7472 795f  _report_country_
-0000efe0: 636f 6465 6060 2e0a 2020 2020 2020 2020  code``..        
-0000eff0: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
-0000f000: 6964 2028 696e 7429 3a0a 2020 2020 2020  id (int):.      
-0000f010: 2020 2020 2020 476f 6f67 6c65 2070 726f        Google pro
-0000f020: 6475 6374 2063 6174 6567 6f72 7920 4944  duct category ID
-0000f030: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-0000f040: 6520 7261 6e6b 696e 6720 666f 722c 0a20  e ranking for,. 
-0000f050: 2020 2020 2020 2020 2020 2072 6570 7265             repre
-0000f060: 7365 6e74 6564 2069 6e20 6047 6f6f 676c  sented in `Googl
-0000f070: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
-0000f080: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
-0000f090: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
-0000f0a0: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
-0000f0b0: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
-0000f0c0: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
-0000f0d0: 2020 2020 2020 2020 5265 7175 6972 6564          Required
-0000f0e0: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
-0000f0f0: 6060 2063 6c61 7573 652e 2049 6620 6120  `` clause. If a 
-0000f100: 6060 5748 4552 4560 6020 636f 6e64 6974  ``WHERE`` condit
-0000f110: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000f120: 6f6e 2060 6072 6570 6f72 745f 6361 7465  on ``report_cate
-0000f130: 676f 7279 5f69 6460 6020 6973 206e 6f74  gory_id`` is not
-0000f140: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
-0000f150: 6520 7175 6572 792c 0a20 2020 2020 2020  e query,.       
-0000f160: 2020 2020 2072 616e 6b69 6e67 7320 666f       rankings fo
-0000f170: 7220 616c 6c20 746f 702d 6c65 7665 6c20  r all top-level 
-0000f180: 6361 7465 676f 7269 6573 2061 7265 2072  categories are r
-0000f190: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
-0000f1a0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-0000f1b0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-0000f1c0: 606f 6e65 6f66 605f 2060 605f 7265 706f  `oneof`_ ``_repo
-0000f1d0: 7274 5f63 6174 6567 6f72 795f 6964 6060  rt_category_id``
-0000f1e0: 2e0a 2020 2020 2020 2020 6272 616e 6420  ..        brand 
-0000f1f0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000f200: 2020 204e 616d 6520 6f66 2074 6865 2062     Name of the b
-0000f210: 7261 6e64 2e0a 0a20 2020 2020 2020 2020  rand...         
-0000f220: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000f230: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000f240: 656f 6660 5f20 6060 5f62 7261 6e64 6060  eof`_ ``_brand``
-0000f250: 2e0a 2020 2020 2020 2020 7261 6e6b 2028  ..        rank (
-0000f260: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-0000f270: 2020 506f 7075 6c61 7269 7479 206f 6620    Popularity of 
-0000f280: 7468 6520 6272 616e 6420 6f6e 2041 6473  the brand on Ads
-0000f290: 2061 6e64 206f 7267 616e 6963 0a20 2020   and organic.   
-0000f2a0: 2020 2020 2020 2020 2073 7572 6661 6365           surface
-0000f2b0: 732c 2069 6e20 7468 6520 7365 6c65 6374  s, in the select
-0000f2c0: 6564 2063 6174 6567 6f72 7920 616e 6420  ed category and 
-0000f2d0: 636f 756e 7472 792c 0a20 2020 2020 2020  country,.       
-0000f2e0: 2020 2020 2062 6173 6564 206f 6e20 7468       based on th
-0000f2f0: 6520 6573 7469 6d61 7465 6420 6e75 6d62  e estimated numb
-0000f300: 6572 206f 6620 756e 6974 7320 736f 6c64  er of units sold
-0000f310: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000f320: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000f330: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000f340: 5f20 6060 5f72 616e 6b60 602e 0a20 2020  _ ``_rank``..   
-0000f350: 2020 2020 2070 7265 7669 6f75 735f 7261       previous_ra
-0000f360: 6e6b 2028 696e 7429 3a0a 2020 2020 2020  nk (int):.      
-0000f370: 2020 2020 2020 506f 7075 6c61 7269 7479        Popularity
-0000f380: 2072 616e 6b20 696e 2074 6865 2070 7265   rank in the pre
-0000f390: 7669 6f75 7320 7765 656b 206f 720a 2020  vious week or.  
-0000f3a0: 2020 2020 2020 2020 2020 6d6f 6e74 682e            month.
-0000f3b0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000f3c0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000f3d0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000f3e0: 2060 605f 7072 6576 696f 7573 5f72 616e   ``_previous_ran
-0000f3f0: 6b60 602e 0a20 2020 2020 2020 2072 656c  k``..        rel
-0000f400: 6174 6976 655f 6465 6d61 6e64 2028 676f  ative_demand (go
-0000f410: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
-0000f420: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
-0000f430: 3162 6574 612e 7479 7065 732e 5265 6c61  1beta.types.Rela
-0000f440: 7469 7665 4465 6d61 6e64 2e52 656c 6174  tiveDemand.Relat
-0000f450: 6976 6544 656d 616e 6445 6e75 6d29 3a0a  iveDemandEnum):.
-0000f460: 2020 2020 2020 2020 2020 2020 4573 7469              Esti
-0000f470: 6d61 7465 6420 6465 6d61 6e64 2069 6e20  mated demand in 
-0000f480: 7265 6c61 7469 6f6e 2074 6f20 7468 6520  relation to the 
-0000f490: 6272 616e 640a 2020 2020 2020 2020 2020  brand.          
-0000f4a0: 2020 7769 7468 2074 6865 2068 6967 6865    with the highe
-0000f4b0: 7374 2070 6f70 756c 6172 6974 7920 7261  st popularity ra
-0000f4c0: 6e6b 2069 6e20 7468 6520 7361 6d65 0a20  nk in the same. 
-0000f4d0: 2020 2020 2020 2020 2020 2063 6174 6567             categ
-0000f4e0: 6f72 7920 616e 6420 636f 756e 7472 792e  ory and country.
-0000f4f0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000f500: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000f510: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000f520: 2060 605f 7265 6c61 7469 7665 5f64 656d   ``_relative_dem
-0000f530: 616e 6460 602e 0a20 2020 2020 2020 2070  and``..        p
-0000f540: 7265 7669 6f75 735f 7265 6c61 7469 7665  revious_relative
-0000f550: 5f64 656d 616e 6420 2867 6f6f 676c 652e  _demand (google.
-0000f560: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-0000f570: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-0000f580: 2e74 7970 6573 2e52 656c 6174 6976 6544  .types.RelativeD
-0000f590: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
-0000f5a0: 6d61 6e64 456e 756d 293a 0a20 2020 2020  mandEnum):.     
-0000f5b0: 2020 2020 2020 2045 7374 696d 6174 6564         Estimated
-0000f5c0: 2064 656d 616e 6420 696e 2072 656c 6174   demand in relat
-0000f5d0: 696f 6e20 746f 2074 6865 2062 7261 6e64  ion to the brand
-0000f5e0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000f5f0: 6820 7468 6520 6869 6768 6573 7420 706f  h the highest po
-0000f600: 7075 6c61 7269 7479 2072 616e 6b20 696e  pularity rank in
-0000f610: 2074 6865 2073 616d 650a 2020 2020 2020   the same.      
-0000f620: 2020 2020 2020 6361 7465 676f 7279 2061        category a
-0000f630: 6e64 2063 6f75 6e74 7279 2069 6e20 7468  nd country in th
-0000f640: 6520 7072 6576 696f 7573 2077 6565 6b20  e previous week 
-0000f650: 6f72 0a20 2020 2020 2020 2020 2020 206d  or.            m
-0000f660: 6f6e 7468 2e0a 0a20 2020 2020 2020 2020  onth...         
-0000f670: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000f680: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000f690: 656f 6660 5f20 6060 5f70 7265 7669 6f75  eof`_ ``_previou
-0000f6a0: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
-0000f6b0: 6460 602e 0a20 2020 2020 2020 2072 656c  d``..        rel
-0000f6c0: 6174 6976 655f 6465 6d61 6e64 5f63 6861  ative_demand_cha
-0000f6d0: 6e67 6520 2867 6f6f 676c 652e 7368 6f70  nge (google.shop
-0000f6e0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
-0000f6f0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
-0000f700: 6573 2e52 656c 6174 6976 6544 656d 616e  es.RelativeDeman
-0000f710: 6443 6861 6e67 6554 7970 652e 5265 6c61  dChangeType.Rela
-0000f720: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
-0000f730: 5479 7065 456e 756d 293a 0a20 2020 2020  TypeEnum):.     
-0000f740: 2020 2020 2020 2043 6861 6e67 6520 696e         Change in
-0000f750: 2074 6865 2065 7374 696d 6174 6564 2064   the estimated d
-0000f760: 656d 616e 642e 2057 6865 7468 6572 2069  emand. Whether i
-0000f770: 740a 2020 2020 2020 2020 2020 2020 726f  t.            ro
-0000f780: 7365 2c20 7361 6e6b 206f 7220 7265 6d61  se, sank or rema
-0000f790: 696e 6564 2066 6c61 742e 0a0a 2020 2020  ined flat...    
-0000f7a0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000f7b0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000f7c0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
-0000f7d0: 6c61 7469 7665 5f64 656d 616e 645f 6368  lative_demand_ch
-0000f7e0: 616e 6765 6060 2e0a 2020 2020 2222 220a  ange``..    """.
-0000f7f0: 0a20 2020 2072 6570 6f72 745f 6461 7465  .    report_date
-0000f800: 3a20 6461 7465 5f70 6232 2e44 6174 6520  : date_pb2.Date 
-0000f810: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000f820: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-0000f830: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-0000f840: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
-0000f850: 6d65 7373 6167 653d 6461 7465 5f70 6232  message=date_pb2
-0000f860: 2e44 6174 652c 0a20 2020 2029 0a20 2020  .Date,.    ).   
-0000f870: 2072 6570 6f72 745f 6772 616e 756c 6172   report_granular
-0000f880: 6974 793a 2022 5265 706f 7274 4772 616e  ity: "ReportGran
-0000f890: 756c 6172 6974 792e 5265 706f 7274 4772  ularity.ReportGr
-0000f8a0: 616e 756c 6172 6974 7945 6e75 6d22 203d  anularityEnum" =
-0000f8b0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000f8c0: 2020 2020 2020 7072 6f74 6f2e 454e 554d        proto.ENUM
-0000f8d0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000f8e0: 3d32 2c0a 2020 2020 2020 2020 6f70 7469  =2,.        opti
-0000f8f0: 6f6e 616c 3d54 7275 652c 0a20 2020 2020  onal=True,.     
-0000f900: 2020 2065 6e75 6d3d 2252 6570 6f72 7447     enum="ReportG
-0000f910: 7261 6e75 6c61 7269 7479 2e52 6570 6f72  ranularity.Repor
-0000f920: 7447 7261 6e75 6c61 7269 7479 456e 756d  tGranularityEnum
-0000f930: 222c 0a20 2020 2029 0a20 2020 2072 6570  ",.    ).    rep
-0000f940: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-0000f950: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000f960: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000f970: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000f980: 2020 206e 756d 6265 723d 332c 0a20 2020     number=3,.   
-0000f990: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000f9a0: 7565 2c0a 2020 2020 290a 2020 2020 7265  ue,.    ).    re
-0000f9b0: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
-0000f9c0: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
-0000f9d0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000f9e0: 746f 2e49 4e54 3634 2c0a 2020 2020 2020  to.INT64,.      
-0000f9f0: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
-0000fa00: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000fa10: 652c 0a20 2020 2029 0a20 2020 2062 7261  e,.    ).    bra
-0000fa20: 6e64 3a20 7374 7220 3d20 7072 6f74 6f2e  nd: str = proto.
-0000fa30: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000fa40: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000fa50: 2020 2020 206e 756d 6265 723d 362c 0a20       number=6,. 
-0000fa60: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000fa70: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000fa80: 7261 6e6b 3a20 696e 7420 3d20 7072 6f74  rank: int = prot
-0000fa90: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000faa0: 2070 726f 746f 2e49 4e54 3634 2c0a 2020   proto.INT64,.  
-0000fab0: 2020 2020 2020 6e75 6d62 6572 3d37 2c0a        number=7,.
-0000fac0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000fad0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000fae0: 2070 7265 7669 6f75 735f 7261 6e6b 3a20   previous_rank: 
-0000faf0: 696e 7420 3d20 7072 6f74 6f2e 4669 656c  int = proto.Fiel
-0000fb00: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000fb10: 2e49 4e54 3634 2c0a 2020 2020 2020 2020  .INT64,.        
-0000fb20: 6e75 6d62 6572 3d38 2c0a 2020 2020 2020  number=8,.      
-0000fb30: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000fb40: 0a20 2020 2029 0a20 2020 2072 656c 6174  .    ).    relat
-0000fb50: 6976 655f 6465 6d61 6e64 3a20 2252 656c  ive_demand: "Rel
-0000fb60: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
-0000fb70: 7469 7665 4465 6d61 6e64 456e 756d 2220  tiveDemandEnum" 
-0000fb80: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000fb90: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-0000fba0: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
-0000fbb0: 723d 392c 0a20 2020 2020 2020 206f 7074  r=9,.        opt
-0000fbc0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000fbd0: 2020 2020 656e 756d 3d22 5265 6c61 7469      enum="Relati
-0000fbe0: 7665 4465 6d61 6e64 2e52 656c 6174 6976  veDemand.Relativ
-0000fbf0: 6544 656d 616e 6445 6e75 6d22 2c0a 2020  eDemandEnum",.  
-0000fc00: 2020 290a 2020 2020 7072 6576 696f 7573    ).    previous
-0000fc10: 5f72 656c 6174 6976 655f 6465 6d61 6e64  _relative_demand
-0000fc20: 3a20 2252 656c 6174 6976 6544 656d 616e  : "RelativeDeman
-0000fc30: 642e 5265 6c61 7469 7665 4465 6d61 6e64  d.RelativeDemand
-0000fc40: 456e 756d 2220 3d20 7072 6f74 6f2e 4669  Enum" = proto.Fi
-0000fc50: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000fc60: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
-0000fc70: 206e 756d 6265 723d 3130 2c0a 2020 2020   number=10,.    
-0000fc80: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000fc90: 652c 0a20 2020 2020 2020 2065 6e75 6d3d  e,.        enum=
-0000fca0: 2252 656c 6174 6976 6544 656d 616e 642e  "RelativeDemand.
-0000fcb0: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
-0000fcc0: 756d 222c 0a20 2020 2029 0a20 2020 2072  um",.    ).    r
-0000fcd0: 656c 6174 6976 655f 6465 6d61 6e64 5f63  elative_demand_c
-0000fce0: 6861 6e67 653a 2022 5265 6c61 7469 7665  hange: "Relative
-0000fcf0: 4465 6d61 6e64 4368 616e 6765 5479 7065  DemandChangeType
-0000fd00: 2e52 656c 6174 6976 6544 656d 616e 6443  .RelativeDemandC
-0000fd10: 6861 6e67 6554 7970 6545 6e75 6d22 203d  hangeTypeEnum" =
-0000fd20: 2028 0a20 2020 2020 2020 2070 726f 746f   (.        proto
-0000fd30: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000fd40: 2020 2020 7072 6f74 6f2e 454e 554d 2c0a      proto.ENUM,.
-0000fd50: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-0000fd60: 6572 3d31 312c 0a20 2020 2020 2020 2020  er=11,.         
-0000fd70: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000fd80: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
-0000fd90: 756d 3d22 5265 6c61 7469 7665 4465 6d61  um="RelativeDema
-0000fda0: 6e64 4368 616e 6765 5479 7065 2e52 656c  ndChangeType.Rel
-0000fdb0: 6174 6976 6544 656d 616e 6443 6861 6e67  ativeDemandChang
-0000fdc0: 6554 7970 6545 6e75 6d22 2c0a 2020 2020  eTypeEnum",.    
-0000fdd0: 2020 2020 290a 2020 2020 290a 0a0a 636c      ).    )...cl
-0000fde0: 6173 7320 436f 6d70 6574 6974 6976 6556  ass CompetitiveV
-0000fdf0: 6973 6962 696c 6974 7943 6f6d 7065 7469  isibilityCompeti
-0000fe00: 746f 7256 6965 7728 7072 6f74 6f2e 4d65  torView(proto.Me
-0000fe10: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
-0000fe20: 4669 656c 6473 2061 7661 696c 6162 6c65  Fields available
-0000fe30: 2066 6f72 2071 7565 7279 2069 6e0a 2020   for query in.  
-0000fe40: 2020 6060 636f 6d70 6574 6974 6976 655f    ``competitive_
-0000fe50: 7669 7369 6269 6c69 7479 5f63 6f6d 7065  visibility_compe
-0000fe60: 7469 746f 725f 7669 6577 6060 2074 6162  titor_view`` tab
-0000fe70: 6c65 2e0a 0a20 2020 2060 436f 6d70 6574  le...    `Compet
-0000fe80: 6974 6976 650a 2020 2020 7669 7369 6269  itive.    visibi
-0000fe90: 6c69 7479 203c 6874 7470 733a 2f2f 7375  lity <https://su
-0000fea0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-0000feb0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
-0000fec0: 722f 3131 3336 3634 3432 3e60 5f5f 0a20  r/11366442>`__. 
-0000fed0: 2020 2072 6570 6f72 7420 7769 7468 2062     report with b
-0000fee0: 7573 696e 6573 7365 7320 7769 7468 2073  usinesses with s
-0000fef0: 696d 696c 6172 2076 6973 6962 696c 6974  imilar visibilit
-0000ff00: 792e 0a0a 2020 2020 5661 6c75 6573 2061  y...    Values a
-0000ff10: 7265 206f 6e6c 7920 7365 7420 666f 7220  re only set for 
-0000ff20: 6669 656c 6473 2072 6571 7565 7374 6564  fields requested
-0000ff30: 2065 7870 6c69 6369 746c 7920 696e 2074   explicitly in t
-0000ff40: 6865 2072 6571 7565 7374 2773 0a20 2020  he request's.   
-0000ff50: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
-0000ff60: 0a20 2020 202e 2e20 5f6f 6e65 6f66 3a20  .    .. _oneof: 
-0000ff70: 6874 7470 733a 2f2f 7072 6f74 6f2d 706c  https://proto-pl
-0000ff80: 7573 2d70 7974 686f 6e2e 7265 6164 7468  us-python.readth
-0000ff90: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-0000ffa0: 6c65 2f66 6965 6c64 732e 6874 6d6c 236f  le/fields.html#o
-0000ffb0: 6e65 6f66 732d 6d75 7475 616c 6c79 2d65  neofs-mutually-e
-0000ffc0: 7863 6c75 7369 7665 2d66 6965 6c64 730a  xclusive-fields.
-0000ffd0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
-0000ffe0: 0a20 2020 2020 2020 2064 6174 6520 2867  .        date (g
-0000fff0: 6f6f 676c 652e 7479 7065 2e64 6174 655f  oogle.type.date_
-00010000: 7062 322e 4461 7465 293a 0a20 2020 2020  pb2.Date):.     
-00010010: 2020 2020 2020 2044 6174 6520 6f66 2074         Date of t
-00010020: 6869 7320 726f 772e 0a0a 2020 2020 2020  his row...      
-00010030: 2020 2020 2020 4120 636f 6e64 6974 696f        A conditio
-00010040: 6e20 6f6e 2060 6064 6174 6560 6020 6973  n on ``date`` is
-00010050: 2072 6571 7569 7265 6420 696e 2074 6865   required in the
-00010060: 2060 6057 4845 5245 6060 2063 6c61 7573   ``WHERE`` claus
-00010070: 652e 0a20 2020 2020 2020 2064 6f6d 6169  e..        domai
-00010080: 6e20 2873 7472 293a 0a20 2020 2020 2020  n (str):.       
-00010090: 2020 2020 2044 6f6d 6169 6e20 6f66 2079       Domain of y
-000100a0: 6f75 7220 636f 6d70 6574 6974 6f72 206f  our competitor o
-000100b0: 7220 796f 7572 2064 6f6d 6169 6e2c 2069  r your domain, i
-000100c0: 660a 2020 2020 2020 2020 2020 2020 2769  f.            'i
-000100d0: 735f 796f 7572 5f64 6f6d 6169 6e27 2069  s_your_domain' i
-000100e0: 7320 7472 7565 2e0a 0a20 2020 2020 2020  s true...       
-000100f0: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
-00010100: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
-00010110: 636c 6175 7365 2e20 4361 6e6e 6f74 2062  clause. Cannot b
-00010120: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
-00010130: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-00010140: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
-00010150: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00010160: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00010170: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00010180: 2060 605f 646f 6d61 696e 6060 2e0a 2020   ``_domain``..  
-00010190: 2020 2020 2020 6973 5f79 6f75 725f 646f        is_your_do
-000101a0: 6d61 696e 2028 626f 6f6c 293a 0a20 2020  main (bool):.   
-000101b0: 2020 2020 2020 2020 2054 7275 6520 6966           True if
-000101c0: 2074 6869 7320 726f 7720 636f 6e74 6169   this row contai
-000101d0: 6e73 2064 6174 6120 666f 7220 796f 7572  ns data for your
-000101e0: 0a20 2020 2020 2020 2020 2020 2064 6f6d  .            dom
-000101f0: 6169 6e2e 0a20 2020 2020 2020 2020 2020  ain..           
-00010200: 2043 616e 6e6f 7420 6265 2066 696c 7465   Cannot be filte
-00010210: 7265 6420 6f6e 2069 6e20 7468 6520 2757  red on in the 'W
-00010220: 4845 5245 2720 636c 6175 7365 2e0a 0a20  HERE' clause... 
-00010230: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00010240: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00010250: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00010260: 5f69 735f 796f 7572 5f64 6f6d 6169 6e60  _is_your_domain`
-00010270: 602e 0a20 2020 2020 2020 2072 6570 6f72  `..        repor
-00010280: 745f 636f 756e 7472 795f 636f 6465 2028  t_country_code (
-00010290: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000102a0: 2020 436f 756e 7472 7920 7768 6572 6520    Country where 
-000102b0: 696d 7072 6573 7369 6f6e 7320 6170 7065  impressions appe
-000102c0: 6172 6564 2e0a 0a20 2020 2020 2020 2020  ared...         
-000102d0: 2020 2052 6571 7569 7265 6420 696e 2074     Required in t
-000102e0: 6865 2060 6053 454c 4543 5460 6020 636c  he ``SELECT`` cl
-000102f0: 6175 7365 2e20 4120 636f 6e64 6974 696f  ause. A conditio
-00010300: 6e20 6f6e 0a20 2020 2020 2020 2020 2020  n on.           
-00010310: 2060 6072 6570 6f72 745f 636f 756e 7472   ``report_countr
-00010320: 795f 636f 6465 6060 2069 7320 7265 7175  y_code`` is requ
-00010330: 6972 6564 2069 6e20 7468 6520 6060 5748  ired in the ``WH
-00010340: 4552 4560 6020 636c 6175 7365 2e0a 0a20  ERE`` clause... 
-00010350: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00010360: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00010370: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00010380: 5f72 6570 6f72 745f 636f 756e 7472 795f  _report_country_
-00010390: 636f 6465 6060 2e0a 2020 2020 2020 2020  code``..        
-000103a0: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
-000103b0: 6964 2028 696e 7429 3a0a 2020 2020 2020  id (int):.      
-000103c0: 2020 2020 2020 476f 6f67 6c65 2070 726f        Google pro
-000103d0: 6475 6374 2063 6174 6567 6f72 7920 4944  duct category ID
-000103e0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-000103f0: 6520 7265 706f 7274 2066 6f72 2c0a 2020  e report for,.  
-00010400: 2020 2020 2020 2020 2020 7265 7072 6573            repres
-00010410: 656e 7465 6420 696e 2060 476f 6f67 6c65  ented in `Google
-00010420: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-00010430: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00010440: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00010450: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00010460: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-00010470: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-00010480: 2020 2020 2020 2052 6571 7569 7265 6420         Required 
-00010490: 696e 2074 6865 2060 6053 454c 4543 5460  in the ``SELECT`
-000104a0: 6020 636c 6175 7365 2e20 4120 636f 6e64  ` clause. A cond
-000104b0: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
-000104c0: 2020 2020 2060 6072 6570 6f72 745f 6361       ``report_ca
-000104d0: 7465 676f 7279 5f69 6460 6020 6973 2072  tegory_id`` is r
-000104e0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-000104f0: 6057 4845 5245 6060 2063 6c61 7573 652e  `WHERE`` clause.
-00010500: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00010510: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00010520: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00010530: 2060 605f 7265 706f 7274 5f63 6174 6567   ``_report_categ
-00010540: 6f72 795f 6964 6060 2e0a 2020 2020 2020  ory_id``..      
-00010550: 2020 7472 6166 6669 635f 736f 7572 6365    traffic_source
-00010560: 2028 676f 6f67 6c65 2e73 686f 7070 696e   (google.shoppin
-00010570: 672e 6d65 7263 6861 6e74 5f72 6570 6f72  g.merchant_repor
-00010580: 7473 5f76 3162 6574 612e 7479 7065 732e  ts_v1beta.types.
-00010590: 5472 6166 6669 6353 6f75 7263 652e 5472  TrafficSource.Tr
-000105a0: 6166 6669 6353 6f75 7263 6545 6e75 6d29  afficSourceEnum)
-000105b0: 3a0a 2020 2020 2020 2020 2020 2020 5472  :.            Tr
-000105c0: 6166 6669 6320 736f 7572 6365 206f 6620  affic source of 
-000105d0: 696d 7072 6573 7369 6f6e 732e 0a0a 2020  impressions...  
-000105e0: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-000105f0: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
-00010600: 4354 6060 2063 6c61 7573 652e 0a0a 2020  CT`` clause...  
-00010610: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00010620: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00010630: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00010640: 7472 6166 6669 635f 736f 7572 6365 6060  traffic_source``
-00010650: 2e0a 2020 2020 2020 2020 7261 6e6b 2028  ..        rank (
-00010660: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00010670: 2020 506f 7369 7469 6f6e 206f 6620 7468    Position of th
-00010680: 6520 646f 6d61 696e 2069 6e20 7468 6520  e domain in the 
-00010690: 7369 6d69 6c61 7220 6275 7369 6e65 7373  similar business
-000106a0: 6573 2072 616e 6b69 6e67 2066 6f72 0a20  es ranking for. 
-000106b0: 2020 2020 2020 2020 2020 2074 6865 2073             the s
-000106c0: 656c 6563 7465 6420 6b65 7973 2028 6060  elected keys (``
-000106d0: 6461 7465 6060 2c20 6060 7265 706f 7274  date``, ``report
-000106e0: 5f63 6174 6567 6f72 795f 6964 6060 2c0a  _category_id``,.
-000106f0: 2020 2020 2020 2020 2020 2020 6060 7265              ``re
-00010700: 706f 7274 5f63 6f75 6e74 7279 5f63 6f64  port_country_cod
-00010710: 6560 602c 2060 6074 7261 6666 6963 5f73  e``, ``traffic_s
-00010720: 6f75 7263 6560 6029 2062 6173 6564 206f  ource``) based o
-00010730: 6e0a 2020 2020 2020 2020 2020 2020 696d  n.            im
-00010740: 7072 6573 7369 6f6e 732e 2031 2069 7320  pressions. 1 is 
-00010750: 7468 6520 6869 6768 6573 742e 0a0a 2020  the highest...  
-00010760: 2020 2020 2020 2020 2020 4361 6e6e 6f74            Cannot
-00010770: 2062 6520 6669 6c74 6572 6564 206f 6e20   be filtered on 
-00010780: 696e 2074 6865 2027 5748 4552 4527 2063  in the 'WHERE' c
-00010790: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
-000107a0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-000107b0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000107c0: 6e65 6f66 605f 2060 605f 7261 6e6b 6060  neof`_ ``_rank``
-000107d0: 2e0a 2020 2020 2020 2020 6164 735f 6f72  ..        ads_or
-000107e0: 6761 6e69 635f 7261 7469 6f20 2866 6c6f  ganic_ratio (flo
-000107f0: 6174 293a 0a20 2020 2020 2020 2020 2020  at):.           
-00010800: 205b 4164 7320 2f20 6f72 6761 6e69 6320   [Ads / organic 
-00010810: 7261 7469 6f5d 0a20 2020 2020 2020 2020  ratio].         
-00010820: 2020 2028 6874 7470 733a 2f2f 7375 7070     (https://supp
-00010830: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f6d  ort.google.com/m
-00010840: 6572 6368 616e 7473 2f61 6e73 7765 722f  erchants/answer/
-00010850: 3131 3336 3634 3432 237a 6970 7079 3d25  11366442#zippy=%
-00010860: 3243 6164 732d 6672 6565 2d72 6174 696f  2Cads-free-ratio
-00010870: 290a 2020 2020 2020 2020 2020 2020 7368  ).            sh
-00010880: 6f77 7320 686f 7720 6f66 7465 6e20 7468  ows how often th
-00010890: 6520 646f 6d61 696e 2072 6563 6569 7665  e domain receive
-000108a0: 7320 696d 7072 6573 7369 6f6e 7320 6672  s impressions fr
-000108b0: 6f6d 0a20 2020 2020 2020 2020 2020 2053  om.            S
-000108c0: 686f 7070 696e 6720 6164 7320 636f 6d70  hopping ads comp
-000108d0: 6172 6564 2074 6f20 6f72 6761 6e69 6320  ared to organic 
-000108e0: 7472 6166 6669 632e 2054 6865 206e 756d  traffic. The num
-000108f0: 6265 7220 6973 0a20 2020 2020 2020 2020  ber is.         
-00010900: 2020 2072 6f75 6e64 6564 2061 6e64 2062     rounded and b
-00010910: 7563 6b65 7465 642e 0a0a 2020 2020 2020  ucketed...      
-00010920: 2020 2020 2020 4361 6e6e 6f74 2062 6520        Cannot be 
-00010930: 6669 6c74 6572 6564 206f 6e20 696e 2074  filtered on in t
-00010940: 6865 2027 5748 4552 4527 2063 6c61 7573  he 'WHERE' claus
-00010950: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00010960: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00010970: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00010980: 605f 2060 605f 6164 735f 6f72 6761 6e69  `_ ``_ads_organi
-00010990: 635f 7261 7469 6f60 602e 0a20 2020 2020  c_ratio``..     
-000109a0: 2020 2070 6167 655f 6f76 6572 6c61 705f     page_overlap_
-000109b0: 7261 7465 2028 666c 6f61 7429 3a0a 2020  rate (float):.  
-000109c0: 2020 2020 2020 2020 2020 5b50 6167 6520            [Page 
-000109d0: 6f76 6572 6c61 7020 7261 7465 5d0a 2020  overlap rate].  
-000109e0: 2020 2020 2020 2020 2020 2868 7474 7073            (https
-000109f0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00010a00: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00010a10: 616e 7377 6572 2f31 3133 3636 3434 3223  answer/11366442#
-00010a20: 7a69 7070 793d 2532 4370 6167 652d 6f76  zippy=%2Cpage-ov
-00010a30: 6572 6c61 702d 7261 7465 290a 2020 2020  erlap-rate).    
-00010a40: 2020 2020 2020 2020 7368 6f77 7320 686f          shows ho
-00010a50: 7720 6672 6571 7565 6e74 6c79 2063 6f6d  w frequently com
-00010a60: 7065 7469 6e67 2072 6574 6169 6c65 7273  peting retailers
-00010a70: e280 9920 6f66 6665 7273 2061 7265 2073  ... offers are s
-00010a80: 686f 776e 0a20 2020 2020 2020 2020 2020  hown.           
-00010a90: 2074 6f67 6574 6865 7220 7769 7468 2079   together with y
-00010aa0: 6f75 7220 6f66 6665 7273 206f 6e20 7468  our offers on th
-00010ab0: 6520 7361 6d65 2070 6167 652e 0a0a 2020  e same page...  
-00010ac0: 2020 2020 2020 2020 2020 4361 6e6e 6f74            Cannot
-00010ad0: 2062 6520 6669 6c74 6572 6564 206f 6e20   be filtered on 
-00010ae0: 696e 2074 6865 2027 5748 4552 4527 2063  in the 'WHERE' c
-00010af0: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
-00010b00: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00010b10: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00010b20: 6e65 6f66 605f 2060 605f 7061 6765 5f6f  neof`_ ``_page_o
-00010b30: 7665 726c 6170 5f72 6174 6560 602e 0a20  verlap_rate``.. 
-00010b40: 2020 2020 2020 2068 6967 6865 725f 706f         higher_po
-00010b50: 7369 7469 6f6e 5f72 6174 6520 2866 6c6f  sition_rate (flo
-00010b60: 6174 293a 0a20 2020 2020 2020 2020 2020  at):.           
-00010b70: 205b 4869 6768 6572 2070 6f73 6974 696f   [Higher positio
-00010b80: 6e20 7261 7465 5d0a 2020 2020 2020 2020  n rate].        
-00010b90: 2020 2020 2868 7474 7073 3a2f 2f73 7570      (https://sup
-00010ba0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-00010bb0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-00010bc0: 2f31 3133 3636 3434 3223 7a69 7070 793d  /11366442#zippy=
-00010bd0: 2532 4368 6967 6865 722d 706f 7369 7469  %2Chigher-positi
-00010be0: 6f6e 2d72 6174 6529 0a20 2020 2020 2020  on-rate).       
-00010bf0: 2020 2020 2073 686f 7773 2068 6f77 206f       shows how o
-00010c00: 6674 656e 2061 2063 6f6d 7065 7469 746f  ften a competito
-00010c10: 72e2 8099 7320 6f66 6665 7220 676f 7420  r...s offer got 
-00010c20: 706c 6163 6564 2069 6e20 6120 6869 6768  placed in a high
-00010c30: 6572 0a20 2020 2020 2020 2020 2020 2070  er.            p
-00010c40: 6f73 6974 696f 6e20 6f6e 2074 6865 2070  osition on the p
-00010c50: 6167 6520 7468 616e 2079 6f75 7220 6f66  age than your of
-00010c60: 6665 722e 0a0a 2020 2020 2020 2020 2020  fer...          
-00010c70: 2020 4361 6e6e 6f74 2062 6520 6669 6c74    Cannot be filt
-00010c80: 6572 6564 206f 6e20 696e 2074 6865 2027  ered on in the '
-00010c90: 5748 4552 4527 2063 6c61 7573 652e 0a0a  WHERE' clause...
-00010ca0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00010cb0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00010cc0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00010cd0: 605f 6869 6768 6572 5f70 6f73 6974 696f  `_higher_positio
-00010ce0: 6e5f 7261 7465 6060 2e0a 2020 2020 2020  n_rate``..      
-00010cf0: 2020 7265 6c61 7469 7665 5f76 6973 6962    relative_visib
-00010d00: 696c 6974 7920 2866 6c6f 6174 293a 0a20  ility (float):. 
-00010d10: 2020 2020 2020 2020 2020 205b 5265 6c61             [Rela
-00010d20: 7469 7665 2076 6973 6962 696c 6974 795d  tive visibility]
-00010d30: 0a20 2020 2020 2020 2020 2020 2028 6874  .            (ht
-00010d40: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
-00010d50: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
-00010d60: 7473 2f61 6e73 7765 722f 3131 3336 3634  ts/answer/113664
-00010d70: 3432 237a 6970 7079 3d25 3243 7265 6c61  42#zippy=%2Crela
-00010d80: 7469 7665 2d76 6973 6962 696c 6974 7929  tive-visibility)
-00010d90: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-00010da0: 7773 2068 6f77 206f 6674 656e 2079 6f75  ws how often you
-00010db0: 7220 636f 6d70 6574 6974 6f72 73e2 8099  r competitors...
-00010dc0: 206f 6666 6572 7320 6172 6520 7368 6f77   offers are show
-00010dd0: 6e20 636f 6d70 6172 6564 0a20 2020 2020  n compared.     
-00010de0: 2020 2020 2020 2074 6f20 796f 7572 206f         to your o
-00010df0: 6666 6572 732e 2049 6e20 6f74 6865 7220  ffers. In other 
-00010e00: 776f 7264 732c 2074 6869 7320 6973 2074  words, this is t
-00010e10: 6865 206e 756d 6265 7220 6f66 0a20 2020  he number of.   
-00010e20: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00010e30: 6564 2069 6d70 7265 7373 696f 6e73 206f  ed impressions o
-00010e40: 6620 6120 636f 6d70 6574 6974 6f72 2072  f a competitor r
-00010e50: 6574 6169 6c65 7220 6469 7669 6465 6420  etailer divided 
-00010e60: 6279 0a20 2020 2020 2020 2020 2020 2074  by.            t
-00010e70: 6865 206e 756d 6265 7220 6f66 2079 6f75  he number of you
-00010e80: 7220 6469 7370 6c61 7965 6420 696d 7072  r displayed impr
-00010e90: 6573 7369 6f6e 7320 6475 7269 6e67 2061  essions during a
-00010ea0: 2073 656c 6563 7465 640a 2020 2020 2020   selected.      
-00010eb0: 2020 2020 2020 7469 6d65 2072 616e 6765        time range
-00010ec0: 2066 6f72 2061 2073 656c 6563 7465 6420   for a selected 
-00010ed0: 7072 6f64 7563 7420 6361 7465 676f 7279  product category
-00010ee0: 2061 6e64 2063 6f75 6e74 7279 2e0a 0a20   and country... 
-00010ef0: 2020 2020 2020 2020 2020 2043 616e 6e6f             Canno
-00010f00: 7420 6265 2066 696c 7465 7265 6420 6f6e  t be filtered on
-00010f10: 2069 6e20 7468 6520 2757 4845 5245 2720   in the 'WHERE' 
-00010f20: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-00010f30: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00010f40: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00010f50: 6f6e 656f 6660 5f20 6060 5f72 656c 6174  oneof`_ ``_relat
-00010f60: 6976 655f 7669 7369 6269 6c69 7479 6060  ive_visibility``
-00010f70: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00010f80: 6174 653a 2064 6174 655f 7062 322e 4461  ate: date_pb2.Da
-00010f90: 7465 203d 2070 726f 746f 2e46 6965 6c64  te = proto.Field
-00010fa0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00010fb0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-00010fc0: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
-00010fd0: 2020 206d 6573 7361 6765 3d64 6174 655f     message=date_
-00010fe0: 7062 322e 4461 7465 2c0a 2020 2020 290a  pb2.Date,.    ).
-00010ff0: 2020 2020 646f 6d61 696e 3a20 7374 7220      domain: str 
-00011000: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00011010: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00011020: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00011030: 6265 723d 322c 0a20 2020 2020 2020 206f  ber=2,.        o
-00011040: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00011050: 2020 290a 2020 2020 6973 5f79 6f75 725f    ).    is_your_
-00011060: 646f 6d61 696e 3a20 626f 6f6c 203d 2070  domain: bool = p
-00011070: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00011080: 2020 2020 7072 6f74 6f2e 424f 4f4c 2c0a      proto.BOOL,.
-00011090: 2020 2020 2020 2020 6e75 6d62 6572 3d33          number=3
-000110a0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-000110b0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-000110c0: 2020 2072 6570 6f72 745f 636f 756e 7472     report_countr
-000110d0: 795f 636f 6465 3a20 7374 7220 3d20 7072  y_code: str = pr
-000110e0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-000110f0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00011100: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00011110: 342c 0a20 2020 2020 2020 206f 7074 696f  4,.        optio
-00011120: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
-00011130: 2020 2020 7265 706f 7274 5f63 6174 6567      report_categ
-00011140: 6f72 795f 6964 3a20 696e 7420 3d20 7072  ory_id: int = pr
-00011150: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00011160: 2020 2070 726f 746f 2e49 4e54 3634 2c0a     proto.INT64,.
-00011170: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
-00011180: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00011190: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-000111a0: 2020 2074 7261 6666 6963 5f73 6f75 7263     traffic_sourc
-000111b0: 653a 2022 5472 6166 6669 6353 6f75 7263  e: "TrafficSourc
-000111c0: 652e 5472 6166 6669 6353 6f75 7263 6545  e.TrafficSourceE
-000111d0: 6e75 6d22 203d 2070 726f 746f 2e46 6965  num" = proto.Fie
-000111e0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-000111f0: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
-00011200: 6e75 6d62 6572 3d36 2c0a 2020 2020 2020  number=6,.      
-00011210: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00011220: 0a20 2020 2020 2020 2065 6e75 6d3d 2254  .        enum="T
-00011230: 7261 6666 6963 536f 7572 6365 2e54 7261  rafficSource.Tra
-00011240: 6666 6963 536f 7572 6365 456e 756d 222c  fficSourceEnum",
-00011250: 0a20 2020 2029 0a20 2020 2072 616e 6b3a  .    ).    rank:
-00011260: 2069 6e74 203d 2070 726f 746f 2e46 6965   int = proto.Fie
-00011270: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00011280: 6f2e 494e 5436 342c 0a20 2020 2020 2020  o.INT64,.       
-00011290: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
-000112a0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-000112b0: 2c0a 2020 2020 290a 2020 2020 6164 735f  ,.    ).    ads_
-000112c0: 6f72 6761 6e69 635f 7261 7469 6f3a 2066  organic_ratio: f
-000112d0: 6c6f 6174 203d 2070 726f 746f 2e46 6965  loat = proto.Fie
-000112e0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-000112f0: 6f2e 444f 5542 4c45 2c0a 2020 2020 2020  o.DOUBLE,.      
-00011300: 2020 6e75 6d62 6572 3d38 2c0a 2020 2020    number=8,.    
-00011310: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00011320: 652c 0a20 2020 2029 0a20 2020 2070 6167  e,.    ).    pag
-00011330: 655f 6f76 6572 6c61 705f 7261 7465 3a20  e_overlap_rate: 
-00011340: 666c 6f61 7420 3d20 7072 6f74 6f2e 4669  float = proto.Fi
-00011350: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00011360: 746f 2e44 4f55 424c 452c 0a20 2020 2020  to.DOUBLE,.     
-00011370: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
-00011380: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00011390: 7565 2c0a 2020 2020 290a 2020 2020 6869  ue,.    ).    hi
-000113a0: 6768 6572 5f70 6f73 6974 696f 6e5f 7261  gher_position_ra
-000113b0: 7465 3a20 666c 6f61 7420 3d20 7072 6f74  te: float = prot
-000113c0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000113d0: 2070 726f 746f 2e44 4f55 424c 452c 0a20   proto.DOUBLE,. 
-000113e0: 2020 2020 2020 206e 756d 6265 723d 3130         number=10
-000113f0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00011400: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00011410: 2020 2072 656c 6174 6976 655f 7669 7369     relative_visi
-00011420: 6269 6c69 7479 3a20 666c 6f61 7420 3d20  bility: float = 
-00011430: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00011440: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
-00011450: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00011460: 723d 3131 2c0a 2020 2020 2020 2020 6f70  r=11,.        op
-00011470: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00011480: 2029 0a0a 0a63 6c61 7373 2043 6f6d 7065   )...class Compe
-00011490: 7469 7469 7665 5669 7369 6269 6c69 7479  titiveVisibility
-000114a0: 546f 704d 6572 6368 616e 7456 6965 7728  TopMerchantView(
-000114b0: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
-000114c0: 2020 2020 7222 2222 4669 656c 6473 2061      r"""Fields a
-000114d0: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
-000114e0: 7279 2069 6e0a 2020 2020 6060 636f 6d70  ry in.    ``comp
-000114f0: 6574 6974 6976 655f 7669 7369 6269 6c69  etitive_visibili
-00011500: 7479 5f74 6f70 5f6d 6572 6368 616e 745f  ty_top_merchant_
-00011510: 7669 6577 6060 2074 6162 6c65 2e0a 0a20  view`` table... 
-00011520: 2020 2060 436f 6d70 6574 6974 6976 650a     `Competitive.
-00011530: 2020 2020 7669 7369 6269 6c69 7479 203c      visibility <
-00011540: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
-00011550: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
-00011560: 616e 7473 2f61 6e73 7765 722f 3131 3336  ants/answer/1136
-00011570: 3634 3432 3e60 5f5f 0a20 2020 2072 6570  6442>`__.    rep
-00011580: 6f72 7420 7769 7468 2062 7573 696e 6573  ort with busines
-00011590: 7320 7769 7468 2068 6967 6865 7374 2076  s with highest v
-000115a0: 6973 6962 696c 6974 792e 0a0a 2020 2020  isibility...    
-000115b0: 5661 6c75 6573 2061 7265 206f 6e6c 7920  Values are only 
-000115c0: 7365 7420 666f 7220 6669 656c 6473 2072  set for fields r
-000115d0: 6571 7565 7374 6564 2065 7870 6c69 6369  equested explici
-000115e0: 746c 7920 696e 2074 6865 2072 6571 7565  tly in the reque
-000115f0: 7374 2773 0a20 2020 2073 6561 7263 6820  st's.    search 
-00011600: 7175 6572 792e 0a0a 0a20 2020 202e 2e20  query....    .. 
-00011610: 5f6f 6e65 6f66 3a20 6874 7470 733a 2f2f  _oneof: https://
-00011620: 7072 6f74 6f2d 706c 7573 2d70 7974 686f  proto-plus-pytho
-00011630: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-00011640: 2f65 6e2f 7374 6162 6c65 2f66 6965 6c64  /en/stable/field
-00011650: 732e 6874 6d6c 236f 6e65 6f66 732d 6d75  s.html#oneofs-mu
-00011660: 7475 616c 6c79 2d65 7863 6c75 7369 7665  tually-exclusive
-00011670: 2d66 6965 6c64 730a 0a20 2020 2041 7474  -fields..    Att
-00011680: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
-00011690: 2064 6174 6520 2867 6f6f 676c 652e 7479   date (google.ty
-000116a0: 7065 2e64 6174 655f 7062 322e 4461 7465  pe.date_pb2.Date
-000116b0: 293a 0a20 2020 2020 2020 2020 2020 2044  ):.            D
-000116c0: 6174 6520 6f66 2074 6869 7320 726f 772e  ate of this row.
-000116d0: 0a0a 2020 2020 2020 2020 2020 2020 4361  ..            Ca
-000116e0: 6e6e 6f74 2062 6520 7365 6c65 6374 6564  nnot be selected
-000116f0: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
-00011700: 6060 2063 6c61 7573 652e 2041 2063 6f6e  `` clause. A con
-00011710: 6469 7469 6f6e 206f 6e0a 2020 2020 2020  dition on.      
-00011720: 2020 2020 2020 6060 6461 7465 6060 2069        ``date`` i
-00011730: 7320 7265 7175 6972 6564 2069 6e20 7468  s required in th
-00011740: 6520 6060 5748 4552 4560 6020 636c 6175  e ``WHERE`` clau
-00011750: 7365 2e0a 2020 2020 2020 2020 646f 6d61  se..        doma
-00011760: 696e 2028 7374 7229 3a0a 2020 2020 2020  in (str):.      
-00011770: 2020 2020 2020 446f 6d61 696e 206f 6620        Domain of 
-00011780: 796f 7572 2063 6f6d 7065 7469 746f 7220  your competitor 
-00011790: 6f72 2079 6f75 7220 646f 6d61 696e 2c20  or your domain, 
-000117a0: 6966 0a20 2020 2020 2020 2020 2020 2027  if.            '
-000117b0: 6973 5f79 6f75 725f 646f 6d61 696e 2720  is_your_domain' 
-000117c0: 6973 2074 7275 652e 0a0a 2020 2020 2020  is true...      
-000117d0: 2020 2020 2020 5265 7175 6972 6564 2069        Required i
-000117e0: 6e20 7468 6520 6060 5345 4c45 4354 6060  n the ``SELECT``
-000117f0: 2063 6c61 7573 652e 2043 616e 6e6f 7420   clause. Cannot 
-00011800: 6265 2066 696c 7465 7265 6420 6f6e 2069  be filtered on i
-00011810: 6e0a 2020 2020 2020 2020 2020 2020 7468  n.            th
-00011820: 6520 2757 4845 5245 2720 636c 6175 7365  e 'WHERE' clause
-00011830: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00011840: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00011850: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00011860: 5f20 6060 5f64 6f6d 6169 6e60 602e 0a20  _ ``_domain``.. 
-00011870: 2020 2020 2020 2069 735f 796f 7572 5f64         is_your_d
-00011880: 6f6d 6169 6e20 2862 6f6f 6c29 3a0a 2020  omain (bool):.  
-00011890: 2020 2020 2020 2020 2020 5472 7565 2069            True i
-000118a0: 6620 7468 6973 2072 6f77 2063 6f6e 7461  f this row conta
-000118b0: 696e 7320 6461 7461 2066 6f72 2079 6f75  ins data for you
-000118c0: 720a 2020 2020 2020 2020 2020 2020 646f  r.            do
-000118d0: 6d61 696e 2e0a 2020 2020 2020 2020 2020  main..          
-000118e0: 2020 4361 6e6e 6f74 2062 6520 6669 6c74    Cannot be filt
-000118f0: 6572 6564 206f 6e20 696e 2074 6865 2027  ered on in the '
-00011900: 5748 4552 4527 2063 6c61 7573 652e 0a0a  WHERE' clause...
-00011910: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00011920: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00011930: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00011940: 605f 6973 5f79 6f75 725f 646f 6d61 696e  `_is_your_domain
-00011950: 6060 2e0a 2020 2020 2020 2020 7265 706f  ``..        repo
-00011960: 7274 5f63 6f75 6e74 7279 5f63 6f64 6520  rt_country_code 
-00011970: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00011980: 2020 2043 6f75 6e74 7279 2077 6865 7265     Country where
-00011990: 2069 6d70 7265 7373 696f 6e73 2061 7070   impressions app
-000119a0: 6561 7265 642e 0a0a 2020 2020 2020 2020  eared...        
-000119b0: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
-000119c0: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
-000119d0: 6c61 7573 652e 2041 2063 6f6e 6469 7469  lause. A conditi
-000119e0: 6f6e 206f 6e0a 2020 2020 2020 2020 2020  on on.          
-000119f0: 2020 6060 7265 706f 7274 5f63 6f75 6e74    ``report_count
-00011a00: 7279 5f63 6f64 6560 6020 6973 2072 6571  ry_code`` is req
-00011a10: 7569 7265 6420 696e 2074 6865 2060 6057  uired in the ``W
-00011a20: 4845 5245 6060 2063 6c61 7573 652e 0a0a  HERE`` clause...
-00011a30: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00011a40: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00011a50: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00011a60: 605f 7265 706f 7274 5f63 6f75 6e74 7279  `_report_country
-00011a70: 5f63 6f64 6560 602e 0a20 2020 2020 2020  _code``..       
-00011a80: 2072 6570 6f72 745f 6361 7465 676f 7279   report_category
-00011a90: 5f69 6420 2869 6e74 293a 0a20 2020 2020  _id (int):.     
-00011aa0: 2020 2020 2020 2047 6f6f 676c 6520 7072         Google pr
-00011ab0: 6f64 7563 7420 6361 7465 676f 7279 2049  oduct category I
-00011ac0: 4420 746f 2063 616c 6375 6c61 7465 2074  D to calculate t
-00011ad0: 6865 2072 6570 6f72 7420 666f 722c 0a20  he report for,. 
-00011ae0: 2020 2020 2020 2020 2020 2072 6570 7265             repre
-00011af0: 7365 6e74 6564 2069 6e20 6047 6f6f 676c  sented in `Googl
-00011b00: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
-00011b10: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
-00011b20: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
-00011b30: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
-00011b40: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
-00011b50: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
-00011b60: 2020 2020 2020 2020 5265 7175 6972 6564          Required
-00011b70: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
-00011b80: 6060 2063 6c61 7573 652e 2041 2063 6f6e  `` clause. A con
-00011b90: 6469 7469 6f6e 206f 6e0a 2020 2020 2020  dition on.      
-00011ba0: 2020 2020 2020 6060 7265 706f 7274 5f63        ``report_c
-00011bb0: 6174 6567 6f72 795f 6964 6060 2069 7320  ategory_id`` is 
-00011bc0: 7265 7175 6972 6564 2069 6e20 7468 6520  required in the 
-00011bd0: 6060 5748 4552 4560 6020 636c 6175 7365  ``WHERE`` clause
-00011be0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00011bf0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00011c00: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00011c10: 5f20 6060 5f72 6570 6f72 745f 6361 7465  _ ``_report_cate
-00011c20: 676f 7279 5f69 6460 602e 0a20 2020 2020  gory_id``..     
-00011c30: 2020 2074 7261 6666 6963 5f73 6f75 7263     traffic_sourc
-00011c40: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
-00011c50: 6e67 2e6d 6572 6368 616e 745f 7265 706f  ng.merchant_repo
-00011c60: 7274 735f 7631 6265 7461 2e74 7970 6573  rts_v1beta.types
-00011c70: 2e54 7261 6666 6963 536f 7572 6365 2e54  .TrafficSource.T
-00011c80: 7261 6666 6963 536f 7572 6365 456e 756d  rafficSourceEnum
-00011c90: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-00011ca0: 7261 6666 6963 2073 6f75 7263 6520 6f66  raffic source of
-00011cb0: 2069 6d70 7265 7373 696f 6e73 2e0a 0a20   impressions... 
-00011cc0: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
-00011cd0: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
-00011ce0: 4543 5460 6020 636c 6175 7365 2e0a 0a20  ECT`` clause... 
-00011cf0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00011d00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00011d10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00011d20: 5f74 7261 6666 6963 5f73 6f75 7263 6560  _traffic_source`
-00011d30: 602e 0a20 2020 2020 2020 2072 616e 6b20  `..        rank 
-00011d40: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
-00011d50: 2020 2050 6f73 6974 696f 6e20 6f66 2074     Position of t
-00011d60: 6865 2064 6f6d 6169 6e20 696e 2074 6865  he domain in the
-00011d70: 2074 6f70 206d 6572 6368 616e 7473 2072   top merchants r
-00011d80: 616e 6b69 6e67 2066 6f72 2074 6865 0a20  anking for the. 
-00011d90: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00011da0: 7465 6420 6b65 7973 2028 6060 6461 7465  ted keys (``date
-00011db0: 6060 2c20 6060 7265 706f 7274 5f63 6174  ``, ``report_cat
-00011dc0: 6567 6f72 795f 6964 6060 2c0a 2020 2020  egory_id``,.    
-00011dd0: 2020 2020 2020 2020 6060 7265 706f 7274          ``report
-00011de0: 5f63 6f75 6e74 7279 5f63 6f64 6560 602c  _country_code``,
-00011df0: 2060 6074 7261 6666 6963 5f73 6f75 7263   ``traffic_sourc
-00011e00: 6560 6029 2062 6173 6564 206f 6e0a 2020  e``) based on.  
-00011e10: 2020 2020 2020 2020 2020 696d 7072 6573            impres
-00011e20: 7369 6f6e 732e 2031 2069 7320 7468 6520  sions. 1 is the 
-00011e30: 6869 6768 6573 742e 0a0a 2020 2020 2020  highest...      
-00011e40: 2020 2020 2020 4361 6e6e 6f74 2062 6520        Cannot be 
-00011e50: 6669 6c74 6572 6564 206f 6e20 696e 2074  filtered on in t
-00011e60: 6865 2027 5748 4552 4527 2063 6c61 7573  he 'WHERE' claus
-00011e70: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00011e80: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00011e90: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00011ea0: 605f 2060 605f 7261 6e6b 6060 2e0a 2020  `_ ``_rank``..  
-00011eb0: 2020 2020 2020 6164 735f 6f72 6761 6e69        ads_organi
-00011ec0: 635f 7261 7469 6f20 2866 6c6f 6174 293a  c_ratio (float):
-00011ed0: 0a20 2020 2020 2020 2020 2020 205b 4164  .            [Ad
-00011ee0: 7320 2f20 6f72 6761 6e69 6320 7261 7469  s / organic rati
-00011ef0: 6f5d 0a20 2020 2020 2020 2020 2020 2028  o].            (
-00011f00: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
-00011f10: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
-00011f20: 616e 7473 2f61 6e73 7765 722f 3131 3336  ants/answer/1136
-00011f30: 3634 3432 237a 6970 7079 3d25 3243 6164  6442#zippy=%2Cad
-00011f40: 732d 6672 6565 2d72 6174 696f 290a 2020  s-free-ratio).  
-00011f50: 2020 2020 2020 2020 2020 7368 6f77 7320            shows 
-00011f60: 686f 7720 6f66 7465 6e20 7468 6520 646f  how often the do
-00011f70: 6d61 696e 2072 6563 6569 7665 7320 696d  main receives im
-00011f80: 7072 6573 7369 6f6e 7320 6672 6f6d 0a20  pressions from. 
-00011f90: 2020 2020 2020 2020 2020 2053 686f 7070             Shopp
-00011fa0: 696e 6720 6164 7320 636f 6d70 6172 6564  ing ads compared
-00011fb0: 2074 6f20 6f72 6761 6e69 6320 7472 6166   to organic traf
-00011fc0: 6669 632e 2054 6865 206e 756d 6265 7220  fic. The number 
-00011fd0: 6973 0a20 2020 2020 2020 2020 2020 2072  is.            r
-00011fe0: 6f75 6e64 6564 2061 6e64 2062 7563 6b65  ounded and bucke
-00011ff0: 7465 642e 0a0a 2020 2020 2020 2020 2020  ted...          
-00012000: 2020 4361 6e6e 6f74 2062 6520 6669 6c74    Cannot be filt
-00012010: 6572 6564 206f 6e20 696e 2074 6865 2027  ered on in the '
-00012020: 5748 4552 4527 2063 6c61 7573 652e 0a0a  WHERE' clause...
-00012030: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00012040: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00012050: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00012060: 605f 6164 735f 6f72 6761 6e69 635f 7261  `_ads_organic_ra
-00012070: 7469 6f60 602e 0a20 2020 2020 2020 2070  tio``..        p
-00012080: 6167 655f 6f76 6572 6c61 705f 7261 7465  age_overlap_rate
-00012090: 2028 666c 6f61 7429 3a0a 2020 2020 2020   (float):.      
-000120a0: 2020 2020 2020 5b50 6167 6520 6f76 6572        [Page over
-000120b0: 6c61 7020 7261 7465 5d0a 2020 2020 2020  lap rate].      
-000120c0: 2020 2020 2020 2868 7474 7073 3a2f 2f73        (https://s
-000120d0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-000120e0: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-000120f0: 6572 2f31 3133 3636 3434 3223 7a69 7070  er/11366442#zipp
-00012100: 793d 2532 4370 6167 652d 6f76 6572 6c61  y=%2Cpage-overla
-00012110: 702d 7261 7465 290a 2020 2020 2020 2020  p-rate).        
-00012120: 2020 2020 7368 6f77 7320 686f 7720 6672      shows how fr
-00012130: 6571 7565 6e74 6c79 2063 6f6d 7065 7469  equently competi
-00012140: 6e67 2072 6574 6169 6c65 7273 e280 9920  ng retailers... 
-00012150: 6f66 6665 7273 2061 7265 2073 686f 776e  offers are shown
-00012160: 0a20 2020 2020 2020 2020 2020 2074 6f67  .            tog
-00012170: 6574 6865 7220 7769 7468 2079 6f75 7220  ether with your 
-00012180: 6f66 6665 7273 206f 6e20 7468 6520 7361  offers on the sa
-00012190: 6d65 2070 6167 652e 0a0a 2020 2020 2020  me page...      
-000121a0: 2020 2020 2020 4361 6e6e 6f74 2062 6520        Cannot be 
-000121b0: 6669 6c74 6572 6564 206f 6e20 696e 2074  filtered on in t
-000121c0: 6865 2027 5748 4552 4527 2063 6c61 7573  he 'WHERE' claus
-000121d0: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-000121e0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000121f0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00012200: 605f 2060 605f 7061 6765 5f6f 7665 726c  `_ ``_page_overl
-00012210: 6170 5f72 6174 6560 602e 0a20 2020 2020  ap_rate``..     
-00012220: 2020 2068 6967 6865 725f 706f 7369 7469     higher_positi
-00012230: 6f6e 5f72 6174 6520 2866 6c6f 6174 293a  on_rate (float):
-00012240: 0a20 2020 2020 2020 2020 2020 205b 4869  .            [Hi
-00012250: 6768 6572 2070 6f73 6974 696f 6e20 7261  gher position ra
-00012260: 7465 5d0a 2020 2020 2020 2020 2020 2020  te].            
-00012270: 2868 7474 7073 3a2f 2f73 7570 706f 7274  (https://support
-00012280: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00012290: 6861 6e74 732f 616e 7377 6572 2f31 3133  hants/answer/113
-000122a0: 3636 3434 3223 7a69 7070 793d 2532 4368  66442#zippy=%2Ch
-000122b0: 6967 6865 722d 706f 7369 7469 6f6e 2d72  igher-position-r
-000122c0: 6174 6529 0a20 2020 2020 2020 2020 2020  ate).           
-000122d0: 2073 686f 7773 2068 6f77 206f 6674 656e   shows how often
-000122e0: 2061 2063 6f6d 7065 7469 746f 72e2 8099   a competitor...
-000122f0: 7320 6f66 6665 7220 676f 7420 706c 6163  s offer got plac
-00012300: 6564 2069 6e20 6120 6869 6768 6572 0a20  ed in a higher. 
-00012310: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
-00012320: 696f 6e20 6f6e 2074 6865 2070 6167 6520  ion on the page 
-00012330: 7468 616e 2079 6f75 7220 6f66 6665 722e  than your offer.
-00012340: 0a0a 2020 2020 2020 2020 2020 2020 4361  ..            Ca
-00012350: 6e6e 6f74 2062 6520 6669 6c74 6572 6564  nnot be filtered
-00012360: 206f 6e20 696e 2074 6865 2027 5748 4552   on in the 'WHER
-00012370: 4527 2063 6c61 7573 652e 0a0a 2020 2020  E' clause...    
-00012380: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00012390: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-000123a0: 6620 606f 6e65 6f66 605f 2060 605f 6869  f `oneof`_ ``_hi
-000123b0: 6768 6572 5f70 6f73 6974 696f 6e5f 7261  gher_position_ra
-000123c0: 7465 6060 2e0a 2020 2020 2222 220a 0a20  te``..    """.. 
-000123d0: 2020 2064 6174 653a 2064 6174 655f 7062     date: date_pb
-000123e0: 322e 4461 7465 203d 2070 726f 746f 2e46  2.Date = proto.F
-000123f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00012400: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-00012410: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
-00012420: 2020 2020 2020 206d 6573 7361 6765 3d64         message=d
-00012430: 6174 655f 7062 322e 4461 7465 2c0a 2020  ate_pb2.Date,.  
-00012440: 2020 290a 2020 2020 646f 6d61 696e 3a20    ).    domain: 
-00012450: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-00012460: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00012470: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-00012480: 206e 756d 6265 723d 322c 0a20 2020 2020   number=2,.     
-00012490: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-000124a0: 2c0a 2020 2020 290a 2020 2020 6973 5f79  ,.    ).    is_y
-000124b0: 6f75 725f 646f 6d61 696e 3a20 626f 6f6c  our_domain: bool
-000124c0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-000124d0: 2020 2020 2020 2020 7072 6f74 6f2e 424f          proto.BO
-000124e0: 4f4c 2c0a 2020 2020 2020 2020 6e75 6d62  OL,.        numb
-000124f0: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
-00012500: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00012510: 2029 0a20 2020 2072 6570 6f72 745f 636f   ).    report_co
-00012520: 756e 7472 795f 636f 6465 3a20 7374 7220  untry_code: str 
-00012530: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00012540: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00012550: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00012560: 6265 723d 342c 0a20 2020 2020 2020 206f  ber=4,.        o
-00012570: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00012580: 2020 290a 2020 2020 7265 706f 7274 5f63    ).    report_c
-00012590: 6174 6567 6f72 795f 6964 3a20 696e 7420  ategory_id: int 
-000125a0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000125b0: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
-000125c0: 3634 2c0a 2020 2020 2020 2020 6e75 6d62  64,.        numb
-000125d0: 6572 3d35 2c0a 2020 2020 2020 2020 6f70  er=5,.        op
-000125e0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-000125f0: 2029 0a20 2020 2074 7261 6666 6963 5f73   ).    traffic_s
-00012600: 6f75 7263 653a 2022 5472 6166 6669 6353  ource: "TrafficS
-00012610: 6f75 7263 652e 5472 6166 6669 6353 6f75  ource.TrafficSou
-00012620: 7263 6545 6e75 6d22 203d 2070 726f 746f  rceEnum" = proto
-00012630: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00012640: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
-00012650: 2020 2020 6e75 6d62 6572 3d36 2c0a 2020      number=6,.  
-00012660: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-00012670: 7275 652c 0a20 2020 2020 2020 2065 6e75  rue,.        enu
-00012680: 6d3d 2254 7261 6666 6963 536f 7572 6365  m="TrafficSource
-00012690: 2e54 7261 6666 6963 536f 7572 6365 456e  .TrafficSourceEn
-000126a0: 756d 222c 0a20 2020 2029 0a20 2020 2072  um",.    ).    r
-000126b0: 616e 6b3a 2069 6e74 203d 2070 726f 746f  ank: int = proto
-000126c0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-000126d0: 7072 6f74 6f2e 494e 5436 342c 0a20 2020  proto.INT64,.   
-000126e0: 2020 2020 206e 756d 6265 723d 372c 0a20       number=7,. 
-000126f0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00012700: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-00012710: 6164 735f 6f72 6761 6e69 635f 7261 7469  ads_organic_rati
-00012720: 6f3a 2066 6c6f 6174 203d 2070 726f 746f  o: float = proto
-00012730: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00012740: 7072 6f74 6f2e 444f 5542 4c45 2c0a 2020  proto.DOUBLE,.  
-00012750: 2020 2020 2020 6e75 6d62 6572 3d38 2c0a        number=8,.
-00012760: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00012770: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-00012780: 2070 6167 655f 6f76 6572 6c61 705f 7261   page_overlap_ra
-00012790: 7465 3a20 666c 6f61 7420 3d20 7072 6f74  te: float = prot
-000127a0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000127b0: 2070 726f 746f 2e44 4f55 424c 452c 0a20   proto.DOUBLE,. 
-000127c0: 2020 2020 2020 206e 756d 6265 723d 392c         number=9,
-000127d0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-000127e0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-000127f0: 2020 6869 6768 6572 5f70 6f73 6974 696f    higher_positio
-00012800: 6e5f 7261 7465 3a20 666c 6f61 7420 3d20  n_rate: float = 
-00012810: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00012820: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
-00012830: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00012840: 723d 3130 2c0a 2020 2020 2020 2020 6f70  r=10,.        op
-00012850: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00012860: 2029 0a0a 0a63 6c61 7373 2043 6f6d 7065   )...class Compe
-00012870: 7469 7469 7665 5669 7369 6269 6c69 7479  titiveVisibility
-00012880: 4265 6e63 686d 6172 6b56 6965 7728 7072  BenchmarkView(pr
-00012890: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-000128a0: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
-000128b0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
-000128c0: 2069 6e0a 2020 2020 6060 636f 6d70 6574   in.    ``compet
-000128d0: 6974 6976 655f 7669 7369 6269 6c69 7479  itive_visibility
-000128e0: 5f62 656e 6368 6d61 726b 5f76 6965 7760  _benchmark_view`
-000128f0: 6020 7461 626c 652e 0a0a 2020 2020 6043  ` table...    `C
-00012900: 6f6d 7065 7469 7469 7665 0a20 2020 2076  ompetitive.    v
-00012910: 6973 6962 696c 6974 7920 3c68 7474 7073  isibility <https
-00012920: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00012930: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00012940: 616e 7377 6572 2f31 3133 3636 3434 323e  answer/11366442>
-00012950: 605f 5f0a 2020 2020 7265 706f 7274 2077  `__.    report w
-00012960: 6974 6820 7468 6520 6361 7465 676f 7279  ith the category
-00012970: 2062 656e 6368 6d61 726b 2e0a 0a20 2020   benchmark...   
-00012980: 2056 616c 7565 7320 6172 6520 6f6e 6c79   Values are only
-00012990: 2073 6574 2066 6f72 2066 6965 6c64 7320   set for fields 
-000129a0: 7265 7175 6573 7465 6420 6578 706c 6963  requested explic
-000129b0: 6974 6c79 2069 6e20 7468 6520 7265 7175  itly in the requ
-000129c0: 6573 7427 730a 2020 2020 7365 6172 6368  est's.    search
-000129d0: 2071 7565 7279 2e0a 0a0a 2020 2020 2e2e   query....    ..
-000129e0: 205f 6f6e 656f 663a 2068 7474 7073 3a2f   _oneof: https:/
-000129f0: 2f70 726f 746f 2d70 6c75 732d 7079 7468  /proto-plus-pyth
-00012a00: 6f6e 2e72 6561 6474 6865 646f 6373 2e69  on.readthedocs.i
-00012a10: 6f2f 656e 2f73 7461 626c 652f 6669 656c  o/en/stable/fiel
-00012a20: 6473 2e68 746d 6c23 6f6e 656f 6673 2d6d  ds.html#oneofs-m
-00012a30: 7574 7561 6c6c 792d 6578 636c 7573 6976  utually-exclusiv
-00012a40: 652d 6669 656c 6473 0a0a 2020 2020 4174  e-fields..    At
-00012a50: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00012a60: 2020 6461 7465 2028 676f 6f67 6c65 2e74    date (google.t
-00012a70: 7970 652e 6461 7465 5f70 6232 2e44 6174  ype.date_pb2.Dat
-00012a80: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00012a90: 4461 7465 206f 6620 7468 6973 2072 6f77  Date of this row
-00012aa0: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-00012ab0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-00012ac0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-00012ad0: 2e20 4120 636f 6e64 6974 696f 6e20 6f6e  . A condition on
-00012ae0: 2060 6064 6174 6560 600a 2020 2020 2020   ``date``.      
-00012af0: 2020 2020 2020 6973 2072 6571 7569 7265        is require
-00012b00: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
-00012b10: 6060 2063 6c61 7573 652e 0a20 2020 2020  `` clause..     
-00012b20: 2020 2072 6570 6f72 745f 636f 756e 7472     report_countr
-00012b30: 795f 636f 6465 2028 7374 7229 3a0a 2020  y_code (str):.  
-00012b40: 2020 2020 2020 2020 2020 436f 756e 7472            Countr
-00012b50: 7920 7768 6572 6520 696d 7072 6573 7369  y where impressi
-00012b60: 6f6e 7320 6170 7065 6172 6564 2e0a 0a20  ons appeared... 
-00012b70: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
-00012b80: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
-00012b90: 4543 5460 6020 636c 6175 7365 2e20 4120  ECT`` clause. A 
-00012ba0: 636f 6e64 6974 696f 6e20 6f6e 0a20 2020  condition on.   
-00012bb0: 2020 2020 2020 2020 2060 6072 6570 6f72           ``repor
-00012bc0: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
-00012bd0: 2069 7320 7265 7175 6972 6564 2069 6e20   is required in 
-00012be0: 7468 6520 6060 5748 4552 4560 6020 636c  the ``WHERE`` cl
-00012bf0: 6175 7365 2e0a 0a20 2020 2020 2020 2020  ause...         
-00012c00: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00012c10: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00012c20: 656f 6660 5f20 6060 5f72 6570 6f72 745f  eof`_ ``_report_
-00012c30: 636f 756e 7472 795f 636f 6465 6060 2e0a  country_code``..
-00012c40: 2020 2020 2020 2020 7265 706f 7274 5f63          report_c
-00012c50: 6174 6567 6f72 795f 6964 2028 696e 7429  ategory_id (int)
-00012c60: 3a0a 2020 2020 2020 2020 2020 2020 476f  :.            Go
-00012c70: 6f67 6c65 2070 726f 6475 6374 2063 6174  ogle product cat
-00012c80: 6567 6f72 7920 4944 2074 6f20 6361 6c63  egory ID to calc
-00012c90: 756c 6174 6520 7468 6520 7265 706f 7274  ulate the report
-00012ca0: 2066 6f72 2c0a 2020 2020 2020 2020 2020   for,.          
-00012cb0: 2020 7265 7072 6573 656e 7465 6420 696e    represented in
-00012cc0: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
-00012cd0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-00012ce0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-00012cf0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-00012d00: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-00012d10: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
-00012d20: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-00012d30: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-00012d40: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-00012d50: 2e20 4120 636f 6e64 6974 696f 6e20 6f6e  . A condition on
-00012d60: 0a20 2020 2020 2020 2020 2020 2060 6072  .            ``r
-00012d70: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
-00012d80: 6460 6020 6973 2072 6571 7569 7265 6420  d`` is required 
-00012d90: 696e 2074 6865 2060 6057 4845 5245 6060  in the ``WHERE``
-00012da0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
-00012db0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00012dc0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00012dd0: 606f 6e65 6f66 605f 2060 605f 7265 706f  `oneof`_ ``_repo
-00012de0: 7274 5f63 6174 6567 6f72 795f 6964 6060  rt_category_id``
-00012df0: 2e0a 2020 2020 2020 2020 7472 6166 6669  ..        traffi
-00012e00: 635f 736f 7572 6365 2028 676f 6f67 6c65  c_source (google
-00012e10: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
-00012e20: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
-00012e30: 612e 7479 7065 732e 5472 6166 6669 6353  a.types.TrafficS
-00012e40: 6f75 7263 652e 5472 6166 6669 6353 6f75  ource.TrafficSou
-00012e50: 7263 6545 6e75 6d29 3a0a 2020 2020 2020  rceEnum):.      
-00012e60: 2020 2020 2020 5472 6166 6669 6320 736f        Traffic so
-00012e70: 7572 6365 206f 6620 696d 7072 6573 7369  urce of impressi
-00012e80: 6f6e 732e 0a0a 2020 2020 2020 2020 2020  ons...          
-00012e90: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
-00012ea0: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
-00012eb0: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
-00012ec0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00012ed0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00012ee0: 6f66 605f 2060 605f 7472 6166 6669 635f  of`_ ``_traffic_
-00012ef0: 736f 7572 6365 6060 2e0a 2020 2020 2020  source``..      
-00012f00: 2020 796f 7572 5f64 6f6d 6169 6e5f 7669    your_domain_vi
-00012f10: 7369 6269 6c69 7479 5f74 7265 6e64 2028  sibility_trend (
-00012f20: 666c 6f61 7429 3a0a 2020 2020 2020 2020  float):.        
-00012f30: 2020 2020 4368 616e 6765 2069 6e20 7669      Change in vi
-00012f40: 7369 6269 6c69 7479 2062 6173 6564 206f  sibility based o
-00012f50: 6e20 696d 7072 6573 7369 6f6e 7320 666f  n impressions fo
-00012f60: 720a 2020 2020 2020 2020 2020 2020 796f  r.            yo
-00012f70: 7572 2064 6f6d 6169 6e20 7769 7468 2072  ur domain with r
-00012f80: 6573 7065 6374 2074 6f20 7468 6520 7374  espect to the st
-00012f90: 6172 7420 6f66 2074 6865 0a20 2020 2020  art of the.     
-00012fa0: 2020 2020 2020 2073 656c 6563 7465 6420         selected 
-00012fb0: 7469 6d65 2072 616e 6765 2028 6f72 2066  time range (or f
-00012fc0: 6972 7374 2064 6179 2077 6974 6820 6e6f  irst day with no
-00012fd0: 6e2d 7a65 726f 0a20 2020 2020 2020 2020  n-zero.         
-00012fe0: 2020 2069 6d70 7265 7373 696f 6e73 292e     impressions).
-00012ff0: 0a0a 2020 2020 2020 2020 2020 2020 4361  ..            Ca
-00013000: 6e6e 6f74 2062 6520 6669 6c74 6572 6564  nnot be filtered
-00013010: 206f 6e20 696e 2074 6865 2027 5748 4552   on in the 'WHER
-00013020: 4527 2063 6c61 7573 652e 0a0a 2020 2020  E' clause...    
-00013030: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00013040: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00013050: 6620 606f 6e65 6f66 605f 2060 605f 796f  f `oneof`_ ``_yo
-00013060: 7572 5f64 6f6d 6169 6e5f 7669 7369 6269  ur_domain_visibi
-00013070: 6c69 7479 5f74 7265 6e64 6060 2e0a 2020  lity_trend``..  
-00013080: 2020 2020 2020 6361 7465 676f 7279 5f62        category_b
-00013090: 656e 6368 6d61 726b 5f76 6973 6962 696c  enchmark_visibil
-000130a0: 6974 795f 7472 656e 6420 2866 6c6f 6174  ity_trend (float
-000130b0: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
-000130c0: 6861 6e67 6520 696e 2076 6973 6962 696c  hange in visibil
-000130d0: 6974 7920 6261 7365 6420 6f6e 2069 6d70  ity based on imp
-000130e0: 7265 7373 696f 6e73 0a20 2020 2020 2020  ressions.       
-000130f0: 2020 2020 2077 6974 6820 7265 7370 6563       with respec
-00013100: 7420 746f 2074 6865 2073 7461 7274 206f  t to the start o
-00013110: 6620 7468 6520 7365 6c65 6374 6564 2074  f the selected t
-00013120: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
-00013130: 7261 6e67 6520 286f 7220 6669 7273 7420  range (or first 
-00013140: 6461 7920 7769 7468 206e 6f6e 2d7a 6572  day with non-zer
-00013150: 6f20 696d 7072 6573 7369 6f6e 7329 0a20  o impressions). 
-00013160: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-00013170: 2063 6f6d 6269 6e65 6420 7365 7420 6f66   combined set of
-00013180: 206d 6572 6368 616e 7473 2077 6974 6820   merchants with 
-00013190: 6869 6768 6573 740a 2020 2020 2020 2020  highest.        
-000131a0: 2020 2020 7669 7369 6269 6c69 7479 2061      visibility a
-000131b0: 7070 726f 7869 6d61 7469 6e67 2074 6865  pproximating the
-000131c0: 206d 6172 6b65 742e 0a0a 2020 2020 2020   market...      
-000131d0: 2020 2020 2020 4361 6e6e 6f74 2062 6520        Cannot be 
-000131e0: 6669 6c74 6572 6564 206f 6e20 696e 2074  filtered on in t
-000131f0: 6865 2027 5748 4552 4527 2063 6c61 7573  he 'WHERE' claus
-00013200: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00013210: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00013220: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00013230: 605f 2060 605f 6361 7465 676f 7279 5f62  `_ ``_category_b
-00013240: 656e 6368 6d61 726b 5f76 6973 6962 696c  enchmark_visibil
-00013250: 6974 795f 7472 656e 6460 602e 0a20 2020  ity_trend``..   
-00013260: 2022 2222 0a0a 2020 2020 6461 7465 3a20   """..    date: 
-00013270: 6461 7465 5f70 6232 2e44 6174 6520 3d20  date_pb2.Date = 
-00013280: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00013290: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-000132a0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-000132b0: 6572 3d31 2c0a 2020 2020 2020 2020 6d65  er=1,.        me
-000132c0: 7373 6167 653d 6461 7465 5f70 6232 2e44  ssage=date_pb2.D
-000132d0: 6174 652c 0a20 2020 2029 0a20 2020 2072  ate,.    ).    r
-000132e0: 6570 6f72 745f 636f 756e 7472 795f 636f  eport_country_co
-000132f0: 6465 3a20 7374 7220 3d20 7072 6f74 6f2e  de: str = proto.
-00013300: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00013310: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00013320: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
-00013330: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00013340: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-00013350: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
-00013360: 6964 3a20 696e 7420 3d20 7072 6f74 6f2e  id: int = proto.
-00013370: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00013380: 726f 746f 2e49 4e54 3634 2c0a 2020 2020  roto.INT64,.    
-00013390: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-000133a0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000133b0: 7275 652c 0a20 2020 2029 0a20 2020 2074  rue,.    ).    t
-000133c0: 7261 6666 6963 5f73 6f75 7263 653a 2022  raffic_source: "
-000133d0: 5472 6166 6669 6353 6f75 7263 652e 5472  TrafficSource.Tr
-000133e0: 6166 6669 6353 6f75 7263 6545 6e75 6d22  afficSourceEnum"
-000133f0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00013400: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
-00013410: 554d 2c0a 2020 2020 2020 2020 6e75 6d62  UM,.        numb
-00013420: 6572 3d34 2c0a 2020 2020 2020 2020 6f70  er=4,.        op
-00013430: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00013440: 2020 2020 2065 6e75 6d3d 2254 7261 6666       enum="Traff
-00013450: 6963 536f 7572 6365 2e54 7261 6666 6963  icSource.Traffic
-00013460: 536f 7572 6365 456e 756d 222c 0a20 2020  SourceEnum",.   
-00013470: 2029 0a20 2020 2079 6f75 725f 646f 6d61   ).    your_doma
-00013480: 696e 5f76 6973 6962 696c 6974 795f 7472  in_visibility_tr
-00013490: 656e 643a 2066 6c6f 6174 203d 2070 726f  end: float = pro
-000134a0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-000134b0: 2020 7072 6f74 6f2e 444f 5542 4c45 2c0a    proto.DOUBLE,.
-000134c0: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
-000134d0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-000134e0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-000134f0: 2020 2063 6174 6567 6f72 795f 6265 6e63     category_benc
-00013500: 686d 6172 6b5f 7669 7369 6269 6c69 7479  hmark_visibility
-00013510: 5f74 7265 6e64 3a20 666c 6f61 7420 3d20  _trend: float = 
-00013520: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00013530: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
-00013540: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00013550: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
-00013560: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00013570: 290a 0a0a 636c 6173 7320 4d61 726b 6574  )...class Market
-00013580: 696e 674d 6574 686f 6428 7072 6f74 6f2e  ingMethod(proto.
-00013590: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-000135a0: 2222 4d61 726b 6574 696e 6720 6d65 7468  ""Marketing meth
-000135b0: 6f64 2075 7365 6420 746f 2070 726f 6d6f  od used to promo
-000135c0: 7465 2079 6f75 7220 7072 6f64 7563 7473  te your products
-000135d0: 206f 6e20 476f 6f67 6c65 0a20 2020 2028   on Google.    (
-000135e0: 6f72 6761 6e69 6320 7665 7273 7573 2061  organic versus a
-000135f0: 6473 292e 0a0a 2020 2020 2222 220a 0a20  ds)...    """.. 
-00013600: 2020 2063 6c61 7373 204d 6172 6b65 7469     class Marketi
-00013610: 6e67 4d65 7468 6f64 456e 756d 2870 726f  ngMethodEnum(pro
-00013620: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
-00013630: 2020 7222 2222 4d61 726b 6574 696e 6720    r"""Marketing 
-00013640: 6d65 7468 6f64 2076 616c 7565 732e 0a0a  method values...
-00013650: 2020 2020 2020 2020 5661 6c75 6573 3a0a          Values:.
-00013660: 2020 2020 2020 2020 2020 2020 4d41 524b              MARK
-00013670: 4554 494e 475f 4d45 5448 4f44 5f45 4e55  ETING_METHOD_ENU
-00013680: 4d5f 554e 5350 4543 4946 4945 4420 2830  M_UNSPECIFIED (0
-00013690: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000136a0: 2020 204e 6f74 2073 7065 6369 6669 6564     Not specified
-000136b0: 2e0a 2020 2020 2020 2020 2020 2020 4f52  ..            OR
-000136c0: 4741 4e49 4320 2831 293a 0a20 2020 2020  GANIC (1):.     
-000136d0: 2020 2020 2020 2020 2020 204f 7267 616e             Organ
-000136e0: 6963 206d 6172 6b65 7469 6e67 2e0a 2020  ic marketing..  
-000136f0: 2020 2020 2020 2020 2020 4144 5320 2832            ADS (2
-00013700: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013710: 2020 2041 6473 2d62 6173 6564 206d 6172     Ads-based mar
-00013720: 6b65 7469 6e67 2e0a 2020 2020 2020 2020  keting..        
-00013730: 2222 220a 2020 2020 2020 2020 4d41 524b  """.        MARK
-00013740: 4554 494e 475f 4d45 5448 4f44 5f45 4e55  ETING_METHOD_ENU
-00013750: 4d5f 554e 5350 4543 4946 4945 4420 3d20  M_UNSPECIFIED = 
-00013760: 300a 2020 2020 2020 2020 4f52 4741 4e49  0.        ORGANI
-00013770: 4320 3d20 310a 2020 2020 2020 2020 4144  C = 1.        AD
-00013780: 5320 3d20 320a 0a0a 636c 6173 7320 5265  S = 2...class Re
-00013790: 706f 7274 4772 616e 756c 6172 6974 7928  portGranularity(
-000137a0: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
-000137b0: 2020 2020 7222 2222 4772 616e 756c 6172      r"""Granular
-000137c0: 6974 7920 6f66 2074 6865 2042 6573 7420  ity of the Best 
-000137d0: 7365 6c6c 6572 7320 7265 706f 7274 2e20  sellers report. 
-000137e0: 4265 7374 2073 656c 6c65 7273 2072 6570  Best sellers rep
-000137f0: 6f72 7473 0a20 2020 2061 7265 2063 6f6d  orts.    are com
-00013800: 7075 7465 6420 6f76 6572 2061 2077 6565  puted over a wee
-00013810: 6b20 616e 6420 6120 6d6f 6e74 6820 7469  k and a month ti
-00013820: 6d65 6672 616d 652e 0a0a 2020 2020 2222  meframe...    ""
-00013830: 220a 0a20 2020 2063 6c61 7373 2052 6570  "..    class Rep
-00013840: 6f72 7447 7261 6e75 6c61 7269 7479 456e  ortGranularityEn
-00013850: 756d 2870 726f 746f 2e45 6e75 6d29 3a0a  um(proto.Enum):.
-00013860: 2020 2020 2020 2020 7222 2222 5265 706f          r"""Repo
-00013870: 7274 2067 7261 6e75 6c61 7269 7479 2076  rt granularity v
-00013880: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
-00013890: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-000138a0: 2020 2020 5245 504f 5254 5f47 5241 4e55      REPORT_GRANU
-000138b0: 4c41 5249 5459 5f45 4e55 4d5f 554e 5350  LARITY_ENUM_UNSP
-000138c0: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-000138d0: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
-000138e0: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
-000138f0: 2020 2020 2020 2020 5745 454b 4c59 2028          WEEKLY (
-00013900: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00013910: 2020 2020 5265 706f 7274 2069 7320 636f      Report is co
-00013920: 6d70 7574 6564 206f 7665 7220 6120 7765  mputed over a we
-00013930: 656b 2074 696d 6566 7261 6d65 2e0a 2020  ek timeframe..  
-00013940: 2020 2020 2020 2020 2020 4d4f 4e54 484c            MONTHL
-00013950: 5920 2832 293a 0a20 2020 2020 2020 2020  Y (2):.         
-00013960: 2020 2020 2020 2052 6570 6f72 7420 6973         Report is
-00013970: 2063 6f6d 7075 7465 6420 6f76 6572 2061   computed over a
-00013980: 206d 6f6e 7468 2074 696d 6566 7261 6d65   month timeframe
-00013990: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000139a0: 2020 2020 2020 5245 504f 5254 5f47 5241        REPORT_GRA
-000139b0: 4e55 4c41 5249 5459 5f45 4e55 4d5f 554e  NULARITY_ENUM_UN
-000139c0: 5350 4543 4946 4945 4420 3d20 300a 2020  SPECIFIED = 0.  
-000139d0: 2020 2020 2020 5745 454b 4c59 203d 2031        WEEKLY = 1
-000139e0: 0a20 2020 2020 2020 204d 4f4e 5448 4c59  .        MONTHLY
-000139f0: 203d 2032 0a0a 0a63 6c61 7373 2052 656c   = 2...class Rel
-00013a00: 6174 6976 6544 656d 616e 6428 7072 6f74  ativeDemand(prot
-00013a10: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00013a20: 7222 2222 5265 6c61 7469 7665 2064 656d  r"""Relative dem
-00013a30: 616e 6420 6f66 2061 2070 726f 6475 6374  and of a product
-00013a40: 2063 6c75 7374 6572 206f 7220 6272 616e   cluster or bran
-00013a50: 6420 696e 2074 6865 2042 6573 740a 2020  d in the Best.  
-00013a60: 2020 7365 6c6c 6572 7320 7265 706f 7274    sellers report
-00013a70: 2e0a 0a20 2020 2022 2222 0a0a 2020 2020  ...    """..    
-00013a80: 636c 6173 7320 5265 6c61 7469 7665 4465  class RelativeDe
-00013a90: 6d61 6e64 456e 756d 2870 726f 746f 2e45  mandEnum(proto.E
-00013aa0: 6e75 6d29 3a0a 2020 2020 2020 2020 7222  num):.        r"
-00013ab0: 2222 5265 6c61 7469 7665 2064 656d 616e  ""Relative deman
-00013ac0: 6420 7661 6c75 6573 2e0a 0a20 2020 2020  d values...     
-00013ad0: 2020 2056 616c 7565 733a 0a20 2020 2020     Values:.     
-00013ae0: 2020 2020 2020 2052 454c 4154 4956 455f         RELATIVE_
-00013af0: 4445 4d41 4e44 5f45 4e55 4d5f 554e 5350  DEMAND_ENUM_UNSP
-00013b00: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-00013b10: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
-00013b20: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
-00013b30: 2020 2020 2020 2020 5645 5259 5f4c 4f57          VERY_LOW
-00013b40: 2028 3130 293a 0a20 2020 2020 2020 2020   (10):.         
-00013b50: 2020 2020 2020 2044 656d 616e 6420 6973         Demand is
-00013b60: 2030 2d35 2520 6f66 2074 6865 2064 656d   0-5% of the dem
-00013b70: 616e 6420 6f66 2074 6865 2068 6967 6865  and of the highe
-00013b80: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
-00013b90: 2020 2072 616e 6b65 6420 7072 6f64 7563     ranked produc
-00013ba0: 7420 636c 7573 7465 7220 6f72 2062 7261  t cluster or bra
-00013bb0: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
-00013bc0: 4c4f 5720 2832 3029 3a0a 2020 2020 2020  LOW (20):.      
-00013bd0: 2020 2020 2020 2020 2020 4465 6d61 6e64            Demand
-00013be0: 2069 7320 362d 3130 2520 6f66 2074 6865   is 6-10% of the
-00013bf0: 2064 656d 616e 6420 6f66 2074 6865 2068   demand of the h
-00013c00: 6967 6865 7374 0a20 2020 2020 2020 2020  ighest.         
-00013c10: 2020 2020 2020 2072 616e 6b65 6420 7072         ranked pr
-00013c20: 6f64 7563 7420 636c 7573 7465 7220 6f72  oduct cluster or
-00013c30: 2062 7261 6e64 2e0a 2020 2020 2020 2020   brand..        
-00013c40: 2020 2020 4d45 4449 554d 2028 3330 293a      MEDIUM (30):
-00013c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c60: 2044 656d 616e 6420 6973 2031 312d 3230   Demand is 11-20
-00013c70: 2520 6f66 2074 6865 2064 656d 616e 6420  % of the demand 
-00013c80: 6f66 2074 6865 2068 6967 6865 7374 0a20  of the highest. 
-00013c90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013ca0: 616e 6b65 6420 7072 6f64 7563 7420 636c  anked product cl
-00013cb0: 7573 7465 7220 6f72 2062 7261 6e64 2e0a  uster or brand..
-00013cc0: 2020 2020 2020 2020 2020 2020 4849 4748              HIGH
-00013cd0: 2028 3430 293a 0a20 2020 2020 2020 2020   (40):.         
-00013ce0: 2020 2020 2020 2044 656d 616e 6420 6973         Demand is
-00013cf0: 2032 312d 3530 2520 6f66 2074 6865 2064   21-50% of the d
-00013d00: 656d 616e 6420 6f66 2074 6865 2068 6967  emand of the hig
-00013d10: 6865 7374 0a20 2020 2020 2020 2020 2020  hest.           
-00013d20: 2020 2020 2072 616e 6b65 6420 7072 6f64       ranked prod
-00013d30: 7563 7420 636c 7573 7465 7220 6f72 2062  uct cluster or b
-00013d40: 7261 6e64 2e0a 2020 2020 2020 2020 2020  rand..          
-00013d50: 2020 5645 5259 5f48 4947 4820 2835 3029    VERY_HIGH (50)
-00013d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013d70: 2020 4465 6d61 6e64 2069 7320 3531 2d31    Demand is 51-1
-00013d80: 3030 2520 6f66 2074 6865 2064 656d 616e  00% of the deman
-00013d90: 6420 6f66 2074 6865 0a20 2020 2020 2020  d of the.       
-00013da0: 2020 2020 2020 2020 2068 6967 6865 7374           highest
-00013db0: 2072 616e 6b65 6420 7072 6f64 7563 7420   ranked product 
-00013dc0: 636c 7573 7465 7220 6f72 2062 7261 6e64  cluster or brand
-00013dd0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00013de0: 2020 2020 2020 5245 4c41 5449 5645 5f44        RELATIVE_D
-00013df0: 454d 414e 445f 454e 554d 5f55 4e53 5045  EMAND_ENUM_UNSPE
-00013e00: 4349 4649 4544 203d 2030 0a20 2020 2020  CIFIED = 0.     
-00013e10: 2020 2056 4552 595f 4c4f 5720 3d20 3130     VERY_LOW = 10
-00013e20: 0a20 2020 2020 2020 204c 4f57 203d 2032  .        LOW = 2
-00013e30: 300a 2020 2020 2020 2020 4d45 4449 554d  0.        MEDIUM
-00013e40: 203d 2033 300a 2020 2020 2020 2020 4849   = 30.        HI
-00013e50: 4748 203d 2034 300a 2020 2020 2020 2020  GH = 40.        
-00013e60: 5645 5259 5f48 4947 4820 3d20 3530 0a0a  VERY_HIGH = 50..
-00013e70: 0a63 6c61 7373 2052 656c 6174 6976 6544  .class RelativeD
-00013e80: 656d 616e 6443 6861 6e67 6554 7970 6528  emandChangeType(
-00013e90: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
-00013ea0: 2020 2020 7222 2222 5265 6c61 7469 7665      r"""Relative
-00013eb0: 2064 656d 616e 6420 6f66 2061 2070 726f   demand of a pro
-00013ec0: 6475 6374 2063 6c75 7374 6572 206f 7220  duct cluster or 
-00013ed0: 6272 616e 6420 696e 2074 6865 2042 6573  brand in the Bes
-00013ee0: 740a 2020 2020 7365 6c6c 6572 7320 7265  t.    sellers re
-00013ef0: 706f 7274 2063 6f6d 7061 7265 6420 746f  port compared to
-00013f00: 2074 6865 2070 7265 7669 6f75 7320 7469   the previous ti
-00013f10: 6d65 2070 6572 696f 642e 0a0a 2020 2020  me period...    
-00013f20: 2222 220a 0a20 2020 2063 6c61 7373 2052  """..    class R
-00013f30: 656c 6174 6976 6544 656d 616e 6443 6861  elativeDemandCha
-00013f40: 6e67 6554 7970 6545 6e75 6d28 7072 6f74  ngeTypeEnum(prot
-00013f50: 6f2e 456e 756d 293a 0a20 2020 2020 2020  o.Enum):.       
-00013f60: 2072 2222 2252 656c 6174 6976 6520 6465   r"""Relative de
-00013f70: 6d61 6e64 2063 6861 6e67 6520 7479 7065  mand change type
-00013f80: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00013f90: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
-00013fa0: 2020 2020 2020 5245 4c41 5449 5645 5f44        RELATIVE_D
-00013fb0: 454d 414e 445f 4348 414e 4745 5f54 5950  EMAND_CHANGE_TYP
-00013fc0: 455f 454e 554d 5f55 4e53 5045 4349 4649  E_ENUM_UNSPECIFI
-00013fd0: 4544 2028 3029 3a0a 2020 2020 2020 2020  ED (0):.        
-00013fe0: 2020 2020 2020 2020 4e6f 7420 7370 6563          Not spec
-00013ff0: 6966 6965 642e 0a20 2020 2020 2020 2020  ified..         
-00014000: 2020 2053 494e 4b45 5220 2831 293a 0a20     SINKER (1):. 
-00014010: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-00014020: 656c 6174 6976 6520 6465 6d61 6e64 2069  elative demand i
-00014030: 7320 6c6f 7765 7220 7468 616e 2074 6865  s lower than the
-00014040: 2070 7265 7669 6f75 730a 2020 2020 2020   previous.      
-00014050: 2020 2020 2020 2020 2020 7469 6d65 2070            time p
-00014060: 6572 696f 642e 0a20 2020 2020 2020 2020  eriod..         
-00014070: 2020 2046 4c41 5420 2832 293a 0a20 2020     FLAT (2):.   
-00014080: 2020 2020 2020 2020 2020 2020 2052 656c               Rel
-00014090: 6174 6976 6520 6465 6d61 6e64 2069 7320  ative demand is 
-000140a0: 6571 7561 6c20 746f 2074 6865 2070 7265  equal to the pre
-000140b0: 7669 6f75 7320 7469 6d65 0a20 2020 2020  vious time.     
-000140c0: 2020 2020 2020 2020 2020 2070 6572 696f             perio
-000140d0: 642e 0a20 2020 2020 2020 2020 2020 2052  d..            R
-000140e0: 4953 4552 2028 3329 3a0a 2020 2020 2020  ISER (3):.      
-000140f0: 2020 2020 2020 2020 2020 5265 6c61 7469            Relati
-00014100: 7665 2064 656d 616e 6420 6973 2068 6967  ve demand is hig
-00014110: 6865 7220 7468 616e 2074 6865 2070 7265  her than the pre
-00014120: 7669 6f75 730a 2020 2020 2020 2020 2020  vious.          
-00014130: 2020 2020 2020 7469 6d65 2070 6572 696f        time perio
-00014140: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-00014150: 2020 2020 2020 2052 454c 4154 4956 455f         RELATIVE_
-00014160: 4445 4d41 4e44 5f43 4841 4e47 455f 5459  DEMAND_CHANGE_TY
-00014170: 5045 5f45 4e55 4d5f 554e 5350 4543 4946  PE_ENUM_UNSPECIF
-00014180: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
-00014190: 5349 4e4b 4552 203d 2031 0a20 2020 2020  SINKER = 1.     
-000141a0: 2020 2046 4c41 5420 3d20 320a 2020 2020     FLAT = 2.    
-000141b0: 2020 2020 5249 5345 5220 3d20 330a 0a0a      RISER = 3...
-000141c0: 636c 6173 7320 5472 6166 6669 6353 6f75  class TrafficSou
-000141d0: 7263 6528 7072 6f74 6f2e 4d65 7373 6167  rce(proto.Messag
-000141e0: 6529 3a0a 2020 2020 7222 2222 5472 6166  e):.    r"""Traf
-000141f0: 6669 6320 736f 7572 6365 206f 6620 696d  fic source of im
-00014200: 7072 6573 7369 6f6e 7320 696e 2074 6865  pressions in the
-00014210: 2043 6f6d 7065 7469 7469 7665 2076 6973   Competitive vis
-00014220: 6962 696c 6974 790a 2020 2020 7265 706f  ibility.    repo
-00014230: 7274 2e0a 0a20 2020 2022 2222 0a0a 2020  rt...    """..  
-00014240: 2020 636c 6173 7320 5472 6166 6669 6353    class TrafficS
-00014250: 6f75 7263 6545 6e75 6d28 7072 6f74 6f2e  ourceEnum(proto.
-00014260: 456e 756d 293a 0a20 2020 2020 2020 2072  Enum):.        r
-00014270: 2222 2254 7261 6666 6963 2073 6f75 7263  """Traffic sourc
-00014280: 6520 7661 6c75 6573 2e0a 0a20 2020 2020  e values...     
-00014290: 2020 2056 616c 7565 733a 0a20 2020 2020     Values:.     
-000142a0: 2020 2020 2020 2054 5241 4646 4943 5f53         TRAFFIC_S
-000142b0: 4f55 5243 455f 454e 554d 5f55 4e53 5045  OURCE_ENUM_UNSPE
-000142c0: 4349 4649 4544 2028 3029 3a0a 2020 2020  CIFIED (0):.    
-000142d0: 2020 2020 2020 2020 2020 2020 4e6f 7420              Not 
-000142e0: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
-000142f0: 2020 2020 2020 204f 5247 414e 4943 2028         ORGANIC (
-00014300: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00014310: 2020 2020 4f72 6761 6e69 6320 7472 6166      Organic traf
-00014320: 6669 632e 0a20 2020 2020 2020 2020 2020  fic..           
-00014330: 2041 4453 2028 3229 3a0a 2020 2020 2020   ADS (2):.      
-00014340: 2020 2020 2020 2020 2020 5472 6166 6669            Traffi
-00014350: 6320 6672 6f6d 2061 6473 2e0a 2020 2020  c from ads..    
-00014360: 2020 2020 2020 2020 414c 4c20 2833 293a          ALL (3):
-00014370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014380: 204f 7267 616e 6963 2061 6e64 2061 6473   Organic and ads
-00014390: 2074 7261 6666 6963 2e0a 2020 2020 2020   traffic..      
-000143a0: 2020 2222 220a 2020 2020 2020 2020 5452    """.        TR
-000143b0: 4146 4649 435f 534f 5552 4345 5f45 4e55  AFFIC_SOURCE_ENU
-000143c0: 4d5f 554e 5350 4543 4946 4945 4420 3d20  M_UNSPECIFIED = 
-000143d0: 300a 2020 2020 2020 2020 4f52 4741 4e49  0.        ORGANI
-000143e0: 4320 3d20 310a 2020 2020 2020 2020 4144  C = 1.        AD
-000143f0: 5320 3d20 320a 2020 2020 2020 2020 414c  S = 2.        AL
-00014400: 4c20 3d20 330a 0a0a 5f5f 616c 6c5f 5f20  L = 3...__all__ 
-00014410: 3d20 7475 706c 6528 736f 7274 6564 285f  = tuple(sorted(_
-00014420: 5f70 726f 746f 6275 665f 5f2e 6d61 6e69  _protobuf__.mani
-00014430: 6665 7374 2929 0a                        fest)).
+0000e830: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
+0000e840: 6f64 653a 2073 7472 203d 2070 726f 746f  ode: str = proto
+0000e850: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000e860: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+0000e870: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
+0000e880: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000e890: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+0000e8a0: 2072 6570 6f72 745f 6361 7465 676f 7279   report_category
+0000e8b0: 5f69 643a 2069 6e74 203d 2070 726f 746f  _id: int = proto
+0000e8c0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000e8d0: 7072 6f74 6f2e 494e 5436 342c 0a20 2020  proto.INT64,.   
+0000e8e0: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
+0000e8f0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000e900: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000e910: 7469 746c 653a 2073 7472 203d 2070 726f  title: str = pro
+0000e920: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+0000e930: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+0000e940: 2020 2020 2020 2020 6e75 6d62 6572 3d36          number=6
+0000e950: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+0000e960: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+0000e970: 2020 2062 7261 6e64 3a20 7374 7220 3d20     brand: str = 
+0000e980: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000e990: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+0000e9a0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+0000e9b0: 723d 372c 0a20 2020 2020 2020 206f 7074  r=7,.        opt
+0000e9c0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000e9d0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
+0000e9e0: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
+0000e9f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000ea00: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000ea10: 2020 2020 6e75 6d62 6572 3d38 2c0a 2020      number=8,.  
+0000ea20: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000ea30: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+0000ea40: 6174 6567 6f72 795f 6c32 3a20 7374 7220  ategory_l2: str 
+0000ea50: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+0000ea60: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+0000ea70: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+0000ea80: 6265 723d 392c 0a20 2020 2020 2020 206f  ber=9,.        o
+0000ea90: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000eaa0: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
+0000eab0: 5f6c 333a 2073 7472 203d 2070 726f 746f  _l3: str = proto
+0000eac0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000ead0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+0000eae0: 2020 2020 2020 6e75 6d62 6572 3d31 302c        number=10,
+0000eaf0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000eb00: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+0000eb10: 2020 6361 7465 676f 7279 5f6c 343a 2073    category_l4: s
+0000eb20: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000eb30: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000eb40: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000eb50: 6e75 6d62 6572 3d31 312c 0a20 2020 2020  number=11,.     
+0000eb60: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000eb70: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
+0000eb80: 676f 7279 5f6c 353a 2073 7472 203d 2070  gory_l5: str = p
+0000eb90: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000eba0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000ebb0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000ebc0: 3d31 322c 0a20 2020 2020 2020 206f 7074  =12,.        opt
+0000ebd0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000ebe0: 290a 2020 2020 7661 7269 616e 745f 6774  ).    variant_gt
+0000ebf0: 696e 733a 204d 7574 6162 6c65 5365 7175  ins: MutableSequ
+0000ec00: 656e 6365 5b73 7472 5d20 3d20 7072 6f74  ence[str] = prot
+0000ec10: 6f2e 5265 7065 6174 6564 4669 656c 6428  o.RepeatedField(
+0000ec20: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+0000ec30: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+0000ec40: 756d 6265 723d 3133 2c0a 2020 2020 290a  umber=13,.    ).
+0000ec50: 2020 2020 696e 7665 6e74 6f72 795f 7374      inventory_st
+0000ec60: 6174 7573 3a20 496e 7665 6e74 6f72 7953  atus: InventoryS
+0000ec70: 7461 7475 7320 3d20 7072 6f74 6f2e 4669  tatus = proto.Fi
+0000ec80: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000ec90: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
+0000eca0: 206e 756d 6265 723d 3134 2c0a 2020 2020   number=14,.    
+0000ecb0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+0000ecc0: 652c 0a20 2020 2020 2020 2065 6e75 6d3d  e,.        enum=
+0000ecd0: 496e 7665 6e74 6f72 7953 7461 7475 732c  InventoryStatus,
+0000ece0: 0a20 2020 2029 0a20 2020 2062 7261 6e64  .    ).    brand
+0000ecf0: 5f69 6e76 656e 746f 7279 5f73 7461 7475  _inventory_statu
+0000ed00: 733a 2049 6e76 656e 746f 7279 5374 6174  s: InventoryStat
+0000ed10: 7573 203d 2070 726f 746f 2e46 6965 6c64  us = proto.Field
+0000ed20: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000ed30: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+0000ed40: 6d62 6572 3d31 352c 0a20 2020 2020 2020  mber=15,.       
+0000ed50: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000ed60: 2020 2020 2020 2020 656e 756d 3d49 6e76          enum=Inv
+0000ed70: 656e 746f 7279 5374 6174 7573 2c0a 2020  entoryStatus,.  
+0000ed80: 2020 290a 2020 2020 7261 6e6b 3a20 696e    ).    rank: in
+0000ed90: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+0000eda0: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
+0000edb0: 4e54 3634 2c0a 2020 2020 2020 2020 6e75  NT64,.        nu
+0000edc0: 6d62 6572 3d31 362c 0a20 2020 2020 2020  mber=16,.       
+0000edd0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000ede0: 2020 2020 290a 2020 2020 7072 6576 696f      ).    previo
+0000edf0: 7573 5f72 616e 6b3a 2069 6e74 203d 2070  us_rank: int = p
+0000ee00: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000ee10: 2020 2020 7072 6f74 6f2e 494e 5436 342c      proto.INT64,
+0000ee20: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000ee30: 3137 2c0a 2020 2020 2020 2020 6f70 7469  17,.        opti
+0000ee40: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000ee50: 0a20 2020 2072 656c 6174 6976 655f 6465  .    relative_de
+0000ee60: 6d61 6e64 3a20 2252 656c 6174 6976 6544  mand: "RelativeD
+0000ee70: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
+0000ee80: 6d61 6e64 456e 756d 2220 3d20 7072 6f74  mandEnum" = prot
+0000ee90: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000eea0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
+0000eeb0: 2020 2020 206e 756d 6265 723d 3138 2c0a       number=18,.
+0000eec0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000eed0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
+0000eee0: 6e75 6d3d 2252 656c 6174 6976 6544 656d  num="RelativeDem
+0000eef0: 616e 642e 5265 6c61 7469 7665 4465 6d61  and.RelativeDema
+0000ef00: 6e64 456e 756d 222c 0a20 2020 2029 0a20  ndEnum",.    ). 
+0000ef10: 2020 2070 7265 7669 6f75 735f 7265 6c61     previous_rela
+0000ef20: 7469 7665 5f64 656d 616e 643a 2022 5265  tive_demand: "Re
+0000ef30: 6c61 7469 7665 4465 6d61 6e64 2e52 656c  lativeDemand.Rel
+0000ef40: 6174 6976 6544 656d 616e 6445 6e75 6d22  ativeDemandEnum"
+0000ef50: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ef60: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
+0000ef70: 554d 2c0a 2020 2020 2020 2020 6e75 6d62  UM,.        numb
+0000ef80: 6572 3d31 392c 0a20 2020 2020 2020 206f  er=19,.        o
+0000ef90: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000efa0: 2020 2020 2020 656e 756d 3d22 5265 6c61        enum="Rela
+0000efb0: 7469 7665 4465 6d61 6e64 2e52 656c 6174  tiveDemand.Relat
+0000efc0: 6976 6544 656d 616e 6445 6e75 6d22 2c0a  iveDemandEnum",.
+0000efd0: 2020 2020 290a 2020 2020 7265 6c61 7469      ).    relati
+0000efe0: 7665 5f64 656d 616e 645f 6368 616e 6765  ve_demand_change
+0000eff0: 3a20 2252 656c 6174 6976 6544 656d 616e  : "RelativeDeman
+0000f000: 6443 6861 6e67 6554 7970 652e 5265 6c61  dChangeType.Rela
+0000f010: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
+0000f020: 5479 7065 456e 756d 2220 3d20 280a 2020  TypeEnum" = (.  
+0000f030: 2020 2020 2020 7072 6f74 6f2e 4669 656c        proto.Fiel
+0000f040: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
+0000f050: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
+0000f060: 2020 2020 2020 206e 756d 6265 723d 3230         number=20
+0000f070: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
+0000f080: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000f090: 2020 2020 2020 2020 2065 6e75 6d3d 2252           enum="R
+0000f0a0: 656c 6174 6976 6544 656d 616e 6443 6861  elativeDemandCha
+0000f0b0: 6e67 6554 7970 652e 5265 6c61 7469 7665  ngeType.Relative
+0000f0c0: 4465 6d61 6e64 4368 616e 6765 5479 7065  DemandChangeType
+0000f0d0: 456e 756d 222c 0a20 2020 2020 2020 2029  Enum",.        )
+0000f0e0: 0a20 2020 2029 0a0a 0a63 6c61 7373 2042  .    )...class B
+0000f0f0: 6573 7453 656c 6c65 7273 4272 616e 6456  estSellersBrandV
+0000f100: 6965 7728 7072 6f74 6f2e 4d65 7373 6167  iew(proto.Messag
+0000f110: 6529 3a0a 2020 2020 7222 2222 4669 656c  e):.    r"""Fiel
+0000f120: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
+0000f130: 2071 7565 7279 2069 6e20 6060 6265 7374   query in ``best
+0000f140: 5f73 656c 6c65 7273 5f62 7261 6e64 5f76  _sellers_brand_v
+0000f150: 6965 7760 6020 7461 626c 652e 0a0a 2020  iew`` table...  
+0000f160: 2020 6042 6573 740a 2020 2020 7365 6c6c    `Best.    sell
+0000f170: 6572 7320 3c68 7474 7073 3a2f 2f73 7570  ers <https://sup
+0000f180: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000f190: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000f1a0: 2f39 3438 3836 3739 3e60 5f5f 0a20 2020  /9488679>`__.   
+0000f1b0: 2072 6570 6f72 7420 7769 7468 2074 6f70   report with top
+0000f1c0: 2062 7261 6e64 732e 0a0a 2020 2020 5661   brands...    Va
+0000f1d0: 6c75 6573 2061 7265 206f 6e6c 7920 7365  lues are only se
+0000f1e0: 7420 666f 7220 6669 656c 6473 2072 6571  t for fields req
+0000f1f0: 7565 7374 6564 2065 7870 6c69 6369 746c  uested explicitl
+0000f200: 7920 696e 2074 6865 2072 6571 7565 7374  y in the request
+0000f210: 2773 0a20 2020 2073 6561 7263 6820 7175  's.    search qu
+0000f220: 6572 792e 0a0a 0a20 2020 202e 2e20 5f6f  ery....    .. _o
+0000f230: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
+0000f240: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
+0000f250: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+0000f260: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
+0000f270: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
+0000f280: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
+0000f290: 6965 6c64 730a 0a20 2020 2041 7474 7269  ields..    Attri
+0000f2a0: 6275 7465 733a 0a20 2020 2020 2020 2072  butes:.        r
+0000f2b0: 6570 6f72 745f 6461 7465 2028 676f 6f67  eport_date (goog
+0000f2c0: 6c65 2e74 7970 652e 6461 7465 5f70 6232  le.type.date_pb2
+0000f2d0: 2e44 6174 6529 3a0a 2020 2020 2020 2020  .Date):.        
+0000f2e0: 2020 2020 5265 706f 7274 2064 6174 652e      Report date.
+0000f2f0: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
+0000f300: 6973 2066 6965 6c64 2063 616e 206f 6e6c  is field can onl
+0000f310: 7920 6265 206f 6e65 206f 6620 7468 650a  y be one of the.
+0000f320: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
+0000f330: 6f77 696e 673a 0a0a 2020 2020 2020 2020  owing:..        
+0000f340: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
+0000f350: 2064 6179 206f 6620 7468 6520 7765 656b   day of the week
+0000f360: 2028 4d6f 6e64 6179 2920 666f 7220 7765   (Monday) for we
+0000f370: 656b 6c79 2072 6570 6f72 7473 2c0a 2020  ekly reports,.  
+0000f380: 2020 2020 2020 2020 2020 2d20 2054 6865            -  The
+0000f390: 2066 6972 7374 2064 6179 206f 6620 7468   first day of th
+0000f3a0: 6520 6d6f 6e74 6820 666f 7220 6d6f 6e74  e month for mont
+0000f3b0: 686c 7920 7265 706f 7274 732e 0a0a 2020  hly reports...  
+0000f3c0: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
+0000f3d0: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
+0000f3e0: 4354 6060 2063 6c61 7573 652e 2049 6620  CT`` clause. If 
+0000f3f0: 6120 6060 5748 4552 4560 6020 636f 6e64  a ``WHERE`` cond
+0000f400: 6974 696f 6e0a 2020 2020 2020 2020 2020  ition.          
+0000f410: 2020 6f6e 2060 6072 6570 6f72 745f 6461    on ``report_da
+0000f420: 7465 6060 2069 7320 6e6f 7420 7370 6563  te`` is not spec
+0000f430: 6966 6965 6420 696e 2074 6865 2071 7565  ified in the que
+0000f440: 7279 2c20 7468 6520 6c61 7465 7374 0a20  ry, the latest. 
+0000f450: 2020 2020 2020 2020 2020 2061 7661 696c             avail
+0000f460: 6162 6c65 2077 6565 6b6c 7920 6f72 206d  able weekly or m
+0000f470: 6f6e 7468 6c79 2072 6570 6f72 7420 6973  onthly report is
+0000f480: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
+0000f490: 2020 2072 6570 6f72 745f 6772 616e 756c     report_granul
+0000f4a0: 6172 6974 7920 2867 6f6f 676c 652e 7368  arity (google.sh
+0000f4b0: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+0000f4c0: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+0000f4d0: 7970 6573 2e52 6570 6f72 7447 7261 6e75  ypes.ReportGranu
+0000f4e0: 6c61 7269 7479 2e52 6570 6f72 7447 7261  larity.ReportGra
+0000f4f0: 6e75 6c61 7269 7479 456e 756d 293a 0a20  nularityEnum):. 
+0000f500: 2020 2020 2020 2020 2020 2047 7261 6e75             Granu
+0000f510: 6c61 7269 7479 206f 6620 7468 6520 7265  larity of the re
+0000f520: 706f 7274 2e20 5468 6520 7261 6e6b 696e  port. The rankin
+0000f530: 6720 6361 6e20 6265 2064 6f6e 6520 6f76  g can be done ov
+0000f540: 6572 2061 0a20 2020 2020 2020 2020 2020  er a.           
+0000f550: 2077 6565 6b20 6f72 2061 206d 6f6e 7468   week or a month
+0000f560: 2074 696d 6566 7261 6d65 2e0a 0a20 2020   timeframe...   
+0000f570: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+0000f580: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+0000f590: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
+0000f5a0: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
+0000f5b0: 2020 2020 2060 6072 6570 6f72 745f 6772       ``report_gr
+0000f5c0: 616e 756c 6172 6974 7960 6020 6973 2072  anularity`` is r
+0000f5d0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
+0000f5e0: 6057 4845 5245 6060 2063 6c61 7573 652e  `WHERE`` clause.
+0000f5f0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000f600: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000f610: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000f620: 2060 605f 7265 706f 7274 5f67 7261 6e75   ``_report_granu
+0000f630: 6c61 7269 7479 6060 2e0a 2020 2020 2020  larity``..      
+0000f640: 2020 7265 706f 7274 5f63 6f75 6e74 7279    report_country
+0000f650: 5f63 6f64 6520 2873 7472 293a 0a20 2020  _code (str):.   
+0000f660: 2020 2020 2020 2020 2043 6f75 6e74 7279           Country
+0000f670: 2077 6865 7265 2074 6865 2072 616e 6b69   where the ranki
+0000f680: 6e67 2069 7320 6361 6c63 756c 6174 6564  ng is calculated
+0000f690: 2e20 5265 7072 6573 656e 7465 6420 696e  . Represented in
+0000f6a0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+0000f6b0: 2049 534f 2033 3136 3620 666f 726d 6174   ISO 3166 format
+0000f6c0: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
+0000f6d0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
+0000f6e0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
+0000f6f0: 2e20 436f 6e64 6974 696f 6e20 6f6e 0a20  . Condition on. 
+0000f700: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
+0000f710: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+0000f720: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
+0000f730: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
+0000f740: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
+0000f750: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000f760: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000f770: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
+0000f780: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
+0000f790: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
+0000f7a0: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
+0000f7b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000f7c0: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
+0000f7d0: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
+0000f7e0: 6c63 756c 6174 6520 7468 6520 7261 6e6b  lculate the rank
+0000f7f0: 696e 6720 666f 722c 0a20 2020 2020 2020  ing for,.       
+0000f800: 2020 2020 2072 6570 7265 7365 6e74 6564       represented
+0000f810: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
+0000f820: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+0000f830: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+0000f840: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+0000f850: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+0000f860: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
+0000f870: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+0000f880: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
+0000f890: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
+0000f8a0: 7573 652e 2049 6620 6120 6060 5748 4552  use. If a ``WHER
+0000f8b0: 4560 6020 636f 6e64 6974 696f 6e0a 2020  E`` condition.  
+0000f8c0: 2020 2020 2020 2020 2020 6f6e 2060 6072            on ``r
+0000f8d0: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
+0000f8e0: 6460 6020 6973 206e 6f74 2073 7065 6369  d`` is not speci
+0000f8f0: 6669 6564 2069 6e20 7468 6520 7175 6572  fied in the quer
+0000f900: 792c 0a20 2020 2020 2020 2020 2020 2072  y,.            r
+0000f910: 616e 6b69 6e67 7320 666f 7220 616c 6c20  ankings for all 
+0000f920: 746f 702d 6c65 7665 6c20 6361 7465 676f  top-level catego
+0000f930: 7269 6573 2061 7265 2072 6574 7572 6e65  ries are returne
+0000f940: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
+0000f950: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+0000f960: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+0000f970: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
+0000f980: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
+0000f990: 2020 2020 6272 616e 6420 2873 7472 293a      brand (str):
+0000f9a0: 0a20 2020 2020 2020 2020 2020 204e 616d  .            Nam
+0000f9b0: 6520 6f66 2074 6865 2062 7261 6e64 2e0a  e of the brand..
+0000f9c0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000f9d0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000f9e0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000f9f0: 6060 5f62 7261 6e64 6060 2e0a 2020 2020  ``_brand``..    
+0000fa00: 2020 2020 7261 6e6b 2028 696e 7429 3a0a      rank (int):.
+0000fa10: 2020 2020 2020 2020 2020 2020 506f 7075              Popu
+0000fa20: 6c61 7269 7479 206f 6620 7468 6520 6272  larity of the br
+0000fa30: 616e 6420 6f6e 2041 6473 2061 6e64 206f  and on Ads and o
+0000fa40: 7267 616e 6963 0a20 2020 2020 2020 2020  rganic.         
+0000fa50: 2020 2073 7572 6661 6365 732c 2069 6e20     surfaces, in 
+0000fa60: 7468 6520 7365 6c65 6374 6564 2063 6174  the selected cat
+0000fa70: 6567 6f72 7920 616e 6420 636f 756e 7472  egory and countr
+0000fa80: 792c 0a20 2020 2020 2020 2020 2020 2062  y,.            b
+0000fa90: 6173 6564 206f 6e20 7468 6520 6573 7469  ased on the esti
+0000faa0: 6d61 7465 6420 6e75 6d62 6572 206f 6620  mated number of 
+0000fab0: 756e 6974 7320 736f 6c64 2e0a 0a20 2020  units sold...   
+0000fac0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+0000fad0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+0000fae0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f72  of `oneof`_ ``_r
+0000faf0: 616e 6b60 602e 0a20 2020 2020 2020 2070  ank``..        p
+0000fb00: 7265 7669 6f75 735f 7261 6e6b 2028 696e  revious_rank (in
+0000fb10: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000fb20: 506f 7075 6c61 7269 7479 2072 616e 6b20  Popularity rank 
+0000fb30: 696e 2074 6865 2070 7265 7669 6f75 7320  in the previous 
+0000fb40: 7765 656b 206f 720a 2020 2020 2020 2020  week or.        
+0000fb50: 2020 2020 6d6f 6e74 682e 0a0a 2020 2020      month...    
+0000fb60: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000fb70: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000fb80: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+0000fb90: 6576 696f 7573 5f72 616e 6b60 602e 0a20  evious_rank``.. 
+0000fba0: 2020 2020 2020 2072 656c 6174 6976 655f         relative_
+0000fbb0: 6465 6d61 6e64 2028 676f 6f67 6c65 2e73  demand (google.s
+0000fbc0: 686f 7070 696e 672e 6d65 7263 6861 6e74  hopping.merchant
+0000fbd0: 5f72 6570 6f72 7473 5f76 3162 6574 612e  _reports_v1beta.
+0000fbe0: 7479 7065 732e 5265 6c61 7469 7665 4465  types.RelativeDe
+0000fbf0: 6d61 6e64 2e52 656c 6174 6976 6544 656d  mand.RelativeDem
+0000fc00: 616e 6445 6e75 6d29 3a0a 2020 2020 2020  andEnum):.      
+0000fc10: 2020 2020 2020 4573 7469 6d61 7465 6420        Estimated 
+0000fc20: 6465 6d61 6e64 2069 6e20 7265 6c61 7469  demand in relati
+0000fc30: 6f6e 2074 6f20 7468 6520 6272 616e 640a  on to the brand.
+0000fc40: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000fc50: 2074 6865 2068 6967 6865 7374 2070 6f70   the highest pop
+0000fc60: 756c 6172 6974 7920 7261 6e6b 2069 6e20  ularity rank in 
+0000fc70: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
+0000fc80: 2020 2020 2063 6174 6567 6f72 7920 616e       category an
+0000fc90: 6420 636f 756e 7472 792e 0a0a 2020 2020  d country...    
+0000fca0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000fcb0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000fcc0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+0000fcd0: 6c61 7469 7665 5f64 656d 616e 6460 602e  lative_demand``.
+0000fce0: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
+0000fcf0: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
+0000fd00: 6420 2867 6f6f 676c 652e 7368 6f70 7069  d (google.shoppi
+0000fd10: 6e67 2e6d 6572 6368 616e 745f 7265 706f  ng.merchant_repo
+0000fd20: 7274 735f 7631 6265 7461 2e74 7970 6573  rts_v1beta.types
+0000fd30: 2e52 656c 6174 6976 6544 656d 616e 642e  .RelativeDemand.
+0000fd40: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
+0000fd50: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+0000fd60: 2045 7374 696d 6174 6564 2064 656d 616e   Estimated deman
+0000fd70: 6420 696e 2072 656c 6174 696f 6e20 746f  d in relation to
+0000fd80: 2074 6865 2062 7261 6e64 0a20 2020 2020   the brand.     
+0000fd90: 2020 2020 2020 2077 6974 6820 7468 6520         with the 
+0000fda0: 6869 6768 6573 7420 706f 7075 6c61 7269  highest populari
+0000fdb0: 7479 2072 616e 6b20 696e 2074 6865 2073  ty rank in the s
+0000fdc0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000fdd0: 6361 7465 676f 7279 2061 6e64 2063 6f75  category and cou
+0000fde0: 6e74 7279 2069 6e20 7468 6520 7072 6576  ntry in the prev
+0000fdf0: 696f 7573 2077 6565 6b20 6f72 0a20 2020  ious week or.   
+0000fe00: 2020 2020 2020 2020 206d 6f6e 7468 2e0a           month..
+0000fe10: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000fe20: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000fe30: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000fe40: 6060 5f70 7265 7669 6f75 735f 7265 6c61  ``_previous_rela
+0000fe50: 7469 7665 5f64 656d 616e 6460 602e 0a20  tive_demand``.. 
+0000fe60: 2020 2020 2020 2072 656c 6174 6976 655f         relative_
+0000fe70: 6465 6d61 6e64 5f63 6861 6e67 6520 2867  demand_change (g
+0000fe80: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
+0000fe90: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
+0000fea0: 7631 6265 7461 2e74 7970 6573 2e52 656c  v1beta.types.Rel
+0000feb0: 6174 6976 6544 656d 616e 6443 6861 6e67  ativeDemandChang
+0000fec0: 6554 7970 652e 5265 6c61 7469 7665 4465  eType.RelativeDe
+0000fed0: 6d61 6e64 4368 616e 6765 5479 7065 456e  mandChangeTypeEn
+0000fee0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+0000fef0: 2043 6861 6e67 6520 696e 2074 6865 2065   Change in the e
+0000ff00: 7374 696d 6174 6564 2064 656d 616e 642e  stimated demand.
+0000ff10: 2057 6865 7468 6572 2069 740a 2020 2020   Whether it.    
+0000ff20: 2020 2020 2020 2020 726f 7365 2c20 7361          rose, sa
+0000ff30: 6e6b 206f 7220 7265 6d61 696e 6564 2066  nk or remained f
+0000ff40: 6c61 742e 0a0a 2020 2020 2020 2020 2020  lat...          
+0000ff50: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000ff60: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000ff70: 6f66 605f 2060 605f 7265 6c61 7469 7665  of`_ ``_relative
+0000ff80: 5f64 656d 616e 645f 6368 616e 6765 6060  _demand_change``
+0000ff90: 2e0a 2020 2020 2222 220a 0a20 2020 2072  ..    """..    r
+0000ffa0: 6570 6f72 745f 6461 7465 3a20 6461 7465  eport_date: date
+0000ffb0: 5f70 6232 2e44 6174 6520 3d20 7072 6f74  _pb2.Date = prot
+0000ffc0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000ffd0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+0000ffe0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+0000fff0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00010000: 653d 6461 7465 5f70 6232 2e44 6174 652c  e=date_pb2.Date,
+00010010: 0a20 2020 2029 0a20 2020 2072 6570 6f72  .    ).    repor
+00010020: 745f 6772 616e 756c 6172 6974 793a 2022  t_granularity: "
+00010030: 5265 706f 7274 4772 616e 756c 6172 6974  ReportGranularit
+00010040: 792e 5265 706f 7274 4772 616e 756c 6172  y.ReportGranular
+00010050: 6974 7945 6e75 6d22 203d 2070 726f 746f  ityEnum" = proto
+00010060: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00010070: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
+00010080: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+00010090: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000100a0: 7275 652c 0a20 2020 2020 2020 2065 6e75  rue,.        enu
+000100b0: 6d3d 2252 6570 6f72 7447 7261 6e75 6c61  m="ReportGranula
+000100c0: 7269 7479 2e52 6570 6f72 7447 7261 6e75  rity.ReportGranu
+000100d0: 6c61 7269 7479 456e 756d 222c 0a20 2020  larityEnum",.   
+000100e0: 2029 0a20 2020 2072 6570 6f72 745f 636f   ).    report_co
+000100f0: 756e 7472 795f 636f 6465 3a20 7374 7220  untry_code: str 
+00010100: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00010110: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00010120: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00010130: 6265 723d 332c 0a20 2020 2020 2020 206f  ber=3,.        o
+00010140: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00010150: 2020 290a 2020 2020 7265 706f 7274 5f63    ).    report_c
+00010160: 6174 6567 6f72 795f 6964 3a20 696e 7420  ategory_id: int 
+00010170: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00010180: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
+00010190: 3634 2c0a 2020 2020 2020 2020 6e75 6d62  64,.        numb
+000101a0: 6572 3d34 2c0a 2020 2020 2020 2020 6f70  er=4,.        op
+000101b0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+000101c0: 2029 0a20 2020 2062 7261 6e64 3a20 7374   ).    brand: st
+000101d0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+000101e0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000101f0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00010200: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
+00010210: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+00010220: 2020 2020 290a 2020 2020 7261 6e6b 3a20      ).    rank: 
+00010230: 696e 7420 3d20 7072 6f74 6f2e 4669 656c  int = proto.Fiel
+00010240: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00010250: 2e49 4e54 3634 2c0a 2020 2020 2020 2020  .INT64,.        
+00010260: 6e75 6d62 6572 3d37 2c0a 2020 2020 2020  number=7,.      
+00010270: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00010280: 0a20 2020 2029 0a20 2020 2070 7265 7669  .    ).    previ
+00010290: 6f75 735f 7261 6e6b 3a20 696e 7420 3d20  ous_rank: int = 
+000102a0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000102b0: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
+000102c0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000102d0: 3d38 2c0a 2020 2020 2020 2020 6f70 7469  =8,.        opti
+000102e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000102f0: 0a20 2020 2072 656c 6174 6976 655f 6465  .    relative_de
+00010300: 6d61 6e64 3a20 2252 656c 6174 6976 6544  mand: "RelativeD
+00010310: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
+00010320: 6d61 6e64 456e 756d 2220 3d20 7072 6f74  mandEnum" = prot
+00010330: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00010340: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
+00010350: 2020 2020 206e 756d 6265 723d 392c 0a20       number=9,. 
+00010360: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00010370: 5472 7565 2c0a 2020 2020 2020 2020 656e  True,.        en
+00010380: 756d 3d22 5265 6c61 7469 7665 4465 6d61  um="RelativeDema
+00010390: 6e64 2e52 656c 6174 6976 6544 656d 616e  nd.RelativeDeman
+000103a0: 6445 6e75 6d22 2c0a 2020 2020 290a 2020  dEnum",.    ).  
+000103b0: 2020 7072 6576 696f 7573 5f72 656c 6174    previous_relat
+000103c0: 6976 655f 6465 6d61 6e64 3a20 2252 656c  ive_demand: "Rel
+000103d0: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
+000103e0: 7469 7665 4465 6d61 6e64 456e 756d 2220  tiveDemandEnum" 
+000103f0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00010400: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
+00010410: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
+00010420: 723d 3130 2c0a 2020 2020 2020 2020 6f70  r=10,.        op
+00010430: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00010440: 2020 2020 2065 6e75 6d3d 2252 656c 6174       enum="Relat
+00010450: 6976 6544 656d 616e 642e 5265 6c61 7469  iveDemand.Relati
+00010460: 7665 4465 6d61 6e64 456e 756d 222c 0a20  veDemandEnum",. 
+00010470: 2020 2029 0a20 2020 2072 656c 6174 6976     ).    relativ
+00010480: 655f 6465 6d61 6e64 5f63 6861 6e67 653a  e_demand_change:
+00010490: 2022 5265 6c61 7469 7665 4465 6d61 6e64   "RelativeDemand
+000104a0: 4368 616e 6765 5479 7065 2e52 656c 6174  ChangeType.Relat
+000104b0: 6976 6544 656d 616e 6443 6861 6e67 6554  iveDemandChangeT
+000104c0: 7970 6545 6e75 6d22 203d 2028 0a20 2020  ypeEnum" = (.   
+000104d0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
+000104e0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+000104f0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
+00010500: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
+00010510: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+00010520: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00010530: 2020 2020 2020 2020 656e 756d 3d22 5265          enum="Re
+00010540: 6c61 7469 7665 4465 6d61 6e64 4368 616e  lativeDemandChan
+00010550: 6765 5479 7065 2e52 656c 6174 6976 6544  geType.RelativeD
+00010560: 656d 616e 6443 6861 6e67 6554 7970 6545  emandChangeTypeE
+00010570: 6e75 6d22 2c0a 2020 2020 2020 2020 290a  num",.        ).
+00010580: 2020 2020 290a 0a0a 636c 6173 7320 436f      )...class Co
+00010590: 6d70 6574 6974 6976 6556 6973 6962 696c  mpetitiveVisibil
+000105a0: 6974 7943 6f6d 7065 7469 746f 7256 6965  ityCompetitorVie
+000105b0: 7728 7072 6f74 6f2e 4d65 7373 6167 6529  w(proto.Message)
+000105c0: 3a0a 2020 2020 7222 2222 4669 656c 6473  :.    r"""Fields
+000105d0: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
+000105e0: 7565 7279 2069 6e0a 2020 2020 6060 636f  uery in.    ``co
+000105f0: 6d70 6574 6974 6976 655f 7669 7369 6269  mpetitive_visibi
+00010600: 6c69 7479 5f63 6f6d 7065 7469 746f 725f  lity_competitor_
+00010610: 7669 6577 6060 2074 6162 6c65 2e0a 0a20  view`` table... 
+00010620: 2020 2060 436f 6d70 6574 6974 6976 650a     `Competitive.
+00010630: 2020 2020 7669 7369 6269 6c69 7479 203c      visibility <
+00010640: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
+00010650: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
+00010660: 616e 7473 2f61 6e73 7765 722f 3131 3336  ants/answer/1136
+00010670: 3634 3432 3e60 5f5f 0a20 2020 2072 6570  6442>`__.    rep
+00010680: 6f72 7420 7769 7468 2062 7573 696e 6573  ort with busines
+00010690: 7365 7320 7769 7468 2073 696d 696c 6172  ses with similar
+000106a0: 2076 6973 6962 696c 6974 792e 0a0a 2020   visibility...  
+000106b0: 2020 5661 6c75 6573 2061 7265 206f 6e6c    Values are onl
+000106c0: 7920 7365 7420 666f 7220 6669 656c 6473  y set for fields
+000106d0: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
+000106e0: 6369 746c 7920 696e 2074 6865 2072 6571  citly in the req
+000106f0: 7565 7374 2773 0a20 2020 2073 6561 7263  uest's.    searc
+00010700: 6820 7175 6572 792e 0a0a 0a20 2020 202e  h query....    .
+00010710: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
+00010720: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
+00010730: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+00010740: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
+00010750: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
+00010760: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
+00010770: 7665 2d66 6965 6c64 730a 0a20 2020 2041  ve-fields..    A
+00010780: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+00010790: 2020 2064 6174 6520 2867 6f6f 676c 652e     date (google.
+000107a0: 7479 7065 2e64 6174 655f 7062 322e 4461  type.date_pb2.Da
+000107b0: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
+000107c0: 2044 6174 6520 6f66 2074 6869 7320 726f   Date of this ro
+000107d0: 772e 0a0a 2020 2020 2020 2020 2020 2020  w...            
+000107e0: 4120 636f 6e64 6974 696f 6e20 6f6e 2060  A condition on `
+000107f0: 6064 6174 6560 6020 6973 2072 6571 7569  `date`` is requi
+00010800: 7265 6420 696e 2074 6865 2060 6057 4845  red in the ``WHE
+00010810: 5245 6060 2063 6c61 7573 652e 0a20 2020  RE`` clause..   
+00010820: 2020 2020 2064 6f6d 6169 6e20 2873 7472       domain (str
+00010830: 293a 0a20 2020 2020 2020 2020 2020 2044  ):.            D
+00010840: 6f6d 6169 6e20 6f66 2079 6f75 7220 636f  omain of your co
+00010850: 6d70 6574 6974 6f72 206f 7220 796f 7572  mpetitor or your
+00010860: 2064 6f6d 6169 6e2c 2069 660a 2020 2020   domain, if.    
+00010870: 2020 2020 2020 2020 2769 735f 796f 7572          'is_your
+00010880: 5f64 6f6d 6169 6e27 2069 7320 7472 7565  _domain' is true
+00010890: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
+000108a0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
+000108b0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
+000108c0: 2e20 4361 6e6e 6f74 2062 6520 6669 6c74  . Cannot be filt
+000108d0: 6572 6564 206f 6e20 696e 0a20 2020 2020  ered on in.     
+000108e0: 2020 2020 2020 2074 6865 2027 5748 4552         the 'WHER
+000108f0: 4527 2063 6c61 7573 652e 0a0a 2020 2020  E' clause...    
+00010900: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00010910: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00010920: 6620 606f 6e65 6f66 605f 2060 605f 646f  f `oneof`_ ``_do
+00010930: 6d61 696e 6060 2e0a 2020 2020 2020 2020  main``..        
+00010940: 6973 5f79 6f75 725f 646f 6d61 696e 2028  is_your_domain (
+00010950: 626f 6f6c 293a 0a20 2020 2020 2020 2020  bool):.         
+00010960: 2020 2054 7275 6520 6966 2074 6869 7320     True if this 
+00010970: 726f 7720 636f 6e74 6169 6e73 2064 6174  row contains dat
+00010980: 6120 666f 7220 796f 7572 0a20 2020 2020  a for your.     
+00010990: 2020 2020 2020 2064 6f6d 6169 6e2e 0a20         domain.. 
+000109a0: 2020 2020 2020 2020 2020 2043 616e 6e6f             Canno
+000109b0: 7420 6265 2066 696c 7465 7265 6420 6f6e  t be filtered on
+000109c0: 2069 6e20 7468 6520 2757 4845 5245 2720   in the 'WHERE' 
+000109d0: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
+000109e0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+000109f0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00010a00: 6f6e 656f 6660 5f20 6060 5f69 735f 796f  oneof`_ ``_is_yo
+00010a10: 7572 5f64 6f6d 6169 6e60 602e 0a20 2020  ur_domain``..   
+00010a20: 2020 2020 2072 6570 6f72 745f 636f 756e       report_coun
+00010a30: 7472 795f 636f 6465 2028 7374 7229 3a0a  try_code (str):.
+00010a40: 2020 2020 2020 2020 2020 2020 436f 756e              Coun
+00010a50: 7472 7920 7768 6572 6520 696d 7072 6573  try where impres
+00010a60: 7369 6f6e 7320 6170 7065 6172 6564 2e0a  sions appeared..
+00010a70: 0a20 2020 2020 2020 2020 2020 2052 6571  .            Req
+00010a80: 7569 7265 6420 696e 2074 6865 2060 6053  uired in the ``S
+00010a90: 454c 4543 5460 6020 636c 6175 7365 2e20  ELECT`` clause. 
+00010aa0: 4120 636f 6e64 6974 696f 6e20 6f6e 0a20  A condition on. 
+00010ab0: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
+00010ac0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+00010ad0: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
+00010ae0: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
+00010af0: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
+00010b00: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00010b10: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00010b20: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
+00010b30: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
+00010b40: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
+00010b50: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
+00010b60: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00010b70: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
+00010b80: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
+00010b90: 6c63 756c 6174 6520 7468 6520 7265 706f  lculate the repo
+00010ba0: 7274 2066 6f72 2c0a 2020 2020 2020 2020  rt for,.        
+00010bb0: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
+00010bc0: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+00010bd0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+00010be0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+00010bf0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+00010c00: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+00010c10: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+00010c20: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+00010c30: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
+00010c40: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
+00010c50: 7365 2e20 4120 636f 6e64 6974 696f 6e20  se. A condition 
+00010c60: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
+00010c70: 6072 6570 6f72 745f 6361 7465 676f 7279  `report_category
+00010c80: 5f69 6460 6020 6973 2072 6571 7569 7265  _id`` is require
+00010c90: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
+00010ca0: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
+00010cb0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00010cc0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00010cd0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+00010ce0: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
+00010cf0: 6060 2e0a 2020 2020 2020 2020 7472 6166  ``..        traf
+00010d00: 6669 635f 736f 7572 6365 2028 676f 6f67  fic_source (goog
+00010d10: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+00010d20: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+00010d30: 6574 612e 7479 7065 732e 5472 6166 6669  eta.types.Traffi
+00010d40: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
+00010d50: 6f75 7263 6545 6e75 6d29 3a0a 2020 2020  ourceEnum):.    
+00010d60: 2020 2020 2020 2020 5472 6166 6669 6320          Traffic 
+00010d70: 736f 7572 6365 206f 6620 696d 7072 6573  source of impres
+00010d80: 7369 6f6e 732e 0a0a 2020 2020 2020 2020  sions...        
+00010d90: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
+00010da0: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
+00010db0: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
+00010dc0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00010dd0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00010de0: 6e65 6f66 605f 2060 605f 7472 6166 6669  neof`_ ``_traffi
+00010df0: 635f 736f 7572 6365 6060 2e0a 2020 2020  c_source``..    
+00010e00: 2020 2020 7261 6e6b 2028 696e 7429 3a0a      rank (int):.
+00010e10: 2020 2020 2020 2020 2020 2020 506f 7369              Posi
+00010e20: 7469 6f6e 206f 6620 7468 6520 646f 6d61  tion of the doma
+00010e30: 696e 2069 6e20 7468 6520 7369 6d69 6c61  in in the simila
+00010e40: 7220 6275 7369 6e65 7373 6573 2072 616e  r businesses ran
+00010e50: 6b69 6e67 2066 6f72 0a20 2020 2020 2020  king for.       
+00010e60: 2020 2020 2074 6865 2073 656c 6563 7465       the selecte
+00010e70: 6420 6b65 7973 2028 6060 6461 7465 6060  d keys (``date``
+00010e80: 2c20 6060 7265 706f 7274 5f63 6174 6567  , ``report_categ
+00010e90: 6f72 795f 6964 6060 2c0a 2020 2020 2020  ory_id``,.      
+00010ea0: 2020 2020 2020 6060 7265 706f 7274 5f63        ``report_c
+00010eb0: 6f75 6e74 7279 5f63 6f64 6560 602c 2060  ountry_code``, `
+00010ec0: 6074 7261 6666 6963 5f73 6f75 7263 6560  `traffic_source`
+00010ed0: 6029 2062 6173 6564 206f 6e0a 2020 2020  `) based on.    
+00010ee0: 2020 2020 2020 2020 696d 7072 6573 7369          impressi
+00010ef0: 6f6e 732e 2031 2069 7320 7468 6520 6869  ons. 1 is the hi
+00010f00: 6768 6573 742e 0a0a 2020 2020 2020 2020  ghest...        
+00010f10: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
+00010f20: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
+00010f30: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
+00010f40: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00010f50: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00010f60: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00010f70: 2060 605f 7261 6e6b 6060 2e0a 2020 2020   ``_rank``..    
+00010f80: 2020 2020 6164 735f 6f72 6761 6e69 635f      ads_organic_
+00010f90: 7261 7469 6f20 2866 6c6f 6174 293a 0a20  ratio (float):. 
+00010fa0: 2020 2020 2020 2020 2020 205b 4164 7320             [Ads 
+00010fb0: 2f20 6f72 6761 6e69 6320 7261 7469 6f5d  / organic ratio]
+00010fc0: 0a20 2020 2020 2020 2020 2020 2028 6874  .            (ht
+00010fd0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+00010fe0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+00010ff0: 7473 2f61 6e73 7765 722f 3131 3336 3634  ts/answer/113664
+00011000: 3432 237a 6970 7079 3d25 3243 6164 732d  42#zippy=%2Cads-
+00011010: 6672 6565 2d72 6174 696f 290a 2020 2020  free-ratio).    
+00011020: 2020 2020 2020 2020 7368 6f77 7320 686f          shows ho
+00011030: 7720 6f66 7465 6e20 7468 6520 646f 6d61  w often the doma
+00011040: 696e 2072 6563 6569 7665 7320 696d 7072  in receives impr
+00011050: 6573 7369 6f6e 7320 6672 6f6d 0a20 2020  essions from.   
+00011060: 2020 2020 2020 2020 2053 686f 7070 696e           Shoppin
+00011070: 6720 6164 7320 636f 6d70 6172 6564 2074  g ads compared t
+00011080: 6f20 6f72 6761 6e69 6320 7472 6166 6669  o organic traffi
+00011090: 632e 2054 6865 206e 756d 6265 7220 6973  c. The number is
+000110a0: 0a20 2020 2020 2020 2020 2020 2072 6f75  .            rou
+000110b0: 6e64 6564 2061 6e64 2062 7563 6b65 7465  nded and buckete
+000110c0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
+000110d0: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+000110e0: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+000110f0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+00011100: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00011110: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00011120: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00011130: 6164 735f 6f72 6761 6e69 635f 7261 7469  ads_organic_rati
+00011140: 6f60 602e 0a20 2020 2020 2020 2070 6167  o``..        pag
+00011150: 655f 6f76 6572 6c61 705f 7261 7465 2028  e_overlap_rate (
+00011160: 666c 6f61 7429 3a0a 2020 2020 2020 2020  float):.        
+00011170: 2020 2020 5b50 6167 6520 6f76 6572 6c61      [Page overla
+00011180: 7020 7261 7465 5d0a 2020 2020 2020 2020  p rate].        
+00011190: 2020 2020 2868 7474 7073 3a2f 2f73 7570      (https://sup
+000111a0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+000111b0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+000111c0: 2f31 3133 3636 3434 3223 7a69 7070 793d  /11366442#zippy=
+000111d0: 2532 4370 6167 652d 6f76 6572 6c61 702d  %2Cpage-overlap-
+000111e0: 7261 7465 290a 2020 2020 2020 2020 2020  rate).          
+000111f0: 2020 7368 6f77 7320 686f 7720 6672 6571    shows how freq
+00011200: 7565 6e74 6c79 2063 6f6d 7065 7469 6e67  uently competing
+00011210: 2072 6574 6169 6c65 7273 e280 9920 6f66   retailers... of
+00011220: 6665 7273 2061 7265 2073 686f 776e 0a20  fers are shown. 
+00011230: 2020 2020 2020 2020 2020 2074 6f67 6574             toget
+00011240: 6865 7220 7769 7468 2079 6f75 7220 6f66  her with your of
+00011250: 6665 7273 206f 6e20 7468 6520 7361 6d65  fers on the same
+00011260: 2070 6167 652e 0a0a 2020 2020 2020 2020   page...        
+00011270: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
+00011280: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
+00011290: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
+000112a0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000112b0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000112c0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000112d0: 2060 605f 7061 6765 5f6f 7665 726c 6170   ``_page_overlap
+000112e0: 5f72 6174 6560 602e 0a20 2020 2020 2020  _rate``..       
+000112f0: 2068 6967 6865 725f 706f 7369 7469 6f6e   higher_position
+00011300: 5f72 6174 6520 2866 6c6f 6174 293a 0a20  _rate (float):. 
+00011310: 2020 2020 2020 2020 2020 205b 4869 6768             [High
+00011320: 6572 2070 6f73 6974 696f 6e20 7261 7465  er position rate
+00011330: 5d0a 2020 2020 2020 2020 2020 2020 2868  ].            (h
+00011340: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+00011350: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+00011360: 6e74 732f 616e 7377 6572 2f31 3133 3636  nts/answer/11366
+00011370: 3434 3223 7a69 7070 793d 2532 4368 6967  442#zippy=%2Chig
+00011380: 6865 722d 706f 7369 7469 6f6e 2d72 6174  her-position-rat
+00011390: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+000113a0: 686f 7773 2068 6f77 206f 6674 656e 2061  hows how often a
+000113b0: 2063 6f6d 7065 7469 746f 72e2 8099 7320   competitor...s 
+000113c0: 6f66 6665 7220 676f 7420 706c 6163 6564  offer got placed
+000113d0: 2069 6e20 6120 6869 6768 6572 0a20 2020   in a higher.   
+000113e0: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
+000113f0: 6e20 6f6e 2074 6865 2070 6167 6520 7468  n on the page th
+00011400: 616e 2079 6f75 7220 6f66 6665 722e 0a0a  an your offer...
+00011410: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
+00011420: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
+00011430: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
+00011440: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+00011450: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00011460: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00011470: 606f 6e65 6f66 605f 2060 605f 6869 6768  `oneof`_ ``_high
+00011480: 6572 5f70 6f73 6974 696f 6e5f 7261 7465  er_position_rate
+00011490: 6060 2e0a 2020 2020 2020 2020 7265 6c61  ``..        rela
+000114a0: 7469 7665 5f76 6973 6962 696c 6974 7920  tive_visibility 
+000114b0: 2866 6c6f 6174 293a 0a20 2020 2020 2020  (float):.       
+000114c0: 2020 2020 205b 5265 6c61 7469 7665 2076       [Relative v
+000114d0: 6973 6962 696c 6974 795d 0a20 2020 2020  isibility].     
+000114e0: 2020 2020 2020 2028 6874 7470 733a 2f2f         (https://
+000114f0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+00011500: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+00011510: 7765 722f 3131 3336 3634 3432 237a 6970  wer/11366442#zip
+00011520: 7079 3d25 3243 7265 6c61 7469 7665 2d76  py=%2Crelative-v
+00011530: 6973 6962 696c 6974 7929 0a20 2020 2020  isibility).     
+00011540: 2020 2020 2020 2073 686f 7773 2068 6f77         shows how
+00011550: 206f 6674 656e 2079 6f75 7220 636f 6d70   often your comp
+00011560: 6574 6974 6f72 73e2 8099 206f 6666 6572  etitors... offer
+00011570: 7320 6172 6520 7368 6f77 6e20 636f 6d70  s are shown comp
+00011580: 6172 6564 0a20 2020 2020 2020 2020 2020  ared.           
+00011590: 2074 6f20 796f 7572 206f 6666 6572 732e   to your offers.
+000115a0: 2049 6e20 6f74 6865 7220 776f 7264 732c   In other words,
+000115b0: 2074 6869 7320 6973 2074 6865 206e 756d   this is the num
+000115c0: 6265 7220 6f66 0a20 2020 2020 2020 2020  ber of.         
+000115d0: 2020 2064 6973 706c 6179 6564 2069 6d70     displayed imp
+000115e0: 7265 7373 696f 6e73 206f 6620 6120 636f  ressions of a co
+000115f0: 6d70 6574 6974 6f72 2072 6574 6169 6c65  mpetitor retaile
+00011600: 7220 6469 7669 6465 6420 6279 0a20 2020  r divided by.   
+00011610: 2020 2020 2020 2020 2074 6865 206e 756d           the num
+00011620: 6265 7220 6f66 2079 6f75 7220 6469 7370  ber of your disp
+00011630: 6c61 7965 6420 696d 7072 6573 7369 6f6e  layed impression
+00011640: 7320 6475 7269 6e67 2061 2073 656c 6563  s during a selec
+00011650: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00011660: 7469 6d65 2072 616e 6765 2066 6f72 2061  time range for a
+00011670: 2073 656c 6563 7465 6420 7072 6f64 7563   selected produc
+00011680: 7420 6361 7465 676f 7279 2061 6e64 2063  t category and c
+00011690: 6f75 6e74 7279 2e0a 0a20 2020 2020 2020  ountry...       
+000116a0: 2020 2020 2043 616e 6e6f 7420 6265 2066       Cannot be f
+000116b0: 696c 7465 7265 6420 6f6e 2069 6e20 7468  iltered on in th
+000116c0: 6520 2757 4845 5245 2720 636c 6175 7365  e 'WHERE' clause
+000116d0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+000116e0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+000116f0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+00011700: 5f20 6060 5f72 656c 6174 6976 655f 7669  _ ``_relative_vi
+00011710: 7369 6269 6c69 7479 6060 2e0a 2020 2020  sibility``..    
+00011720: 2222 220a 0a20 2020 2064 6174 653a 2064  """..    date: d
+00011730: 6174 655f 7062 322e 4461 7465 203d 2070  ate_pb2.Date = p
+00011740: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00011750: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+00011760: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+00011770: 723d 312c 0a20 2020 2020 2020 206d 6573  r=1,.        mes
+00011780: 7361 6765 3d64 6174 655f 7062 322e 4461  sage=date_pb2.Da
+00011790: 7465 2c0a 2020 2020 290a 2020 2020 646f  te,.    ).    do
+000117a0: 6d61 696e 3a20 7374 7220 3d20 7072 6f74  main: str = prot
+000117b0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000117c0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+000117d0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+000117e0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+000117f0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00011800: 2020 6973 5f79 6f75 725f 646f 6d61 696e    is_your_domain
+00011810: 3a20 626f 6f6c 203d 2070 726f 746f 2e46  : bool = proto.F
+00011820: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00011830: 6f74 6f2e 424f 4f4c 2c0a 2020 2020 2020  oto.BOOL,.      
+00011840: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
+00011850: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00011860: 652c 0a20 2020 2029 0a20 2020 2072 6570  e,.    ).    rep
+00011870: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+00011880: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+00011890: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000118a0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000118b0: 2020 206e 756d 6265 723d 342c 0a20 2020     number=4,.   
+000118c0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+000118d0: 7565 2c0a 2020 2020 290a 2020 2020 7265  ue,.    ).    re
+000118e0: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
+000118f0: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
+00011900: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00011910: 746f 2e49 4e54 3634 2c0a 2020 2020 2020  to.INT64,.      
+00011920: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
+00011930: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00011940: 652c 0a20 2020 2029 0a20 2020 2074 7261  e,.    ).    tra
+00011950: 6666 6963 5f73 6f75 7263 653a 2022 5472  ffic_source: "Tr
+00011960: 6166 6669 6353 6f75 7263 652e 5472 6166  afficSource.Traf
+00011970: 6669 6353 6f75 7263 6545 6e75 6d22 203d  ficSourceEnum" =
+00011980: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00011990: 2020 2020 2020 7072 6f74 6f2e 454e 554d        proto.ENUM
+000119a0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000119b0: 3d36 2c0a 2020 2020 2020 2020 6f70 7469  =6,.        opti
+000119c0: 6f6e 616c 3d54 7275 652c 0a20 2020 2020  onal=True,.     
+000119d0: 2020 2065 6e75 6d3d 2254 7261 6666 6963     enum="Traffic
+000119e0: 536f 7572 6365 2e54 7261 6666 6963 536f  Source.TrafficSo
+000119f0: 7572 6365 456e 756d 222c 0a20 2020 2029  urceEnum",.    )
+00011a00: 0a20 2020 2072 616e 6b3a 2069 6e74 203d  .    rank: int =
+00011a10: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00011a20: 2020 2020 2020 7072 6f74 6f2e 494e 5436        proto.INT6
+00011a30: 342c 0a20 2020 2020 2020 206e 756d 6265  4,.        numbe
+00011a40: 723d 372c 0a20 2020 2020 2020 206f 7074  r=7,.        opt
+00011a50: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00011a60: 290a 2020 2020 6164 735f 6f72 6761 6e69  ).    ads_organi
+00011a70: 635f 7261 7469 6f3a 2066 6c6f 6174 203d  c_ratio: float =
+00011a80: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00011a90: 2020 2020 2020 7072 6f74 6f2e 444f 5542        proto.DOUB
+00011aa0: 4c45 2c0a 2020 2020 2020 2020 6e75 6d62  LE,.        numb
+00011ab0: 6572 3d38 2c0a 2020 2020 2020 2020 6f70  er=8,.        op
+00011ac0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00011ad0: 2029 0a20 2020 2070 6167 655f 6f76 6572   ).    page_over
+00011ae0: 6c61 705f 7261 7465 3a20 666c 6f61 7420  lap_rate: float 
+00011af0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00011b00: 2020 2020 2020 2070 726f 746f 2e44 4f55         proto.DOU
+00011b10: 424c 452c 0a20 2020 2020 2020 206e 756d  BLE,.        num
+00011b20: 6265 723d 392c 0a20 2020 2020 2020 206f  ber=9,.        o
+00011b30: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00011b40: 2020 290a 2020 2020 6869 6768 6572 5f70    ).    higher_p
+00011b50: 6f73 6974 696f 6e5f 7261 7465 3a20 666c  osition_rate: fl
+00011b60: 6f61 7420 3d20 7072 6f74 6f2e 4669 656c  oat = proto.Fiel
+00011b70: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00011b80: 2e44 4f55 424c 452c 0a20 2020 2020 2020  .DOUBLE,.       
+00011b90: 206e 756d 6265 723d 3130 2c0a 2020 2020   number=10,.    
+00011ba0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00011bb0: 652c 0a20 2020 2029 0a20 2020 2072 656c  e,.    ).    rel
+00011bc0: 6174 6976 655f 7669 7369 6269 6c69 7479  ative_visibility
+00011bd0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
+00011be0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00011bf0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
+00011c00: 2020 2020 206e 756d 6265 723d 3131 2c0a       number=11,.
+00011c10: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00011c20: 3d54 7275 652c 0a20 2020 2029 0a0a 0a63  =True,.    )...c
+00011c30: 6c61 7373 2043 6f6d 7065 7469 7469 7665  lass Competitive
+00011c40: 5669 7369 6269 6c69 7479 546f 704d 6572  VisibilityTopMer
+00011c50: 6368 616e 7456 6965 7728 7072 6f74 6f2e  chantView(proto.
+00011c60: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+00011c70: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
+00011c80: 6c65 2066 6f72 2071 7565 7279 2069 6e0a  le for query in.
+00011c90: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
+00011ca0: 655f 7669 7369 6269 6c69 7479 5f74 6f70  e_visibility_top
+00011cb0: 5f6d 6572 6368 616e 745f 7669 6577 6060  _merchant_view``
+00011cc0: 2074 6162 6c65 2e0a 0a20 2020 2060 436f   table...    `Co
+00011cd0: 6d70 6574 6974 6976 650a 2020 2020 7669  mpetitive.    vi
+00011ce0: 7369 6269 6c69 7479 203c 6874 7470 733a  sibility <https:
+00011cf0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+00011d00: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+00011d10: 6e73 7765 722f 3131 3336 3634 3432 3e60  nswer/11366442>`
+00011d20: 5f5f 0a20 2020 2072 6570 6f72 7420 7769  __.    report wi
+00011d30: 7468 2062 7573 696e 6573 7320 7769 7468  th business with
+00011d40: 2068 6967 6865 7374 2076 6973 6962 696c   highest visibil
+00011d50: 6974 792e 0a0a 2020 2020 5661 6c75 6573  ity...    Values
+00011d60: 2061 7265 206f 6e6c 7920 7365 7420 666f   are only set fo
+00011d70: 7220 6669 656c 6473 2072 6571 7565 7374  r fields request
+00011d80: 6564 2065 7870 6c69 6369 746c 7920 696e  ed explicitly in
+00011d90: 2074 6865 2072 6571 7565 7374 2773 0a20   the request's. 
+00011da0: 2020 2073 6561 7263 6820 7175 6572 792e     search query.
+00011db0: 0a0a 0a20 2020 202e 2e20 5f6f 6e65 6f66  ...    .. _oneof
+00011dc0: 3a20 6874 7470 733a 2f2f 7072 6f74 6f2d  : https://proto-
+00011dd0: 706c 7573 2d70 7974 686f 6e2e 7265 6164  plus-python.read
+00011de0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00011df0: 6162 6c65 2f66 6965 6c64 732e 6874 6d6c  able/fields.html
+00011e00: 236f 6e65 6f66 732d 6d75 7475 616c 6c79  #oneofs-mutually
+00011e10: 2d65 7863 6c75 7369 7665 2d66 6965 6c64  -exclusive-field
+00011e20: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
+00011e30: 733a 0a20 2020 2020 2020 2064 6174 6520  s:.        date 
+00011e40: 2867 6f6f 676c 652e 7479 7065 2e64 6174  (google.type.dat
+00011e50: 655f 7062 322e 4461 7465 293a 0a20 2020  e_pb2.Date):.   
+00011e60: 2020 2020 2020 2020 2044 6174 6520 6f66           Date of
+00011e70: 2074 6869 7320 726f 772e 0a0a 2020 2020   this row...    
+00011e80: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+00011e90: 6520 7365 6c65 6374 6564 2069 6e20 7468  e selected in th
+00011ea0: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
+00011eb0: 7573 652e 2041 2063 6f6e 6469 7469 6f6e  use. A condition
+00011ec0: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+00011ed0: 6060 6461 7465 6060 2069 7320 7265 7175  ``date`` is requ
+00011ee0: 6972 6564 2069 6e20 7468 6520 6060 5748  ired in the ``WH
+00011ef0: 4552 4560 6020 636c 6175 7365 2e0a 2020  ERE`` clause..  
+00011f00: 2020 2020 2020 646f 6d61 696e 2028 7374        domain (st
+00011f10: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00011f20: 446f 6d61 696e 206f 6620 796f 7572 2063  Domain of your c
+00011f30: 6f6d 7065 7469 746f 7220 6f72 2079 6f75  ompetitor or you
+00011f40: 7220 646f 6d61 696e 2c20 6966 0a20 2020  r domain, if.   
+00011f50: 2020 2020 2020 2020 2027 6973 5f79 6f75           'is_you
+00011f60: 725f 646f 6d61 696e 2720 6973 2074 7275  r_domain' is tru
+00011f70: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00011f80: 5265 7175 6972 6564 2069 6e20 7468 6520  Required in the 
+00011f90: 6060 5345 4c45 4354 6060 2063 6c61 7573  ``SELECT`` claus
+00011fa0: 652e 2043 616e 6e6f 7420 6265 2066 696c  e. Cannot be fil
+00011fb0: 7465 7265 6420 6f6e 2069 6e0a 2020 2020  tered on in.    
+00011fc0: 2020 2020 2020 2020 7468 6520 2757 4845          the 'WHE
+00011fd0: 5245 2720 636c 6175 7365 2e0a 0a20 2020  RE' clause...   
+00011fe0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00011ff0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+00012000: 6f66 2060 6f6e 656f 6660 5f20 6060 5f64  of `oneof`_ ``_d
+00012010: 6f6d 6169 6e60 602e 0a20 2020 2020 2020  omain``..       
+00012020: 2069 735f 796f 7572 5f64 6f6d 6169 6e20   is_your_domain 
+00012030: 2862 6f6f 6c29 3a0a 2020 2020 2020 2020  (bool):.        
+00012040: 2020 2020 5472 7565 2069 6620 7468 6973      True if this
+00012050: 2072 6f77 2063 6f6e 7461 696e 7320 6461   row contains da
+00012060: 7461 2066 6f72 2079 6f75 720a 2020 2020  ta for your.    
+00012070: 2020 2020 2020 2020 646f 6d61 696e 2e0a          domain..
+00012080: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
+00012090: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
+000120a0: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
+000120b0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+000120c0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+000120d0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+000120e0: 606f 6e65 6f66 605f 2060 605f 6973 5f79  `oneof`_ ``_is_y
+000120f0: 6f75 725f 646f 6d61 696e 6060 2e0a 2020  our_domain``..  
+00012100: 2020 2020 2020 7265 706f 7274 5f63 6f75        report_cou
+00012110: 6e74 7279 5f63 6f64 6520 2873 7472 293a  ntry_code (str):
+00012120: 0a20 2020 2020 2020 2020 2020 2043 6f75  .            Cou
+00012130: 6e74 7279 2077 6865 7265 2069 6d70 7265  ntry where impre
+00012140: 7373 696f 6e73 2061 7070 6561 7265 642e  ssions appeared.
+00012150: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00012160: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+00012170: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
+00012180: 2041 2063 6f6e 6469 7469 6f6e 206f 6e0a   A condition on.
+00012190: 2020 2020 2020 2020 2020 2020 6060 7265              ``re
+000121a0: 706f 7274 5f63 6f75 6e74 7279 5f63 6f64  port_country_cod
+000121b0: 6560 6020 6973 2072 6571 7569 7265 6420  e`` is required 
+000121c0: 696e 2074 6865 2060 6057 4845 5245 6060  in the ``WHERE``
+000121d0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+000121e0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+000121f0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00012200: 606f 6e65 6f66 605f 2060 605f 7265 706f  `oneof`_ ``_repo
+00012210: 7274 5f63 6f75 6e74 7279 5f63 6f64 6560  rt_country_code`
+00012220: 602e 0a20 2020 2020 2020 2072 6570 6f72  `..        repor
+00012230: 745f 6361 7465 676f 7279 5f69 6420 2869  t_category_id (i
+00012240: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00012250: 2047 6f6f 676c 6520 7072 6f64 7563 7420   Google product 
+00012260: 6361 7465 676f 7279 2049 4420 746f 2063  category ID to c
+00012270: 616c 6375 6c61 7465 2074 6865 2072 6570  alculate the rep
+00012280: 6f72 7420 666f 722c 0a20 2020 2020 2020  ort for,.       
+00012290: 2020 2020 2072 6570 7265 7365 6e74 6564       represented
+000122a0: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
+000122b0: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+000122c0: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+000122d0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+000122e0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+000122f0: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
+00012300: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+00012310: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
+00012320: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
+00012330: 7573 652e 2041 2063 6f6e 6469 7469 6f6e  use. A condition
+00012340: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+00012350: 6060 7265 706f 7274 5f63 6174 6567 6f72  ``report_categor
+00012360: 795f 6964 6060 2069 7320 7265 7175 6972  y_id`` is requir
+00012370: 6564 2069 6e20 7468 6520 6060 5748 4552  ed in the ``WHER
+00012380: 4560 6020 636c 6175 7365 2e0a 0a20 2020  E`` clause...   
+00012390: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+000123a0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+000123b0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f72  of `oneof`_ ``_r
+000123c0: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
+000123d0: 6460 602e 0a20 2020 2020 2020 2074 7261  d``..        tra
+000123e0: 6666 6963 5f73 6f75 7263 6520 2867 6f6f  ffic_source (goo
+000123f0: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
+00012400: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
+00012410: 6265 7461 2e74 7970 6573 2e54 7261 6666  beta.types.Traff
+00012420: 6963 536f 7572 6365 2e54 7261 6666 6963  icSource.Traffic
+00012430: 536f 7572 6365 456e 756d 293a 0a20 2020  SourceEnum):.   
+00012440: 2020 2020 2020 2020 2054 7261 6666 6963           Traffic
+00012450: 2073 6f75 7263 6520 6f66 2069 6d70 7265   source of impre
+00012460: 7373 696f 6e73 2e0a 0a20 2020 2020 2020  ssions...       
+00012470: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
+00012480: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
+00012490: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
+000124a0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+000124b0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+000124c0: 6f6e 656f 6660 5f20 6060 5f74 7261 6666  oneof`_ ``_traff
+000124d0: 6963 5f73 6f75 7263 6560 602e 0a20 2020  ic_source``..   
+000124e0: 2020 2020 2072 616e 6b20 2869 6e74 293a       rank (int):
+000124f0: 0a20 2020 2020 2020 2020 2020 2050 6f73  .            Pos
+00012500: 6974 696f 6e20 6f66 2074 6865 2064 6f6d  ition of the dom
+00012510: 6169 6e20 696e 2074 6865 2074 6f70 206d  ain in the top m
+00012520: 6572 6368 616e 7473 2072 616e 6b69 6e67  erchants ranking
+00012530: 2066 6f72 2074 6865 0a20 2020 2020 2020   for the.       
+00012540: 2020 2020 2073 656c 6563 7465 6420 6b65       selected ke
+00012550: 7973 2028 6060 6461 7465 6060 2c20 6060  ys (``date``, ``
+00012560: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
+00012570: 6964 6060 2c0a 2020 2020 2020 2020 2020  id``,.          
+00012580: 2020 6060 7265 706f 7274 5f63 6f75 6e74    ``report_count
+00012590: 7279 5f63 6f64 6560 602c 2060 6074 7261  ry_code``, ``tra
+000125a0: 6666 6963 5f73 6f75 7263 6560 6029 2062  ffic_source``) b
+000125b0: 6173 6564 206f 6e0a 2020 2020 2020 2020  ased on.        
+000125c0: 2020 2020 696d 7072 6573 7369 6f6e 732e      impressions.
+000125d0: 2031 2069 7320 7468 6520 6869 6768 6573   1 is the highes
+000125e0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+000125f0: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+00012600: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+00012610: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+00012620: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00012630: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00012640: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00012650: 7261 6e6b 6060 2e0a 2020 2020 2020 2020  rank``..        
+00012660: 6164 735f 6f72 6761 6e69 635f 7261 7469  ads_organic_rati
+00012670: 6f20 2866 6c6f 6174 293a 0a20 2020 2020  o (float):.     
+00012680: 2020 2020 2020 205b 4164 7320 2f20 6f72         [Ads / or
+00012690: 6761 6e69 6320 7261 7469 6f5d 0a20 2020  ganic ratio].   
+000126a0: 2020 2020 2020 2020 2028 6874 7470 733a           (https:
+000126b0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+000126c0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+000126d0: 6e73 7765 722f 3131 3336 3634 3432 237a  nswer/11366442#z
+000126e0: 6970 7079 3d25 3243 6164 732d 6672 6565  ippy=%2Cads-free
+000126f0: 2d72 6174 696f 290a 2020 2020 2020 2020  -ratio).        
+00012700: 2020 2020 7368 6f77 7320 686f 7720 6f66      shows how of
+00012710: 7465 6e20 7468 6520 646f 6d61 696e 2072  ten the domain r
+00012720: 6563 6569 7665 7320 696d 7072 6573 7369  eceives impressi
+00012730: 6f6e 7320 6672 6f6d 0a20 2020 2020 2020  ons from.       
+00012740: 2020 2020 2053 686f 7070 696e 6720 6164       Shopping ad
+00012750: 7320 636f 6d70 6172 6564 2074 6f20 6f72  s compared to or
+00012760: 6761 6e69 6320 7472 6166 6669 632e 2054  ganic traffic. T
+00012770: 6865 206e 756d 6265 7220 6973 0a20 2020  he number is.   
+00012780: 2020 2020 2020 2020 2072 6f75 6e64 6564           rounded
+00012790: 2061 6e64 2062 7563 6b65 7465 642e 0a0a   and bucketed...
+000127a0: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
+000127b0: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
+000127c0: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
+000127d0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+000127e0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+000127f0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00012800: 606f 6e65 6f66 605f 2060 605f 6164 735f  `oneof`_ ``_ads_
+00012810: 6f72 6761 6e69 635f 7261 7469 6f60 602e  organic_ratio``.
+00012820: 0a20 2020 2020 2020 2070 6167 655f 6f76  .        page_ov
+00012830: 6572 6c61 705f 7261 7465 2028 666c 6f61  erlap_rate (floa
+00012840: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00012850: 5b50 6167 6520 6f76 6572 6c61 7020 7261  [Page overlap ra
+00012860: 7465 5d0a 2020 2020 2020 2020 2020 2020  te].            
+00012870: 2868 7474 7073 3a2f 2f73 7570 706f 7274  (https://support
+00012880: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
+00012890: 6861 6e74 732f 616e 7377 6572 2f31 3133  hants/answer/113
+000128a0: 3636 3434 3223 7a69 7070 793d 2532 4370  66442#zippy=%2Cp
+000128b0: 6167 652d 6f76 6572 6c61 702d 7261 7465  age-overlap-rate
+000128c0: 290a 2020 2020 2020 2020 2020 2020 7368  ).            sh
+000128d0: 6f77 7320 686f 7720 6672 6571 7565 6e74  ows how frequent
+000128e0: 6c79 2063 6f6d 7065 7469 6e67 2072 6574  ly competing ret
+000128f0: 6169 6c65 7273 e280 9920 6f66 6665 7273  ailers... offers
+00012900: 2061 7265 2073 686f 776e 0a20 2020 2020   are shown.     
+00012910: 2020 2020 2020 2074 6f67 6574 6865 7220         together 
+00012920: 7769 7468 2079 6f75 7220 6f66 6665 7273  with your offers
+00012930: 206f 6e20 7468 6520 7361 6d65 2070 6167   on the same pag
+00012940: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00012950: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+00012960: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+00012970: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+00012980: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00012990: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000129a0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+000129b0: 7061 6765 5f6f 7665 726c 6170 5f72 6174  page_overlap_rat
+000129c0: 6560 602e 0a20 2020 2020 2020 2068 6967  e``..        hig
+000129d0: 6865 725f 706f 7369 7469 6f6e 5f72 6174  her_position_rat
+000129e0: 6520 2866 6c6f 6174 293a 0a20 2020 2020  e (float):.     
+000129f0: 2020 2020 2020 205b 4869 6768 6572 2070         [Higher p
+00012a00: 6f73 6974 696f 6e20 7261 7465 5d0a 2020  osition rate].  
+00012a10: 2020 2020 2020 2020 2020 2868 7474 7073            (https
+00012a20: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+00012a30: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+00012a40: 616e 7377 6572 2f31 3133 3636 3434 3223  answer/11366442#
+00012a50: 7a69 7070 793d 2532 4368 6967 6865 722d  zippy=%2Chigher-
+00012a60: 706f 7369 7469 6f6e 2d72 6174 6529 0a20  position-rate). 
+00012a70: 2020 2020 2020 2020 2020 2073 686f 7773             shows
+00012a80: 2068 6f77 206f 6674 656e 2061 2063 6f6d   how often a com
+00012a90: 7065 7469 746f 72e2 8099 7320 6f66 6665  petitor...s offe
+00012aa0: 7220 676f 7420 706c 6163 6564 2069 6e20  r got placed in 
+00012ab0: 6120 6869 6768 6572 0a20 2020 2020 2020  a higher.       
+00012ac0: 2020 2020 2070 6f73 6974 696f 6e20 6f6e       position on
+00012ad0: 2074 6865 2070 6167 6520 7468 616e 2079   the page than y
+00012ae0: 6f75 7220 6f66 6665 722e 0a0a 2020 2020  our offer...    
+00012af0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+00012b00: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+00012b10: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+00012b20: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+00012b30: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00012b40: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00012b50: 6f66 605f 2060 605f 6869 6768 6572 5f70  of`_ ``_higher_p
+00012b60: 6f73 6974 696f 6e5f 7261 7465 6060 2e0a  osition_rate``..
+00012b70: 2020 2020 2222 220a 0a20 2020 2064 6174      """..    dat
+00012b80: 653a 2064 6174 655f 7062 322e 4461 7465  e: date_pb2.Date
+00012b90: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00012ba0: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00012bb0: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00012bc0: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
+00012bd0: 206d 6573 7361 6765 3d64 6174 655f 7062   message=date_pb
+00012be0: 322e 4461 7465 2c0a 2020 2020 290a 2020  2.Date,.    ).  
+00012bf0: 2020 646f 6d61 696e 3a20 7374 7220 3d20    domain: str = 
+00012c00: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00012c10: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00012c20: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00012c30: 723d 322c 0a20 2020 2020 2020 206f 7074  r=2,.        opt
+00012c40: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00012c50: 290a 2020 2020 6973 5f79 6f75 725f 646f  ).    is_your_do
+00012c60: 6d61 696e 3a20 626f 6f6c 203d 2070 726f  main: bool = pro
+00012c70: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00012c80: 2020 7072 6f74 6f2e 424f 4f4c 2c0a 2020    proto.BOOL,.  
+00012c90: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
+00012ca0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00012cb0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00012cc0: 2072 6570 6f72 745f 636f 756e 7472 795f   report_country_
+00012cd0: 636f 6465 3a20 7374 7220 3d20 7072 6f74  code: str = prot
+00012ce0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00012cf0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00012d00: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
+00012d10: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00012d20: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00012d30: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
+00012d40: 795f 6964 3a20 696e 7420 3d20 7072 6f74  y_id: int = prot
+00012d50: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00012d60: 2070 726f 746f 2e49 4e54 3634 2c0a 2020   proto.INT64,.  
+00012d70: 2020 2020 2020 6e75 6d62 6572 3d35 2c0a        number=5,.
+00012d80: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00012d90: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00012da0: 2074 7261 6666 6963 5f73 6f75 7263 653a   traffic_source:
+00012db0: 2022 5472 6166 6669 6353 6f75 7263 652e   "TrafficSource.
+00012dc0: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
+00012dd0: 6d22 203d 2070 726f 746f 2e46 6965 6c64  m" = proto.Field
+00012de0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00012df0: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+00012e00: 6d62 6572 3d36 2c0a 2020 2020 2020 2020  mber=6,.        
+00012e10: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00012e20: 2020 2020 2020 2065 6e75 6d3d 2254 7261         enum="Tra
+00012e30: 6666 6963 536f 7572 6365 2e54 7261 6666  fficSource.Traff
+00012e40: 6963 536f 7572 6365 456e 756d 222c 0a20  icSourceEnum",. 
+00012e50: 2020 2029 0a20 2020 2072 616e 6b3a 2069     ).    rank: i
+00012e60: 6e74 203d 2070 726f 746f 2e46 6965 6c64  nt = proto.Field
+00012e70: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00012e80: 494e 5436 342c 0a20 2020 2020 2020 206e  INT64,.        n
+00012e90: 756d 6265 723d 372c 0a20 2020 2020 2020  umber=7,.       
+00012ea0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+00012eb0: 2020 2020 290a 2020 2020 6164 735f 6f72      ).    ads_or
+00012ec0: 6761 6e69 635f 7261 7469 6f3a 2066 6c6f  ganic_ratio: flo
+00012ed0: 6174 203d 2070 726f 746f 2e46 6965 6c64  at = proto.Field
+00012ee0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00012ef0: 444f 5542 4c45 2c0a 2020 2020 2020 2020  DOUBLE,.        
+00012f00: 6e75 6d62 6572 3d38 2c0a 2020 2020 2020  number=8,.      
+00012f10: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00012f20: 0a20 2020 2029 0a20 2020 2070 6167 655f  .    ).    page_
+00012f30: 6f76 6572 6c61 705f 7261 7465 3a20 666c  overlap_rate: fl
+00012f40: 6f61 7420 3d20 7072 6f74 6f2e 4669 656c  oat = proto.Fiel
+00012f50: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00012f60: 2e44 4f55 424c 452c 0a20 2020 2020 2020  .DOUBLE,.       
+00012f70: 206e 756d 6265 723d 392c 0a20 2020 2020   number=9,.     
+00012f80: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00012f90: 2c0a 2020 2020 290a 2020 2020 6869 6768  ,.    ).    high
+00012fa0: 6572 5f70 6f73 6974 696f 6e5f 7261 7465  er_position_rate
+00012fb0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
+00012fc0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00012fd0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
+00012fe0: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
+00012ff0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00013000: 3d54 7275 652c 0a20 2020 2029 0a0a 0a63  =True,.    )...c
+00013010: 6c61 7373 2043 6f6d 7065 7469 7469 7665  lass Competitive
+00013020: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
+00013030: 6172 6b56 6965 7728 7072 6f74 6f2e 4d65  arkView(proto.Me
+00013040: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
+00013050: 4669 656c 6473 2061 7661 696c 6162 6c65  Fields available
+00013060: 2066 6f72 2071 7565 7279 2069 6e0a 2020   for query in.  
+00013070: 2020 6060 636f 6d70 6574 6974 6976 655f    ``competitive_
+00013080: 7669 7369 6269 6c69 7479 5f62 656e 6368  visibility_bench
+00013090: 6d61 726b 5f76 6965 7760 6020 7461 626c  mark_view`` tabl
+000130a0: 652e 0a0a 2020 2020 6043 6f6d 7065 7469  e...    `Competi
+000130b0: 7469 7665 0a20 2020 2076 6973 6962 696c  tive.    visibil
+000130c0: 6974 7920 3c68 7474 7073 3a2f 2f73 7570  ity <https://sup
+000130d0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+000130e0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+000130f0: 2f31 3133 3636 3434 323e 605f 5f0a 2020  /11366442>`__.  
+00013100: 2020 7265 706f 7274 2077 6974 6820 7468    report with th
+00013110: 6520 6361 7465 676f 7279 2062 656e 6368  e category bench
+00013120: 6d61 726b 2e0a 0a20 2020 2056 616c 7565  mark...    Value
+00013130: 7320 6172 6520 6f6e 6c79 2073 6574 2066  s are only set f
+00013140: 6f72 2066 6965 6c64 7320 7265 7175 6573  or fields reques
+00013150: 7465 6420 6578 706c 6963 6974 6c79 2069  ted explicitly i
+00013160: 6e20 7468 6520 7265 7175 6573 7427 730a  n the request's.
+00013170: 2020 2020 7365 6172 6368 2071 7565 7279      search query
+00013180: 2e0a 0a0a 2020 2020 2e2e 205f 6f6e 656f  ....    .. _oneo
+00013190: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
+000131a0: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
+000131b0: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+000131c0: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
+000131d0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
+000131e0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
+000131f0: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
+00013200: 6573 3a0a 2020 2020 2020 2020 6461 7465  es:.        date
+00013210: 2028 676f 6f67 6c65 2e74 7970 652e 6461   (google.type.da
+00013220: 7465 5f70 6232 2e44 6174 6529 3a0a 2020  te_pb2.Date):.  
+00013230: 2020 2020 2020 2020 2020 4461 7465 206f            Date o
+00013240: 6620 7468 6973 2072 6f77 2e0a 0a20 2020  f this row...   
+00013250: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+00013260: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+00013270: 5460 6020 636c 6175 7365 2e20 4120 636f  T`` clause. A co
+00013280: 6e64 6974 696f 6e20 6f6e 2060 6064 6174  ndition on ``dat
+00013290: 6560 600a 2020 2020 2020 2020 2020 2020  e``.            
+000132a0: 6973 2072 6571 7569 7265 6420 696e 2074  is required in t
+000132b0: 6865 2060 6057 4845 5245 6060 2063 6c61  he ``WHERE`` cla
+000132c0: 7573 652e 0a20 2020 2020 2020 2072 6570  use..        rep
+000132d0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+000132e0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+000132f0: 2020 2020 436f 756e 7472 7920 7768 6572      Country wher
+00013300: 6520 696d 7072 6573 7369 6f6e 7320 6170  e impressions ap
+00013310: 7065 6172 6564 2e0a 0a20 2020 2020 2020  peared...       
+00013320: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
+00013330: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
+00013340: 636c 6175 7365 2e20 4120 636f 6e64 6974  clause. A condit
+00013350: 696f 6e20 6f6e 0a20 2020 2020 2020 2020  ion on.         
+00013360: 2020 2060 6072 6570 6f72 745f 636f 756e     ``report_coun
+00013370: 7472 795f 636f 6465 6060 2069 7320 7265  try_code`` is re
+00013380: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+00013390: 5748 4552 4560 6020 636c 6175 7365 2e0a  WHERE`` clause..
+000133a0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+000133b0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+000133c0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000133d0: 6060 5f72 6570 6f72 745f 636f 756e 7472  ``_report_countr
+000133e0: 795f 636f 6465 6060 2e0a 2020 2020 2020  y_code``..      
+000133f0: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
+00013400: 795f 6964 2028 696e 7429 3a0a 2020 2020  y_id (int):.    
+00013410: 2020 2020 2020 2020 476f 6f67 6c65 2070          Google p
+00013420: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00013430: 4944 2074 6f20 6361 6c63 756c 6174 6520  ID to calculate 
+00013440: 7468 6520 7265 706f 7274 2066 6f72 2c0a  the report for,.
+00013450: 2020 2020 2020 2020 2020 2020 7265 7072              repr
+00013460: 6573 656e 7465 6420 696e 2060 476f 6f67  esented in `Goog
+00013470: 6c65 2773 2070 726f 6475 6374 0a20 2020  le's product.   
+00013480: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
+00013490: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
+000134a0: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+000134b0: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
+000134c0: 3332 3434 3336 3e60 5f5f 2e0a 0a20 2020  324436>`__...   
+000134d0: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+000134e0: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+000134f0: 5460 6020 636c 6175 7365 2e20 4120 636f  T`` clause. A co
+00013500: 6e64 6974 696f 6e20 6f6e 0a20 2020 2020  ndition on.     
+00013510: 2020 2020 2020 2060 6072 6570 6f72 745f         ``report_
+00013520: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
+00013530: 2072 6571 7569 7265 6420 696e 2074 6865   required in the
+00013540: 2060 6057 4845 5245 6060 2063 6c61 7573   ``WHERE`` claus
+00013550: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00013560: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00013570: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00013580: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
+00013590: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
+000135a0: 2020 2020 7472 6166 6669 635f 736f 7572      traffic_sour
+000135b0: 6365 2028 676f 6f67 6c65 2e73 686f 7070  ce (google.shopp
+000135c0: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+000135d0: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+000135e0: 732e 5472 6166 6669 6353 6f75 7263 652e  s.TrafficSource.
+000135f0: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
+00013600: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00013610: 5472 6166 6669 6320 736f 7572 6365 206f  Traffic source o
+00013620: 6620 696d 7072 6573 7369 6f6e 732e 0a0a  f impressions...
+00013630: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+00013640: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
+00013650: 4c45 4354 6060 2063 6c61 7573 652e 0a0a  LECT`` clause...
+00013660: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00013670: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00013680: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00013690: 605f 7472 6166 6669 635f 736f 7572 6365  `_traffic_source
+000136a0: 6060 2e0a 2020 2020 2020 2020 796f 7572  ``..        your
+000136b0: 5f64 6f6d 6169 6e5f 7669 7369 6269 6c69  _domain_visibili
+000136c0: 7479 5f74 7265 6e64 2028 666c 6f61 7429  ty_trend (float)
+000136d0: 3a0a 2020 2020 2020 2020 2020 2020 4368  :.            Ch
+000136e0: 616e 6765 2069 6e20 7669 7369 6269 6c69  ange in visibili
+000136f0: 7479 2062 6173 6564 206f 6e20 696d 7072  ty based on impr
+00013700: 6573 7369 6f6e 7320 666f 720a 2020 2020  essions for.    
+00013710: 2020 2020 2020 2020 796f 7572 2064 6f6d          your dom
+00013720: 6169 6e20 7769 7468 2072 6573 7065 6374  ain with respect
+00013730: 2074 6f20 7468 6520 7374 6172 7420 6f66   to the start of
+00013740: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00013750: 2073 656c 6563 7465 6420 7469 6d65 2072   selected time r
+00013760: 616e 6765 2028 6f72 2066 6972 7374 2064  ange (or first d
+00013770: 6179 2077 6974 6820 6e6f 6e2d 7a65 726f  ay with non-zero
+00013780: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+00013790: 7265 7373 696f 6e73 292e 0a0a 2020 2020  ressions)...    
+000137a0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+000137b0: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+000137c0: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+000137d0: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+000137e0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000137f0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00013800: 6f66 605f 2060 605f 796f 7572 5f64 6f6d  of`_ ``_your_dom
+00013810: 6169 6e5f 7669 7369 6269 6c69 7479 5f74  ain_visibility_t
+00013820: 7265 6e64 6060 2e0a 2020 2020 2020 2020  rend``..        
+00013830: 6361 7465 676f 7279 5f62 656e 6368 6d61  category_benchma
+00013840: 726b 5f76 6973 6962 696c 6974 795f 7472  rk_visibility_tr
+00013850: 656e 6420 2866 6c6f 6174 293a 0a20 2020  end (float):.   
+00013860: 2020 2020 2020 2020 2043 6861 6e67 6520           Change 
+00013870: 696e 2076 6973 6962 696c 6974 7920 6261  in visibility ba
+00013880: 7365 6420 6f6e 2069 6d70 7265 7373 696f  sed on impressio
+00013890: 6e73 0a20 2020 2020 2020 2020 2020 2077  ns.            w
+000138a0: 6974 6820 7265 7370 6563 7420 746f 2074  ith respect to t
+000138b0: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+000138c0: 7365 6c65 6374 6564 2074 696d 650a 2020  selected time.  
+000138d0: 2020 2020 2020 2020 2020 7261 6e67 6520            range 
+000138e0: 286f 7220 6669 7273 7420 6461 7920 7769  (or first day wi
+000138f0: 7468 206e 6f6e 2d7a 6572 6f20 696d 7072  th non-zero impr
+00013900: 6573 7369 6f6e 7329 0a20 2020 2020 2020  essions).       
+00013910: 2020 2020 2066 6f72 2061 2063 6f6d 6269       for a combi
+00013920: 6e65 6420 7365 7420 6f66 206d 6572 6368  ned set of merch
+00013930: 616e 7473 2077 6974 6820 6869 6768 6573  ants with highes
+00013940: 740a 2020 2020 2020 2020 2020 2020 7669  t.            vi
+00013950: 7369 6269 6c69 7479 2061 7070 726f 7869  sibility approxi
+00013960: 6d61 7469 6e67 2074 6865 206d 6172 6b65  mating the marke
+00013970: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+00013980: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+00013990: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+000139a0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+000139b0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+000139c0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000139d0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+000139e0: 6361 7465 676f 7279 5f62 656e 6368 6d61  category_benchma
+000139f0: 726b 5f76 6973 6962 696c 6974 795f 7472  rk_visibility_tr
+00013a00: 656e 6460 602e 0a20 2020 2022 2222 0a0a  end``..    """..
+00013a10: 2020 2020 6461 7465 3a20 6461 7465 5f70      date: date_p
+00013a20: 6232 2e44 6174 6520 3d20 7072 6f74 6f2e  b2.Date = proto.
+00013a30: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00013a40: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+00013a50: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
+00013a60: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+00013a70: 6461 7465 5f70 6232 2e44 6174 652c 0a20  date_pb2.Date,. 
+00013a80: 2020 2029 0a20 2020 2072 6570 6f72 745f     ).    report_
+00013a90: 636f 756e 7472 795f 636f 6465 3a20 7374  country_code: st
+00013aa0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00013ab0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00013ac0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00013ad0: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
+00013ae0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+00013af0: 2020 2020 290a 2020 2020 7265 706f 7274      ).    report
+00013b00: 5f63 6174 6567 6f72 795f 6964 3a20 696e  _category_id: in
+00013b10: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+00013b20: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
+00013b30: 4e54 3634 2c0a 2020 2020 2020 2020 6e75  NT64,.        nu
+00013b40: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+00013b50: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00013b60: 2020 2029 0a20 2020 2074 7261 6666 6963     ).    traffic
+00013b70: 5f73 6f75 7263 653a 2022 5472 6166 6669  _source: "Traffi
+00013b80: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
+00013b90: 6f75 7263 6545 6e75 6d22 203d 2070 726f  ourceEnum" = pro
+00013ba0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00013bb0: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+00013bc0: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
+00013bd0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00013be0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
+00013bf0: 6e75 6d3d 2254 7261 6666 6963 536f 7572  num="TrafficSour
+00013c00: 6365 2e54 7261 6666 6963 536f 7572 6365  ce.TrafficSource
+00013c10: 456e 756d 222c 0a20 2020 2029 0a20 2020  Enum",.    ).   
+00013c20: 2079 6f75 725f 646f 6d61 696e 5f76 6973   your_domain_vis
+00013c30: 6962 696c 6974 795f 7472 656e 643a 2066  ibility_trend: f
+00013c40: 6c6f 6174 203d 2070 726f 746f 2e46 6965  loat = proto.Fie
+00013c50: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00013c60: 6f2e 444f 5542 4c45 2c0a 2020 2020 2020  o.DOUBLE,.      
+00013c70: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
+00013c80: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00013c90: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
+00013ca0: 6567 6f72 795f 6265 6e63 686d 6172 6b5f  egory_benchmark_
+00013cb0: 7669 7369 6269 6c69 7479 5f74 7265 6e64  visibility_trend
+00013cc0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
+00013cd0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00013ce0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
+00013cf0: 2020 2020 206e 756d 6265 723d 362c 0a20       number=6,. 
+00013d00: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00013d10: 5472 7565 2c0a 2020 2020 290a 0a0a 636c  True,.    )...cl
+00013d20: 6173 7320 4d61 726b 6574 696e 674d 6574  ass MarketingMet
+00013d30: 686f 6428 7072 6f74 6f2e 4d65 7373 6167  hod(proto.Messag
+00013d40: 6529 3a0a 2020 2020 7222 2222 4d61 726b  e):.    r"""Mark
+00013d50: 6574 696e 6720 6d65 7468 6f64 2075 7365  eting method use
+00013d60: 6420 746f 2070 726f 6d6f 7465 2079 6f75  d to promote you
+00013d70: 7220 7072 6f64 7563 7473 206f 6e20 476f  r products on Go
+00013d80: 6f67 6c65 0a20 2020 2028 6f72 6761 6e69  ogle.    (organi
+00013d90: 6320 7665 7273 7573 2061 6473 292e 0a0a  c versus ads)...
+00013da0: 2020 2020 2222 220a 0a20 2020 2063 6c61      """..    cla
+00013db0: 7373 204d 6172 6b65 7469 6e67 4d65 7468  ss MarketingMeth
+00013dc0: 6f64 456e 756d 2870 726f 746f 2e45 6e75  odEnum(proto.Enu
+00013dd0: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
+00013de0: 4d61 726b 6574 696e 6720 6d65 7468 6f64  Marketing method
+00013df0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00013e00: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
+00013e10: 2020 2020 2020 4d41 524b 4554 494e 475f        MARKETING_
+00013e20: 4d45 5448 4f44 5f45 4e55 4d5f 554e 5350  METHOD_ENUM_UNSP
+00013e30: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
+00013e40: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
+00013e50: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
+00013e60: 2020 2020 2020 2020 4f52 4741 4e49 4320          ORGANIC 
+00013e70: 2831 293a 0a20 2020 2020 2020 2020 2020  (1):.           
+00013e80: 2020 2020 204f 7267 616e 6963 206d 6172       Organic mar
+00013e90: 6b65 7469 6e67 2e0a 2020 2020 2020 2020  keting..        
+00013ea0: 2020 2020 4144 5320 2832 293a 0a20 2020      ADS (2):.   
+00013eb0: 2020 2020 2020 2020 2020 2020 2041 6473               Ads
+00013ec0: 2d62 6173 6564 206d 6172 6b65 7469 6e67  -based marketing
+00013ed0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00013ee0: 2020 2020 2020 4d41 524b 4554 494e 475f        MARKETING_
+00013ef0: 4d45 5448 4f44 5f45 4e55 4d5f 554e 5350  METHOD_ENUM_UNSP
+00013f00: 4543 4946 4945 4420 3d20 300a 2020 2020  ECIFIED = 0.    
+00013f10: 2020 2020 4f52 4741 4e49 4320 3d20 310a      ORGANIC = 1.
+00013f20: 2020 2020 2020 2020 4144 5320 3d20 320a          ADS = 2.
+00013f30: 0a0a 636c 6173 7320 5265 706f 7274 4772  ..class ReportGr
+00013f40: 616e 756c 6172 6974 7928 7072 6f74 6f2e  anularity(proto.
+00013f50: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+00013f60: 2222 4772 616e 756c 6172 6974 7920 6f66  ""Granularity of
+00013f70: 2074 6865 2042 6573 7420 7365 6c6c 6572   the Best seller
+00013f80: 7320 7265 706f 7274 2e20 4265 7374 2073  s report. Best s
+00013f90: 656c 6c65 7273 2072 6570 6f72 7473 0a20  ellers reports. 
+00013fa0: 2020 2061 7265 2063 6f6d 7075 7465 6420     are computed 
+00013fb0: 6f76 6572 2061 2077 6565 6b20 616e 6420  over a week and 
+00013fc0: 6120 6d6f 6e74 6820 7469 6d65 6672 616d  a month timefram
+00013fd0: 652e 0a0a 2020 2020 2222 220a 0a20 2020  e...    """..   
+00013fe0: 2063 6c61 7373 2052 6570 6f72 7447 7261   class ReportGra
+00013ff0: 6e75 6c61 7269 7479 456e 756d 2870 726f  nularityEnum(pro
+00014000: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
+00014010: 2020 7222 2222 5265 706f 7274 2067 7261    r"""Report gra
+00014020: 6e75 6c61 7269 7479 2076 616c 7565 732e  nularity values.
+00014030: 0a0a 2020 2020 2020 2020 5661 6c75 6573  ..        Values
+00014040: 3a0a 2020 2020 2020 2020 2020 2020 5245  :.            RE
+00014050: 504f 5254 5f47 5241 4e55 4c41 5249 5459  PORT_GRANULARITY
+00014060: 5f45 4e55 4d5f 554e 5350 4543 4946 4945  _ENUM_UNSPECIFIE
+00014070: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
+00014080: 2020 2020 2020 204e 6f74 2073 7065 6369         Not speci
+00014090: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
+000140a0: 2020 5745 454b 4c59 2028 3129 3a0a 2020    WEEKLY (1):.  
+000140b0: 2020 2020 2020 2020 2020 2020 2020 5265                Re
+000140c0: 706f 7274 2069 7320 636f 6d70 7574 6564  port is computed
+000140d0: 206f 7665 7220 6120 7765 656b 2074 696d   over a week tim
+000140e0: 6566 7261 6d65 2e0a 2020 2020 2020 2020  eframe..        
+000140f0: 2020 2020 4d4f 4e54 484c 5920 2832 293a      MONTHLY (2):
+00014100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014110: 2052 6570 6f72 7420 6973 2063 6f6d 7075   Report is compu
+00014120: 7465 6420 6f76 6572 2061 206d 6f6e 7468  ted over a month
+00014130: 2074 696d 6566 7261 6d65 2e0a 2020 2020   timeframe..    
+00014140: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014150: 5245 504f 5254 5f47 5241 4e55 4c41 5249  REPORT_GRANULARI
+00014160: 5459 5f45 4e55 4d5f 554e 5350 4543 4946  TY_ENUM_UNSPECIF
+00014170: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
+00014180: 5745 454b 4c59 203d 2031 0a20 2020 2020  WEEKLY = 1.     
+00014190: 2020 204d 4f4e 5448 4c59 203d 2032 0a0a     MONTHLY = 2..
+000141a0: 0a63 6c61 7373 2052 656c 6174 6976 6544  .class RelativeD
+000141b0: 656d 616e 6428 7072 6f74 6f2e 4d65 7373  emand(proto.Mess
+000141c0: 6167 6529 3a0a 2020 2020 7222 2222 5265  age):.    r"""Re
+000141d0: 6c61 7469 7665 2064 656d 616e 6420 6f66  lative demand of
+000141e0: 2061 2070 726f 6475 6374 2063 6c75 7374   a product clust
+000141f0: 6572 206f 7220 6272 616e 6420 696e 2074  er or brand in t
+00014200: 6865 2042 6573 740a 2020 2020 7365 6c6c  he Best.    sell
+00014210: 6572 7320 7265 706f 7274 2e0a 0a20 2020  ers report...   
+00014220: 2022 2222 0a0a 2020 2020 636c 6173 7320   """..    class 
+00014230: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
+00014240: 756d 2870 726f 746f 2e45 6e75 6d29 3a0a  um(proto.Enum):.
+00014250: 2020 2020 2020 2020 7222 2222 5265 6c61          r"""Rela
+00014260: 7469 7665 2064 656d 616e 6420 7661 6c75  tive demand valu
+00014270: 6573 2e0a 0a20 2020 2020 2020 2056 616c  es...        Val
+00014280: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
+00014290: 2052 454c 4154 4956 455f 4445 4d41 4e44   RELATIVE_DEMAND
+000142a0: 5f45 4e55 4d5f 554e 5350 4543 4946 4945  _ENUM_UNSPECIFIE
+000142b0: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
+000142c0: 2020 2020 2020 204e 6f74 2073 7065 6369         Not speci
+000142d0: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
+000142e0: 2020 5645 5259 5f4c 4f57 2028 3130 293a    VERY_LOW (10):
+000142f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014300: 2044 656d 616e 6420 6973 2030 2d35 2520   Demand is 0-5% 
+00014310: 6f66 2074 6865 2064 656d 616e 6420 6f66  of the demand of
+00014320: 2074 6865 2068 6967 6865 7374 0a20 2020   the highest.   
+00014330: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+00014340: 6b65 6420 7072 6f64 7563 7420 636c 7573  ked product clus
+00014350: 7465 7220 6f72 2062 7261 6e64 2e0a 2020  ter or brand..  
+00014360: 2020 2020 2020 2020 2020 4c4f 5720 2832            LOW (2
+00014370: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
+00014380: 2020 2020 4465 6d61 6e64 2069 7320 362d      Demand is 6-
+00014390: 3130 2520 6f66 2074 6865 2064 656d 616e  10% of the deman
+000143a0: 6420 6f66 2074 6865 2068 6967 6865 7374  d of the highest
+000143b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000143c0: 2072 616e 6b65 6420 7072 6f64 7563 7420   ranked product 
+000143d0: 636c 7573 7465 7220 6f72 2062 7261 6e64  cluster or brand
+000143e0: 2e0a 2020 2020 2020 2020 2020 2020 4d45  ..            ME
+000143f0: 4449 554d 2028 3330 293a 0a20 2020 2020  DIUM (30):.     
+00014400: 2020 2020 2020 2020 2020 2044 656d 616e             Deman
+00014410: 6420 6973 2031 312d 3230 2520 6f66 2074  d is 11-20% of t
+00014420: 6865 2064 656d 616e 6420 6f66 2074 6865  he demand of the
+00014430: 2068 6967 6865 7374 0a20 2020 2020 2020   highest.       
+00014440: 2020 2020 2020 2020 2072 616e 6b65 6420           ranked 
+00014450: 7072 6f64 7563 7420 636c 7573 7465 7220  product cluster 
+00014460: 6f72 2062 7261 6e64 2e0a 2020 2020 2020  or brand..      
+00014470: 2020 2020 2020 4849 4748 2028 3430 293a        HIGH (40):
+00014480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014490: 2044 656d 616e 6420 6973 2032 312d 3530   Demand is 21-50
+000144a0: 2520 6f66 2074 6865 2064 656d 616e 6420  % of the demand 
+000144b0: 6f66 2074 6865 2068 6967 6865 7374 0a20  of the highest. 
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000144d0: 616e 6b65 6420 7072 6f64 7563 7420 636c  anked product cl
+000144e0: 7573 7465 7220 6f72 2062 7261 6e64 2e0a  uster or brand..
+000144f0: 2020 2020 2020 2020 2020 2020 5645 5259              VERY
+00014500: 5f48 4947 4820 2835 3029 3a0a 2020 2020  _HIGH (50):.    
+00014510: 2020 2020 2020 2020 2020 2020 4465 6d61              Dema
+00014520: 6e64 2069 7320 3531 2d31 3030 2520 6f66  nd is 51-100% of
+00014530: 2074 6865 2064 656d 616e 6420 6f66 2074   the demand of t
+00014540: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00014550: 2020 2068 6967 6865 7374 2072 616e 6b65     highest ranke
+00014560: 6420 7072 6f64 7563 7420 636c 7573 7465  d product cluste
+00014570: 7220 6f72 2062 7261 6e64 2e0a 2020 2020  r or brand..    
+00014580: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014590: 5245 4c41 5449 5645 5f44 454d 414e 445f  RELATIVE_DEMAND_
+000145a0: 454e 554d 5f55 4e53 5045 4349 4649 4544  ENUM_UNSPECIFIED
+000145b0: 203d 2030 0a20 2020 2020 2020 2056 4552   = 0.        VER
+000145c0: 595f 4c4f 5720 3d20 3130 0a20 2020 2020  Y_LOW = 10.     
+000145d0: 2020 204c 4f57 203d 2032 300a 2020 2020     LOW = 20.    
+000145e0: 2020 2020 4d45 4449 554d 203d 2033 300a      MEDIUM = 30.
+000145f0: 2020 2020 2020 2020 4849 4748 203d 2034          HIGH = 4
+00014600: 300a 2020 2020 2020 2020 5645 5259 5f48  0.        VERY_H
+00014610: 4947 4820 3d20 3530 0a0a 0a63 6c61 7373  IGH = 50...class
+00014620: 2052 656c 6174 6976 6544 656d 616e 6443   RelativeDemandC
+00014630: 6861 6e67 6554 7970 6528 7072 6f74 6f2e  hangeType(proto.
+00014640: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+00014650: 2222 5265 6c61 7469 7665 2064 656d 616e  ""Relative deman
+00014660: 6420 6f66 2061 2070 726f 6475 6374 2063  d of a product c
+00014670: 6c75 7374 6572 206f 7220 6272 616e 6420  luster or brand 
+00014680: 696e 2074 6865 2042 6573 740a 2020 2020  in the Best.    
+00014690: 7365 6c6c 6572 7320 7265 706f 7274 2063  sellers report c
+000146a0: 6f6d 7061 7265 6420 746f 2074 6865 2070  ompared to the p
+000146b0: 7265 7669 6f75 7320 7469 6d65 2070 6572  revious time per
+000146c0: 696f 642e 0a0a 2020 2020 2222 220a 0a20  iod...    """.. 
+000146d0: 2020 2063 6c61 7373 2052 656c 6174 6976     class Relativ
+000146e0: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
+000146f0: 6545 6e75 6d28 7072 6f74 6f2e 456e 756d  eEnum(proto.Enum
+00014700: 293a 0a20 2020 2020 2020 2072 2222 2252  ):.        r"""R
+00014710: 656c 6174 6976 6520 6465 6d61 6e64 2063  elative demand c
+00014720: 6861 6e67 6520 7479 7065 2076 616c 7565  hange type value
+00014730: 732e 0a0a 2020 2020 2020 2020 5661 6c75  s...        Valu
+00014740: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00014750: 5245 4c41 5449 5645 5f44 454d 414e 445f  RELATIVE_DEMAND_
+00014760: 4348 414e 4745 5f54 5950 455f 454e 554d  CHANGE_TYPE_ENUM
+00014770: 5f55 4e53 5045 4349 4649 4544 2028 3029  _UNSPECIFIED (0)
+00014780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014790: 2020 4e6f 7420 7370 6563 6966 6965 642e    Not specified.
+000147a0: 0a20 2020 2020 2020 2020 2020 2053 494e  .            SIN
+000147b0: 4b45 5220 2831 293a 0a20 2020 2020 2020  KER (1):.       
+000147c0: 2020 2020 2020 2020 2052 656c 6174 6976           Relativ
+000147d0: 6520 6465 6d61 6e64 2069 7320 6c6f 7765  e demand is lowe
+000147e0: 7220 7468 616e 2074 6865 2070 7265 7669  r than the previ
+000147f0: 6f75 730a 2020 2020 2020 2020 2020 2020  ous.            
+00014800: 2020 2020 7469 6d65 2070 6572 696f 642e      time period.
+00014810: 0a20 2020 2020 2020 2020 2020 2046 4c41  .            FLA
+00014820: 5420 2832 293a 0a20 2020 2020 2020 2020  T (2):.         
+00014830: 2020 2020 2020 2052 656c 6174 6976 6520         Relative 
+00014840: 6465 6d61 6e64 2069 7320 6571 7561 6c20  demand is equal 
+00014850: 746f 2074 6865 2070 7265 7669 6f75 7320  to the previous 
+00014860: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
+00014870: 2020 2020 2070 6572 696f 642e 0a20 2020       period..   
+00014880: 2020 2020 2020 2020 2052 4953 4552 2028           RISER (
+00014890: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
+000148a0: 2020 2020 5265 6c61 7469 7665 2064 656d      Relative dem
+000148b0: 616e 6420 6973 2068 6967 6865 7220 7468  and is higher th
+000148c0: 616e 2074 6865 2070 7265 7669 6f75 730a  an the previous.
+000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148e0: 7469 6d65 2070 6572 696f 642e 0a20 2020  time period..   
+000148f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014900: 2052 454c 4154 4956 455f 4445 4d41 4e44   RELATIVE_DEMAND
+00014910: 5f43 4841 4e47 455f 5459 5045 5f45 4e55  _CHANGE_TYPE_ENU
+00014920: 4d5f 554e 5350 4543 4946 4945 4420 3d20  M_UNSPECIFIED = 
+00014930: 300a 2020 2020 2020 2020 5349 4e4b 4552  0.        SINKER
+00014940: 203d 2031 0a20 2020 2020 2020 2046 4c41   = 1.        FLA
+00014950: 5420 3d20 320a 2020 2020 2020 2020 5249  T = 2.        RI
+00014960: 5345 5220 3d20 330a 0a0a 636c 6173 7320  SER = 3...class 
+00014970: 5472 6166 6669 6353 6f75 7263 6528 7072  TrafficSource(pr
+00014980: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+00014990: 2020 7222 2222 5472 6166 6669 6320 736f    r"""Traffic so
+000149a0: 7572 6365 206f 6620 696d 7072 6573 7369  urce of impressi
+000149b0: 6f6e 7320 696e 2074 6865 2043 6f6d 7065  ons in the Compe
+000149c0: 7469 7469 7665 2076 6973 6962 696c 6974  titive visibilit
+000149d0: 790a 2020 2020 7265 706f 7274 2e0a 0a20  y.    report... 
+000149e0: 2020 2022 2222 0a0a 2020 2020 636c 6173     """..    clas
+000149f0: 7320 5472 6166 6669 6353 6f75 7263 6545  s TrafficSourceE
+00014a00: 6e75 6d28 7072 6f74 6f2e 456e 756d 293a  num(proto.Enum):
+00014a10: 0a20 2020 2020 2020 2072 2222 2254 7261  .        r"""Tra
+00014a20: 6666 6963 2073 6f75 7263 6520 7661 6c75  ffic source valu
+00014a30: 6573 2e0a 0a20 2020 2020 2020 2056 616c  es...        Val
+00014a40: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
+00014a50: 2054 5241 4646 4943 5f53 4f55 5243 455f   TRAFFIC_SOURCE_
+00014a60: 454e 554d 5f55 4e53 5045 4349 4649 4544  ENUM_UNSPECIFIED
+00014a70: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
+00014a80: 2020 2020 2020 4e6f 7420 7370 6563 6966        Not specif
+00014a90: 6965 642e 0a20 2020 2020 2020 2020 2020  ied..           
+00014aa0: 204f 5247 414e 4943 2028 3129 3a0a 2020   ORGANIC (1):.  
+00014ab0: 2020 2020 2020 2020 2020 2020 2020 4f72                Or
+00014ac0: 6761 6e69 6320 7472 6166 6669 632e 0a20  ganic traffic.. 
+00014ad0: 2020 2020 2020 2020 2020 2041 4453 2028             ADS (
+00014ae0: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
+00014af0: 2020 2020 5472 6166 6669 6320 6672 6f6d      Traffic from
+00014b00: 2061 6473 2e0a 2020 2020 2020 2020 2020   ads..          
+00014b10: 2020 414c 4c20 2833 293a 0a20 2020 2020    ALL (3):.     
+00014b20: 2020 2020 2020 2020 2020 204f 7267 616e             Organ
+00014b30: 6963 2061 6e64 2061 6473 2074 7261 6666  ic and ads traff
+00014b40: 6963 2e0a 2020 2020 2020 2020 2222 220a  ic..        """.
+00014b50: 2020 2020 2020 2020 5452 4146 4649 435f          TRAFFIC_
+00014b60: 534f 5552 4345 5f45 4e55 4d5f 554e 5350  SOURCE_ENUM_UNSP
+00014b70: 4543 4946 4945 4420 3d20 300a 2020 2020  ECIFIED = 0.    
+00014b80: 2020 2020 4f52 4741 4e49 4320 3d20 310a      ORGANIC = 1.
+00014b90: 2020 2020 2020 2020 4144 5320 3d20 320a          ADS = 2.
+00014ba0: 2020 2020 2020 2020 414c 4c20 3d20 330a          ALL = 3.
+00014bb0: 0a0a 5f5f 616c 6c5f 5f20 3d20 7475 706c  ..__all__ = tupl
+00014bc0: 6528 736f 7274 6564 285f 5f70 726f 746f  e(sorted(__proto
+00014bd0: 6275 665f 5f2e 6d61 6e69 6665 7374 2929  buf__.manifest))
+00014be0: 0a                                       .
```

### Comparing `google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/PKG-INFO` & `google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-reports
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Merchant Reports API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reports
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-reports-0.1.5/google_shopping_merchant_reports.egg-info/SOURCES.txt` & `google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.5/setup.py` & `google-shopping-merchant-reports-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/tests/__init__.py` & `google-shopping-merchant-reports-0.1.6/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/tests/unit/__init__.py` & `google-shopping-merchant-reports-0.1.6/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/tests/unit/gapic/__init__.py` & `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/tests/unit/gapic/merchant_reports_v1beta/__init__.py` & `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-reports-0.1.5/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py` & `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1136,15 +1136,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.search(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == reports.SearchRequest()
+        request = reports.SearchRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_search_empty_call():
@@ -1159,14 +1160,66 @@
     with mock.patch.object(type(client.transport.search), "__call__") as call:
         client.search()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == reports.SearchRequest()
 
 
+def test_search_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ReportServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = reports.SearchRequest(
+        parent="parent_value",
+        query="query_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search), "__call__") as call:
+        client.search(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == reports.SearchRequest(
+            parent="parent_value",
+            query="query_value",
+            page_token="page_token_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_search_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ReportServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            reports.SearchResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.search()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == reports.SearchRequest()
+
+
 @pytest.mark.asyncio
 async def test_search_async(
     transport: str = "grpc_asyncio", request_type=reports.SearchRequest
 ):
     client = ReportServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1185,15 +1238,16 @@
             )
         )
         response = await client.search(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == reports.SearchRequest()
+        request = reports.SearchRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
```

