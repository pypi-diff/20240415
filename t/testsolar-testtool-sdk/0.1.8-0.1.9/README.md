# Comparing `tmp/testsolar-testtool-sdk-0.1.8.tar.gz` & `tmp/testsolar_testtool_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.1.8.tar", last modified: Thu Apr 11 12:12:10 2024, max compression
+gzip compressed data, was "testsolar_testtool_sdk-0.1.9.tar", last modified: Mon Apr 15 08:46:20 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.1.8.tar` & `testsolar_testtool_sdk-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.101981 testsolar-testtool-sdk-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 12:12:10.101981 testsolar-testtool-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:12:10.101981 testsolar-testtool-sdk-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.097981 testsolar-testtool-sdk-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.097981 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.097981 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.101981 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 12:12:10.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-11 12:12:10.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:12:10.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 12:12:10.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 12:12:10.000000 testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:12:10.097981 testsolar-testtool-sdk-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-11 12:11:44.000000 testsolar-testtool-sdk-0.1.8/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1.8/LICENSE` & `testsolar_testtool_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/pipe_reader.py` & `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk/reporter.py` & `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.8/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.8/tests/test_report.py` & `testsolar_testtool_sdk-0.1.9/tests/test_report.py`

 * *Files identical despite different names*

