# Comparing `tmp/erc20-limiter-0.0.3.tar.gz` & `tmp/erc20-limiter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erc20-limiter-0.0.3.tar", last modified: Thu Aug  3 15:54:42 2023, max compression
+gzip compressed data, was "erc20-limiter-0.1.0.tar", last modified: Mon Apr 15 10:39:46 2024, max compression
```

## Comparing `erc20-limiter-0.0.3.tar` & `erc20-limiter-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-07-28 09:50:15.000000 erc20-limiter-0.0.3/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-07-28 12:43:39.000000 erc20-limiter-0.0.3/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.0.3/erc20_limiter/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     5428 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1602 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2279 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     6340 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1923 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2623 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4978 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1338 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2054 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.0.3/erc20_limiter/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2688 2023-08-03 12:50:12.000000 erc20-limiter-0.0.3/erc20_limiter/index.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.0.3/erc20_limiter/limiter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.0.3/erc20_limiter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1914 2023-08-03 12:51:31.000000 erc20-limiter-0.0.3/erc20_limiter/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      837 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-27 16:54:14.000000 erc20-limiter-0.0.3/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      797 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.0.3/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       58 2023-07-27 16:55:11.000000 erc20-limiter-0.0.3/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.0.3/tests/test_base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1550 2023-08-03 12:51:44.000000 erc20-limiter-0.0.3/tests/test_index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-07-28 09:50:15.000000 erc20-limiter-0.1.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-07-28 12:43:39.000000 erc20-limiter-0.1.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/erc20_limiter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.1.0/erc20_limiter/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/erc20_limiter/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5428 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/Limiter.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1602 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/Limiter.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2279 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/Limiter.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     6340 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1923 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2623 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4978 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1338 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2054 2023-08-03 15:51:50.000000 erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.1.0/erc20_limiter/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2688 2023-08-03 12:50:12.000000 erc20-limiter-0.1.0/erc20_limiter/index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.1.0/erc20_limiter/limiter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/erc20_limiter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.1.0/erc20_limiter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1914 2023-08-03 12:51:31.000000 erc20-limiter-0.1.0/erc20_limiter/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/erc20_limiter.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2024-04-15 10:39:46.000000 erc20-limiter-0.1.0/erc20_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      837 2024-04-15 10:39:46.000000 erc20-limiter-0.1.0/erc20_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-15 10:39:46.000000 erc20-limiter-0.1.0/erc20_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2024-04-15 10:39:46.000000 erc20-limiter-0.1.0/erc20_limiter.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       14 2024-04-15 10:39:46.000000 erc20-limiter-0.1.0/erc20_limiter.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2024-04-15 10:09:57.000000 erc20-limiter-0.1.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      797 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.1.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       71 2024-04-15 10:11:43.000000 erc20-limiter-0.1.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:39:46.246606 erc20-limiter-0.1.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.1.0/tests/test_base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1550 2023-08-03 12:51:44.000000 erc20-limiter-0.1.0/tests/test_index.py
```

### Comparing `erc20-limiter-0.0.3/LICENSE` & `erc20-limiter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/PKG-INFO` & `erc20-limiter-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.3
+Version: 0.1.0
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,8 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.2
```

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/Limiter.bin` & `erc20-limiter-0.1.0/erc20_limiter/data/Limiter.bin`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/Limiter.json` & `erc20-limiter-0.1.0/erc20_limiter/data/Limiter.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/Limiter.metadata.json` & `erc20-limiter-0.1.0/erc20_limiter/data/Limiter.metadata.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.bin` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.bin`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.json` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.metadata.json` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterIndex.metadata.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.bin` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.bin`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.json` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.metadata.json` & `erc20-limiter-0.1.0/erc20_limiter/data/LimiterTokenRegistry.metadata.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/index.py` & `erc20-limiter-0.1.0/erc20_limiter/index.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/limiter.py` & `erc20-limiter-0.1.0/erc20_limiter/limiter.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter/unittest/base.py` & `erc20-limiter-0.1.0/erc20_limiter/unittest/base.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/erc20_limiter.egg-info/PKG-INFO` & `erc20-limiter-0.1.0/erc20_limiter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.3
+Version: 0.1.0
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,8 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.2
```

### Comparing `erc20-limiter-0.0.3/erc20_limiter.egg-info/SOURCES.txt` & `erc20-limiter-0.1.0/erc20_limiter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/setup.cfg` & `erc20-limiter-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erc20-limiter
-version = 0.0.3
+version = 0.1.0
 description = ERC20 balance limit registry
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/erc20-limiter/log.html
 keywords = 
 	dlt
 	blockchain
```

### Comparing `erc20-limiter-0.0.3/tests/test_base.py` & `erc20-limiter-0.1.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.3/tests/test_index.py` & `erc20-limiter-0.1.0/tests/test_index.py`

 * *Files identical despite different names*

