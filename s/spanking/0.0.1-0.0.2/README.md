# Comparing `tmp/spanking-0.0.1.tar.gz` & `tmp/spanking-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanking-0.0.1.tar", last modified: Sat Apr 13 22:53:46 2024, max compression
+gzip compressed data, was "spanking-0.0.2.tar", last modified: Sun Apr 14 21:05:47 2024, max compression
```

## Comparing `spanking-0.0.1.tar` & `spanking-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:53:46.543383 spanking-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 22:53:38.000000 spanking-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-13 22:53:46.543383 spanking-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 22:53:38.000000 spanking-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:53:46.543383 spanking-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-13 22:53:38.000000 spanking-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:53:46.543383 spanking-0.0.1/spanking/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 22:53:38.000000 spanking-0.0.1/spanking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 22:53:38.000000 spanking-0.0.1/spanking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-13 22:53:38.000000 spanking-0.0.1/spanking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:53:46.543383 spanking-0.0.1/spanking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 22:53:46.000000 spanking-0.0.1/spanking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 21:05:38.000000 spanking-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 21:05:47.525440 spanking-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-14 21:05:38.000000 spanking-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:05:47.525440 spanking-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-14 21:05:38.000000 spanking-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/spanking/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 21:05:38.000000 spanking-0.0.2/spanking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:05:47.525440 spanking-0.0.2/spanking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:05:47.000000 spanking-0.0.2/spanking.egg-info/top_level.txt
```

### Comparing `spanking-0.0.1/LICENSE` & `spanking-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spanking-0.0.1/setup.py` & `spanking-0.0.2/setup.py`

 * *Files identical despite different names*

