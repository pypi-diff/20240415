# Comparing `tmp/secloadsdk-0.0.5.tar.gz` & `tmp/secloadsdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secloadsdk-0.0.5.tar", last modified: Sun Apr 14 21:41:22 2024, max compression
+gzip compressed data, was "secloadsdk-0.0.6.tar", last modified: Sun Apr 14 22:00:14 2024, max compression
```

## Comparing `secloadsdk-0.0.5.tar` & `secloadsdk-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.845004 secloadsdk-0.0.5/
--rw-r--r--   0 equsjd    (1000) equsjd    (1000)     2963 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/PKG-INFO
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     2622 2024-04-14 21:39:48.000000 secloadsdk-0.0.5/README.md
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/SecLoad/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 secloadsdk-0.0.5/SecLoad/__init__.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4852 2024-04-14 19:25:56.000000 secloadsdk-0.0.5/SecLoad/apihandlers.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 secloadsdk-0.0.5/SecLoad/enums.py
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 21:41:22.841004 secloadsdk-0.0.5/SecLoadSDK.egg-info/
--rw-r--r--   0 equsjd    (1000) equsjd    (1000)     2963 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/PKG-INFO
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      247 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/SOURCES.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/dependency_links.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/requires.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 21:41:22.000000 secloadsdk-0.0.5/SecLoadSDK.egg-info/top_level.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 21:41:22.845004 secloadsdk-0.0.5/setup.cfg
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      755 2024-04-14 21:41:05.000000 secloadsdk-0.0.5/setup.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 22:00:14.034319 secloadsdk-0.0.6/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)     3281 2024-04-14 22:00:14.030319 secloadsdk-0.0.6/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     2940 2024-04-14 21:55:56.000000 secloadsdk-0.0.6/README.md
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 22:00:14.030319 secloadsdk-0.0.6/SecLoad/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 secloadsdk-0.0.6/SecLoad/__init__.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4852 2024-04-14 19:25:56.000000 secloadsdk-0.0.6/SecLoad/apihandlers.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 secloadsdk-0.0.6/SecLoad/enums.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 22:00:14.030319 secloadsdk-0.0.6/SecLoadSDK.egg-info/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)     3281 2024-04-14 22:00:14.000000 secloadsdk-0.0.6/SecLoadSDK.egg-info/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      247 2024-04-14 22:00:14.000000 secloadsdk-0.0.6/SecLoadSDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 22:00:14.000000 secloadsdk-0.0.6/SecLoadSDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 22:00:14.000000 secloadsdk-0.0.6/SecLoadSDK.egg-info/requires.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 22:00:14.000000 secloadsdk-0.0.6/SecLoadSDK.egg-info/top_level.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 22:00:14.034319 secloadsdk-0.0.6/setup.cfg
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      755 2024-04-14 21:59:39.000000 secloadsdk-0.0.6/setup.py
```

### Comparing `secloadsdk-0.0.5/PKG-INFO` & `secloadsdk-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1
-Name: SecLoadSDK
-Version: 0.0.5
-Summary: SecLoad SDK package for Roblox Script Builder APIs.
-Author: equsjd
-Keywords: roblox
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Requires-Dist: requests_html
-Requires-Dist: lxml_html_clean
-
 # Secload SDK
 ##### Made for Roblox SB games
 ##### Created by equsjd and the help of Cparke
+
+![PyPI - Version](https://img.shields.io/pypi/v/secloadsdk)![PyPI - License](https://img.shields.io/pypi/l/SecLoadSDK?link=https%3A%2F%2Fsecload.scriptlang.com%2Flicense)![Discord](https://img.shields.io/discord/1178213683839651891?logo=discord&logoColor=FFF&color=454FBF&link=https%3A%2F%2Fdiscord.gg%2FJJhxSTn6Nk)
+
 # Usage
 ## Installation
 To install, run this in a CLI. It should automatically install the dependancies too
 ```sh
 pip install secloadsdk
 ```
 
@@ -100,8 +91,8 @@
 
 secload.AddScript()
 secload.RemoveScript()
 secload.OverwriteScript()
 secload.GetScriptSource() # -> returns a string with the script source
 secload.ListScripts() # -> returns a python list
 secload.GenerateKey() # -> returns the script EXAMPLE: require(idhere)("key", "key2", "username", true)
-```
+```
```

### Comparing `secloadsdk-0.0.5/SecLoad/__init__.py` & `secloadsdk-0.0.6/SecLoad/__init__.py`

 * *Files identical despite different names*

### Comparing `secloadsdk-0.0.5/SecLoad/apihandlers.py` & `secloadsdk-0.0.6/SecLoad/apihandlers.py`

 * *Files identical despite different names*

### Comparing `secloadsdk-0.0.5/SecLoadSDK.egg-info/PKG-INFO` & `secloadsdk-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: SecLoadSDK
-Version: 0.0.5
+Version: 0.0.6
 Summary: SecLoad SDK package for Roblox Script Builder APIs.
 Author: equsjd
 Keywords: roblox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: requests_html
 Requires-Dist: lxml_html_clean
 
 # Secload SDK
 ##### Made for Roblox SB games
 ##### Created by equsjd and the help of Cparke
+
+![PyPI - Version](https://img.shields.io/pypi/v/secloadsdk)![PyPI - License](https://img.shields.io/pypi/l/SecLoadSDK?link=https%3A%2F%2Fsecload.scriptlang.com%2Flicense)![Discord](https://img.shields.io/discord/1178213683839651891?logo=discord&logoColor=FFF&color=454FBF&link=https%3A%2F%2Fdiscord.gg%2FJJhxSTn6Nk)
+
 # Usage
 ## Installation
 To install, run this in a CLI. It should automatically install the dependancies too
 ```sh
 pip install secloadsdk
 ```
```

### Comparing `secloadsdk-0.0.5/setup.py` & `secloadsdk-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'SecLoad SDK package for Roblox Script Builder APIs.'
 
 # Setting up
 setup(
         name="SecLoadSDK", 
         version=VERSION,
         author="equsjd",
```

