# Comparing `tmp/psd2fabric-0.1.3.tar.gz` & `tmp/psd2fabric-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psd2fabric-0.1.3.tar", last modified: Mon Apr 15 12:17:51 2024, max compression
+gzip compressed data, was "psd2fabric-0.1.4.tar", last modified: Mon Apr 15 12:19:05 2024, max compression
```

## Comparing `psd2fabric-0.1.3.tar` & `psd2fabric-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.352164 psd2fabric-0.1.3/
--rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:17:51.351942 psd2fabric-0.1.3/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-02-05 07:08:02.000000 psd2fabric-0.1.3/README.md
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.348355 psd2fabric-0.1.3/psd2fabric/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.350058 psd2fabric-0.1.3/psd2fabric/fabric/
--rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/fabric/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      533 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/fabric/group.py
--rw-r--r--   0 haibing    (501) staff       (20)      398 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/fabric/image.py
--rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/fabric/text.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.350720 psd2fabric-0.1.3/psd2fabric/parser/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/parser/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.351154 psd2fabric-0.1.3/psd2fabric/parser/effects/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/parser/effects/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/parser/effects/coloroverlay_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/parser/effects/stroke_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/parser/group_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      516 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/parser/image_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/parser/psd_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/parser/type_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      288 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/psd_fabric.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.351427 psd2fabric-0.1.3/psd2fabric/render/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.3/psd2fabric/render/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-15 11:42:40.000000 psd2fabric-0.1.3/psd2fabric/render/json_render.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:17:51.351649 psd2fabric-0.1.3/psd2fabric.egg-info/
--rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)      738 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/SOURCES.txt
--rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/dependency_links.txt
--rw-r--r--   0 haibing    (501) staff       (20)       51 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/entry_points.txt
--rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/requires.txt
--rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-15 12:17:51.000000 psd2fabric-0.1.3/psd2fabric.egg-info/top_level.txt
--rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-15 12:17:51.352216 psd2fabric-0.1.3/setup.cfg
--rw-r--r--   0 haibing    (501) staff       (20)      297 2024-04-15 12:17:49.000000 psd2fabric-0.1.3/setup.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.075761 psd2fabric-0.1.4/
+-rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:19:05.075502 psd2fabric-0.1.4/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-02-05 07:08:02.000000 psd2fabric-0.1.4/README.md
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.070697 psd2fabric-0.1.4/psd2fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.073252 psd2fabric-0.1.4/psd2fabric/fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/fabric/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      533 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/fabric/group.py
+-rw-r--r--   0 haibing    (501) staff       (20)      398 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/fabric/image.py
+-rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/fabric/text.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.073954 psd2fabric-0.1.4/psd2fabric/parser/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/parser/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.074526 psd2fabric-0.1.4/psd2fabric/parser/effects/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/parser/effects/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/parser/effects/coloroverlay_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/parser/effects/stroke_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/parser/group_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      516 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/parser/image_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/parser/psd_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/parser/type_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      288 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/psd_fabric.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.074887 psd2fabric-0.1.4/psd2fabric/render/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.4/psd2fabric/render/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-15 11:42:40.000000 psd2fabric-0.1.4/psd2fabric/render/json_render.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:19:05.075171 psd2fabric-0.1.4/psd2fabric.egg-info/
+-rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)      738 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       41 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/entry_points.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/requires.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-15 12:19:05.000000 psd2fabric-0.1.4/psd2fabric.egg-info/top_level.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-15 12:19:05.075816 psd2fabric-0.1.4/setup.cfg
+-rw-r--r--   0 haibing    (501) staff       (20)      287 2024-04-15 12:19:01.000000 psd2fabric-0.1.4/setup.py
```

### Comparing `psd2fabric-0.1.3/README.md` & `psd2fabric-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/fabric/__init__.py` & `psd2fabric-0.1.4/psd2fabric/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/fabric/group.py` & `psd2fabric-0.1.4/psd2fabric/fabric/group.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/fabric/text.py` & `psd2fabric-0.1.4/psd2fabric/fabric/text.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/parser/image_parser.py` & `psd2fabric-0.1.4/psd2fabric/parser/image_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/parser/psd_parser.py` & `psd2fabric-0.1.4/psd2fabric/parser/psd_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric/parser/type_parser.py` & `psd2fabric-0.1.4/psd2fabric/parser/type_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.3/psd2fabric.egg-info/SOURCES.txt` & `psd2fabric-0.1.4/psd2fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

