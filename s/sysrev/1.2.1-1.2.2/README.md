# Comparing `tmp/sysrev-1.2.1.tar.gz` & `tmp/sysrev-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.2.1.tar", last modified: Sun Apr 14 21:04:08 2024, max compression
+gzip compressed data, was "sysrev-1.2.2.tar", last modified: Mon Apr 15 13:30:44 2024, max compression
```

## Comparing `sysrev-1.2.1.tar` & `sysrev-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-14 21:04:08.424497 sysrev-1.2.1/
--rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-14 21:04:08.424497 sysrev-1.2.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2024-04-14 21:02:22.000000 sysrev-1.2.1/README
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-14 21:04:08.424497 sysrev-1.2.1/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)      425 2024-04-14 21:01:40.000000 sysrev-1.2.1/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-14 21:04:08.424497 sysrev-1.2.1/sysrev.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-14 21:04:08.000000 sysrev-1.2.1/sysrev.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      193 2024-04-14 21:04:08.000000 sysrev-1.2.1/sysrev.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-14 21:04:08.000000 sysrev-1.2.1/sysrev.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-14 21:03:58.000000 sysrev-1.2.1/sysrev.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1000) tom       (1000)       24 2024-04-14 21:04:08.000000 sysrev-1.2.1/sysrev.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        7 2024-04-14 21:04:08.000000 sysrev-1.2.1/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.701321 sysrev-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:30:44.701321 sysrev-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:30:39.000000 sysrev-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:30:44.701321 sysrev-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:30:39.000000 sysrev-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.697321 sysrev-1.2.2/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:30:39.000000 sysrev-1.2.2/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-15 13:30:39.000000 sysrev-1.2.2/sysrev/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:30:44.701321 sysrev-1.2.2/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:30:44.000000 sysrev-1.2.2/sysrev.egg-info/top_level.txt
```

