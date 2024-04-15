# Comparing `tmp/psd2fabric-0.1.tar.gz` & `tmp/psd2fabric-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psd2fabric-0.1.tar", last modified: Sat Apr 13 03:44:41 2024, max compression
+gzip compressed data, was "psd2fabric-0.2.tar", last modified: Mon Apr 15 11:55:57 2024, max compression
```

## Comparing `psd2fabric-0.1.tar` & `psd2fabric-0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.631854 psd2fabric-0.1/
--rw-r--r--   0 haibing    (501) staff       (20)       85 2024-04-13 03:44:41.631391 psd2fabric-0.1/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-04-13 03:35:22.000000 psd2fabric-0.1/README.md
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.617384 psd2fabric-0.1/psd2fabric/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.623324 psd2fabric-0.1/psd2fabric/fabric/
--rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/fabric/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      533 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/fabric/group.py
--rw-r--r--   0 haibing    (501) staff       (20)      398 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/fabric/image.py
--rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/fabric/text.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.627352 psd2fabric-0.1/psd2fabric/parser/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/parser/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.629524 psd2fabric-0.1/psd2fabric/parser/effects/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/parser/effects/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/parser/effects/coloroverlay_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/parser/effects/stroke_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/parser/group_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      516 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/parser/image_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/parser/psd_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/parser/type_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      288 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/psd_fabric.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.630649 psd2fabric-0.1/psd2fabric/render/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-01-03 14:13:52.000000 psd2fabric-0.1/psd2fabric/render/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-13 03:35:23.000000 psd2fabric-0.1/psd2fabric/render/json_render.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-13 03:44:41.619954 psd2fabric-0.1/psd2fabric.egg-info/
--rw-r--r--   0 haibing    (501) staff       (20)       85 2024-04-13 03:44:41.000000 psd2fabric-0.1/psd2fabric.egg-info/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)      701 2024-04-13 03:44:41.000000 psd2fabric-0.1/psd2fabric.egg-info/SOURCES.txt
--rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-13 03:44:41.000000 psd2fabric-0.1/psd2fabric.egg-info/dependency_links.txt
--rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-13 03:44:41.000000 psd2fabric-0.1/psd2fabric.egg-info/requires.txt
--rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-13 03:44:41.000000 psd2fabric-0.1/psd2fabric.egg-info/top_level.txt
--rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-13 03:44:41.631956 psd2fabric-0.1/setup.cfg
--rw-r--r--   0 haibing    (501) staff       (20)      184 2024-01-03 14:30:49.000000 psd2fabric-0.1/setup.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.574142 psd2fabric-0.2/
+-rw-r--r--   0 haibing    (501) staff       (20)       85 2024-04-15 11:55:57.573870 psd2fabric-0.2/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-02-05 07:08:02.000000 psd2fabric-0.2/README.md
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.570030 psd2fabric-0.2/psd2fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.571710 psd2fabric-0.2/psd2fabric/fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/fabric/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      533 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/fabric/group.py
+-rw-r--r--   0 haibing    (501) staff       (20)      398 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/fabric/image.py
+-rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/fabric/text.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.572372 psd2fabric-0.2/psd2fabric/parser/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/parser/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.572826 psd2fabric-0.2/psd2fabric/parser/effects/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/parser/effects/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/parser/effects/coloroverlay_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/parser/effects/stroke_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/parser/group_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      516 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/parser/image_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/parser/psd_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/parser/type_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      288 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/psd_fabric.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.573069 psd2fabric-0.2/psd2fabric/render/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.2/psd2fabric/render/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-15 11:42:40.000000 psd2fabric-0.2/psd2fabric/render/json_render.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 11:55:57.573281 psd2fabric-0.2/psd2fabric.egg-info/
+-rw-r--r--   0 haibing    (501) staff       (20)       85 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)      738 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       55 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/entry_points.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/requires.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-15 11:55:57.000000 psd2fabric-0.2/psd2fabric.egg-info/top_level.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-15 11:55:57.574204 psd2fabric-0.2/setup.cfg
+-rw-r--r--   0 haibing    (501) staff       (20)      299 2024-04-15 11:53:50.000000 psd2fabric-0.2/setup.py
```

### Comparing `psd2fabric-0.1/README.md` & `psd2fabric-0.2/README.md`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/fabric/__init__.py` & `psd2fabric-0.2/psd2fabric/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/fabric/group.py` & `psd2fabric-0.2/psd2fabric/fabric/group.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/fabric/text.py` & `psd2fabric-0.2/psd2fabric/fabric/text.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/parser/image_parser.py` & `psd2fabric-0.2/psd2fabric/parser/image_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/parser/psd_parser.py` & `psd2fabric-0.2/psd2fabric/parser/psd_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric/parser/type_parser.py` & `psd2fabric-0.2/psd2fabric/parser/type_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1/psd2fabric.egg-info/SOURCES.txt` & `psd2fabric-0.2/psd2fabric.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 psd2fabric/__init__.py
 psd2fabric/psd_fabric.py
 psd2fabric.egg-info/PKG-INFO
 psd2fabric.egg-info/SOURCES.txt
 psd2fabric.egg-info/dependency_links.txt
+psd2fabric.egg-info/entry_points.txt
 psd2fabric.egg-info/requires.txt
 psd2fabric.egg-info/top_level.txt
 psd2fabric/fabric/__init__.py
 psd2fabric/fabric/group.py
 psd2fabric/fabric/image.py
 psd2fabric/fabric/text.py
 psd2fabric/parser/__init__.py
```

