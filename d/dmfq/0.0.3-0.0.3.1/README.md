# Comparing `tmp/dmfq-0.0.3.tar.gz` & `tmp/dmfq-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dmfq-0.0.3.tar", last modified: Mon Mar 25 04:25:26 2024, max compression
+gzip compressed data, was "dist/dmfq-0.0.3.1.tar", last modified: Mon Apr 15 11:50:39 2024, max compression
```

## Comparing `dmfq-0.0.3.tar` & `dmfq-0.0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-03-25 04:25:26.000000 dmfq-0.0.3/
--rw-rw-r--   0 hjy       (1000) hjy       (1000)     1068 2024-03-20 12:18:50.000000 dmfq-0.0.3/LICENSE
--rw-rw-r--   0 hjy       (1000) hjy       (1000)      179 2024-03-25 04:25:26.000000 dmfq-0.0.3/PKG-INFO
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        0 2024-03-20 12:12:36.000000 dmfq-0.0.3/README.md
-drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq/
--rw-rw-r--   0 hjy       (1000) hjy       (1000)       46 2024-03-23 08:41:40.000000 dmfq-0.0.3/dmfq/__init__.py
--rw-rw-r--   0 hjy       (1000) hjy       (1000)     6591 2024-03-25 04:24:49.000000 dmfq-0.0.3/dmfq/dmfq.py
-drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq/utils/
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        0 2024-03-20 12:12:55.000000 dmfq-0.0.3/dmfq/utils/__init__.py
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        1 2024-03-23 08:31:09.000000 dmfq-0.0.3/dmfq/utils_train.py
-drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/
--rw-rw-r--   0 hjy       (1000) hjy       (1000)      179 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/PKG-INFO
--rw-rw-r--   0 hjy       (1000) hjy       (1000)      238 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/SOURCES.txt
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        1 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/dependency_links.txt
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        6 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/requires.txt
--rw-rw-r--   0 hjy       (1000) hjy       (1000)        5 2024-03-25 04:25:26.000000 dmfq-0.0.3/dmfq.egg-info/top_level.txt
--rw-rw-r--   0 hjy       (1000) hjy       (1000)       38 2024-03-25 04:25:26.000000 dmfq-0.0.3/setup.cfg
--rw-rw-r--   0 hjy       (1000) hjy       (1000)      434 2024-03-23 08:10:46.000000 dmfq-0.0.3/setup.py
+drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)     1068 2024-03-20 12:18:50.000000 dmfq-0.0.3.1/LICENSE
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)      181 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/PKG-INFO
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        0 2024-03-20 12:12:36.000000 dmfq-0.0.3.1/README.md
+drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq/
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)       46 2024-03-23 08:41:40.000000 dmfq-0.0.3.1/dmfq/__init__.py
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)     8608 2024-04-11 13:42:11.000000 dmfq-0.0.3.1/dmfq/dmfq.py
+drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq/utils/
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        0 2024-03-20 12:12:55.000000 dmfq-0.0.3.1/dmfq/utils/__init__.py
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        1 2024-03-23 08:31:09.000000 dmfq-0.0.3.1/dmfq/utils_train.py
+drwxrwxr-x   0 hjy       (1000) hjy       (1000)        0 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)      181 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/PKG-INFO
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)      238 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/SOURCES.txt
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        1 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/dependency_links.txt
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        6 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/requires.txt
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)        5 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/dmfq.egg-info/top_level.txt
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)       38 2024-04-15 11:50:39.000000 dmfq-0.0.3.1/setup.cfg
+-rw-rw-r--   0 hjy       (1000) hjy       (1000)      436 2024-03-27 08:26:19.000000 dmfq-0.0.3.1/setup.py
```

### Comparing `dmfq-0.0.3/LICENSE` & `dmfq-0.0.3.1/LICENSE`

 * *Files identical despite different names*

