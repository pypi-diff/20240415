# Comparing `tmp/efriser-0.1.6.tar.gz` & `tmp/efriser-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.6.tar", last modified: Sat Apr 13 19:27:40 2024, max compression
+gzip compressed data, was "efriser-0.1.7.tar", last modified: Mon Apr 15 06:00:16 2024, max compression
```

## Comparing `efriser-0.1.6.tar` & `efriser-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:27:40.422437 efriser-0.1.6/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 19:27:40.422437 efriser-0.1.6/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      197 2024-04-13 18:03:20.000000 efriser-0.1.6/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:27:40.422437 efriser-0.1.6/efris/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      136 2024-04-13 19:20:15.000000 efriser-0.1.6/efris/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6242 2024-04-13 19:26:19.000000 efriser-0.1.6/efris/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.6/efris/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.6/efris/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.6/efris/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.6/efris/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:27:40.422437 efriser-0.1.6/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 19:27:40.000000 efriser-0.1.6/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-13 19:27:40.000000 efriser-0.1.6/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 19:27:40.000000 efriser-0.1.6/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 19:27:40.000000 efriser-0.1.6/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-13 19:27:40.000000 efriser-0.1.6/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 19:27:40.422437 efriser-0.1.6/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 19:27:28.000000 efriser-0.1.6/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     2357 2024-04-15 06:00:16.813632 efriser-0.1.7/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1871 2024-04-15 05:59:48.000000 efriser-0.1.7/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/efris/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      136 2024-04-13 19:20:15.000000 efriser-0.1.7/efris/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6242 2024-04-13 19:26:19.000000 efriser-0.1.7/efris/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.7/efris/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.7/efris/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.7/efris/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.7/efris/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     2357 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-15 06:00:16.813632 efriser-0.1.7/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      721 2024-04-15 05:59:58.000000 efriser-0.1.7/setup.py
```

### Comparing `efriser-0.1.6/efris/invoicing.py` & `efriser-0.1.7/efris/invoicing.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.6/efris/output_cleaner.py` & `efriser-0.1.7/efris/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.6/efris/services.py` & `efriser-0.1.7/efris/services.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.6/efris/utils.py` & `efriser-0.1.7/efris/utils.py`

 * *Files identical despite different names*

