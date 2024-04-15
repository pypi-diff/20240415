# Comparing `tmp/dialog-workflow-local-0.0.95.tar.gz` & `tmp/dialog_workflow_local-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.95.tar", last modified: Fri Apr 12 04:18:20 2024, max compression
+gzip compressed data, was "dialog_workflow_local-0.0.96.tar", last modified: Mon Apr 15 04:06:56 2024, max compression
```

## Comparing `dialog-workflow-local-0.0.95.tar` & `dialog_workflow_local-0.0.96.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:18:20.940053 dialog-workflow-local-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 04:18:20.940053 dialog-workflow-local-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:18:20.936053 dialog-workflow-local-0.0.95/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:18:20.940053 dialog-workflow-local-0.0.95/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29813 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:18:20.940053 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 04:18:20.000000 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 04:18:20.000000 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:18:20.000000 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 04:18:20.000000 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 04:18:20.000000 dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 04:18:20.940053 dialog-workflow-local-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 04:17:55.000000 dialog-workflow-local-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:06:56.698418 dialog_workflow_local-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 04:06:56.694418 dialog_workflow_local-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:06:56.690418 dialog_workflow_local-0.0.96/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:06:56.694418 dialog_workflow_local-0.0.96/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29813 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:06:56.694418 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 04:06:56.000000 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 04:06:56.000000 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:06:56.000000 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 04:06:56.000000 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 04:06:56.000000 dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:06:56.698418 dialog_workflow_local-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 04:06:26.000000 dialog_workflow_local-0.0.96/setup.py
```

### Comparing `dialog-workflow-local-0.0.95/PKG-INFO` & `dialog_workflow_local-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.95
+Version: 0.0.96
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.95/README.md` & `dialog_workflow_local-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local/src/Constants.py` & `dialog_workflow_local-0.0.96/dialog_workflow_local/src/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local/src/DialogWorkflow.py` & `dialog_workflow_local-0.0.96/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local/src/ProfileContext.py` & `dialog_workflow_local-0.0.96/dialog_workflow_local/src/ProfileContext.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local/src/action.py` & `dialog_workflow_local-0.0.96/dialog_workflow_local/src/action.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local/src/utils.py` & `dialog_workflow_local-0.0.96/dialog_workflow_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.95/dialog_workflow_local.egg-info/PKG-INFO` & `dialog_workflow_local-0.0.96/dialog_workflow_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.95
+Version: 0.0.96
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.95/setup.py` & `dialog_workflow_local-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.95',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.96',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

