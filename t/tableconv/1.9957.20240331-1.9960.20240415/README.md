# Comparing `tmp/tableconv-1.9957.20240331.tar.gz` & `tmp/tableconv-1.9960.20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableconv-1.9957.20240331.tar", last modified: Tue Apr  2 20:43:56 2024, max compression
+gzip compressed data, was "tableconv-1.9960.20240415.tar", last modified: Mon Apr 15 01:53:36 2024, max compression
```

## Comparing `tableconv-1.9957.20240331.tar` & `tableconv-1.9960.20240415.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     9456 2024-03-31 06:03:00.000000 tableconv-1.9957.20240331/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9957.20240331/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv/
--rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       73 2024-03-31 06:34:11.000000 tableconv-1.9957.20240331/tableconv/__version__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv/adapters/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/tableconv/adapters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/tableconv/adapters/df/
--rw-rw-r--   0 john      (1000) john      (1000)     1047 2024-03-31 04:52:25.000000 tableconv-1.9957.20240331/tableconv/adapters/df/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/ascii.py
--rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_athena.py
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_dynamodb.py
--rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_logs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1756 2024-01-19 23:13:24.000000 tableconv-1.9957.20240331/tableconv/adapters/df/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9957.20240331/tableconv/adapters/df/example.py
--rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9957.20240331/tableconv/adapters/df/file_adapter_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)    13407 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/gsheets.py
--rw-rw-r--   0 john      (1000) john      (1000)     1925 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/jc.py
--rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9957.20240331/tableconv/adapters/df/jira.py
--rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/json.py
--rw-rw-r--   0 john      (1000) john      (1000)      589 2024-03-31 06:31:52.000000 tableconv-1.9957.20240331/tableconv/adapters/df/leveldb.py
--rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/nested_list.py
--rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9957.20240331/tableconv/adapters/df/numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-03-31 06:31:52.000000 tableconv-1.9957.20240331/tableconv/adapters/df/osquery.py
--rw-rw-r--   0 john      (1000) john      (1000)     9186 2024-03-31 05:55:31.000000 tableconv-1.9957.20240331/tableconv/adapters/df/pandas_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/python.py
--rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/rdbms.py
--rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/smart_sheet.py
--rw-r--r--   0 john      (1000) john      (1000)      881 2024-03-31 05:43:04.000000 tableconv-1.9957.20240331/tableconv/adapters/df/sql_literal.py
--rw-rw-r--   0 john      (1000) john      (1000)     7714 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/sumo_logic.py
--rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/text_array.py
--rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/yaml.py
--rw-rw-r--   0 john      (1000) john      (1000)    17462 2024-03-31 06:07:39.000000 tableconv-1.9957.20240331/tableconv/core.py
--rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9957.20240331/tableconv/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3542 2024-03-31 06:33:22.000000 tableconv-1.9957.20240331/tableconv/in_memory_query.py
--rw-rw-r--   0 john      (1000) john      (1000)     5884 2024-01-19 23:11:36.000000 tableconv-1.9957.20240331/tableconv/interactive.py
--rw-rw-r--   0 john      (1000) john      (1000)    11527 2024-03-31 05:59:27.000000 tableconv-1.9957.20240331/tableconv/main.py
--rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/parse_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/uri.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1336 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       66 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      243 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       27 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/tableconv_daemon/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9957.20240331/tableconv_daemon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9957.20240331/tableconv_daemon/main.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.353058 tableconv-1.9960.20240415/
+-rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9960.20240415/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9960.20240415/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-15 01:53:36.353058 tableconv-1.9960.20240415/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     9456 2024-03-31 06:03:00.000000 tableconv-1.9960.20240415/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-15 01:53:36.353058 tableconv-1.9960.20240415/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9960.20240415/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.349058 tableconv-1.9960.20240415/tableconv/
+-rw-rw-r--   0 john      (1000) john      (1000)      400 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2024-04-15 01:53:25.000000 tableconv-1.9960.20240415/tableconv/__version__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.349058 tableconv-1.9960.20240415/tableconv/adapters/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9960.20240415/tableconv/adapters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.353058 tableconv-1.9960.20240415/tableconv/adapters/df/
+-rw-rw-r--   0 john      (1000) john      (1000)     1047 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/adapters/df/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4264 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/ascii.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14948 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/adapters/df/aws_athena.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9960.20240415/tableconv/adapters/df/aws_dynamodb.py
+-rw-r--r--   0 john      (1000) john      (1000)     2394 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/aws_logs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1756 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9960.20240415/tableconv/adapters/df/example.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2526 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/file_adapter_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16012 2024-04-15 01:53:13.000000 tableconv-1.9960.20240415/tableconv/adapters/df/gsheets.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1925 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/jc.py
+-rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9960.20240415/tableconv/adapters/df/jira.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6463 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/adapters/df/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)      589 2024-03-31 06:31:52.000000 tableconv-1.9960.20240415/tableconv/adapters/df/leveldb.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1876 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/nested_list.py
+-rw-r--r--   0 john      (1000) john      (1000)     1509 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-03-31 06:31:52.000000 tableconv-1.9960.20240415/tableconv/adapters/df/osquery.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9186 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/pandas_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1293 2024-04-15 01:23:58.000000 tableconv-1.9960.20240415/tableconv/adapters/df/python.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5805 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/adapters/df/rdbms.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2494 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/adapters/df/smart_sheet.py
+-rw-r--r--   0 john      (1000) john      (1000)      881 2024-03-31 05:43:04.000000 tableconv-1.9960.20240415/tableconv/adapters/df/sql_literal.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7714 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/adapters/df/sumo_logic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9960.20240415/tableconv/adapters/df/text_array.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9960.20240415/tableconv/adapters/df/yaml.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17462 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/core.py
+-rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9960.20240415/tableconv/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3542 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/in_memory_query.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5884 2024-04-15 01:16:55.000000 tableconv-1.9960.20240415/tableconv/interactive.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11909 2024-04-15 01:49:07.000000 tableconv-1.9960.20240415/tableconv/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)      726 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/parse_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2024-04-15 01:15:11.000000 tableconv-1.9960.20240415/tableconv/uri.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.349058 tableconv-1.9960.20240415/tableconv.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1336 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       66 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      243 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       27 2024-04-15 01:53:36.000000 tableconv-1.9960.20240415/tableconv.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 01:53:36.353058 tableconv-1.9960.20240415/tableconv_daemon/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9960.20240415/tableconv_daemon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9960.20240415/tableconv_daemon/main.py
```

### Comparing `tableconv-1.9957.20240331/LICENSE` & `tableconv-1.9960.20240415/LICENSE`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/PKG-INFO` & `tableconv-1.9960.20240415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9957.20240331
+Version: 1.9960.20240415
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9957.20240331/README.md` & `tableconv-1.9960.20240415/README.md`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/setup.py` & `tableconv-1.9960.20240415/setup.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/__init__.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/__init__.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/ascii.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/ascii.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/aws_athena.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/aws_athena.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/aws_dynamodb.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/aws_logs.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/aws_logs.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/base.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/base.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/file_adapter_mixin.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/file_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/gsheets.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/gsheets.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,28 @@
 logger = logging.getLogger(__name__)
 
 
 def list_ljust(ls, n, fill_value=None):
     return ls + [fill_value] * (n - len(ls))
 
 
+def integer_to_spreadsheet_column_str(i):
+    i += 1
+    result = ""
+    while i > 0:
+        i -= 1
+        result = chr(i % 26 + ord("A")) + result
+        i //= 26
+    return result
+
+
+def coords_to_spreadsheet_cell_str(coord):
+    return f"{integer_to_spreadsheet_column_str(coord[1])}{coord[2]}"
+
+
 def get_sheet_properties(spreadsheet_data, sheet_name):
     for sheet in spreadsheet_data["sheets"]:
         if sheet["properties"]["title"] == sheet_name:
             return sheet["properties"]
     raise KeyError(f"Sheet {sheet_name} not found")
 
 
@@ -177,33 +191,69 @@
             }
         }
         googlesheets.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body={"requests": [request]}).execute()
 
     @staticmethod
     def _serialize_df(df):
         serialized_records = [list(record) for record in df.values]
+        oversize_cells = []
 
         df = df.replace({np.nan: None})
         for i, row in enumerate(serialized_records):
             for j, obj in enumerate(row):
                 if isinstance(obj, datetime.datetime):
                     if type(obj) == type(pd.NaT):  # noqa: E721
                         # Not A Time. i.e. NULL.
                         serialized_records[i][j] = ""
                     else:
                         if obj.tzinfo is not None:
                             obj = obj.astimezone(datetime.timezone.utc)
-                        # WARNING: In effect, this line is causing naive datetimes to be reinterpreted as UTC.
-                        serialized_records[i][j] = obj.strftime("%Y-%m-%d %H:%M:%S")
+                        # Extremely contentious formatting choices here.
+                        # We can use a time format that Google Sheets recognizes/parses, but in the process dropping
+                        # timezone information, obj.strftime("%Y-%m-%d %H:%M:%S")
+                        # Or we can use a format that ghseets cannot recognize, but close to one, better than iso8601:
+                        serialized_records[i][j] = obj.strftime("%Y-%m-%d %H:%M:%S %Z")
+                elif isinstance(obj, datetime.timedelta):
+                    serialized_records[i][j] = str(obj)
+                    # The above is a human readable way of encoding time delta. Extremely contentious though.
+                    # For reference, the ways offered by Pandas IO in its JSON module are:
+                    #   epoch: Format as a number, units of seconds. equivalent to .total_seconds()
+                    #   iso: The fairly obscure ISO8601 "duration" (aka *P*eriod) formatting standard.
+                    #        example: "P11DT14H50M12S"
                 elif isinstance(obj, list) or isinstance(obj, dict):
                     serialized_records[i][j] = str(obj)
                 elif hasattr(obj, "dtype"):
                     serialized_records[i][j] = obj.item()
                 if isinstance(serialized_records[i][j], float) and math.isnan(serialized_records[i][j]):
                     serialized_records[i][j] = None
+                MAX_CELL_SIZE = 50000
+                if isinstance(serialized_records[i][j], str) and len(serialized_records[i][j]) > MAX_CELL_SIZE:
+                    serialized_records[i][j] = serialized_records[i][j][:MAX_CELL_SIZE]
+                    oversize_cells.append((i, j))
+        if oversize_cells:
+            if len(oversize_cells) == 1:
+                plural = ""
+            else:
+                plural = "s"
+            if len(oversize_cells) <= 5:
+                coord_strs = (f"{integer_to_spreadsheet_column_str(coord[0])}{coord[1]}" for coord in oversize_cells)
+                example_cells_str = " (" + (", ".join(coord_strs)) + ")"
+            elif all((coord[1] == oversize_cells[0][1] for coord in oversize_cells)):
+                # All oversize cells are from a single column
+                example_cells_str = f" (all in column {integer_to_spreadsheet_column_str(oversize_cells[0][1])})"
+            else:
+                coord_strs = (
+                    f"{integer_to_spreadsheet_column_str(coord[0])}{coord[1]}" for coord in oversize_cells[:3]
+                )
+                example_cells_str = " (Ex: " + (", ".join(coord_strs)) + ", and more)"
+
+            logger.warning(
+                f"Truncated {len(oversize_cells)} cell{plural}{example_cells_str} to their first 50000 characters to "
+                + " fit within Google Sheets max cell size limit."
+            )
         return serialized_records
 
     @staticmethod
     def dump(df, uri):
         import googleapiclient
 
         parsed_uri = parse_uri(uri)
```

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/jc.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/jc.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/json.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/json.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/leveldb.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/leveldb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/nested_list.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/nested_list.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/numbers.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/numbers.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/osquery.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/osquery.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/pandas_io.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/pandas_io.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/python.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/python.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import ast
-import subprocess
-
 import pandas as pd
 
 from tableconv.exceptions import SourceParseError
 from tableconv.adapters.df.base import Adapter, register_adapter
 from tableconv.adapters.df.file_adapter_mixin import FileAdapterMixin
 
 
@@ -26,20 +24,12 @@
                     f"Every element of the input {scheme} must be a Python dict. "
                     f"(element {i + 1} in input was a Python {type(item)})"
                 )
         return pd.json_normalize(raw_array)
 
     @staticmethod
     def dump_text_data(df, scheme, params):
-        raw = str(df.to_dict(orient="records"))
-        # TODO: This is not an acceptable way to invoke Black. Use its API instead. Black also should only be an
-        # optional dependency.
-        process = subprocess.Popen(
-            ["black", "-"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE
-        )
-        process.communicate(raw.encode("utf-8"))
-        process.wait()
-        output, stderr = process.communicate()
-        if process.returncode != 0:
-            # fail gracefullly
-            return raw
-        return output.decode()
+        import pprint
+
+        # using pprint instead of repr because it can indent.
+        # reprlib in python 3.12+ can too, but I'm preferring pprint for backwards compat.
+        return pprint.pformat(df.to_dict(orient="records"), indent=4)
```

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/rdbms.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/rdbms.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/smart_sheet.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/smart_sheet.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/sql_literal.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/sql_literal.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/sumo_logic.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/sumo_logic.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/text_array.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/text_array.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/adapters/df/yaml.py` & `tableconv-1.9960.20240415/tableconv/adapters/df/yaml.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/core.py` & `tableconv-1.9960.20240415/tableconv/core.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/exceptions.py` & `tableconv-1.9960.20240415/tableconv/exceptions.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/in_memory_query.py` & `tableconv-1.9960.20240415/tableconv/in_memory_query.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/interactive.py` & `tableconv-1.9960.20240415/tableconv/interactive.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/main.py` & `tableconv-1.9960.20240415/tableconv/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 import logging
 import logging.config
 import os
 import sys
 import textwrap
 from typing import Union
 
+from duckdb import __version__ as DUCKDB_VERSION_STR
+from pandas import __version__ as PD_VERSION_STR
+
 from tableconv.__version__ import __version__
 from tableconv.adapters.df import adapters, read_adapters, write_adapters
 from tableconv.adapters.df.base import NoConfigurationOptionsAvailable
 from tableconv.core import load_url, parse_source_url, resolve_query_arg, validate_coercion_schema
 from tableconv.exceptions import DataError, InvalidQueryError, InvalidURLError
 from tableconv.interactive import os_open, run_interactive_shell
 from tableconv.uri import parse_uri
 
 logger = logging.getLogger(__name__)
 
+PROG = os.path.basename(sys.argv[0])
+PY_VERSION_STR = f'{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}'
+
 
 def get_supported_schemes_list_str() -> str:
     descriptions = []
     for scheme, adapter in adapters.items():
         disclaimer = ""
         if scheme not in write_adapters:
             disclaimer = "(source only)"
@@ -81,15 +87,15 @@
 
     def error(self, message):
         raise argparse.ArgumentError(None, message)
 
 
 def raise_argparse_style_error(error: Union[str, Exception], usage=None):
     if usage:
-        print(f"usage: {usage % dict(prog=os.path.basename(sys.argv[0]))}", file=sys.stderr)
+        print(f"usage: {usage % dict(prog=PROG)}", file=sys.stderr)
     if isinstance(error, Exception):
         logger.debug(error, exc_info=True)
     print(f"error: {error}", file=sys.stderr)
     sys.exit(1)
 
 
 def run_configuration_mode(argv):
@@ -180,21 +186,22 @@
     parser.add_argument("-o", "--dest", "--out", "--output", dest="DEST_URL", type=str, help="Specify the data destination URL. If this destination already exists, be aware that the default behavior is to overwrite.")  # noqa: E501
     parser.add_argument("-i", "--interactive", action="store_true", help="Enter interactive REPL query mode.")  # noqa: E501
     parser.add_argument("--open", dest="open_dest", action="store_true", help="Open resulting file/url in the operating system desktop environment. (not supported for all destination types)")  # noqa: E501
     parser.add_argument("--schema", "--coerce-schema", dest="schema_coercion", default=None, help="Coerce source schema according to a schema definition. (WARNING: experimental feature)")  # noqa: E501
     parser.add_argument("--restrict-schema", dest="restrict_schema", action="store_true", help="Exclude all columns not included in the SCHEMA_COERCION definition. (WARNING: experimental feature)")  # noqa: E501
     parser.add_argument("--autocache", "--cache", action="store_true", help="Cache network data, and reuse cached data.")  # noqa: E501
     parser.add_argument("-v", "--verbose", "--debug", dest="verbose", action="store_true", help="Show debug details, including API calls and error sources.")  # noqa: E501
-    parser.add_argument("--version", action="version", help="Show version number and exit", version=f"%(prog)s {__version__}")  # noqa: E501
+    parser.add_argument("--version", action='version', help="Show version number and exit", version=f"{PROG} {__version__} (Python {PY_VERSION_STR}, DuckDB {DUCKDB_VERSION_STR}, Pandas {PD_VERSION_STR})")  # noqa: E501
     parser.add_argument("--quiet", action="store_true", help="Only display errors.")
     parser.add_argument("--print", "--print-dest", action="store_true", help="Print resulting URL/path to stdout, for chaining with other commands.")  # noqa: E501
-    parser.add_argument("--debug-shell", "--pandas-debug-shell", "--debug-pandas-shell", action="store_true", help=argparse.SUPPRESS)  # noqa: E501
+    parser.add_argument("--debug-shell", "--pandas-debug-shell", "--debug-pandas-shell", "--debug_shell", action="store_true", help=argparse.SUPPRESS)  # noqa: E501
     parser.add_argument("--daemon", action="store_true", help="Tableconv startup time (python startup time) is slow. To mitigate that, you can first run tableconv as a daemon, and then all future invocations (while daemon is still alive) will be fast.  (WARNING: experimental feature)")  # noqa: E501
 
     if argv and argv[0] in ("configure", "--configure"):
+        # This is a hidden feature because it is very incomplete right now.
         run_configuration_mode(argv)
         sys.exit(0)
 
     try:
         args = parser.parse_args(argv)
         if args.quiet and args.verbose:
             raise argparse.ArgumentError(
```

### Comparing `tableconv-1.9957.20240331/tableconv/parse_time.py` & `tableconv-1.9960.20240415/tableconv/parse_time.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv/uri.py` & `tableconv-1.9960.20240415/tableconv/uri.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv.egg-info/PKG-INFO` & `tableconv-1.9960.20240415/tableconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9957.20240331
+Version: 1.9960.20240415
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9957.20240331/tableconv.egg-info/SOURCES.txt` & `tableconv-1.9960.20240415/tableconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableconv-1.9957.20240331/tableconv_daemon/main.py` & `tableconv-1.9960.20240415/tableconv_daemon/main.py`

 * *Files identical despite different names*

