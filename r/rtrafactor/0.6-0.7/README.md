# Comparing `tmp/rtrafactor-0.6.tar.gz` & `tmp/rtrafactor-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrafactor-0.6.tar", last modified: Fri Apr 12 11:20:14 2024, max compression
+gzip compressed data, was "rtrafactor-0.7.tar", last modified: Mon Apr 15 10:26:10 2024, max compression
```

## Comparing `rtrafactor-0.6.tar` & `rtrafactor-0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 11:20:14.240883 rtrafactor-0.6/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 11:20:14.240603 rtrafactor-0.6/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 11:20:14.239531 rtrafactor-0.6/rtrafactor/
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.6/rtrafactor/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.6/rtrafactor/webconnect.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 11:20:14.240306 rtrafactor-0.6/rtrafactor.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 11:20:14.000000 rtrafactor-0.6/rtrafactor.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 11:20:14.000000 rtrafactor-0.6/rtrafactor.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 11:20:14.000000 rtrafactor-0.6/rtrafactor.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       44 2024-04-12 11:20:14.000000 rtrafactor-0.6/rtrafactor.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 11:20:14.000000 rtrafactor-0.6/rtrafactor.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 11:20:14.240939 rtrafactor-0.6/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      496 2024-04-12 11:20:03.000000 rtrafactor-0.6/setup.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 11:20:14.240439 rtrafactor-0.6/tests/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.6/tests/test_webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-15 10:26:10.878372 rtrafactor-0.7/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-15 10:22:40.000000 rtrafactor-0.7/LICENSE
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      257 2024-04-15 10:26:10.877761 rtrafactor-0.7/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-15 10:26:10.874418 rtrafactor-0.7/rtrafactor/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.7/rtrafactor/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.7/rtrafactor/webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-15 10:26:10.876107 rtrafactor-0.7/rtrafactor.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      257 2024-04-15 10:26:10.000000 rtrafactor-0.7/rtrafactor.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      258 2024-04-15 10:26:10.000000 rtrafactor-0.7/rtrafactor.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-15 10:26:10.000000 rtrafactor-0.7/rtrafactor.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       44 2024-04-15 10:26:10.000000 rtrafactor-0.7/rtrafactor.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-15 10:26:10.000000 rtrafactor-0.7/rtrafactor.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-15 10:26:10.878555 rtrafactor-0.7/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      496 2024-04-15 10:26:08.000000 rtrafactor-0.7/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-15 10:26:10.876377 rtrafactor-0.7/tests/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.7/tests/test_webconnect.py
```

### Comparing `rtrafactor-0.6/rtrafactor/__init__.py` & `rtrafactor-0.7/rtrafactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rtrafactor-0.6/rtrafactor/webconnect.py` & `rtrafactor-0.7/rtrafactor/webconnect.py`

 * *Files identical despite different names*

