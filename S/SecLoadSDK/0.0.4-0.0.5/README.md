# Comparing `tmp/secloadsdk-0.0.4.tar.gz` & `tmp/secloadsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secloadsdk-0.0.4.tar", last modified: Sun Apr 14 19:28:04 2024, max compression
+gzip compressed data, was "secloadsdk-0.0.5.tar", last modified: Sun Apr 14 21:41:22 2024, max compression
```

## Comparing `secloadsdk-0.0.4.tar` & `secloadsdk-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:28:04.226999 secloadsdk-0.0.4/
--rw-r--r--   0 equsjd    (1000) equsjd    (1000)      299 2024-04-14 19:28:04.222999 secloadsdk-0.0.4/PKG-INFO
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:28:04.222999 secloadsdk-0.0.4/SecLoad/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 secloadsdk-0.0.4/SecLoad/__init__.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4852 2024-04-14 19:25:56.000000 secloadsdk-0.0.4/SecLoad/apihandlers.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 secloadsdk-0.0.4/SecLoad/enums.py
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:28:04.222999 secloadsdk-0.0.4/SecLoadSDK.egg-info/
--rw-r--r--   0 equsjd    (1000) equsjd    (1000)      299 2024-04-14 19:28:04.000000 secloadsdk-0.0.4/SecLoadSDK.egg-info/PKG-INFO
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      237 2024-04-14 19:28:04.000000 secloadsdk-0.0.4/SecLoadSDK.egg-info/SOURCES.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 19:28:04.000000 secloadsdk-0.0.4/SecLoadSDK.egg-info/dependency_links.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 19:28:04.000000 secloadsdk-0.0.4/SecLoadSDK.egg-info/requires.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 19:28:04.000000 secloadsdk-0.0.4/SecLoadSDK.egg-info/top_level.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 19:28:04.226999 secloadsdk-0.0.4/setup.cfg
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      531 2024-04-14 19:27:41.000000 secloadsdk-0.0.4/setup.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.845004 secloadsdk-0.0.5/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)     2963 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     2622 2024-04-14 21:39:48.000000 secloadsdk-0.0.5/README.md
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/SecLoad/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 secloadsdk-0.0.5/SecLoad/__init__.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4852 2024-04-14 19:25:56.000000 secloadsdk-0.0.5/SecLoad/apihandlers.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 secloadsdk-0.0.5/SecLoad/enums.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/SecLoadSDK.egg-info/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)     2963 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      247 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/requires.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/top_level.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 21:41:22.845004 secloadsdk-0.0.5/setup.cfg
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      755 2024-04-14 21:41:05.000000 secloadsdk-0.0.5/setup.py
```

### Comparing `secloadsdk-0.0.4/SecLoad/__init__.py` & `secloadsdk-0.0.5/SecLoad/__init__.py`

 * *Files identical despite different names*

### Comparing `secloadsdk-0.0.4/SecLoad/apihandlers.py` & `secloadsdk-0.0.5/SecLoad/apihandlers.py`

 * *Files identical despite different names*

### Comparing `secloadsdk-0.0.4/setup.py` & `secloadsdk-0.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'SecLoad SDK package for Roblox Script Builder APIs.'
 
 # Setting up
 setup(
         name="SecLoadSDK", 
         version=VERSION,
         author="equsjd",
         description=DESCRIPTION,
+        long_description=long_description,
+        long_description_content_type='text/markdown',
         packages=find_packages(),
         install_requires=['requests_html', 'lxml_html_clean'],
         
         keywords=['roblox'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Programming Language :: Python :: 3",
```

