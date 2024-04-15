# Comparing `tmp/lookout_config-1.1.0.tar.gz` & `tmp/lookout_config-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookout_config-1.1.0.tar", last modified: Mon Apr 15 02:35:31 2024, max compression
+gzip compressed data, was "lookout_config-1.1.1.tar", last modified: Mon Apr 15 06:57:06 2024, max compression
```

## Comparing `lookout_config-1.1.0.tar` & `lookout_config-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 02:35:31.793450 lookout_config-1.1.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 02:35:31.793450 lookout_config-1.1.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-15 02:34:22.000000 lookout_config-1.1.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 02:35:31.793450 lookout_config-1.1.0/lookout_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6529 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/generate_cameras.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/generate_urdf.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 02:35:31.793450 lookout_config-1.1.0/lookout_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/schemas/lookout.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 02:35:31.793450 lookout_config-1.1.0/lookout_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-15 02:34:22.000000 lookout_config-1.1.0/lookout_config/test/lookout_config_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 02:35:31.793450 lookout_config-1.1.0/lookout_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 02:35:31.000000 lookout_config-1.1.0/lookout_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-15 02:35:31.000000 lookout_config-1.1.0/lookout_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 02:35:31.000000 lookout_config-1.1.0/lookout_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-15 02:35:31.000000 lookout_config-1.1.0/lookout_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-15 02:35:31.000000 lookout_config-1.1.0/lookout_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 02:35:17.000000 lookout_config-1.1.0/lookout_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-15 02:35:31.793450 lookout_config-1.1.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 02:34:22.000000 lookout_config-1.1.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 06:57:06.528328 lookout_config-1.1.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 06:57:06.528328 lookout_config-1.1.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-15 06:56:10.000000 lookout_config-1.1.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 06:57:06.528328 lookout_config-1.1.1/lookout_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6529 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/generate_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/generate_urdf.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 06:57:06.528328 lookout_config-1.1.1/lookout_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/schemas/lookout.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 06:57:06.528328 lookout_config-1.1.1/lookout_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-15 06:56:10.000000 lookout_config-1.1.1/lookout_config/test/lookout_config_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 06:57:06.528328 lookout_config-1.1.1/lookout_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 06:57:06.000000 lookout_config-1.1.1/lookout_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-15 06:57:06.000000 lookout_config-1.1.1/lookout_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 06:57:06.000000 lookout_config-1.1.1/lookout_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-15 06:57:06.000000 lookout_config-1.1.1/lookout_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-15 06:57:06.000000 lookout_config-1.1.1/lookout_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 06:56:55.000000 lookout_config-1.1.1/lookout_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-15 06:57:06.528328 lookout_config-1.1.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 06:56:10.000000 lookout_config-1.1.1/setup.py
```

### Comparing `lookout_config-1.1.0/PKG-INFO` & `lookout_config-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.1.0/README.md` & `lookout_config-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lookout_config-1.1.0/lookout_config/__init__.py` & `lookout_config-1.1.1/lookout_config/__init__.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.1.0/lookout_config/generate_cameras.py` & `lookout_config-1.1.1/lookout_config/generate_cameras.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.1.0/lookout_config/generate_urdf.py` & `lookout_config-1.1.1/lookout_config/generate_urdf.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.1.0/lookout_config/schemas/lookout.schema.json` & `lookout_config-1.1.1/lookout_config/schemas/lookout.schema.json`

 * *Files identical despite different names*

### Comparing `lookout_config-1.1.0/lookout_config.egg-info/PKG-INFO` & `lookout_config-1.1.1/lookout_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.1.0/setup.cfg` & `lookout_config-1.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lookout_config
-version = 1.1.0
+version = 1.1.1
 url = https://github.com/Greenroom-Robotics/lookout
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

