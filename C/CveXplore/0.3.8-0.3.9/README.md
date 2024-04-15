# Comparing `tmp/CveXplore-0.3.8.tar.gz` & `tmp/CveXplore-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CveXplore-0.3.8.tar", last modified: Fri Oct 13 14:50:28 2023, max compression
+gzip compressed data, was "CveXplore-0.3.9.tar", last modified: Tue Oct 17 15:27:06 2023, max compression
```

## Comparing `CveXplore-0.3.8.tar` & `CveXplore-0.3.9.tar`

### file list

```diff
@@ -1,102 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.211284 CveXplore-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/.schema_version
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/api_base_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/api/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/connection/api_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/helpers/cve_search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/api/nvd_nist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/nvd_nist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/api/nvd_nist/nvd_nist_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cli_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/cpe_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cpe_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cpe_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/cve_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cve_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/cve_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/db_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/db_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/db_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/find_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/find_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/find_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/mutex_options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/mutex_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/mutex_options/mutex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/cli_cmds/stats_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/stats_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/cli_cmds/stats_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/cpe_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/data_source_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/common/db_obj_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore/database/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/connection/mongo_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.211284 CveXplore-0.3.8/CveXplore/database/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/helpers/cpe_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/helpers/cvesearch_mongo_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/helpers/generic_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/helpers/specific_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.211284 CveXplore-0.3.8/CveXplore/database/maintenance/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/DatabaseSchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/DownloadHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/IJSONHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/LogHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    52200 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/Sources_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/api_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15970 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/content_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/db_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/main_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/database/maintenance/worker_q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.211284 CveXplore-0.3.8/CveXplore/errors/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/errors/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/errors/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/errors/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.211284 CveXplore-0.3.8/CveXplore/objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/capec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/cpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/cves.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/cvexplore_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/cwe.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-13 14:50:20.000000 CveXplore-0.3.8/CveXplore/objects/via4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 14:50:28.207285 CveXplore-0.3.8/CveXplore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-13 14:50:28.000000 CveXplore-0.3.8/CveXplore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-13 14:50:20.000000 CveXplore-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-13 14:50:20.000000 CveXplore-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-13 14:50:28.211284 CveXplore-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15684 2023-10-13 14:50:20.000000 CveXplore-0.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-13 14:50:20.000000 CveXplore-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 14:50:28.211284 CveXplore-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-10-13 14:50:20.000000 CveXplore-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.265117 CveXplore-0.3.9/CveXplore/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/.schema_version
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/api_base_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/connection/api_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/helpers/cve_search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/nvd_nist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/nvd_nist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/nvd_nist/nvd_nist_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/mutex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/cpe_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/data_source_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/db_obj_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/connection/mongo_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/cpe_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/cvesearch_mongo_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/generic_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/specific_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/database/maintenance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/DatabaseSchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/DownloadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/IJSONHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/LogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52189 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/Sources_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/Toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/api_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/content_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/db_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/main_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/worker_q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/capec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cves.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cvexplore_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/via4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.265117 CveXplore-0.3.9/CveXplore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-17 15:26:55.000000 CveXplore-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-17 15:27:06.277118 CveXplore-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15684 2023-10-17 15:26:55.000000 CveXplore-0.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-17 15:26:55.000000 CveXplore-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 15:27:06.277118 CveXplore-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-10-17 15:26:55.000000 CveXplore-0.3.9/setup.py
```

### Comparing `CveXplore-0.3.8/CveXplore/LICENSE` & `CveXplore-0.3.9/CveXplore/LICENSE`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/api/api_base_class.py` & `CveXplore-0.3.9/CveXplore/api/api_base_class.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/api/connection/api_db.py` & `CveXplore-0.3.9/CveXplore/api/connection/api_db.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/api/helpers/cve_search_api.py` & `CveXplore-0.3.9/CveXplore/api/helpers/cve_search_api.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/api/nvd_nist/nvd_nist_api.py` & `CveXplore-0.3.9/CveXplore/api/nvd_nist/nvd_nist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,19 +59,17 @@
         self.datasource = namedtuple("datasource", "CVE CPE")(1, 2)
 
         self.datasource_mapping = {1: "cves", 2: "cpes"}
 
         self.max_page_length = namedtuple("max_page_length", "CVE CPE")(2000, 10000)
 
     def get_url_only(self, resource: dict = None, data: int = 1) -> str:
-
         return self._build_url(resource=resource, data=data)
 
     def _build_url(self, resource: dict = None, data: int = 1) -> str:
-
         if resource is not None:
             resource = urlencode(resource)
             if data == self.datasource.CVE:
                 if self.filter_rejected:
                     return f"{self.baseurl}/rest/json/{self.datasource_mapping[data]}/{self.api_path}/?noRejected&{resource}"
                 else:
                     return f"{self.baseurl}/rest/json/{self.datasource_mapping[data]}/{self.api_path}/?{resource}"
@@ -91,15 +89,14 @@
         method: str,
         resource: dict,
         session: requests.Session,
         data: dict = None,
         timeout: int = 60,
         return_response_object: bool = False,
     ):
-
         requests.packages.urllib3.disable_warnings()
 
         request_api_resource = {
             "headers": self.myheaders,
             "verify": self.verify,
             "timeout": timeout,
             "proxies": self.proxies,
@@ -134,15 +131,14 @@
             raise Exception(err)
 
     def __repr__(self):
         """return a string representation of the obj"""
         return f"<< NvdNistApi:{self.baseurl} >>"
 
     def get_cves_from_start_year(self):
-
         start_date = datetime(int(self.config.CVE_START_YEAR), 1, 1, 0, 0, 0, 0)
         start_date_iso = start_date.isoformat()
 
         end_date = start_date + timedelta(days=120)
         end_date_iso = end_date.isoformat()
 
         resource = {
@@ -154,15 +150,14 @@
 
     def check_date_range(
         self,
         resource: dict = None,
         last_mod_start_date: datetime = None,
         last_mod_end_date: datetime = None,
     ):
-
         # Check if diff > 120 days
         diff = last_mod_end_date - last_mod_start_date
 
         if diff.days > 120:
             delta = diff.days - 120
             last_mod_end_date = last_mod_end_date - timedelta(delta)
             self.logger.warning(
@@ -199,15 +194,14 @@
 
     def get_all_data(
         self,
         data_type: str,
         last_mod_start_date: datetime = None,
         last_mod_end_date: datetime = None,
     ):
-
         resource = {}
 
         if last_mod_start_date is not None and last_mod_end_date is not None:
             self.logger.debug(f"Getting all updated {data_type}s....")
             resource = self.check_date_range(
                 resource=resource,
                 last_mod_start_date=last_mod_start_date,
@@ -219,15 +213,14 @@
         data = self.get_count(
             getattr(self.datasource, data_type.upper()),
             last_mod_start_date=last_mod_start_date,
             last_mod_end_date=last_mod_end_date,
         )
 
         if isinstance(data, int):
-
             for each_data in ApiData(
                 results_per_page=getattr(self.max_page_length, data_type.upper()),
                 start_index=0,
                 total_results=data,
                 api_handle=self,
                 data_source=getattr(self.datasource, data_type.upper()),
                 resource=resource,
@@ -306,20 +299,18 @@
 
         self.workload = None
 
     def __iter__(self):
         return self
 
     def __next__(self):
-
         if (
             self._current_index < self._total_results
             or self._page_length == self._total_results
         ):
-
             start_time = time.time()
 
             if not self.last_stop_time == 0:
                 # adhering to best practices @https://nvd.nist.gov/general/news/API-Key-Announcement
                 # which advises to sleep for 6 seconds, so we add this to the 30 seconds rolling window; hence 36
                 sleep_time = start_time - self.last_stop_time
                 if sleep_time <= 36:
@@ -364,15 +355,14 @@
             self.logger.debug(f"Elapsed run time: {elapsed_time}")
 
             return ret_data
 
         raise StopIteration
 
     def process_async(self):
-
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
         results = loop.run_until_complete(self.fetch_all(loop))
 
         return results
 
     @retry(retry_policy)
```

### Comparing `CveXplore-0.3.8/CveXplore/cli.py` & `CveXplore-0.3.9/CveXplore/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
 import click
 import click_completion.core
 
+from CveXplore.cli_cmds.capec_cmds import commands as group6
+from CveXplore.cli_cmds.cwe_cmds import commands as group7
 from CveXplore.cli_cmds.cpe_cmds import commands as group5
 from CveXplore.cli_cmds.cve_cmds import commands as group2
 from CveXplore.cli_cmds.db_cmds import commands as group4
 from CveXplore.cli_cmds.find_cmds import commands as group1
 from CveXplore.cli_cmds.stats_cmds import commands as group3
 from CveXplore.main import CveXplore
 
@@ -19,14 +21,18 @@
 @click.option("-v", "--version", is_flag=True, help="Show the current version and exit")
 @click.pass_context
 def main(ctx, version):
     ctx.obj = {"data_source": CveXplore()}
     if version:
         click.echo(ctx.obj["data_source"].version)
         exit(0)
+    if ctx.invoked_subcommand is None:
+        click.echo(main.get_help(ctx))
 
 
 main.add_command(group1.search_cmd)
 main.add_command(group2.cve_cmd)
 main.add_command(group3.stats_cmd)
 main.add_command(group4.db_cmd)
 main.add_command(group5.cpe_cmd)
+main.add_command(group6.capec_cmd)
+main.add_command(group7.cwe_cmd)
```

### Comparing `CveXplore-0.3.8/CveXplore/cli_cmds/cli_utils/utils.py` & `CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 from collections import defaultdict
-from pprint import pformat
 
 import click
 import pandas as pd
 from dicttoxml import dicttoxml
 
 
 def format_output(format_type, input_list):
@@ -37,18 +36,12 @@
             output = dicttoxml(temp_dict, custom_root="CveXplore")
         elif isinstance(input_list, dict):
             output = dicttoxml(input_list, custom_root="CveXplore")
 
     return output
 
 
-def printer(input_data, pretty=False, output="json"):
+def printer(input_data, output="json"):
     if isinstance(input_data, list):
-        if not pretty:
-            click.echo(format_output(output, input_data))
-        else:
-            click.secho(pformat(input_data, indent=4), bold=True, fg="blue")
+        click.echo(format_output(output, input_data))
     elif isinstance(input_data, dict):
-        if not pretty:
-            click.echo(input_data)
-        else:
-            click.secho(pformat(input_data, indent=4), bold=True, fg="blue")
+        click.echo(input_data)
```

### Comparing `CveXplore-0.3.8/CveXplore/cli_cmds/cpe_cmds/commands.py` & `CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pprint import pformat
-
 import click
 import pymongo
 
 from CveXplore.cli_cmds.cli_utils.utils import printer
 from CveXplore.cli_cmds.mutex_options.mutex import Mutex
 
 
@@ -13,42 +11,67 @@
     if ctx.invoked_subcommand is None:
         click.echo(cpe_cmd.get_help(ctx))
 
 
 @cpe_cmd.group(
     "search",
     invoke_without_command=True,
-    help="Search for cpe entries by name or title. Results are sorted ASCENDING by default",
+    help="Search for cpe entries by name, vendor or title. Results are sorted ASCENDING by default",
 )
 @click.option(
     "-n",
     "--name",
     default=False,
     is_flag=True,
     help="Search by name",
     cls=Mutex,
-    not_required_if=["title", "vendor"],
+    not_required_if=["field", "cpe", "title", "vendor", "field_list"],
 )
 @click.option(
     "-t",
     "--title",
     default=True,
     is_flag=True,
     help="Search by title (default)",
     cls=Mutex,
-    not_required_if=["name", "vendor"],
+    not_required_if=["field", "cpe", "name", "vendor", "field_list"],
 )
 @click.option(
     "-v",
     "--vendor",
     default=False,
     is_flag=True,
     help="Search by vendor",
     cls=Mutex,
-    not_required_if=["name", "title"],
+    not_required_if=["field", "cpe", "name", "title", "field_list"],
+)
+@click.option(
+    "-c",
+    "--cpe",
+    help="Search for CPE's (could be multiple) by id",
+    multiple=True,
+    cls=Mutex,
+    not_required_if=["field_list", "name", "title", "vendor"],
+)
+@click.option(
+    "-f",
+    "--field",
+    help="Field to return (could be multiple)",
+    multiple=True,
+    cls=Mutex,
+    not_required_if=["field_list", "name", "title", "vendor"],
+)
+@click.option(
+    "-fl",
+    "--field_list",
+    help="Return a field list for this collection",
+    multiple=True,
+    is_flag=True,
+    cls=Mutex,
+    not_required_if=["field", "cpe", "name", "title", "vendor"],
 )
 @click.option(
     "-m",
     "--match",
     help="Use match for searching",
     cls=Mutex,
     not_required_if=["regex"],
@@ -68,46 +91,38 @@
     default=False,
     is_flag=True,
     help="If adding CVE's search for vulnerable products and not for vulnerable configurations",
 )
 @click.option("-l", "--limit", default=10, help="Search limit")
 @click.option("-s", "--sort", is_flag=True, help="Sort DESCENDING")
 @click.option(
-    "--pretty",
-    is_flag=True,
-    help="Pretty print the output",
-    cls=Mutex,
-    not_required_if=["output"],
-)
-@click.option(
     "-o",
     "--output",
     default="json",
     help="Set the desired output format (defaults to json)",
     type=click.Choice(["json", "csv", "xml", "html"], case_sensitive=False),
-    cls=Mutex,
-    not_required_if=["pretty"],
 )
 @click.pass_context
 def search_cmd(
     ctx,
     name,
     title,
     vendor,
+    cpe,
+    field,
+    field_list,
     match,
     regex,
     deprecated,
     cve,
     product_search,
     limit,
     sort,
-    pretty,
     output,
 ):
-
     if not name and not vendor and title:
         search_by = "title"
     elif name and not vendor and title:
         search_by = "cpeName"
     else:
         search_by = "vendor"
 
@@ -136,23 +151,28 @@
         else:
             ret_list = (
                 getattr(getattr(ctx.obj["data_source"], "cpe"), search_by)
                 .find(match)
                 .limit(limit)
                 .sort(search_by, sorting)
             )
+    elif cpe:
+        ret_list = getattr(ctx.obj["data_source"], "cpe").mget_by_id(*cpe)
+    elif field_list:
+        ret_list = getattr(ctx.obj["data_source"], "cpe").field_list()
     else:
         click.echo(search_cmd.get_help(ctx))
         return
 
     if cve:
         result = [result.to_cve_summary(product_search) for result in ret_list]
+    elif cpe:
+        result = [result.to_dict(*field) for result in ret_list]
+    elif isinstance(ret_list, set):
+        result = sorted([result for result in ret_list])
     else:
         result = [result.to_dict() for result in ret_list]
 
     if ctx.invoked_subcommand is None:
-        printer(input_data=result, pretty=pretty, output=output)
+        printer(input_data=result, output=output)
     else:
-        if pretty:
-            ctx.obj["RESULT"] = pformat(result, indent=4)
-        else:
-            ctx.obj["RESULT"] = result
+        ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.8/CveXplore/cli_cmds/db_cmds/commands.py` & `CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 
 @click.group(
     "database", invoke_without_command=True, help="Database update / populate commands"
 )
 @click.pass_context
 def db_cmd(ctx):
-    pass
+    if ctx.invoked_subcommand is None:
+        click.echo(db_cmd.get_help(ctx))
 
 
 @db_cmd.group("update", invoke_without_command=True, help="Update the database")
 @click.pass_context
 def update_cmd(ctx):
     ctx.obj["data_source"].database.update()
 
@@ -26,27 +27,27 @@
 def initialize_cmd(ctx):
     ctx.obj["data_source"].database.initialize()
 
 
 @db_cmd.group("sources", invoke_without_command=True, help="Database source management")
 @click.pass_context
 def sources_cmd(ctx):
-    pass
+    if ctx.invoked_subcommand is None:
+        click.echo(sources_cmd.get_help(ctx))
 
 
 @sources_cmd.group("show", invoke_without_command=True, help="Show sources")
-@click.option("--pretty", is_flag=True, help="Pretty print the output")
 @click.pass_context
-def show_cmd(ctx, pretty):
+def show_cmd(ctx):
     config = Configuration()
 
     if ctx.invoked_subcommand is None:
-        printer(input_data=config.SOURCES, pretty=pretty)
+        printer(input_data=[config.SOURCES])
     else:
-        printer(input_data=config.SOURCES, pretty=pretty)
+        printer(input_data=[config.SOURCES])
 
 
 @sources_cmd.group("set", invoke_without_command=True, help="Set sources")
 @click.option(
     "-k",
     "--key",
     help="Set the source key",
@@ -60,21 +61,21 @@
     sources = config.SOURCES
 
     sources[key] = value
 
     with open(os.path.join(config.USER_HOME_DIR, ".sources.ini"), "w") as f:
         f.write(json.dumps(sources))
 
-    printer(input_data={"SOURCES SET TO": sources}, pretty=True)
+    printer(input_data=[{"SOURCES SET TO": sources}])
 
 
 @sources_cmd.group("reset", invoke_without_command=True, help="Set sources")
 @click.pass_context
 def reset_cmd(ctx):
     config = Configuration()
 
     sources = config.DEFAULT_SOURCES
 
     with open(os.path.join(config.USER_HOME_DIR, ".sources.ini"), "w") as f:
         f.write(json.dumps(sources))
 
-    printer(input_data={"SOURCES RESET TO": sources}, pretty=True)
+    printer(input_data=[{"SOURCES RESET TO": sources}])
```

### Comparing `CveXplore-0.3.8/CveXplore/cli_cmds/find_cmds/commands.py` & `CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from pprint import pformat
-
 import click
 
 from CveXplore.cli_cmds.cli_utils.utils import printer
-from CveXplore.cli_cmds.mutex_options.mutex import Mutex
 
 
 @click.group(
     "find",
     invoke_without_command=True,
     help="Perform find queries on a single collection",
 )
@@ -18,39 +15,27 @@
     type=click.Choice(["capec", "cpe", "cwe", "via4", "cves"], case_sensitive=False),
     help="Collection to query",
 )
 @click.option("-f", "--field", required=True, help="Field to query")
 @click.option("-v", "--value", required=True, help="Value to query")
 @click.option("-l", "--limit", default=10, help="Query limit")
 @click.option(
-    "--pretty",
-    is_flag=True,
-    help="Pretty print the output",
-    cls=Mutex,
-    not_required_if=["output"],
-)
-@click.option(
     "-o",
     "--output",
     default="json",
     help="Set the desired output format (defaults to json)",
     type=click.Choice(["json", "csv", "xml", "html"], case_sensitive=False),
-    cls=Mutex,
-    not_required_if=["pretty"],
 )
 @click.pass_context
-def search_cmd(ctx, collection, field, value, limit, pretty, output):
+def search_cmd(ctx, collection, field, value, limit, output):
     ret_list = ctx.obj["data_source"].get_single_store_entries(
         (collection, {field: value.upper()}), limit=limit
     )
     try:
         result = [result.to_dict() for result in ret_list]
     except TypeError:
         result = []
 
     if ctx.invoked_subcommand is None:
-        printer(input_data=result, pretty=pretty, output=output)
+        printer(input_data=result, output=output)
     else:
-        if pretty:
-            ctx.obj["RESULT"] = pformat(result, indent=4)
-        else:
-            ctx.obj["RESULT"] = result
+        ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.8/CveXplore/cli_cmds/mutex_options/mutex.py` & `CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/mutex.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         self.not_required_if: list = kwargs.pop("not_required_if")
 
         if not hasattr(self, "not_required_if"):
             raise AssertionError("'not_required_if' parameter required")
 
         kwargs["help"] = (
             kwargs.get("help", "")
-            + ". *** Option is mutually exclusive with the option(s): '"
+            + ". \n\n*** Option is mutually exclusive with the option(s): '"
             + ", ".join(self.not_required_if)
             + "'. ***"
         ).strip()
         super(Mutex, self).__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         current_opt: bool = self.name in opts
```

### Comparing `CveXplore-0.3.8/CveXplore/common/config.py` & `CveXplore-0.3.9/CveXplore/common/config.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/common/cpe_converters.py` & `CveXplore-0.3.9/CveXplore/common/cpe_converters.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/common/data_source_connection.py` & `CveXplore-0.3.9/CveXplore/common/data_source_connection.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/connection/mongo_db.py` & `CveXplore-0.3.9/CveXplore/database/connection/mongo_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,30 +50,28 @@
                     "store_{}".format(each),
                     CveSearchCollection(database=self._dbclient, name=each),
                 )
 
         atexit.register(self.disconnect)
 
     def get_collections_details(self):
-
         for each in self._dbclient.list_collections():
             yield each
 
     def set_handlers_for_collections(self):
         for each in self._dbclient.list_collection_names():
             if not hasattr(self, each):
                 setattr(
                     self,
                     "store_{}".format(each),
                     CveSearchCollection(database=self._dbclient, name=each),
                 )
 
     @property
     def get_collection_names(self):
-
         return self._dbclient.list_collection_names()
 
     def disconnect(self):
         """
         Disconnect from mongodb
         """
         if self.client is not None:
```

### Comparing `CveXplore-0.3.8/CveXplore/database/helpers/cpe_conversion.py` & `CveXplore-0.3.9/CveXplore/database/helpers/cpe_conversion.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/helpers/cvesearch_mongo_database.py` & `CveXplore-0.3.9/CveXplore/database/helpers/cvesearch_mongo_database.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/helpers/generic_db.py` & `CveXplore-0.3.9/CveXplore/database/helpers/generic_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Generic database functions
 ==========================
 """
 import re
+from functools import reduce
+from typing import Union, Iterable
 
 from CveXplore.common.data_source_connection import DatasourceConnection
 from CveXplore.common.db_mapping import database_mapping
+from CveXplore.objects.cvexplore_object import CveXploreObject
 
 
 class GenericDatabaseFactory(DatasourceConnection):
     """
     The GenericDatabaseFactory handles the creation of general, collection based, functions which provide an instance
     of CveXplore functions that apply to the given collection.
     """
@@ -72,14 +75,42 @@
             try:
                 doc_id = str(doc_id)
             except ValueError:
                 return "Provided value is not a string nor can it be cast to one"
 
         return self._datasource_collection_connection.find_one({"id": doc_id})
 
+    def mget_by_id(self, *doc_ids: str) -> Union[Iterable[CveXploreObject], Iterable]:
+        """
+        Method to fetch a specific collection entry via it's id number
+        """
+        ret_data = []
+        for doc_id in doc_ids:
+            data = self.get_by_id(doc_id=doc_id)
+            if data is not None:
+                ret_data.append(data)
+
+        if len(ret_data) >= 1:
+            return sorted(ret_data, key=lambda x: x.id)
+        else:
+            return ret_data
+
+    def field_list(self) -> set:
+        """
+        Method to fetch all field names from a specific collection
+        """
+        return reduce(
+            lambda all_keys, rec_keys: all_keys | set(rec_keys),
+            map(
+                lambda d: d.to_dict(),
+                [self._datasource_collection_connection.find_one()],
+            ),
+            set(),
+        )
+
     def __repr__(self):
         """String representation of object"""
         return "<< GenericDatabaseFactory:{} >>".format(self._collection)
 
 
 class GenericDatabaseFieldsFunctions(DatasourceConnection):
     """
```

### Comparing `CveXplore-0.3.8/CveXplore/database/helpers/specific_db.py` & `CveXplore-0.3.9/CveXplore/database/helpers/specific_db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Specific database functions
 ===========================
 """
 import re
-from typing import List
+from typing import List, Union, Iterable
 
 from pymongo import DESCENDING
 
 from CveXplore.database.helpers.generic_db import GenericDatabaseFactory
+from CveXplore.errors.validation import CveNumberValidationError
 from CveXplore.objects.cvexplore_object import CveXploreObject
 
 
 class CvesDatabaseFunctions(GenericDatabaseFactory):
     """
     The CvesDatabaseFunctions is a specific class that provides the cves attribute of a CveXplore instance additional
     functions that only apply to the 'cves' collection
@@ -34,14 +35,41 @@
         )
 
         if len(the_result) != 0:
             return the_result
         else:
             return None
 
+    def get_by_id(self, doc_id: str):
+        """
+        Method to retrieve a single CVE from the database by its CVE ID number.
+        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
+        """
+        # first try to match full cve number format
+        reg_match = re.compile(r"[cC][vV][eE]-\d{4}-\d{4,10}")
+        if reg_match.match(doc_id) is not None:
+            doc_id = doc_id.upper()
+        else:
+            part_match = re.compile(r"\d{4}-\d{4,10}")
+            if part_match.match(doc_id) is not None:
+                doc_id = f"CVE-{doc_id}"
+            else:
+                raise CveNumberValidationError(
+                    "Could not validate the CVE number. The number format should be either "
+                    "CVE-2000-0001, cve-2000-0001 or 2000-0001."
+                )
+
+        if not isinstance(doc_id, str):
+            try:
+                doc_id = str(doc_id)
+            except ValueError:
+                return "Provided value is not a string nor can it be cast to one"
+
+        return self._datasource_collection_connection.find_one({"id": doc_id})
+
     def __repr__(self):
         """String representation of object"""
         return "<< CvesDatabaseFunctions:{} >>".format(self._collection)
 
 
 class CpeDatabaseFunctions(GenericDatabaseFactory):
     """
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/DatabaseSchemaChecker.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/DatabaseSchemaChecker.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         # hack for db_updater.py to put this class in the posts variable and run the update method
         self.logger.info("Updating schema version")
         self.update()
         self.logger.info("Update schema version done!")
 
     def update(self):
         try:
-
             current_record = list(self.dbh.find({}))
 
             if len(current_record) != 0:
                 current_record[0]["version"] = self.schema_version["version"]
                 current_record[0]["rebuild_needed"] = self.schema_version[
                     "rebuild_needed"
                 ]
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/DownloadHandler.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/DownloadHandler.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/IJSONHandler.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/IJSONHandler.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/LogHandler.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/LogHandler.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/Sources_process.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/Sources_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,15 @@
         self.last_modified = datetime.datetime.now()
 
         self.logger.debug(
             f"do_process = {self.do_process}; is_update = {self.is_update}"
         )
 
         if self.do_process:
-
             if not self.is_update:
-
                 total_results = self.api_handler.get_count(
                     self.api_handler.datasource.CPE
                 )
 
                 self.logger.info(f"Preparing to download {total_results} CPE entries")
 
                 with tqdm(
@@ -752,17 +750,15 @@
         self.last_modified = datetime.datetime.now()
 
         self.logger.debug(
             f"do_process = {self.do_process}; is_update = {self.is_update}"
         )
 
         if self.do_process:
-
             if not self.is_update:
-
                 total_results = self.api_handler.get_count(
                     self.api_handler.datasource.CVE
                 )
 
                 self.logger.info(f"Preparing to download {total_results} CVE entries")
 
                 with tqdm(
@@ -855,15 +851,14 @@
         self.process_downloads()
 
         self.logger.info("Finished CVE database update")
 
         return self.last_modified
 
     def populate(self):
-
         self.logger.info("CVE database population started")
 
         self.logger.info(
             "Starting CVE database population starting from year: {}".format(
                 cveStartYear
             )
         )
@@ -896,15 +891,14 @@
         super().__init__(self.feed_type, self.prefix)
 
         self.feed_url = Configuration.getFeedURL(self.feed_type.lower())
 
         self.logger = logging.getLogger("VIADownloads")
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
-
         working_dir, filename = file_tuple
 
         for cve in self.ijson_handler.fetch(filename=filename, prefix=self.prefix):
             x = 0
             for key, val in cve.items():
                 entry_dict = {"id": key}
                 entry_dict.update(val)
@@ -926,15 +920,14 @@
             shutil.rmtree(working_dir)
         except Exception as err:
             self.logger.error(
                 "Failed to remove working dir; error produced: {}".format(err)
             )
 
     def process_item(self, item: dict):
-
         if self.is_update:
             self.queue.put(
                 DatabaseAction(
                     action=DatabaseAction.actions.UpdateOne,
                     collection=self.feed_type.lower(),
                     doc=item,
                 )
@@ -987,15 +980,14 @@
 
         # make parser
         self.parser = make_parser()
         self.ch = CapecHandler()
         self.parser.setContentHandler(self.ch)
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
-
         working_dir, filename = file_tuple
 
         self.parser.parse(filename)
         x = 0
         for attack in self.ch.capec:
             self.process_item(attack)
             x += 1
@@ -1049,15 +1041,14 @@
 
         # make parser
         self.parser = make_parser()
         self.ch = CWEHandler()
         self.parser.setContentHandler(self.ch)
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
-
         working_dir, filename = file_tuple
 
         for f in glob.glob(f"{working_dir}/*.xml"):
             filename = f
 
         self.parser.parse(f"file://{filename}")
         x = 0
@@ -1109,15 +1100,14 @@
 
 class DatabaseIndexer(object):
     """
     Class processing the Mongodb indexes
     """
 
     def __init__(self):
-
         database = MongoDBConnection(**json.loads(os.getenv("MONGODB_CON_DETAILS")))
         self.database = database._dbclient
 
         self.indexes = {
             "cpe": [
                 MongoUniqueIndex(index=[("id", ASCENDING)], name="id", unique=True),
                 MongoAddIndex(index=[("vendor", ASCENDING)], name="vendor"),
@@ -1171,15 +1161,14 @@
 
         self.logger = logging.getLogger("DatabaseIndexer")
 
     def getInfo(self, collection: str):
         return sanitize(self.database["info"].find_one({"db": collection}))
 
     def create_indexes(self, collection: str = None):
-
         if collection is not None:
             try:
                 for each in self.indexes[collection]:
                     if isinstance(each, MongoUniqueIndex):
                         self.setIndex(
                             collection, each.index, name=each.name, unique=each.unique
                         )
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/api_handlers.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/api_handlers.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/content_handlers.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/content_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         self.techniques = []
 
         self.taxonomy_mapping = defaultdict(dict)
 
         self.execution_flow = defaultdict(dict)
 
     def startElement(self, name, attrs):
-
         if name == "Attack_Pattern_Catalog":
             self.Attack_Pattern_Catalog_tag = True
         if name == "Attack_Patterns" and self.Attack_Pattern_Catalog_tag:
             self.Attack_Patterns_tag = True
         if name == "Attack_Pattern" and self.Attack_Patterns_tag:
             self.Attack_Pattern_tag = True
 
@@ -226,15 +225,14 @@
                 else:
                     # attack with subtechniques use cut_entry
                     url = "https://attack.mitre.org/techniques/T{}/{}".format(
                         cut_entry[0], cut_entry[1]
                     )
 
             elif self.taxonomy_name == "WASC":
-
                 if "/" in self.entry_name_ch:
                     url = "http://projects.webappsec.org/{}".format(
                         self.entry_name_ch.replace("/", " and ").replace(" ", "-")
                     )
                 else:
                     url = "http://projects.webappsec.org/{}".format(
                         self.entry_name_ch.replace(" ", "-")
@@ -381,15 +379,14 @@
         self.description_tag = False
         self.category_tag = False
         self.weakness_tag = False
         self.weakness_relationships_tag = False
         self.category_relationships_tag = False
 
     def startElement(self, name, attrs):
-
         if name == "Weakness":
             self.weakness_tag = True
             self.statement = ""
             self.weaknessabs = attrs.get("Abstraction")
             self.name = attrs.get("Name")
             self.idname = attrs.get("ID")
             self.status = attrs.get("Status")
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/db_action.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/db_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pymongo import InsertOne, UpdateOne
 
 
 class DatabaseAction(object):
     actions = collections.namedtuple("Actions", "InsertOne UpdateOne")(0, 1)
 
     def __init__(self, action: actions, collection: str, doc: dict):
-
         self.action = action
         self.collection = collection
         self.doc = doc
 
     @property
     def entry(self):
         if self.action == self.actions.InsertOne:
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/file_handlers.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/file_handlers.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/main_updater.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/main_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         """
         if update_source is not None:
             if not isinstance(update_source, str | list):
                 raise ValueError("Wrong 'update_source' parameter type received!")
 
         try:
             if update_source is None:
-
                 for source in self.sources:
                     up = source["updater"]()
                     up.update()
 
             elif isinstance(update_source, list):
                 for source in update_source:
                     try:
```

### Comparing `CveXplore-0.3.8/CveXplore/database/maintenance/worker_q.py` & `CveXplore-0.3.9/CveXplore/database/maintenance/worker_q.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from queue import Empty, Queue
 
 from CveXplore.database.maintenance.db_action import DatabaseAction
 
 
 class WorkerQueue(Queue):
     def __init__(self, name: str, maxsize: int = 0):
-
         super().__init__(maxsize)
         self.name = name
         self.maxsize = maxsize
 
         self.closed = False
 
     def __len__(self):
```

### Comparing `CveXplore-0.3.8/CveXplore/main.py` & `CveXplore-0.3.9/CveXplore/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ====
 """
 import functools
 import json
 import os
 import re
 from collections import defaultdict
-from typing import List, Tuple
+from typing import List, Tuple, Union, Iterable
 
 from pymongo import DESCENDING
 
 from CveXplore.api.connection.api_db import ApiDatabaseSource
 from CveXplore.common.cpe_converters import from2to3CPE
 from CveXplore.common.db_mapping import database_mapping
 from CveXplore.database.connection.mongo_db import MongoDBConnection
@@ -266,14 +266,28 @@
                 raise CveNumberValidationError(
                     "Could not validate the CVE number. The number format should be either "
                     "CVE-2000-0001, cve-2000-0001 or 2000-0001."
                 )
 
         return self.get_single_store_entry("cves", {"id": cve_id})
 
+    def cves_by_id(self, *cve_ids: str) -> Union[Iterable[CveXploreObject], Iterable]:
+        """
+        Method to retrieve a multiple CVE's from the database by its CVE ID number.
+        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
+        """
+        ret_data = []
+        for cve_id in cve_ids:
+            ret_data.append(self.cve_by_id(cve_id=cve_id))
+
+        if len(ret_data) >= 1:
+            return sorted(ret_data, key=lambda x: x.id)
+        else:
+            return ret_data
+
     def capec_by_cwe_id(self, cwe_id: int) -> List[CveXploreObject] | None:
         """
         Method to retrieve capecs related to a specific CWE ID
         """
 
         cwe = self.get_single_store_entry("cwe", {"id": cwe_id})
 
@@ -306,15 +320,14 @@
         Property returning the stats from the database. Stats consist of the time last modified and the document count
         per cvedb store in the database.
         """
 
         stats = defaultdict(dict)
 
         if not isinstance(self.datasource, ApiDatabaseSource):
-
             if hasattr(self.datasource, "store_info"):
                 results = self.datasource.store_info.find({})
                 for each in results:
                     each.pop("_id")
                     db = each["db"]
                     each.pop("db")
```

### Comparing `CveXplore-0.3.8/CveXplore/objects/capec.py` & `CveXplore-0.3.9/CveXplore/objects/capec.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class Capec(DatasourceConnection):
     """
     Capec database object
     """
 
     def __init__(self, **kwargs):
-
         super().__init__("capec")
 
         for each in kwargs:
             setattr(self, each, kwargs[each])
 
     def iter_related_weaknessess(self):
         """
```

### Comparing `CveXplore-0.3.8/CveXplore/objects/cpe.py` & `CveXplore-0.3.9/CveXplore/objects/cpe.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class Cpe(DatasourceConnection):
     """
     Cpe database object
     """
 
     def __init__(self, **kwargs):
-
         super().__init__("cpe")
 
         for each in kwargs:
             setattr(self, each, kwargs[each])
 
     def iter_cves_matching_cpe(self, vuln_prod_search: bool = False):
         """
```

### Comparing `CveXplore-0.3.8/CveXplore/objects/cves.py` & `CveXplore-0.3.9/CveXplore/objects/cves.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 class Cves(DatasourceConnection):
     """
     Cves database object
     """
 
     def __init__(self, **kwargs):
-
         super().__init__("cves")
 
         for each in kwargs:
             setattr(self, each, kwargs[each])
 
         if hasattr(self, "cwe"):
             if isinstance(self.cwe, str):
```

### Comparing `CveXplore-0.3.8/CveXplore/objects/cwe.py` & `CveXplore-0.3.9/CveXplore/objects/cwe.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class Cwe(DatasourceConnection):
     """
     Cwe database object
     """
 
     def __init__(self, **kwargs):
-
         super().__init__("cwe")
 
         for each in kwargs:
             setattr(self, each, kwargs[each])
 
     def iter_related_weaknessess(self):
         """
```

### Comparing `CveXplore-0.3.8/CveXplore.egg-info/PKG-INFO` & `CveXplore-0.3.9/CveXplore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CveXplore
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for interacting with cve-search
 Home-page: https://github.com/cve-search/CveXplore
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Documentation, https://cve-search.github.io/CveXplore/
 Project-URL: Issues, https://github.com/cve-search/CveXplore/issues
```

### Comparing `CveXplore-0.3.8/CveXplore.egg-info/SOURCES.txt` & `CveXplore-0.3.9/CveXplore.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 CveXplore/api/connection/__init__.py
 CveXplore/api/connection/api_db.py
 CveXplore/api/helpers/__init__.py
 CveXplore/api/helpers/cve_search_api.py
 CveXplore/api/nvd_nist/__init__.py
 CveXplore/api/nvd_nist/nvd_nist_api.py
 CveXplore/cli_cmds/__init__.py
+CveXplore/cli_cmds/capec_cmds/__init__.py
+CveXplore/cli_cmds/capec_cmds/commands.py
 CveXplore/cli_cmds/cli_utils/__init__.py
 CveXplore/cli_cmds/cli_utils/utils.py
 CveXplore/cli_cmds/cpe_cmds/__init__.py
 CveXplore/cli_cmds/cpe_cmds/commands.py
 CveXplore/cli_cmds/cve_cmds/__init__.py
 CveXplore/cli_cmds/cve_cmds/commands.py
+CveXplore/cli_cmds/cwe_cmds/__init__.py
+CveXplore/cli_cmds/cwe_cmds/commands.py
 CveXplore/cli_cmds/db_cmds/__init__.py
 CveXplore/cli_cmds/db_cmds/commands.py
 CveXplore/cli_cmds/find_cmds/__init__.py
 CveXplore/cli_cmds/find_cmds/commands.py
 CveXplore/cli_cmds/mutex_options/__init__.py
 CveXplore/cli_cmds/mutex_options/mutex.py
 CveXplore/cli_cmds/stats_cmds/__init__.py
```

### Comparing `CveXplore-0.3.8/LICENSE` & `CveXplore-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/PKG-INFO` & `CveXplore-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CveXplore
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for interacting with cve-search
 Home-page: https://github.com/cve-search/CveXplore
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Documentation, https://cve-search.github.io/CveXplore/
 Project-URL: Issues, https://github.com/cve-search/CveXplore/issues
```

### Comparing `CveXplore-0.3.8/README.rst` & `CveXplore-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.8/setup.py` & `CveXplore-0.3.9/setup.py`

 * *Files identical despite different names*

