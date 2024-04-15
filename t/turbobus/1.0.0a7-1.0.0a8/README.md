# Comparing `tmp/turbobus-1.0.0a7.tar.gz` & `tmp/turbobus-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbobus-1.0.0a7.tar", last modified: Sun Apr 14 15:02:40 2024, max compression
+gzip compressed data, was "turbobus-1.0.0a8.tar", last modified: Sun Apr 14 20:45:22 2024, max compression
```

## Comparing `turbobus-1.0.0a7.tar` & `turbobus-1.0.0a8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.549468 turbobus-1.0.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.549468 turbobus-1.0.0a7/turbobus/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/turbobus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/turbobus/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/turbobus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/top_level.txt
```

### Comparing `turbobus-1.0.0a7/pyproject.toml` & `turbobus-1.0.0a8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "turbobus"
 version = "1.0.0-alpha.0"
-description = "TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python"
+description = "TurboBus is an implementation of Command Responsibility Segregation pattern in python"
 authors = ["Christopher A. Flores <christopher.flores@codexitos.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `turbobus-1.0.0a7/setup.py` & `turbobus-1.0.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/tests/test.py` & `turbobus-1.0.0a8/tests/test.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/tests/test_command.py` & `turbobus-1.0.0a8/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/tests/test_constants.py` & `turbobus-1.0.0a8/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/turbobus/command.py` & `turbobus-1.0.0a8/turbobus/command.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/turbobus/exception.py` & `turbobus-1.0.0a8/turbobus/exception.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a7/turbobus/injection.py` & `turbobus-1.0.0a8/turbobus/injection.py`

 * *Files identical despite different names*

