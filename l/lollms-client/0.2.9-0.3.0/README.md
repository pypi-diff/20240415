# Comparing `tmp/lollms_client-0.2.9.tar.gz` & `tmp/lollms_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.2.9.tar", last modified: Thu Apr 11 22:35:00 2024, max compression
+gzip compressed data, was "lollms_client-0.3.0.tar", last modified: Mon Apr 15 00:18:23 2024, max compression
```

## Comparing `lollms_client-0.2.9.tar` & `lollms_client-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 22:35:00.448047 lollms_client-0.2.9/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-11 22:35:00.446972 lollms_client-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 22:35:00.424966 lollms_client-0.2.9/lollms_client/
--rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.9/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-04-11 22:34:40.000000 lollms_client-0.2.9/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.9/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.9/lollms_client/lollms_types.py
-drwxrwxrwx   0        0        0        0 2024-04-11 22:35:00.445977 lollms_client-0.2.9/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-11 22:35:00.000000 lollms_client-0.2.9/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-11 22:35:00.000000 lollms_client-0.2.9/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 22:35:00.000000 lollms_client-0.2.9/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 22:35:00.000000 lollms_client-0.2.9/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 22:35:00.000000 lollms_client-0.2.9/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 22:35:00.448047 lollms_client-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-11 22:34:47.000000 lollms_client-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:18:23.580191 lollms_client-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-15 00:18:23.579191 lollms_client-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 00:18:23.558191 lollms_client-0.3.0/lollms_client/
+-rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.3.0/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    13006 2024-04-11 22:34:40.000000 lollms_client-0.3.0/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.3.0/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.3.0/lollms_client/lollms_types.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:18:23.578190 lollms_client-0.3.0/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-15 00:18:23.000000 lollms_client-0.3.0/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-04-15 00:18:23.000000 lollms_client-0.3.0/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:18:23.000000 lollms_client-0.3.0/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 00:18:23.000000 lollms_client-0.3.0/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 00:18:23.000000 lollms_client-0.3.0/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:18:23.580191 lollms_client-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-04-14 20:20:19.000000 lollms_client-0.3.0/setup.py
```

### Comparing `lollms_client-0.2.9/LICENSE` & `lollms_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.9/PKG-INFO` & `lollms_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.9
+Version: 0.3.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.9/README.md` & `lollms_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.9/lollms_client/lollms_core.py` & `lollms_client-0.3.0/lollms_client/lollms_core.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.9/lollms_client/lollms_tasks.py` & `lollms_client-0.3.0/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.9/lollms_client/lollms_types.py` & `lollms_client-0.3.0/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.9/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.3.0/lollms_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.9
+Version: 0.3.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.9/setup.py` & `lollms_client-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+with open('requirements.txt', 'r') as f:
+    install_requires = f.read().splitlines()
+    
 setuptools.setup(
     name="lollms_client",
-    version="0.2.9",
+    version="0.3.0",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

