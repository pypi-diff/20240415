# Comparing `tmp/composio_autogen-0.1.99.tar.gz` & `tmp/composio_autogen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.99.tar", last modified: Fri Apr 12 15:24:39 2024, max compression
+gzip compressed data, was "composio_autogen-0.2.0.tar", last modified: Mon Apr 15 09:07:59 2024, max compression
```

## Comparing `composio_autogen-0.1.99.tar` & `composio_autogen-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:39.749721 composio_autogen-0.1.99/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-12 15:24:39.749506 composio_autogen-0.1.99/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.99/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:39.748555 composio_autogen-0.1.99/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)      100 2024-04-12 09:34:34.000000 composio_autogen-0.1.99/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     8467 2024-04-12 01:14:55.000000 composio_autogen-0.1.99/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:39.749336 composio_autogen-0.1.99/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-12 15:24:39.000000 composio_autogen-0.1.99/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-12 15:24:39.000000 composio_autogen-0.1.99/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:24:39.000000 composio_autogen-0.1.99/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-12 15:24:39.000000 composio_autogen-0.1.99/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-12 15:24:39.000000 composio_autogen-0.1.99/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-12 15:24:05.000000 composio_autogen-0.1.99/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:24:39.749756 composio_autogen-0.1.99/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-12 15:24:05.000000 composio_autogen-0.1.99/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:59.444744 composio_autogen-0.2.0/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-15 09:07:59.444500 composio_autogen-0.2.0/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-15 07:39:40.000000 composio_autogen-0.2.0/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:59.443208 composio_autogen-0.2.0/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      100 2024-04-15 07:39:40.000000 composio_autogen-0.2.0/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     8467 2024-04-15 07:39:40.000000 composio_autogen-0.2.0/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:59.444243 composio_autogen-0.2.0/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-15 09:07:59.000000 composio_autogen-0.2.0/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-15 09:07:59.000000 composio_autogen-0.2.0/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-15 09:07:59.000000 composio_autogen-0.2.0/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-04-15 09:07:59.000000 composio_autogen-0.2.0/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-15 09:07:59.000000 composio_autogen-0.2.0/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-15 09:07:06.000000 composio_autogen-0.2.0/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-15 09:07:59.444798 composio_autogen-0.2.0/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      840 2024-04-15 09:07:06.000000 composio_autogen-0.2.0/setup.py
```

### Comparing `composio_autogen-0.1.99/PKG-INFO` & `composio_autogen-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.99
+Version: 0.2.0
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.99
+Requires-Dist: composio_core===0.2.0
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.99/README.md` & `composio_autogen-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.99/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.2.0/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.99/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.2.0/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.99
+Version: 0.2.0
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.99
+Requires-Dist: composio_core===0.2.0
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.99/setup.py` & `composio_autogen-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.99",
+    version="0.2.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

