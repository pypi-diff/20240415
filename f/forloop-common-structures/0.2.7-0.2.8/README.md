# Comparing `tmp/forloop_common_structures-0.2.7.tar.gz` & `tmp/forloop_common_structures-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_common_structures-0.2.7.tar", last modified: Tue Apr  9 16:33:35 2024, max compression
+gzip compressed data, was "forloop_common_structures-0.2.8.tar", last modified: Mon Apr 15 11:28:23 2024, max compression
```

## Comparing `forloop_common_structures-0.2.7.tar` & `forloop_common_structures-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:33:35.680895 forloop_common_structures-0.2.7/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      569 2024-04-09 16:33:35.679663 forloop_common_structures-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       27 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:33:35.492722 forloop_common_structures-0.2.7/forloop_common_structures/
--rw-rw-rw-   0        0        0       61 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:33:35.678676 forloop_common_structures-0.2.7/forloop_common_structures/core/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/__init__.py
--rw-rw-rw-   0        0        0      290 2024-04-08 16:59:44.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/database.py
--rw-rw-rw-   0        0        0      414 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/dataset.py
--rw-rw-rw-   0        0        0      576 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/dbtable.py
--rw-rw-rw-   0        0        0      566 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/edge.py
--rw-rw-rw-   0        0        0      498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/file.py
--rw-rw-rw-   0        0        0     1498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/initial_variable.py
--rw-rw-rw-   0        0        0     5017 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/job.py
--rw-rw-rw-   0        0        0     6034 2024-02-22 17:35:42.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/node.py
--rw-rw-rw-   0        0        0      872 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/pipeline.py
--rw-rw-rw-   0        0        0      477 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/popup.py
--rw-rw-rw-   0        0        0     1104 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/project.py
--rw-rw-rw-   0        0        0      788 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/result.py
--rw-rw-rw-   0        0        0      404 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/script.py
--rw-rw-rw-   0        0        0      757 2024-04-09 16:33:10.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/session.py
--rw-rw-rw-   0        0        0      359 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/trigger.py
--rw-rw-rw-   0        0        0      230 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/user.py
--rw-rw-rw-   0        0        0      254 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/user_flow_step.py
--rw-rw-rw-   0        0        0     1575 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.7/forloop_common_structures/core/variable.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:33:35.526240 forloop_common_structures-0.2.7/forloop_common_structures.egg-info/
--rw-rw-rw-   0        0        0      569 2024-04-09 16:33:35.000000 forloop_common_structures-0.2.7/forloop_common_structures.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-04-09 16:33:35.000000 forloop_common_structures-0.2.7/forloop_common_structures.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:33:35.000000 forloop_common_structures-0.2.7/forloop_common_structures.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-09 16:33:35.000000 forloop_common_structures-0.2.7/forloop_common_structures.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:33:35.680895 forloop_common_structures-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      823 2024-04-09 16:33:15.000000 forloop_common_structures-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:23.881169 forloop_common_structures-0.2.8/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      569 2024-04-15 11:28:23.881169 forloop_common_structures-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:23.648454 forloop_common_structures-0.2.8/forloop_common_structures/
+-rw-rw-rw-   0        0        0       61 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:23.879212 forloop_common_structures-0.2.8/forloop_common_structures/core/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/__init__.py
+-rw-rw-rw-   0        0        0      305 2024-04-15 11:27:44.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/database.py
+-rw-rw-rw-   0        0        0      414 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/dataset.py
+-rw-rw-rw-   0        0        0      576 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/dbtable.py
+-rw-rw-rw-   0        0        0      566 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/edge.py
+-rw-rw-rw-   0        0        0      498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/file.py
+-rw-rw-rw-   0        0        0     1498 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/initial_variable.py
+-rw-rw-rw-   0        0        0     5017 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/job.py
+-rw-rw-rw-   0        0        0     6034 2024-02-22 17:35:42.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/node.py
+-rw-rw-rw-   0        0        0      872 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/pipeline.py
+-rw-rw-rw-   0        0        0      477 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/popup.py
+-rw-rw-rw-   0        0        0     1104 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/project.py
+-rw-rw-rw-   0        0        0      788 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/result.py
+-rw-rw-rw-   0        0        0      404 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/script.py
+-rw-rw-rw-   0        0        0      757 2024-04-09 16:33:10.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/session.py
+-rw-rw-rw-   0        0        0      359 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/trigger.py
+-rw-rw-rw-   0        0        0      230 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/user.py
+-rw-rw-rw-   0        0        0      254 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/user_flow_step.py
+-rw-rw-rw-   0        0        0     1575 2024-02-22 17:35:35.000000 forloop_common_structures-0.2.8/forloop_common_structures/core/variable.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:28:23.677769 forloop_common_structures-0.2.8/forloop_common_structures.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-15 11:28:23.000000 forloop_common_structures-0.2.8/forloop_common_structures.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-04-15 11:28:23.000000 forloop_common_structures-0.2.8/forloop_common_structures.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:28:23.000000 forloop_common_structures-0.2.8/forloop_common_structures.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-15 11:28:23.000000 forloop_common_structures-0.2.8/forloop_common_structures.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:28:23.881169 forloop_common_structures-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      823 2024-04-15 11:28:00.000000 forloop_common_structures-0.2.8/setup.py
```

### Comparing `forloop_common_structures-0.2.7/LICENSE` & `forloop_common_structures-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/PKG-INFO` & `forloop_common_structures-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_common_structures
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package contains open source core structures and schemas within Forloop.ai execution core and API
 Home-page: https://github.com/ForloopAI/forloop_common_structures
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/dbtable.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/dbtable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/edge.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/edge.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/initial_variable.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/initial_variable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/job.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/job.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/node.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/node.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/pipeline.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/project.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/project.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/result.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/result.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/session.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/session.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures/core/variable.py` & `forloop_common_structures-0.2.8/forloop_common_structures/core/variable.py`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures.egg-info/PKG-INFO` & `forloop_common_structures-0.2.8/forloop_common_structures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-common-structures
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package contains open source core structures and schemas within Forloop.ai execution core and API
 Home-page: https://github.com/ForloopAI/forloop_common_structures
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_common_structures-0.2.7/forloop_common_structures.egg-info/SOURCES.txt` & `forloop_common_structures-0.2.8/forloop_common_structures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_common_structures-0.2.7/setup.py` & `forloop_common_structures-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_common_structures',
-    version='0.2.7',
+    version='0.2.8',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source core structures and schemas within Forloop.ai execution core and API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_common_structures',
     packages=setuptools.find_packages(),
```

