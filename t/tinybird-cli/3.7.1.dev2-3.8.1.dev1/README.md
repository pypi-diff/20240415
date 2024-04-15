# Comparing `tmp/tinybird-cli-3.7.1.dev2.tar.gz` & `tmp/tinybird-cli-3.8.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.7.1.dev2.tar", last modified: Fri Apr 12 10:12:56 2024, max compression
+gzip compressed data, was "tinybird-cli-3.8.1.dev1.tar", last modified: Mon Apr 15 08:36:57 2024, max compression
```

## Comparing `tinybird-cli-3.7.1.dev2.tar` & `tinybird-cli-3.8.1.dev1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:56.002241 tinybird-cli-3.7.1.dev2/
--rw-r--r--   0 root         (0) root         (0)    68066 2024-04-12 10:12:56.002241 tinybird-cli-3.7.1.dev2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 10:12:56.002241 tinybird-cli-3.7.1.dev2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:55.999241 tinybird-cli-3.7.1.dev2/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:55.999241 tinybird-cli-3.7.1.dev2/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46575 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212073 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59111 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41181 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    76994 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11523 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:56.001241 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64836 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    29931 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:56.001241 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-12 10:12:49.000000 tinybird-cli-3.7.1.dev2/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:12:56.002241 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68066 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-12 10:12:55.000000 tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.838098 tinybird-cli-3.8.1.dev1/
+-rw-r--r--   0 root         (0) root         (0)    68035 2024-04-15 08:36:57.838098 tinybird-cli-3.8.1.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 08:36:57.838098 tinybird-cli-3.8.1.dev1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.835098 tinybird-cli-3.8.1.dev1/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.835098 tinybird-cli-3.8.1.dev1/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46575 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212073 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59111 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41181 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    76994 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11523 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.837098 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64836 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    29931 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.837098 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-15 08:36:52.000000 tinybird-cli-3.8.1.dev1/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:36:57.838098 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68035 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-15 08:36:57.000000 tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.7.1.dev2/PKG-INFO` & `tinybird-cli-3.8.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.7.1.dev2
+Version: 3.8.1.dev1
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -15,23 +15,19 @@
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 
 ---------
 
-3.7.1.dev2
+3.8.0
 ************
 
-- `Changed` Upgrade clickhouse-toolset to 0.30dev0
 - `Added` Support for S3IAM role for ingest
-
-3.7.1.dev1
-************
-
+- `Changed` Upgrade clickhouse-toolset to 0.30dev0
 - `Changed` Decouple cli from connector_settings module
 
 3.7.0
 ************
 
 - `Changed` fixed major version of tinybird-cli to lower than 4 when using `tb init --git`
 - `Changed` behavior when running `tb deploy` on a branch to push the connection settings to the backend. This change is the backend that decides what to do.
```

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/ch_utils/constants.py` & `tinybird-cli-3.8.1.dev1/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/ch_utils/engine.py` & `tinybird-cli-3.8.1.dev1/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/check_pypi.py` & `tinybird-cli-3.8.1.dev1/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/client.py` & `tinybird-cli-3.8.1.dev1/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/config.py` & `tinybird-cli-3.8.1.dev1/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/connectors.py` & `tinybird-cli-3.8.1.dev1/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/context.py` & `tinybird-cli-3.8.1.dev1/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/datafile.py` & `tinybird-cli-3.8.1.dev1/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/datatypes.py` & `tinybird-cli-3.8.1.dev1/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/feedback_manager.py` & `tinybird-cli-3.8.1.dev1/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/git_settings.py` & `tinybird-cli-3.8.1.dev1/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/sql.py` & `tinybird-cli-3.8.1.dev1/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/sql_template.py` & `tinybird-cli-3.8.1.dev1/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/sql_template_fmt.py` & `tinybird-cli-3.8.1.dev1/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/sql_toolset.py` & `tinybird-cli-3.8.1.dev1/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/syncasync.py` & `tinybird-cli-3.8.1.dev1/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.8.1.dev1/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird/tornado_template.py` & `tinybird-cli-3.8.1.dev1/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.7.1.dev2
+Version: 3.8.1.dev1
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -15,23 +15,19 @@
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 
 ---------
 
-3.7.1.dev2
+3.8.0
 ************
 
-- `Changed` Upgrade clickhouse-toolset to 0.30dev0
 - `Added` Support for S3IAM role for ingest
-
-3.7.1.dev1
-************
-
+- `Changed` Upgrade clickhouse-toolset to 0.30dev0
 - `Changed` Decouple cli from connector_settings module
 
 3.7.0
 ************
 
 - `Changed` fixed major version of tinybird-cli to lower than 4 when using `tb init --git`
 - `Changed` behavior when running `tb deploy` on a branch to push the connection settings to the backend. This change is the backend that decides what to do.
```

### Comparing `tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.7.1.dev2/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.8.1.dev1/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

