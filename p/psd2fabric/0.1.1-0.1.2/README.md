# Comparing `tmp/psd2fabric-0.1.1.tar.gz` & `tmp/psd2fabric-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psd2fabric-0.1.1.tar", last modified: Mon Apr 15 12:11:34 2024, max compression
+gzip compressed data, was "psd2fabric-0.1.2.tar", last modified: Mon Apr 15 12:14:25 2024, max compression
```

## Comparing `psd2fabric-0.1.1.tar` & `psd2fabric-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.806330 psd2fabric-0.1.1/
--rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:11:34.806081 psd2fabric-0.1.1/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-02-05 07:08:02.000000 psd2fabric-0.1.1/README.md
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.801694 psd2fabric-0.1.1/psd2fabric/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.803634 psd2fabric-0.1.1/psd2fabric/fabric/
--rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/fabric/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      533 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/fabric/group.py
--rw-r--r--   0 haibing    (501) staff       (20)      398 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/fabric/image.py
--rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/fabric/text.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.804513 psd2fabric-0.1.1/psd2fabric/parser/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/parser/__init__.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.805106 psd2fabric-0.1.1/psd2fabric/parser/effects/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/parser/effects/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/parser/effects/coloroverlay_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/parser/effects/stroke_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/parser/group_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      516 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/parser/image_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/parser/psd_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/parser/type_parser.py
--rw-r--r--   0 haibing    (501) staff       (20)      288 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/psd_fabric.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.805411 psd2fabric-0.1.1/psd2fabric/render/
--rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.1/psd2fabric/render/__init__.py
--rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-15 11:42:40.000000 psd2fabric-0.1.1/psd2fabric/render/json_render.py
-drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:11:34.805776 psd2fabric-0.1.1/psd2fabric.egg-info/
--rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/PKG-INFO
--rw-r--r--   0 haibing    (501) staff       (20)      738 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/SOURCES.txt
--rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/dependency_links.txt
--rw-r--r--   0 haibing    (501) staff       (20)       36 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/entry_points.txt
--rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/requires.txt
--rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-15 12:11:34.000000 psd2fabric-0.1.1/psd2fabric.egg-info/top_level.txt
--rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-15 12:11:34.806395 psd2fabric-0.1.1/setup.cfg
--rw-r--r--   0 haibing    (501) staff       (20)      282 2024-04-15 12:11:24.000000 psd2fabric-0.1.1/setup.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.987159 psd2fabric-0.1.2/
+-rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:14:25.986952 psd2fabric-0.1.2/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)     1752 2024-02-05 07:08:02.000000 psd2fabric-0.1.2/README.md
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.982883 psd2fabric-0.1.2/psd2fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.984962 psd2fabric-0.1.2/psd2fabric/fabric/
+-rw-r--r--   0 haibing    (501) staff       (20)     1706 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/fabric/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      533 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/fabric/group.py
+-rw-r--r--   0 haibing    (501) staff       (20)      398 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/fabric/image.py
+-rw-r--r--   0 haibing    (501) staff       (20)     1522 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/fabric/text.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.985699 psd2fabric-0.1.2/psd2fabric/parser/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/parser/__init__.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.986149 psd2fabric-0.1.2/psd2fabric/parser/effects/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/parser/effects/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      343 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/parser/effects/coloroverlay_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      346 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/parser/effects/stroke_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/parser/group_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      516 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/parser/image_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2423 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/parser/psd_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)     2409 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/parser/type_parser.py
+-rw-r--r--   0 haibing    (501) staff       (20)      288 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/psd_fabric.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.986381 psd2fabric-0.1.2/psd2fabric/render/
+-rw-r--r--   0 haibing    (501) staff       (20)        0 2024-02-05 07:08:03.000000 psd2fabric-0.1.2/psd2fabric/render/__init__.py
+-rw-r--r--   0 haibing    (501) staff       (20)      498 2024-04-15 11:42:40.000000 psd2fabric-0.1.2/psd2fabric/render/json_render.py
+drwxr-xr-x   0 haibing    (501) staff       (20)        0 2024-04-15 12:14:25.986688 psd2fabric-0.1.2/psd2fabric.egg-info/
+-rw-r--r--   0 haibing    (501) staff       (20)       87 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/PKG-INFO
+-rw-r--r--   0 haibing    (501) staff       (20)      738 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 haibing    (501) staff       (20)        1 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       40 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/entry_points.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       18 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/requires.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       11 2024-04-15 12:14:25.000000 psd2fabric-0.1.2/psd2fabric.egg-info/top_level.txt
+-rw-r--r--   0 haibing    (501) staff       (20)       38 2024-04-15 12:14:25.987218 psd2fabric-0.1.2/setup.cfg
+-rw-r--r--   0 haibing    (501) staff       (20)      286 2024-04-15 12:14:17.000000 psd2fabric-0.1.2/setup.py
```

### Comparing `psd2fabric-0.1.1/README.md` & `psd2fabric-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/fabric/__init__.py` & `psd2fabric-0.1.2/psd2fabric/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/fabric/group.py` & `psd2fabric-0.1.2/psd2fabric/fabric/group.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/fabric/text.py` & `psd2fabric-0.1.2/psd2fabric/fabric/text.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/parser/image_parser.py` & `psd2fabric-0.1.2/psd2fabric/parser/image_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/parser/psd_parser.py` & `psd2fabric-0.1.2/psd2fabric/parser/psd_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric/parser/type_parser.py` & `psd2fabric-0.1.2/psd2fabric/parser/type_parser.py`

 * *Files identical despite different names*

### Comparing `psd2fabric-0.1.1/psd2fabric.egg-info/SOURCES.txt` & `psd2fabric-0.1.2/psd2fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

