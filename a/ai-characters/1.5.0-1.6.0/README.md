# Comparing `tmp/ai_characters-1.5.0.tar.gz` & `tmp/ai_characters-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_characters-1.5.0.tar", last modified: Mon Apr  1 23:55:27 2024, max compression
+gzip compressed data, was "ai_characters-1.6.0.tar", last modified: Mon Apr 15 02:44:40 2024, max compression
```

## Comparing `ai_characters-1.5.0.tar` & `ai_characters-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:55:27.485581 ai_characters-1.5.0/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.5.0/LICENSE
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.5.0/MANIFEST.in
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1181 2024-04-01 23:55:27.485287 ai_characters-1.5.0/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.5.0/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:55:27.485044 ai_characters-1.5.0/ai_characters.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1181 2024-04-01 23:55:27.000000 ai_characters-1.5.0/ai_characters.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 23:55:27.000000 ai_characters-1.5.0/ai_characters.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 23:55:27.000000 ai_characters-1.5.0/ai_characters.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       74 2024-04-01 23:55:27.000000 ai_characters-1.5.0/ai_characters.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 23:55:27.000000 ai_characters-1.5.0/ai_characters.egg-info/top_level.txt
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:55:27.484177 ai_characters-1.5.0/aic/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3018 2024-04-01 23:53:19.000000 ai_characters-1.5.0/aic/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.5.0/aic/agent.schema.json
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 23:55:27.485625 ai_characters-1.5.0/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 23:55:12.000000 ai_characters-1.5.0/setup.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:55:27.484652 ai_characters-1.5.0/tests/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.5.0/tests/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.5.0/tests/test_aic.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-15 02:44:40.111271 ai_characters-1.6.0/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.6.0/LICENSE
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.6.0/MANIFEST.in
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1216 2024-04-15 02:44:40.110996 ai_characters-1.6.0/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.6.0/README.md
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-15 02:44:40.110775 ai_characters-1.6.0/ai_characters.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1216 2024-04-15 02:44:40.000000 ai_characters-1.6.0/ai_characters.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-15 02:44:40.000000 ai_characters-1.6.0/ai_characters.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-15 02:44:40.000000 ai_characters-1.6.0/ai_characters.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       94 2024-04-15 02:44:40.000000 ai_characters-1.6.0/ai_characters.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-15 02:44:40.000000 ai_characters-1.6.0/ai_characters.egg-info/top_level.txt
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-15 02:44:40.110185 ai_characters-1.6.0/aic/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3081 2024-04-15 02:41:15.000000 ai_characters-1.6.0/aic/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-15 02:38:34.000000 ai_characters-1.6.0/aic/agent.schema.json
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-15 02:44:40.111316 ai_characters-1.6.0/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-15 02:44:25.000000 ai_characters-1.6.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-15 02:44:40.110508 ai_characters-1.6.0/tests/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.6.0/tests/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.6.0/tests/test_aic.py
```

### Comparing `ai_characters-1.5.0/LICENSE` & `ai_characters-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_characters-1.5.0/PKG-INFO` & `ai_characters-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ai_characters
-Version: 1.5.0
+Version: 1.6.0
 Summary: Client for AI Characters
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-storage==2.16
 Requires-Dist: jsonschema==4.21
 Requires-Dist: aic_tools==1.0.0
+Requires-Dist: aic_tools_fs==0.0.1
 Requires-Dist: crewai==0.22
 
 # YourPackageName
 
 AICharacters (AIC) is a Python client library for service AICharacters that stores different AI characters, mostly tailored for use with Crew AI. It includes functionality to download character configurations from the service, validate them against a predefined schema, and utilize these characters in various contexts.
 
 ## Features
```

### Comparing `ai_characters-1.5.0/README.md` & `ai_characters-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_characters-1.5.0/ai_characters.egg-info/PKG-INFO` & `ai_characters-1.6.0/ai_characters.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ai_characters
-Version: 1.5.0
+Version: 1.6.0
 Summary: Client for AI Characters
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-storage==2.16
 Requires-Dist: jsonschema==4.21
 Requires-Dist: aic_tools==1.0.0
+Requires-Dist: aic_tools_fs==0.0.1
 Requires-Dist: crewai==0.22
 
 # YourPackageName
 
 AICharacters (AIC) is a Python client library for service AICharacters that stores different AI characters, mostly tailored for use with Crew AI. It includes functionality to download character configurations from the service, validate them against a predefined schema, and utilize these characters in various contexts.
 
 ## Features
```

### Comparing `ai_characters-1.5.0/aic/__init__.py` & `ai_characters-1.6.0/aic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from google.cloud import storage
 from jsonschema import validate
 from typing import List, Any
 from pkg_resources import resource_string, resource_exists
 from crewai import Agent
 from aic_tools.datetime import get_datetime
+from aic_tools_fs import ls, cat
 
 import json
 
 BUCKET_NAME="ai-characters"
 TOOLS = {
-    "DATETIME": get_datetime
+    "DATETIME": get_datetime,
+    "ls": ls,
+    "cat": cat
 }
 
 class AICharacter:
     def __init__(self, version: str, roleName: str, backstory: str, tools: List[str]):
         self.version = version
         self.roleName = roleName
         self.backstory = backstory
```

### Comparing `ai_characters-1.5.0/aic/agent.schema.json` & `ai_characters-1.6.0/aic/agent.schema.json`

 * *Files identical despite different names*

### Comparing `ai_characters-1.5.0/setup.py` & `ai_characters-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='ai_characters',
-    version='1.5.0',
+    version='1.6.0',
     packages=find_packages(),
     description='Client for AI Characters',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
```

### Comparing `ai_characters-1.5.0/tests/test_aic.py` & `ai_characters-1.6.0/tests/test_aic.py`

 * *Files identical despite different names*

