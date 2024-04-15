# Comparing `tmp/mageic_common-0.1.0.tar.gz` & `tmp/mageic_common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mageic_common-0.1.0.tar", last modified: Mon Apr 15 15:56:50 2024, max compression
+gzip compressed data, was "mageic_common-0.2.0.tar", last modified: Mon Apr 15 16:57:01 2024, max compression
```

## Comparing `mageic_common-0.1.0.tar` & `mageic_common-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.861306 mageic_common-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 15:56:44.000000 mageic_common-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 15:56:50.861306 mageic_common-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 15:56:44.000000 mageic_common-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.857306 mageic_common-0.1.0/mageic_common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.857306 mageic_common-0.1.0/mageic_common/enum/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.857306 mageic_common-0.1.0/mageic_common/enum/models/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/face_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/enum/models/upscaler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.857306 mageic_common-0.1.0/mageic_common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.861306 mageic_common-0.1.0/mageic_common/models/io/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-15 15:56:44.000000 mageic_common-0.1.0/mageic_common/models/io/moderation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:56:50.861306 mageic_common-0.1.0/mageic_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 15:56:50.000000 mageic_common-0.1.0/mageic_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-15 15:56:50.000000 mageic_common-0.1.0/mageic_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:56:50.000000 mageic_common-0.1.0/mageic_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 15:56:50.000000 mageic_common-0.1.0/mageic_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 15:56:50.000000 mageic_common-0.1.0/mageic_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:56:50.861306 mageic_common-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 15:56:44.000000 mageic_common-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.374429 mageic_common-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 16:56:51.000000 mageic_common-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 16:57:01.374429 mageic_common-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 16:56:51.000000 mageic_common-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.366429 mageic_common-0.2.0/mageic_common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.370429 mageic_common-0.2.0/mageic_common/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.370429 mageic_common-0.2.0/mageic_common/enum/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/apps/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.370429 mageic_common-0.2.0/mageic_common/enum/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/face_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/enum/models/upscaler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.370429 mageic_common-0.2.0/mageic_common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.370429 mageic_common-0.2.0/mageic_common/models/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/backend/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/backend/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.374429 mageic_common-0.2.0/mageic_common/models/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-15 16:56:51.000000 mageic_common-0.2.0/mageic_common/models/io/moderation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:57:01.374429 mageic_common-0.2.0/mageic_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 16:57:01.000000 mageic_common-0.2.0/mageic_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 16:57:01.000000 mageic_common-0.2.0/mageic_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:57:01.000000 mageic_common-0.2.0/mageic_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 16:57:01.000000 mageic_common-0.2.0/mageic_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 16:57:01.000000 mageic_common-0.2.0/mageic_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:57:01.374429 mageic_common-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 16:56:51.000000 mageic_common-0.2.0/setup.py
```

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/__init__.py` & `mageic_common-0.2.0/mageic_common/enum/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/adapter.py` & `mageic_common-0.2.0/mageic_common/enum/models/adapter.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/base.py` & `mageic_common-0.2.0/mageic_common/enum/models/base.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/controlnet.py` & `mageic_common-0.2.0/mageic_common/enum/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/face_analysis.py` & `mageic_common-0.2.0/mageic_common/enum/models/face_analysis.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/scheduler.py` & `mageic_common-0.2.0/mageic_common/enum/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/enum/models/upscaler.py` & `mageic_common-0.2.0/mageic_common/enum/models/upscaler.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/__init__.py` & `mageic_common-0.2.0/mageic_common/models/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/adapter.py` & `mageic_common-0.2.0/mageic_common/models/io/adapter.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/app.py` & `mageic_common-0.2.0/mageic_common/models/io/app.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/base.py` & `mageic_common-0.2.0/mageic_common/models/io/base.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/controlnet.py` & `mageic_common-0.2.0/mageic_common/models/io/controlnet.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common/models/io/moderation.py` & `mageic_common-0.2.0/mageic_common/models/io/moderation.py`

 * *Files identical despite different names*

### Comparing `mageic_common-0.1.0/mageic_common.egg-info/SOURCES.txt` & `mageic_common-0.2.0/mageic_common.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 mageic_common/__init__.py
 mageic_common.egg-info/PKG-INFO
 mageic_common.egg-info/SOURCES.txt
 mageic_common.egg-info/dependency_links.txt
 mageic_common.egg-info/requires.txt
 mageic_common.egg-info/top_level.txt
 mageic_common/enum/__init__.py
+mageic_common/enum/apps/__init__.py
+mageic_common/enum/apps/type.py
 mageic_common/enum/models/__init__.py
 mageic_common/enum/models/adapter.py
 mageic_common/enum/models/base.py
 mageic_common/enum/models/controlnet.py
 mageic_common/enum/models/face_analysis.py
 mageic_common/enum/models/scheduler.py
 mageic_common/enum/models/upscaler.py
 mageic_common/models/__init__.py
+mageic_common/models/backend/__init__.py
+mageic_common/models/backend/run.py
+mageic_common/models/backend/test.py
 mageic_common/models/io/__init__.py
 mageic_common/models/io/adapter.py
 mageic_common/models/io/app.py
 mageic_common/models/io/base.py
 mageic_common/models/io/controlnet.py
 mageic_common/models/io/moderation.py
```

### Comparing `mageic_common-0.1.0/setup.py` & `mageic_common-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Read the contents of your requirements.txt file
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="mageic-common",
-    version="0.1.0",
+    version="0.2.0",
     author="Gregory D. Hunkins",
     author_email="greg@ollano.com",
     packages=find_packages(),
     license=open("LICENSE.txt").read(),
     long_description=open("README.md").read(),
     install_requires=required,
 )
```

