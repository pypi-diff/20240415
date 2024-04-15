# Comparing `tmp/sysrev-1.2.2.tar.gz` & `tmp/sysrev-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.2.2.tar", last modified: Mon Apr 15 13:30:44 2024, max compression
+gzip compressed data, was "sysrev-1.2.3.tar", last modified: Mon Apr 15 13:38:51 2024, max compression
```

## Comparing `sysrev-1.2.2.tar` & `sysrev-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.701321 sysrev-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:30:44.701321 sysrev-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:30:39.000000 sysrev-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:30:44.701321 sysrev-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:30:39.000000 sysrev-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.697321 sysrev-1.2.2/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:30:39.000000 sysrev-1.2.2/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-15 13:30:39.000000 sysrev-1.2.2/sysrev/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.701321 sysrev-1.2.2/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:38:50.993237 sysrev-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:38:50.993237 sysrev-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:38:45.000000 sysrev-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:38:50.993237 sysrev-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:38:45.000000 sysrev-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:38:50.993237 sysrev-1.2.3/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 13:38:45.000000 sysrev-1.2.3/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-15 13:38:45.000000 sysrev-1.2.3/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:38:50.993237 sysrev-1.2.3/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:38:50.000000 sysrev-1.2.3/sysrev.egg-info/top_level.txt
```

### Comparing `sysrev-1.2.2/PKG-INFO` & `sysrev-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.2.2
+Version: 1.2.3
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.2.2/setup.py` & `sysrev-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.2.2',
+    version='1.2.3',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.2.2/sysrev/funcs.py` & `sysrev-1.2.3/sysrev/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if label_type == 'boolean':
             return self.handle_boolean(label_value)
         elif label_type in ['categorical', 'string']:
             return self.handle_categorical_or_string(label_value)
         else:
             raise ValueError("Invalid label type")
         
-class SysrevClient():
+class Client():
     
     def __init__(self, api_key, base_url="https://www.sysrev.com"):
         self.api_key = api_key
         self.base_url = base_url
     
     def get_project_info(self, project_id):
         endpoint = f"{self.base_url}/api-json/project-info"
```

### Comparing `sysrev-1.2.2/sysrev.egg-info/PKG-INFO` & `sysrev-1.2.3/sysrev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.2.2
+Version: 1.2.3
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```
