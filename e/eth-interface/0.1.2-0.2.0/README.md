# Comparing `tmp/eth-interface-0.1.2.tar.gz` & `tmp/eth-interface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eth-interface-0.1.2.tar", last modified: Tue Jun  6 13:02:49 2023, max compression
+gzip compressed data, was "eth-interface-0.2.0.tar", last modified: Mon Apr 15 10:38:47 2024, max compression
```

## Comparing `eth-interface-0.1.2.tar` & `eth-interface-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/
--rw-r--r--   0 lash      (1000) lash      (1000)       47 2023-03-24 18:44:26.000000 eth-interface-0.1.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-06-06 13:02:49.446622 eth-interface-0.1.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.443289 eth-interface-0.1.2/eth_interface/
--rw-r--r--   0 lash      (1000) lash      (1000)       27 2023-03-24 16:39:09.000000 eth-interface-0.1.2/eth_interface/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1060 2023-03-24 16:36:49.000000 eth-interface-0.1.2/eth_interface/eip165.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/eth_interface/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-24 16:58:23.000000 eth-interface-0.1.2/eth_interface/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      808 2023-06-06 12:49:06.000000 eth-interface-0.1.2/eth_interface/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/eth_interface.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      390 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-11-13 17:36:26.000000 eth-interface-0.1.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      769 2023-06-06 13:02:49.446622 eth-interface-0.1.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      613 2021-05-02 14:25:37.000000 eth-interface-0.1.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2022-11-13 17:36:56.000000 eth-interface-0.1.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     1980 2023-06-06 12:56:03.000000 eth-interface-0.1.2/tests/test_eip165.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:38:47.496607 eth-interface-0.2.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)       47 2023-03-24 18:44:26.000000 eth-interface-0.2.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      676 2024-04-15 10:38:47.496607 eth-interface-0.2.0/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:38:47.496607 eth-interface-0.2.0/eth_interface/
+-rw-r--r--   0 lash      (1000) lash      (1000)       27 2023-03-24 16:39:09.000000 eth-interface-0.2.0/eth_interface/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1060 2023-03-24 16:36:49.000000 eth-interface-0.2.0/eth_interface/eip165.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:38:47.496607 eth-interface-0.2.0/eth_interface/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-24 16:58:23.000000 eth-interface-0.2.0/eth_interface/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      808 2023-06-06 12:49:06.000000 eth-interface-0.2.0/eth_interface/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:38:47.496607 eth-interface-0.2.0/eth_interface.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      676 2024-04-15 10:38:47.000000 eth-interface-0.2.0/eth_interface.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      390 2024-04-15 10:38:47.000000 eth-interface-0.2.0/eth_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-15 10:38:47.000000 eth-interface-0.2.0/eth_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2024-04-15 10:38:47.000000 eth-interface-0.2.0/eth_interface.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       14 2024-04-15 10:38:47.000000 eth-interface-0.2.0/eth_interface.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2024-04-15 09:56:32.000000 eth-interface-0.2.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      769 2024-04-15 10:38:47.496607 eth-interface-0.2.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      613 2021-05-02 14:25:37.000000 eth-interface-0.2.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       38 2024-04-15 10:30:07.000000 eth-interface-0.2.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-15 10:38:47.496607 eth-interface-0.2.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1980 2023-06-06 12:56:03.000000 eth-interface-0.2.0/tests/test_eip165.py
```

### Comparing `eth-interface-0.1.2/PKG-INFO` & `eth-interface-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-interface
-Version: 0.1.2
+Version: 0.2.0
 Summary: EIP165 interface
 Home-page: https://git.defalsify.org/eth-interface
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
+Requires-Dist: chainlib-eth~=0.6.2
```

### Comparing `eth-interface-0.1.2/eth_interface/eip165.py` & `eth-interface-0.2.0/eth_interface/eip165.py`

 * *Files identical despite different names*

### Comparing `eth-interface-0.1.2/eth_interface/unittest/base.py` & `eth-interface-0.2.0/eth_interface/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-interface-0.1.2/eth_interface.egg-info/PKG-INFO` & `eth-interface-0.2.0/eth_interface.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-interface
-Version: 0.1.2
+Version: 0.2.0
 Summary: EIP165 interface
 Home-page: https://git.defalsify.org/eth-interface
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
+Requires-Dist: chainlib-eth~=0.6.2
```

### Comparing `eth-interface-0.1.2/setup.cfg` & `eth-interface-0.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-interface
-version = 0.1.2
+version = 0.2.0
 description = EIP165 interface
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-interface
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-interface-0.1.2/setup.py` & `eth-interface-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `eth-interface-0.1.2/tests/test_eip165.py` & `eth-interface-0.2.0/tests/test_eip165.py`

 * *Files identical despite different names*

