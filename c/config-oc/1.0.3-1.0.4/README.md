# Comparing `tmp/config-oc-1.0.3.tar.gz` & `tmp/config-oc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-oc-1.0.3.tar", last modified: Thu Dec  7 15:57:35 2023, max compression
+gzip compressed data, was "config-oc-1.0.4.tar", last modified: Mon Apr 15 14:18:27 2024, max compression
```

## Comparing `config-oc-1.0.3.tar` & `config-oc-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-12-07 15:57:35.309038 config-oc-1.0.3/
--rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-05-26 22:40:09.000000 config-oc-1.0.3/LICENSE
--rw-rw-r--   0 bast      (1000) bast      (1000)     9019 2023-12-07 15:57:35.309038 config-oc-1.0.3/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)     8374 2023-08-24 11:23:25.000000 config-oc-1.0.3/README.md
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-12-07 15:57:35.309038 config-oc-1.0.3/config/
--rw-rw-r--   0 bast      (1000) bast      (1000)      401 2023-06-24 13:32:34.000000 config-oc-1.0.3/config/__init__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)      145 2023-05-27 00:29:25.000000 config-oc-1.0.3/config/__main__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     2321 2023-06-24 12:40:15.000000 config-oc-1.0.3/config/conf.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     2190 2023-12-07 15:55:14.000000 config-oc-1.0.3/config/data.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-12-07 15:57:35.309038 config-oc-1.0.3/config_oc.egg-info/
--rw-rw-r--   0 bast      (1000) bast      (1000)     9019 2023-12-07 15:57:35.000000 config-oc-1.0.3/config_oc.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)      296 2023-12-07 15:57:35.000000 config-oc-1.0.3/config_oc.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-12-07 15:57:35.000000 config-oc-1.0.3/config_oc.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)       39 2023-12-07 15:57:35.000000 config-oc-1.0.3/config_oc.egg-info/requires.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        7 2023-12-07 15:57:35.000000 config-oc-1.0.3/config_oc.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-10-10 14:45:31.000000 config-oc-1.0.3/config_oc.egg-info/zip-safe
--rw-rw-r--   0 bast      (1000) bast      (1000)       79 2023-12-07 15:57:35.309038 config-oc-1.0.3/setup.cfg
--rw-rw-r--   0 bast      (1000) bast      (1000)      869 2023-12-07 15:54:53.000000 config-oc-1.0.3/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-15 14:18:27.138722 config-oc-1.0.4/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-05-26 22:40:09.000000 config-oc-1.0.4/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)     9019 2024-04-15 14:18:27.138722 config-oc-1.0.4/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)     8374 2023-08-24 11:23:25.000000 config-oc-1.0.4/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-15 14:18:27.138722 config-oc-1.0.4/config/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      616 2024-04-15 14:12:32.000000 config-oc-1.0.4/config/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)      145 2023-05-27 00:29:25.000000 config-oc-1.0.4/config/__main__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2321 2023-06-24 12:40:15.000000 config-oc-1.0.4/config/conf.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2190 2023-12-07 15:57:54.000000 config-oc-1.0.4/config/data.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-15 14:18:27.138722 config-oc-1.0.4/config_oc.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     9019 2024-04-15 14:18:27.000000 config-oc-1.0.4/config_oc.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      296 2024-04-15 14:18:27.000000 config-oc-1.0.4/config_oc.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-04-15 14:18:27.000000 config-oc-1.0.4/config_oc.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       39 2024-04-15 14:18:27.000000 config-oc-1.0.4/config_oc.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        7 2024-04-15 14:18:27.000000 config-oc-1.0.4/config_oc.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-10-10 14:45:31.000000 config-oc-1.0.4/config_oc.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2024-04-15 14:18:27.138722 config-oc-1.0.4/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)      869 2024-04-15 14:05:22.000000 config-oc-1.0.4/setup.py
```

### Comparing `config-oc-1.0.3/LICENSE` & `config-oc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `config-oc-1.0.3/PKG-INFO` & `config-oc-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-oc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Handles loading loading configuration files based on hostname
 Home-page: https://ouroboroscoding.com/config/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/config/
 Project-URL: Source, https://github.com/ouroboroscoding/config-python
```

### Comparing `config-oc-1.0.3/README.md` & `config-oc-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `config-oc-1.0.3/config/conf.py` & `config-oc-1.0.4/config/conf.py`

 * *Files identical despite different names*

### Comparing `config-oc-1.0.3/config/data.py` & `config-oc-1.0.4/config/data.py`

 * *Files identical despite different names*

### Comparing `config-oc-1.0.3/config_oc.egg-info/PKG-INFO` & `config-oc-1.0.4/config_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-oc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Handles loading loading configuration files based on hostname
 Home-page: https://ouroboroscoding.com/config/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/config/
 Project-URL: Source, https://github.com/ouroboroscoding/config-python
```

### Comparing `config-oc-1.0.3/setup.py` & `config-oc-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='config-oc',
-	version='1.0.3',
+	version='1.0.4',
 	description='Handles loading loading configuration files based on hostname',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/config/',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/config/',
 		'Source': 'https://github.com/ouroboroscoding/config-python',
```

