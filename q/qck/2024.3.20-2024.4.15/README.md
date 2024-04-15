# Comparing `tmp/qck-2024.3.20.tar.gz` & `tmp/qck-2024.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qck-2024.3.20.tar", last modified: Wed Mar 20 14:27:06 2024, max compression
+gzip compressed data, was "qck-2024.4.15.tar", last modified: Mon Apr 15 15:50:31 2024, max compression
```

## Comparing `qck-2024.3.20.tar` & `qck-2024.4.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-20 14:27:06.508632 qck-2024.3.20/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1069 2024-01-31 12:01:46.000000 qck-2024.3.20/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1782 2024-03-20 14:27:06.508632 qck-2024.3.20/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1022 2024-03-20 14:23:17.000000 qck-2024.3.20/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-20 14:27:06.508632 qck-2024.3.20/qck.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1782 2024-03-20 14:27:05.000000 qck-2024.3.20/qck.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      233 2024-03-20 14:27:06.000000 qck-2024.3.20/qck.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-03-20 14:27:05.000000 qck-2024.3.20/qck.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2024-03-20 14:27:05.000000 qck-2024.3.20/qck.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-01-31 11:59:17.000000 qck-2024.3.20/qck.egg-info/not-zip-safe
--rw-r--r--   0 daniel    (1000) daniel    (1000)       56 2024-03-20 14:27:05.000000 qck-2024.3.20/qck.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        4 2024-03-20 14:27:05.000000 qck-2024.3.20/qck.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3387 2024-03-20 14:23:17.000000 qck-2024.3.20/qck.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      670 2024-03-20 14:27:06.512632 qck-2024.3.20/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-01-31 10:47:37.000000 qck-2024.3.20/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:50:31.390324 qck-2024.4.15/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1069 2024-01-31 12:01:46.000000 qck-2024.4.15/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2599 2024-04-15 15:50:31.390324 qck-2024.4.15/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1623 2024-04-15 15:44:28.000000 qck-2024.4.15/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-15 15:50:31.390324 qck-2024.4.15/qck.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2599 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      233 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-01-31 11:59:17.000000 qck-2024.4.15/qck.egg-info/not-zip-safe
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       56 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        4 2024-04-15 15:50:31.000000 qck-2024.4.15/qck.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3830 2024-04-15 15:44:28.000000 qck-2024.4.15/qck.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      716 2024-04-15 15:50:31.390324 qck-2024.4.15/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-01-31 10:47:37.000000 qck-2024.4.15/setup.py
```

### Comparing `qck-2024.3.20/LICENSE` & `qck-2024.4.15/LICENSE`

 * *Files identical despite different names*

